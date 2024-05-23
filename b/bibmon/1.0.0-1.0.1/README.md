# Comparing `tmp/bibmon-1.0.0.tar.gz` & `tmp/bibmon-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibmon-1.0.0.tar", last modified: Thu May 23 16:09:40 2024, max compression
+gzip compressed data, was "bibmon-1.0.1.tar", last modified: Thu May 23 19:42:08 2024, max compression
```

## Comparing `bibmon-1.0.0.tar` & `bibmon-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 16:09:40.471651 bibmon-1.0.0/
--rw-rw-rw-   0        0        0    11354 2024-02-12 23:27:53.000000 bibmon-1.0.0/LICENSE.md
--rw-rw-rw-   0        0        0     3712 2024-05-23 16:09:40.471651 bibmon-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3299 2024-02-15 11:36:41.000000 bibmon-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 16:09:40.376730 bibmon-1.0.0/bibmon/
--rw-rw-rw-   0        0        0      637 2024-02-12 22:13:00.000000 bibmon-1.0.0/bibmon/__init__.py
--rw-rw-rw-   0        0        0     1311 2024-02-12 17:11:14.000000 bibmon-1.0.0/bibmon/_alarms.py
--rw-rw-rw-   0        0        0    26114 2024-02-12 23:12:13.000000 bibmon-1.0.0/bibmon/_bibmon_tools.py
--rw-rw-rw-   0        0        0    40572 2024-02-12 17:10:29.000000 bibmon-1.0.0/bibmon/_generic_model.py
--rw-rw-rw-   0        0        0     3186 2024-02-12 23:18:38.000000 bibmon-1.0.0/bibmon/_load_data.py
--rw-rw-rw-   0        0        0     3825 2024-02-12 17:34:17.000000 bibmon-1.0.0/bibmon/_pca.py
--rw-rw-rw-   0        0        0    12323 2024-02-12 23:09:24.000000 bibmon-1.0.0/bibmon/_preprocess.py
--rw-rw-rw-   0        0        0     5213 2024-02-12 17:25:57.000000 bibmon-1.0.0/bibmon/_sklearn_regressor.py
--rw-rw-rw-   0        0        0     2839 2024-05-23 15:21:27.000000 bibmon-1.0.0/bibmon/_template_generic_model_childs.py
-drwxrwxrwx   0        0        0        0 2024-05-23 16:09:40.425140 bibmon-1.0.0/bibmon.egg-info/
--rw-rw-rw-   0        0        0     3712 2024-05-23 16:09:39.000000 bibmon-1.0.0/bibmon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2024-05-23 16:09:40.000000 bibmon-1.0.0/bibmon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 16:09:39.000000 bibmon-1.0.0/bibmon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2024-05-23 16:09:39.000000 bibmon-1.0.0/bibmon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-23 16:09:39.000000 bibmon-1.0.0/bibmon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 16:09:40.471651 bibmon-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      897 2024-05-23 16:08:53.000000 bibmon-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 16:09:40.471651 bibmon-1.0.0/test/
--rw-rw-rw-   0        0        0     8749 2024-02-12 21:54:51.000000 bibmon-1.0.0/test/test_models.py
--rw-rw-rw-   0        0        0     2099 2024-02-12 10:52:41.000000 bibmon-1.0.0/test/test_preprocess.py
--rw-rw-rw-   0        0        0     2278 2024-02-12 10:54:36.000000 bibmon-1.0.0/test/test_tools.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:42:08.281554 bibmon-1.0.1/
+-rw-rw-rw-   0        0        0    11554 2024-05-23 18:28:30.000000 bibmon-1.0.1/LICENSE.md
+-rw-rw-rw-   0        0        0     3604 2024-05-23 19:42:08.281554 bibmon-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3248 2024-05-23 18:28:30.000000 bibmon-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 19:42:08.170932 bibmon-1.0.1/bibmon/
+-rw-rw-rw-   0        0        0      647 2024-05-23 18:28:30.000000 bibmon-1.0.1/bibmon/__init__.py
+-rw-rw-rw-   0        0        0     1357 2024-05-23 18:28:30.000000 bibmon-1.0.1/bibmon/_alarms.py
+-rw-rw-rw-   0        0        0    26808 2024-05-23 18:28:30.000000 bibmon-1.0.1/bibmon/_bibmon_tools.py
+-rw-rw-rw-   0        0        0    41603 2024-05-23 18:28:30.000000 bibmon-1.0.1/bibmon/_generic_model.py
+-rw-rw-rw-   0        0        0     2953 2024-05-23 19:25:42.000000 bibmon-1.0.1/bibmon/_load_data.py
+-rw-rw-rw-   0        0        0     3941 2024-05-23 18:28:30.000000 bibmon-1.0.1/bibmon/_pca.py
+-rw-rw-rw-   0        0        0    12716 2024-05-23 18:28:30.000000 bibmon-1.0.1/bibmon/_preprocess.py
+-rw-rw-rw-   0        0        0     5359 2024-05-23 18:28:30.000000 bibmon-1.0.1/bibmon/_sklearn_regressor.py
+-rw-rw-rw-   0        0        0     2922 2024-05-23 18:28:30.000000 bibmon-1.0.1/bibmon/_template_generic_model_childs.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:42:08.233909 bibmon-1.0.1/bibmon/real_process_data/
+-rw-rw-rw-   0        0        0        0 2024-05-23 19:26:32.000000 bibmon-1.0.1/bibmon/real_process_data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:42:08.233909 bibmon-1.0.1/bibmon/tennessee_eastman/
+-rw-rw-rw-   0        0        0        0 2024-05-23 19:26:32.000000 bibmon-1.0.1/bibmon/tennessee_eastman/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:42:08.225902 bibmon-1.0.1/bibmon.egg-info/
+-rw-rw-rw-   0        0        0     3604 2024-05-23 19:42:07.000000 bibmon-1.0.1/bibmon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      529 2024-05-23 19:42:07.000000 bibmon-1.0.1/bibmon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 19:42:07.000000 bibmon-1.0.1/bibmon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2024-05-23 19:42:07.000000 bibmon-1.0.1/bibmon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-23 19:42:07.000000 bibmon-1.0.1/bibmon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 19:42:08.281554 bibmon-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      932 2024-05-23 19:38:58.000000 bibmon-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:42:08.265913 bibmon-1.0.1/test/
+-rw-rw-rw-   0        0        0     8977 2024-05-23 18:28:30.000000 bibmon-1.0.1/test/test_models.py
+-rw-rw-rw-   0        0        0     2160 2024-05-23 18:28:30.000000 bibmon-1.0.1/test/test_preprocess.py
+-rw-rw-rw-   0        0        0     2340 2024-05-23 18:28:30.000000 bibmon-1.0.1/test/test_tools.py
```

### Comparing `bibmon-1.0.0/LICENSE.md` & `bibmon-1.0.1/LICENSE.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

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
-   Copyright 2022 Petróleo Brasileiro S.A.
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
+   Copyright 2022 Petróleo Brasileiro S.A.
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
    limitations under the License.
```

### Comparing `bibmon-1.0.0/PKG-INFO` & `bibmon-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibmon
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library with routines for data-driven process monitoring.
 Home-page: https://github.com/petrobras/bibmon
 Author: BibMon developers
 Author-email: cc-bibmon@petrobras.com.br
 License: Apache 2.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -21,17 +21,17 @@
 # BibMon
 
 `BibMon` (from the Portuguese ***Bib**lioteca de **Mon**itoramento de Processos*, or Process Monitoring Library) is a Python package that provides deviation-based predictive models for fault detection, soft sensing, and process condition monitoring.
 
 Installation
 ----------------------
 
-`BibMon` can be installed locally using `pip`. In the root directory of the package, which contains the `setup.py` file, type the following command:
+`BibMon` can be installed using `pip`:
 
-    pip install -e .
+    pip install bibmon
 
 Available Models
 ----------------------
 
 * PCA (Principal Component Analysis);
 * any regressor that uses the `scikit-learn` interface.
```

### Comparing `bibmon-1.0.0/README.md` & `bibmon-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-[![Apache 2.0][apache-shield]][apache] 
-[![CC BY 4.0][cc-by-shield]][cc-by]
-
-[apache]: https://opensource.org/licenses/Apache-2.0
-[apache-shield]: https://img.shields.io/badge/License-Apache_2.0-blue.svg
-[cc-by]: http://creativecommons.org/licenses/by/4.0/
-[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
-
-# BibMon
-
-`BibMon` (from the Portuguese ***Bib**lioteca de **Mon**itoramento de Processos*, or Process Monitoring Library) is a Python package that provides deviation-based predictive models for fault detection, soft sensing, and process condition monitoring.
-
-Installation
-----------------------
-
-`BibMon` can be installed locally using `pip`. In the root directory of the package, which contains the `setup.py` file, type the following command:
-
-    pip install -e .
-
-Available Models
-----------------------
-
-* PCA (Principal Component Analysis);
-* any regressor that uses the `scikit-learn` interface.
-
-Usage
-----------------------
-
-Essentially, the library is used in two steps:
-
-1. In the training step, a model is generated that captures the relationships between variables in the normal process condition;
-2. In the prediction step, process data is compared to the model's predictions, resulting in deviations; if these deviations exceed a predefined limit, alarms are triggered.
-
-Specifically, the implemented control charts are based on squared prediction error (SPE).
-
-The examples in the `notebooks/` directory demonstrate the main functionalities of `BibMon`. The API reference can be generated using the Sphynx package from the files in the `docs/` directory.
-
-Features
-----------------------
-
-The resources offered by `BibMon` are:
-
-* Application in online systems: a trained `BibMon` model can be used for online analysis with both individual samples and data windows. For each sample or window, a prediction is made, the model state is updated, and alarms are calculated.
-* Compatibility, within the same architecture, of regression models (i.e., virtual sensors, containing separate X and Y data, such as RandomForest) and reconstruction models (containing only X data, such as PCA).
-* Preprocessing pipelines that take into account the differences between X and Y data and between training and testing stages.
-* Possibility of programming different alarm logics.
-* Easy extensibility through inheritance (there is a class called `GenericModel` that implements all the common functionality for various models and can be used as a base for implementing new models). For details, consult the `CONTRIBUTING.md` file.
-* Convenience functions for performing automatic offline analysis and plotting control charts.
-* Real and simulated process datasets available for importing.
-* Comparative tables to automate the performance analysis of different models.
-* Automatic hyperparameter tuning.
-
-Contributing
-----------------------
-
-BibMon is an open-source project driven by the community. If you would like to contribute to the project, please refer to the [CONTRIBUTING.md](https://github.com/petrobras/bibmon/blob/main/CONTRIBUTING.md) file.
-
+[![Apache 2.0][apache-shield]][apache] 
+[![CC BY 4.0][cc-by-shield]][cc-by]
+
+[apache]: https://opensource.org/licenses/Apache-2.0
+[apache-shield]: https://img.shields.io/badge/License-Apache_2.0-blue.svg
+[cc-by]: http://creativecommons.org/licenses/by/4.0/
+[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
+
+# BibMon
+
+`BibMon` (from the Portuguese ***Bib**lioteca de **Mon**itoramento de Processos*, or Process Monitoring Library) is a Python package that provides deviation-based predictive models for fault detection, soft sensing, and process condition monitoring.
+
+Installation
+----------------------
+
+`BibMon` can be installed using `pip`:
+
+    pip install bibmon
+
+Available Models
+----------------------
+
+* PCA (Principal Component Analysis);
+* any regressor that uses the `scikit-learn` interface.
+
+Usage
+----------------------
+
+Essentially, the library is used in two steps:
+
+1. In the training step, a model is generated that captures the relationships between variables in the normal process condition;
+2. In the prediction step, process data is compared to the model's predictions, resulting in deviations; if these deviations exceed a predefined limit, alarms are triggered.
+
+Specifically, the implemented control charts are based on squared prediction error (SPE).
+
+The examples in the `notebooks/` directory demonstrate the main functionalities of `BibMon`. The API reference can be generated using the Sphynx package from the files in the `docs/` directory.
+
+Features
+----------------------
+
+The resources offered by `BibMon` are:
+
+* Application in online systems: a trained `BibMon` model can be used for online analysis with both individual samples and data windows. For each sample or window, a prediction is made, the model state is updated, and alarms are calculated.
+* Compatibility, within the same architecture, of regression models (i.e., virtual sensors, containing separate X and Y data, such as RandomForest) and reconstruction models (containing only X data, such as PCA).
+* Preprocessing pipelines that take into account the differences between X and Y data and between training and testing stages.
+* Possibility of programming different alarm logics.
+* Easy extensibility through inheritance (there is a class called `GenericModel` that implements all the common functionality for various models and can be used as a base for implementing new models). For details, consult the `CONTRIBUTING.md` file.
+* Convenience functions for performing automatic offline analysis and plotting control charts.
+* Real and simulated process datasets available for importing.
+* Comparative tables to automate the performance analysis of different models.
+* Automatic hyperparameter tuning.
+
+Contributing
+----------------------
+
+BibMon is an open-source project driven by the community. If you would like to contribute to the project, please refer to the [CONTRIBUTING.md](https://github.com/petrobras/bibmon/blob/main/CONTRIBUTING.md) file.
+
 The package originated from research projects conducted in collaboration between the Chemical Engineering Program at COPPE/UFRJ and the Leopoldo Américo Miguez de Mello Research Center (CENPES/Petrobras).
```

### Comparing `bibmon-1.0.0/bibmon/__init__.py` & `bibmon-1.0.1/bibmon/__init__.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from ._pca import PCA
-from ._sklearn_regressor import sklearnRegressor
-from ._preprocess import PreProcess
-from ._load_data import load_tennessee_eastman, load_real_data
-from ._bibmon_tools import train_val_test_split, complete_analysis, comparative_table, spearmanr_dendrogram, create_df_with_dates, create_df_with_noise, align_dfs_by_rows
-
-__all__ = ['PCA','sklearnRegressor', 'PreProcess',
-           'load_tennessee_eastman', 'load_real_data', 
-           'train_val_test_split', 'complete_analysis', 'comparative_table',
-	       'spearmanr_dendrogram', 'create_df_with_dates',
+from ._pca import PCA
+from ._sklearn_regressor import sklearnRegressor
+from ._preprocess import PreProcess
+from ._load_data import load_tennessee_eastman, load_real_data
+from ._bibmon_tools import train_val_test_split, complete_analysis, comparative_table, spearmanr_dendrogram, create_df_with_dates, create_df_with_noise, align_dfs_by_rows
+
+__all__ = ['PCA','sklearnRegressor', 'PreProcess',
+           'load_tennessee_eastman', 'load_real_data', 
+           'train_val_test_split', 'complete_analysis', 'comparative_table',
+	       'spearmanr_dendrogram', 'create_df_with_dates',
            'create_df_with_noise', 'align_dfs_by_rows']
```

### Comparing `bibmon-1.0.0/bibmon/_alarms.py` & `bibmon-1.0.1/bibmon/_alarms.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-import numpy as np
-
-###############################################################################
-
-def detecOutlier(data, lim, count = False, count_limit = 1):
-    """
-    Detects outliers in the given data using a specified limit.
-
-    Parameters
-    ----------
-    data: array-like
-        The input data to be analyzed.
-    lim: float
-        The limit value used to detect outliers.
-    count: bool, optional
-        If True, counts the number of outliers 
-        exceeding the limit. Default is False.
-    count_limit: int, optional
-        The maximum number of outliers allowed. 
-        Default is 1.
-
-    Returns
-    ----------
-    alarm: ndarray or int
-        If count is False, returns an array indicating 
-        the outliers (0 for values below or equal to lim,
-        1 for values above lim).
-        If count is True, returns the number of outliers 
-        exceeding the limit.
-    """
-
-    if np.isnan(data).any():
-        data = np.nan_to_num(data)
-
-    if count == False:
-        alarm = np.copy(data)
-        alarm = np.where(alarm<=lim, 0, alarm)
-        alarm = np.where(alarm>lim, 1, alarm)
-        return alarm
-    else:
-        alarm = 0
-        local_count = np.count_nonzero(data > lim)
-        if local_count > count_limit:
-            alarm = +1
-        return alarm
-        
+import numpy as np
+
+###############################################################################
+
+def detecOutlier(data, lim, count = False, count_limit = 1):
+    """
+    Detects outliers in the given data using a specified limit.
+
+    Parameters
+    ----------
+    data: array-like
+        The input data to be analyzed.
+    lim: float
+        The limit value used to detect outliers.
+    count: bool, optional
+        If True, counts the number of outliers 
+        exceeding the limit. Default is False.
+    count_limit: int, optional
+        The maximum number of outliers allowed. 
+        Default is 1.
+
+    Returns
+    ----------
+    alarm: ndarray or int
+        If count is False, returns an array indicating 
+        the outliers (0 for values below or equal to lim,
+        1 for values above lim).
+        If count is True, returns the number of outliers 
+        exceeding the limit.
+    """
+
+    if np.isnan(data).any():
+        data = np.nan_to_num(data)
+
+    if count == False:
+        alarm = np.copy(data)
+        alarm = np.where(alarm<=lim, 0, alarm)
+        alarm = np.where(alarm>lim, 1, alarm)
+        return alarm
+    else:
+        alarm = 0
+        local_count = np.count_nonzero(data > lim)
+        if local_count > count_limit:
+            alarm = +1
+        return alarm
+
```

### Comparing `bibmon-1.0.0/bibmon/_bibmon_tools.py` & `bibmon-1.0.1/bibmon/_bibmon_tools.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,695 +1,695 @@
-import numpy as np
-import pandas as pd
-from datetime import datetime
-import matplotlib.pyplot as plt
-
-###############################################################################
-
-def create_df_with_dates (array, 
-                          start = '2020-01-01 00:00:00', 
-                          freq = '1min'):
-    """
-    Parameters
-    ----------
-    array: pandas.DataFrame or numpy.array
-        Original data.
-    start: string, optional
-        Start timestamp.
-    freq: string, optional
-        Sampling interval.
-    Returns
-    ----------                
-    df: pandas.DataFrame
-        Processed data.
-    """    
-    df = pd.DataFrame(array)
-    df.index = pd.date_range(start = start, 
-                             periods = df.shape[0],
-                             freq=freq)
-    return df
-
-###############################################################################
-
-def create_df_with_noise (array, 
-                          noise_frac, 
-                          max_index_for_noise):
-    """
-    Adds artificial measurement noise to data.
-    
-    Parameters
-    ----------
-    array: pandas.DataFrame or numpy.array
-        Original data.
-    noise_frac: float 
-        Fraction (between 0 and 1) of the total amplitude of the variable
-        that will be used as the noise standard deviation.
-    max_index_for_noise: int
-        Maximum index to consider the amplitude 
-        in the standard deviation calculation.
-    Returns
-    ----------                
-    df: pandas.DataFrame
-        Processed data.
-    """    
-
-    df = pd.DataFrame(array)
-
-    sigma_noise = noise_frac*(np.amax(array[:max_index_for_noise,:], 
-                                      axis=0)-
-                              np.amin(array[:max_index_for_noise,:], 
-                                      axis=0))
-
-    for i in range(df.shape[1]):
-        df.iloc[:,i] = (df.iloc[:,i] + 
-                        sigma_noise[i]*np.random.randn(df.shape[0]))
-        
-    return df
-    
-###############################################################################
-
-def align_dfs_by_rows (df1, df2):
-    """
-    Aligns DataFrames by rows.
-
-    Parameters
-    ----------
-    df1, df2: pandas.DataFrame
-        Original data.
-    Returns
-    ----------                
-    new_df1, new_df2: pandas.DataFrame
-        Processed data.
-    """
-    
-    new_df1 = df1.loc[df1.index.isin(df2.index)]
-    new_df2 = df2.loc[df2.index.isin(df1.index)]
-
-    return new_df1, new_df2
-
-###############################################################################
-
-def spearmanr_dendrogram(df, figsize = (18,8)):
-    """
-    Generates a dendrogram of Spearman correlations.
-    
-    Parameters
-    ----------
-    df: pandas.DataFrame
-        Dados to be analyzed.
-    figsize: tuple of ints, optional
-        Figure dimensions.
-    """   
-    import scipy.cluster.hierarchy
-    import scipy.stats
-    
-    df = pd.DataFrame(df)
-    
-    corr = np.round(scipy.stats.spearmanr(df).correlation, 4)
-    corr_condensed = scipy.cluster.hierarchy.distance.squareform(1-corr)
-    z = scipy.cluster.hierarchy.linkage(corr_condensed, method='average')
-    plt.figure(figsize=figsize)
-    scipy.cluster.hierarchy.dendrogram(z, labels = df.columns.tolist(), 
-                                       orientation='left', leaf_font_size=16)
-    plt.xlabel('Spearman Correlation')
-    plt.ylabel('Variable clusters')
-    plt.show()
-
-###############################################################################
-
-def train_val_test_split (data, start_train, end_train, 
-                          end_validation, end_test, 
-                          tags_X = None, tags_Y = None):
-    """
-    Separates the data into consecutive portions of 
-    train, validation, and test, returning 3 DataFrames.
-    It can also separate into predictor variables (X) and 
-    predicted variables (Y), which in this case will return 6 DataFrames.
-        
-    Parameters
-    ----------
-    data: pandas.DataFrame
-        Data to be separated.
-    start_train: string
-        Start timestamp of the train portion.
-    end_train: string
-        End timestamp of the train portion.
-    end_validation: string
-        End timestamp of the validation portion.
-    end_test: string
-        End timestamp of the test portion.
-    tags_X: list of strings
-        Variables to be considered in the X set.
-    tags_Y: list of strings
-        Variables to be considered in the Y set.
-    Returns
-    ----------                
-    : pandas.DataFrames
-        Separated data.
-    """               
-    train_data = data.loc[start_train:end_train]
-    validation_data = data.loc[end_train:end_validation].iloc[1:,:]
-    test_data = data.loc[end_validation:end_test].iloc[1:,:]
-
-    if tags_Y is not None:
-
-        if not isinstance(tags_Y, list): tags_Y = [tags_Y]
-        
-        train_data_Y = train_data.loc[:,tags_Y]
-        validation_data_Y = validation_data.loc[:,tags_Y]
-        test_data_Y = test_data.loc[:,tags_Y]
-
-        if tags_X is not None:
-
-            if not isinstance(tags_X, list): tags_X = [tags_X]
-            
-            train_data_X = train_data.loc[:,tags_X]
-            validation_data_X = validation_data.loc[:,tags_X]
-            test_data_X = test_data.loc[:,tags_X]
-
-        else:
-
-            dif = train_data.columns.difference(train_data_Y.columns)
-            train_data_X = train_data[dif]
-            validation_data_X = validation_data[dif]
-            test_data_X = test_data[dif]
-            
-        return (train_data_X, validation_data_X, test_data_X, 
-                train_data_Y, validation_data_Y, test_data_Y)
-            
-    else:
-        
-        if tags_X is not None:
-
-            if not isinstance(tags_X, list): tags_Y = [tags_X]
-            
-            train_data = train_data.loc[:,tags_X]
-            validation_data = validation_data.loc[:,tags_X]
-            test_data = test_data.loc[:,tags_X]           
-            
-        return (train_data, validation_data, test_data)
-            
-###############################################################################
-
-def complete_analysis (model, X_train, X_validation, X_test, 
-                       Y_train = None , Y_validation = None, Y_test = None,
-                       lim_conf = 0.99,
-                       f_pp_train = ['remove_empty_variables',
-                                     'ffill_nan',
-                                     'remove_frozen_variables',
-                                     'normalize'],
-                       a_pp_train = None,
-                       f_pp_test = ['replace_nan_with_values',
-                                    'normalize'],
-                       a_pp_test = None,
-                       logy = True, 
-                       metrics = None, 
-                       X_pred_to_plot = None,
-                       count_limit = 1,
-                       count_window_size = 0,
-                       fault_start = None,
-                       fault_end = None):
-    """
-    Performs a complete monitoring analysis, with train, validation, and test.
-
-    Parameters
-    ----------
-    model: BibMon model
-        Model to be considered in the analysis.
-    X_train: pandas.DataFrame or numpy.array
-        Training data X.
-    X_validation: pandas.DataFrame or numpy.array
-        Validation data X.
-    X_test: pandas.DataFrame or numpy.array
-        Test data X.
-    Y_train: pandas.DataFrame or numpy.array, optional
-        Training data Y.
-    Y_validation: pandas.DataFrame or numpy.array, optional
-        Validation data Y.
-    Y_test: pandas.DataFrame or numpy.array, optional
-        Test data Y.
-    lim_conf: float, optional
-        Confidence limit for the detection index.
-    f_pp_train: list, optional
-        List containing strings with names of functions to be used 
-        in pre-processing the train data (the functions are defined in the 
-        PreProcess class, in the BibMon_Tools.py file).
-    a_pp_train: dict, optional
-        Dictionary containing the parameters to be provided
-        to each function to perform pre-processing of the train data, in
-        the format {'functionname__argname': argvalue, ...}.
-    f_pp_test: list, optional
-        List containing strings with names of functions to be used 
-        in pre-processing the test data (the functions are defined in the 
-        PreProcess class, in the BibMon_Tools.py file).
-    a_pp_test: dict, optional
-        Dictionary containing the parameters to be provided
-        to each function to perform pre-processing of the test data, in
-        the format {'functionname__argname': argvalue, ...}.
-    logy: boolean, optional
-        If use logarithmic scale in the SPE plots.
-    metrics: list of functions, optional
-        Functions for calculating metrics to be displayed in the title of 
-        the graph.
-    X_pred_to_plot: string, optional
-        In case the model is a reconstruction model (i.e., self.has_Y = False),
-        indicates which column of X to plot along with the prediction.
-    count_limit: int, optional
-        Limit of points to be considered in the window 
-        for the count alarm to sound.
-    count_window_size: int, optional
-        Window sizes used in count alarm calculation. 
-    fault_start: string, optional
-        Start timestamp of the fault.
-    fault_end: string, optional
-        End timestamp of the fault.
-    """               
-    fig, ax = plt.subplots(3,2, figsize = (15,12))
-
-    cond_to_plot_pred = (model.has_Y or 
-                        ((not model.has_Y) and (X_pred_to_plot is not None)))
-
-    ######## TRAINING ########
-
-    model.fit(X_train, Y_train, 
-              f_pp = f_pp_train,
-              a_pp = a_pp_train,
-              f_pp_test = f_pp_test,
-              a_pp_test = a_pp_test,
-              lim_conf = lim_conf,
-              redefine_limit = False)
-                                
-    # PLOTTING SPE
-                
-    model.plot_SPE(ax = ax[0,0], logy = logy)
-    ax[0,0].set_title('Training')
-
-    # PLOTTING PREDICTIONS
-
-    if cond_to_plot_pred:
-        model.plot_predictions(ax = ax[0,1], train_or_test = 'train', 
-                               X_pred_to_plot = X_pred_to_plot,
-                               metrics = metrics)
-
-    ######## VALIDATION ########
-
-    model.predict(X_validation, Y_validation, 
-                  count_window_size = count_window_size, 
-                  redefine_limit = True)
-
-    # PLOTTING SPE
-
-    model.plot_SPE(ax = ax[1,0], train_or_test = 'test', logy = logy)
-    ax[1,0].set_title('Validation')
-
-    # PLOTTING PREDICTIONS
-
-    if cond_to_plot_pred:
-        model.plot_predictions(ax = ax[1,1], train_or_test = 'test', 
-                               X_pred_to_plot = X_pred_to_plot, 
-                               metrics = metrics)
-        
-    ######## TEST ########
-        
-    model.predict(X_test, Y_test, 
-                  count_window_size = count_window_size, 
-                  count_limit = count_limit,
-                  redefine_limit = False)
-
-    # PLOTTING SPE
-
-    model.plot_SPE(ax = ax[2,0], train_or_test = 'test', logy = logy)
-    ax[2,0].set_title('Test')
-
-    if fault_start is not None:
-        ax[2,0].axvline(datetime.strptime(str(fault_start),
-                                          '%Y-%m-%d %H:%M:%S'), ls = '--')
-    if fault_end is not None:
-        ax[2,0].axvline(datetime.strptime(str(fault_end),
-                                          '%Y-%m-%d %H:%M:%S'), ls = '--')
-
-    # PLOTTING PREDICTIONS
-
-    if cond_to_plot_pred:
-        model.plot_predictions(ax = ax[2,1], train_or_test = 'test', 
-                               X_pred_to_plot = X_pred_to_plot,
-                               metrics = metrics)
-
-        if fault_start is not None:
-            ax[2,1].axvline(datetime.strptime(str(fault_start),
-                                              '%Y-%m-%d %H:%M:%S'), ls = '--')
-        if fault_end is not None:
-            ax[2,1].axvline(datetime.strptime(str(fault_end),
-                                              '%Y-%m-%d %H:%M:%S'), ls = '--')
-        
-    fig.tight_layout();
-            
-##############################################################################
-
-def comparative_table (models, X_train, X_validation, X_test, 
-                       Y_train = None , Y_validation = None, Y_test = None,
-                       lim_conf = 0.99,
-                       f_pp_train = ['remove_empty_variables',
-                                     'ffill_nan',
-                                     'remove_frozen_variables',
-                                     'normalize'],
-                       a_pp_train = None,
-                       f_pp_test = ['replace_nan_with_values',
-                                    'normalize'],
-                       a_pp_test = None,
-                       logy = True, metrics = None,
-                       X_pred_to_plot = None,
-                       count_limit = 1,
-                       count_window_size = 0,
-                       fault_start = None,
-                       fault_end = None,
-                       mask = None,
-                       times = True,
-                       plot_SPE = True,
-                       plot_predictions = True,
-                       fit_model = True):
-
-    """
-    Performs complete monitoring analysis of multiple models and builds
-    comparative result tables.
-
-    Parameters
-    ----------
-    models: list of BibMon models
-        Models to be considered in the analysis.
-    X_train: pandas.DataFrame or numpy.array
-        Training data X.
-    X_validation: pandas.DataFrame or numpy.array
-        Validation data X.
-    X_test: pandas.DataFrame or numpy.array
-        Test data X.
-    Y_train: pandas.DataFrame or numpy.array, optional
-        Training data Y.
-    Y_validation: pandas.DataFrame or numpy.array, optional
-        Validation data Y.
-    Y_test: pandas.DataFrame or numpy.array, optional
-        Test data Y.
-    lim_conf: float, optional
-        Confidence limit for the detection index.
-    f_pp_train: list, optional
-        List containing strings with names of functions to be used 
-        in pre-processing the train data (the functions are defined in the 
-        PreProcess class, in the BibMon_Tools.py file).
-    a_pp_train: dict, optional
-        Dictionary containing the parameters to be provided
-        to each function to perform pre-processing of the train data, in
-        the format {'functionname__argname': argvalue, ...}.
-    f_pp_test: list, optional
-        List containing strings with names of functions to be used 
-        in pre-processing the test data (the functions are defined in the 
-        PreProcess class, in the BibMon_Tools.py file).
-    a_pp_test: dict, optional
-        Dictionary containing the parameters to be provided
-        to each function to perform pre-processing of the test data, in
-        the format {'functionname__argname': argvalue, ...}.
-    logy: boolean, optional
-        If use logarithmic scale in the SPE plots.
-    metrics: list of functions, optional
-        Functions for calculating metrics to be displayed in the title of 
-        the graph.
-    X_pred_to_plot: string, optional
-        In case the model is a reconstruction model (i.e., self.has_Y = False),
-        indicates which column of X to plot along with the prediction.
-    count_limit: int, optional
-        Limit of points to be considered in the window 
-        for the count alarm to sound.
-    count_window_size: int, optional
-        Window sizes used in count alarm calculation.
-    fault_start: string, optional
-        Start timestamp of the fault.
-    fault_end: string, optional
-        End timestamp of the fault.
-    mask: numpy.array, optional
-        Boolean array indicating the indices where the process is
-        in fault.
-    times: boolean, optional
-        If execution times should be calculated.
-    plot_SPE: boolean, optional
-        If SPE plots should be plotted.
-    plot_predictions: boolean, optional
-        If prediction plots should be plotted.
-    fit_model: boolean, optional
-        If models should be trained.
-    Returns
-    ----------
-    : list of pandas.DataFrames
-        List with the generated tables (prediction and/or detection).
-    """
-    
-    n = len(models)
-
-    if plot_SPE:
-        fig_spe, ax_spe = plt.subplots(n, 3, figsize = (15, 4*n))
-
-    if plot_predictions:
-        fig_pred, ax_pred = plt.subplots(n, 3, figsize = (15, 4*n))
-        
-    train_metrics = {}     
-    validation_metrics = {}        
-    test_metrics = {}        
-
-    detection_alarms = {}
-    false_detection_rates = {}
-    false_alarm_rates = {}
-
-    for i in range(len(models)):
-        
-        model = models[i]
-        
-        cond_to_plot_pred = (model.has_Y or 
-                            ((not model.has_Y) and 
-                            (X_pred_to_plot is not None)))
-
-        ######## TRAINING ########
-        
-        if fit_model:
-            model.fit(X_train, Y_train, 
-                      f_pp = f_pp_train,
-                      a_pp = a_pp_train, 
-                      f_pp_test = f_pp_test,
-                      a_pp_test = a_pp_test,
-                      lim_conf = lim_conf,
-                      redefine_limit = False)
-        
-        # TERMS FOR PREDICTION TABLE
-        
-        if metrics is not None:
-            if model.has_Y:
-                true = model.Y_train_orig
-                pred = model.Y_train_pred_orig
-            else:
-                if X_pred_to_plot is not None:
-                    true = model.X_train_orig[X_pred_to_plot]
-                    pred = model.X_train_pred_orig[X_pred_to_plot]                
-            for mr in metrics:
-                true, pred = align_dfs_by_rows(true.dropna(), pred)
-                train_metrics[model.name+': '+mr.__name__] = mr(true, pred)
-                                    
-        # PLOTTING SPE
-                
-        if plot_SPE:
-            model.plot_SPE(ax = ax_spe[i,0], logy = logy)
-            ax_spe[i,0].set_title('Training')
-
-        # PLOTTING PREDICTIONS
-            
-        if plot_predictions:
-            if cond_to_plot_pred:
-                model.plot_predictions(ax = ax_pred[i,0], 
-                                        train_or_test = 'train', 
-                                        X_pred_to_plot = X_pred_to_plot,
-                                        metrics = metrics)
-
-        ######## VALIDATION ########
-                
-        model.predict(X_validation, Y_validation, 
-                      count_window_size = count_window_size, 
-                      redefine_limit = True)
-
-        # TERMS FOR PREDICTION TABLE
-        
-        if metrics is not None:
-            if model.has_Y:
-                true = model.Y_test_orig
-                pred = model.Y_test_pred_orig
-            else:
-                if X_pred_to_plot is not None:
-                    true = model.X_test_orig[X_pred_to_plot]
-                    pred = model.X_test_pred_orig[X_pred_to_plot]                
-            for mr in metrics:
-                true, pred = align_dfs_by_rows(true.dropna(), pred)
-                validation_metrics[model.name+': '+mr.__name__]= mr(true, pred)
-
-        # PLOTTING SPE
-                
-        if plot_SPE:
-            model.plot_SPE(ax = ax_spe[i,1], train_or_test = 'test', 
-                           logy=logy)
-            ax_spe[i,1].set_title(model.name+'\n\nValidation')
-
-        # PLOTTING PREDICTIONS
-            
-        if plot_predictions:
-            if cond_to_plot_pred:
-                model.plot_predictions(ax = ax_pred[i,1], 
-                                       train_or_test = 'test', 
-                                       X_pred_to_plot = X_pred_to_plot, 
-                                       metrics = metrics)
-                ax_pred[i,1].set_title(model.name+'\n\n'+
-                                       ax_pred[i,1].get_title())
-                
-        ######## TEST ########
-                
-        model.predict(X_test, Y_test, 
-                      count_window_size = count_window_size, 
-                      count_limit = count_limit,
-                      redefine_limit = False)
-
-        # TERMS FOR PREDICTION TABLE
-        
-        if metrics is not None:
-            if model.has_Y:
-                true = model.Y_test_orig
-                pred = model.Y_test_pred_orig
-            else:
-                if X_pred_to_plot is not None:
-                    true = model.X_test_orig[X_pred_to_plot]
-                    pred = model.X_test_pred_orig[X_pred_to_plot]                
-            for mr in metrics:
-                true, pred = align_dfs_by_rows(true.dropna(), pred)
-                test_metrics[model.name+': '+mr.__name__] =  mr(true, pred)
-
-        # TERMS FOR DETECTION TABLE
-        
-        if mask is None:
-            if fault_start is not None:            
-                for key, value in model.alarms.items():
-                    if fault_end is not None:
-                        detection_alarms[model.name+': '+key] = \
-                            value[fault_start:fault_end][:-1].mean()
-                        false_detection_rates[model.name+': '+key] = \
-                            pd.concat([value[:fault_start][:-1], 
-                                    value[fault_end:]]).mean()
-                    else:
-                        detection_alarms[model.name+': '+key] = \
-                            value[fault_start:fault_end].mean()
-                        false_detection_rates[model.name+': '+key] = \
-                            value[:fault_start][:-1].mean()
-        else:
-            for key, value in model.alarms.items():
-                detection_alarms[model.name+': '+key] = \
-                    mask[mask==1].eq(value[value==1]).astype(int).mean()
-                false_detection_rates[model.name+': '+key] = \
-                    1-mask[mask==0].eq(value[value==0]).astype(int).mean()
-
-        # PLOTTING SPE
-                
-        if plot_SPE:
-
-            model.plot_SPE(ax = ax_spe[i,2], train_or_test='test',
-                           logy = logy)
-            ax_spe[i,2].set_title('Test')
-            
-            if fault_start is not None:
-                ax_spe[i,2].axvline(datetime.strptime(str(fault_start),
-                                                      '%Y-%m-%d %H:%M:%S'), 
-                                                      ls='--')
-            if fault_end is not None:
-                ax_spe[i,2].axvline(datetime.strptime(str(fault_end),
-                                                      '%Y-%m-%d %H:%M:%S'), 
-                                                      ls='--')
-
-        # PLOTTING PREDICTIONS
-                
-        if plot_predictions:
-            if cond_to_plot_pred:
-                model.plot_predictions(ax = ax_pred[i,2], 
-                                        train_or_test = 'test', 
-                                        X_pred_to_plot = X_pred_to_plot,
-                                        metrics = metrics)
-                if fault_start is not None:
-                    ax_pred[i,2].axvline(datetime.strptime(str(fault_start),
-                                                 '%Y-%m-%d %H:%M:%S'), ls='--')
-                if fault_end is not None:
-                    ax_pred[i,2].axvline(datetime.strptime(str(fault_end),
-                                                 '%Y-%m-%d %H:%M:%S'), ls='--')
-
-        if plot_SPE:            
-            fig_spe.tight_layout();
-        if plot_predictions:
-            fig_pred.tight_layout();
-            
-    ######## GENERATING FINAL TABLES ########
-        
-    return_tables = []
-        
-    # PREDICTION
-
-    if metrics is not None:
-
-        prediction_table = pd.DataFrame([train_metrics, validation_metrics,
-                                         test_metrics], 
-                                        index = ['Train',
-                                                 'Validation',
-                                                 'Test']).T
-                                                            
-        models_names = [models[i].name for i in range(len(models))]
-        metrics_names = [metrics[i].__name__ for i in range(len(metrics))]
-        
-        iterables = [models_names, metrics_names]
-
-        index = pd.MultiIndex.from_product(iterables, 
-                                           names = ['Models', 'Metrics'])
-        
-        message = ("The MultiIndex table is not of the right size. "+
-                   "This could happen when two models have the same name.")
-        
-        try:
-            prediction_table.index = index
-        except ValueError as err:
-            raise ValueError(message) from err
-        
-        return_tables.append(prediction_table.swaplevel().sort_index(axis=0))
-
-    # DETECTION     
-        
-    if fault_start is not None:
-        
-        detection_table = pd.DataFrame([detection_alarms, 
-                                        false_detection_rates],
-                                       index = ['FDR','FAR']).T
-        
-        models_names = [models[i].name for i in range(len(models))]
-        alarms_names = [list(model.alarms.keys())[i] for i in 
-                range(len(list(model.alarms.keys())))]  
-        
-        iterables = [models_names, alarms_names]
-
-        index = pd.MultiIndex.from_product(iterables, 
-                                        names = ['Models', 'Alarms'])
-        
-        detection_table.index = index
-
-        return_tables.append(detection_table.swaplevel().sort_index(axis=0))
-        
-    # COMPUTATIONAL TIMES
-        
-    if times:
-        
-        times_dict = {}
-        
-        times_dict['Train'] = [1e6*models[i].train_time/X_train.shape[0]
-                        for i in range(len(models))]
-        times_dict['Test'] = [1e6*models[i].test_time/X_test.shape[0] 
-                        for i in range(len(models))]
-        
-        times_df = pd.DataFrame(times_dict, 
-                        index=[models[i].name for i in range(len(models))])
-        
-        return_tables.append(times_df)
-        
+import numpy as np
+import pandas as pd
+from datetime import datetime
+import matplotlib.pyplot as plt
+
+###############################################################################
+
+def create_df_with_dates (array, 
+                          start = '2020-01-01 00:00:00', 
+                          freq = '1min'):
+    """
+    Parameters
+    ----------
+    array: pandas.DataFrame or numpy.array
+        Original data.
+    start: string, optional
+        Start timestamp.
+    freq: string, optional
+        Sampling interval.
+    Returns
+    ----------                
+    df: pandas.DataFrame
+        Processed data.
+    """    
+    df = pd.DataFrame(array)
+    df.index = pd.date_range(start = start, 
+                             periods = df.shape[0],
+                             freq=freq)
+    return df
+
+###############################################################################
+
+def create_df_with_noise (array, 
+                          noise_frac, 
+                          max_index_for_noise):
+    """
+    Adds artificial measurement noise to data.
+    
+    Parameters
+    ----------
+    array: pandas.DataFrame or numpy.array
+        Original data.
+    noise_frac: float 
+        Fraction (between 0 and 1) of the total amplitude of the variable
+        that will be used as the noise standard deviation.
+    max_index_for_noise: int
+        Maximum index to consider the amplitude 
+        in the standard deviation calculation.
+    Returns
+    ----------                
+    df: pandas.DataFrame
+        Processed data.
+    """    
+
+    df = pd.DataFrame(array)
+
+    sigma_noise = noise_frac*(np.amax(array[:max_index_for_noise,:], 
+                                      axis=0)-
+                              np.amin(array[:max_index_for_noise,:], 
+                                      axis=0))
+
+    for i in range(df.shape[1]):
+        df.iloc[:,i] = (df.iloc[:,i] + 
+                        sigma_noise[i]*np.random.randn(df.shape[0]))
+        
+    return df
+    
+###############################################################################
+
+def align_dfs_by_rows (df1, df2):
+    """
+    Aligns DataFrames by rows.
+
+    Parameters
+    ----------
+    df1, df2: pandas.DataFrame
+        Original data.
+    Returns
+    ----------                
+    new_df1, new_df2: pandas.DataFrame
+        Processed data.
+    """
+    
+    new_df1 = df1.loc[df1.index.isin(df2.index)]
+    new_df2 = df2.loc[df2.index.isin(df1.index)]
+
+    return new_df1, new_df2
+
+###############################################################################
+
+def spearmanr_dendrogram(df, figsize = (18,8)):
+    """
+    Generates a dendrogram of Spearman correlations.
+    
+    Parameters
+    ----------
+    df: pandas.DataFrame
+        Dados to be analyzed.
+    figsize: tuple of ints, optional
+        Figure dimensions.
+    """   
+    import scipy.cluster.hierarchy
+    import scipy.stats
+    
+    df = pd.DataFrame(df)
+    
+    corr = np.round(scipy.stats.spearmanr(df).correlation, 4)
+    corr_condensed = scipy.cluster.hierarchy.distance.squareform(1-corr)
+    z = scipy.cluster.hierarchy.linkage(corr_condensed, method='average')
+    plt.figure(figsize=figsize)
+    scipy.cluster.hierarchy.dendrogram(z, labels = df.columns.tolist(), 
+                                       orientation='left', leaf_font_size=16)
+    plt.xlabel('Spearman Correlation')
+    plt.ylabel('Variable clusters')
+    plt.show()
+
+###############################################################################
+
+def train_val_test_split (data, start_train, end_train, 
+                          end_validation, end_test, 
+                          tags_X = None, tags_Y = None):
+    """
+    Separates the data into consecutive portions of 
+    train, validation, and test, returning 3 DataFrames.
+    It can also separate into predictor variables (X) and 
+    predicted variables (Y), which in this case will return 6 DataFrames.
+        
+    Parameters
+    ----------
+    data: pandas.DataFrame
+        Data to be separated.
+    start_train: string
+        Start timestamp of the train portion.
+    end_train: string
+        End timestamp of the train portion.
+    end_validation: string
+        End timestamp of the validation portion.
+    end_test: string
+        End timestamp of the test portion.
+    tags_X: list of strings
+        Variables to be considered in the X set.
+    tags_Y: list of strings
+        Variables to be considered in the Y set.
+    Returns
+    ----------                
+    : pandas.DataFrames
+        Separated data.
+    """               
+    train_data = data.loc[start_train:end_train]
+    validation_data = data.loc[end_train:end_validation].iloc[1:,:]
+    test_data = data.loc[end_validation:end_test].iloc[1:,:]
+
+    if tags_Y is not None:
+
+        if not isinstance(tags_Y, list): tags_Y = [tags_Y]
+        
+        train_data_Y = train_data.loc[:,tags_Y]
+        validation_data_Y = validation_data.loc[:,tags_Y]
+        test_data_Y = test_data.loc[:,tags_Y]
+
+        if tags_X is not None:
+
+            if not isinstance(tags_X, list): tags_X = [tags_X]
+            
+            train_data_X = train_data.loc[:,tags_X]
+            validation_data_X = validation_data.loc[:,tags_X]
+            test_data_X = test_data.loc[:,tags_X]
+
+        else:
+
+            dif = train_data.columns.difference(train_data_Y.columns)
+            train_data_X = train_data[dif]
+            validation_data_X = validation_data[dif]
+            test_data_X = test_data[dif]
+            
+        return (train_data_X, validation_data_X, test_data_X, 
+                train_data_Y, validation_data_Y, test_data_Y)
+            
+    else:
+        
+        if tags_X is not None:
+
+            if not isinstance(tags_X, list): tags_Y = [tags_X]
+            
+            train_data = train_data.loc[:,tags_X]
+            validation_data = validation_data.loc[:,tags_X]
+            test_data = test_data.loc[:,tags_X]           
+            
+        return (train_data, validation_data, test_data)
+            
+###############################################################################
+
+def complete_analysis (model, X_train, X_validation, X_test, 
+                       Y_train = None , Y_validation = None, Y_test = None,
+                       lim_conf = 0.99,
+                       f_pp_train = ['remove_empty_variables',
+                                     'ffill_nan',
+                                     'remove_frozen_variables',
+                                     'normalize'],
+                       a_pp_train = None,
+                       f_pp_test = ['replace_nan_with_values',
+                                    'normalize'],
+                       a_pp_test = None,
+                       logy = True, 
+                       metrics = None, 
+                       X_pred_to_plot = None,
+                       count_limit = 1,
+                       count_window_size = 0,
+                       fault_start = None,
+                       fault_end = None):
+    """
+    Performs a complete monitoring analysis, with train, validation, and test.
+
+    Parameters
+    ----------
+    model: BibMon model
+        Model to be considered in the analysis.
+    X_train: pandas.DataFrame or numpy.array
+        Training data X.
+    X_validation: pandas.DataFrame or numpy.array
+        Validation data X.
+    X_test: pandas.DataFrame or numpy.array
+        Test data X.
+    Y_train: pandas.DataFrame or numpy.array, optional
+        Training data Y.
+    Y_validation: pandas.DataFrame or numpy.array, optional
+        Validation data Y.
+    Y_test: pandas.DataFrame or numpy.array, optional
+        Test data Y.
+    lim_conf: float, optional
+        Confidence limit for the detection index.
+    f_pp_train: list, optional
+        List containing strings with names of functions to be used 
+        in pre-processing the train data (the functions are defined in the 
+        PreProcess class, in the BibMon_Tools.py file).
+    a_pp_train: dict, optional
+        Dictionary containing the parameters to be provided
+        to each function to perform pre-processing of the train data, in
+        the format {'functionname__argname': argvalue, ...}.
+    f_pp_test: list, optional
+        List containing strings with names of functions to be used 
+        in pre-processing the test data (the functions are defined in the 
+        PreProcess class, in the BibMon_Tools.py file).
+    a_pp_test: dict, optional
+        Dictionary containing the parameters to be provided
+        to each function to perform pre-processing of the test data, in
+        the format {'functionname__argname': argvalue, ...}.
+    logy: boolean, optional
+        If use logarithmic scale in the SPE plots.
+    metrics: list of functions, optional
+        Functions for calculating metrics to be displayed in the title of 
+        the graph.
+    X_pred_to_plot: string, optional
+        In case the model is a reconstruction model (i.e., self.has_Y = False),
+        indicates which column of X to plot along with the prediction.
+    count_limit: int, optional
+        Limit of points to be considered in the window 
+        for the count alarm to sound.
+    count_window_size: int, optional
+        Window sizes used in count alarm calculation. 
+    fault_start: string, optional
+        Start timestamp of the fault.
+    fault_end: string, optional
+        End timestamp of the fault.
+    """               
+    fig, ax = plt.subplots(3,2, figsize = (15,12))
+
+    cond_to_plot_pred = (model.has_Y or 
+                        ((not model.has_Y) and (X_pred_to_plot is not None)))
+
+    ######## TRAINING ########
+
+    model.fit(X_train, Y_train, 
+              f_pp = f_pp_train,
+              a_pp = a_pp_train,
+              f_pp_test = f_pp_test,
+              a_pp_test = a_pp_test,
+              lim_conf = lim_conf,
+              redefine_limit = False)
+                                
+    # PLOTTING SPE
+                
+    model.plot_SPE(ax = ax[0,0], logy = logy)
+    ax[0,0].set_title('Training')
+
+    # PLOTTING PREDICTIONS
+
+    if cond_to_plot_pred:
+        model.plot_predictions(ax = ax[0,1], train_or_test = 'train', 
+                               X_pred_to_plot = X_pred_to_plot,
+                               metrics = metrics)
+
+    ######## VALIDATION ########
+
+    model.predict(X_validation, Y_validation, 
+                  count_window_size = count_window_size, 
+                  redefine_limit = True)
+
+    # PLOTTING SPE
+
+    model.plot_SPE(ax = ax[1,0], train_or_test = 'test', logy = logy)
+    ax[1,0].set_title('Validation')
+
+    # PLOTTING PREDICTIONS
+
+    if cond_to_plot_pred:
+        model.plot_predictions(ax = ax[1,1], train_or_test = 'test', 
+                               X_pred_to_plot = X_pred_to_plot, 
+                               metrics = metrics)
+        
+    ######## TEST ########
+        
+    model.predict(X_test, Y_test, 
+                  count_window_size = count_window_size, 
+                  count_limit = count_limit,
+                  redefine_limit = False)
+
+    # PLOTTING SPE
+
+    model.plot_SPE(ax = ax[2,0], train_or_test = 'test', logy = logy)
+    ax[2,0].set_title('Test')
+
+    if fault_start is not None:
+        ax[2,0].axvline(datetime.strptime(str(fault_start),
+                                          '%Y-%m-%d %H:%M:%S'), ls = '--')
+    if fault_end is not None:
+        ax[2,0].axvline(datetime.strptime(str(fault_end),
+                                          '%Y-%m-%d %H:%M:%S'), ls = '--')
+
+    # PLOTTING PREDICTIONS
+
+    if cond_to_plot_pred:
+        model.plot_predictions(ax = ax[2,1], train_or_test = 'test', 
+                               X_pred_to_plot = X_pred_to_plot,
+                               metrics = metrics)
+
+        if fault_start is not None:
+            ax[2,1].axvline(datetime.strptime(str(fault_start),
+                                              '%Y-%m-%d %H:%M:%S'), ls = '--')
+        if fault_end is not None:
+            ax[2,1].axvline(datetime.strptime(str(fault_end),
+                                              '%Y-%m-%d %H:%M:%S'), ls = '--')
+        
+    fig.tight_layout();
+            
+##############################################################################
+
+def comparative_table (models, X_train, X_validation, X_test, 
+                       Y_train = None , Y_validation = None, Y_test = None,
+                       lim_conf = 0.99,
+                       f_pp_train = ['remove_empty_variables',
+                                     'ffill_nan',
+                                     'remove_frozen_variables',
+                                     'normalize'],
+                       a_pp_train = None,
+                       f_pp_test = ['replace_nan_with_values',
+                                    'normalize'],
+                       a_pp_test = None,
+                       logy = True, metrics = None,
+                       X_pred_to_plot = None,
+                       count_limit = 1,
+                       count_window_size = 0,
+                       fault_start = None,
+                       fault_end = None,
+                       mask = None,
+                       times = True,
+                       plot_SPE = True,
+                       plot_predictions = True,
+                       fit_model = True):
+
+    """
+    Performs complete monitoring analysis of multiple models and builds
+    comparative result tables.
+
+    Parameters
+    ----------
+    models: list of BibMon models
+        Models to be considered in the analysis.
+    X_train: pandas.DataFrame or numpy.array
+        Training data X.
+    X_validation: pandas.DataFrame or numpy.array
+        Validation data X.
+    X_test: pandas.DataFrame or numpy.array
+        Test data X.
+    Y_train: pandas.DataFrame or numpy.array, optional
+        Training data Y.
+    Y_validation: pandas.DataFrame or numpy.array, optional
+        Validation data Y.
+    Y_test: pandas.DataFrame or numpy.array, optional
+        Test data Y.
+    lim_conf: float, optional
+        Confidence limit for the detection index.
+    f_pp_train: list, optional
+        List containing strings with names of functions to be used 
+        in pre-processing the train data (the functions are defined in the 
+        PreProcess class, in the BibMon_Tools.py file).
+    a_pp_train: dict, optional
+        Dictionary containing the parameters to be provided
+        to each function to perform pre-processing of the train data, in
+        the format {'functionname__argname': argvalue, ...}.
+    f_pp_test: list, optional
+        List containing strings with names of functions to be used 
+        in pre-processing the test data (the functions are defined in the 
+        PreProcess class, in the BibMon_Tools.py file).
+    a_pp_test: dict, optional
+        Dictionary containing the parameters to be provided
+        to each function to perform pre-processing of the test data, in
+        the format {'functionname__argname': argvalue, ...}.
+    logy: boolean, optional
+        If use logarithmic scale in the SPE plots.
+    metrics: list of functions, optional
+        Functions for calculating metrics to be displayed in the title of 
+        the graph.
+    X_pred_to_plot: string, optional
+        In case the model is a reconstruction model (i.e., self.has_Y = False),
+        indicates which column of X to plot along with the prediction.
+    count_limit: int, optional
+        Limit of points to be considered in the window 
+        for the count alarm to sound.
+    count_window_size: int, optional
+        Window sizes used in count alarm calculation.
+    fault_start: string, optional
+        Start timestamp of the fault.
+    fault_end: string, optional
+        End timestamp of the fault.
+    mask: numpy.array, optional
+        Boolean array indicating the indices where the process is
+        in fault.
+    times: boolean, optional
+        If execution times should be calculated.
+    plot_SPE: boolean, optional
+        If SPE plots should be plotted.
+    plot_predictions: boolean, optional
+        If prediction plots should be plotted.
+    fit_model: boolean, optional
+        If models should be trained.
+    Returns
+    ----------
+    : list of pandas.DataFrames
+        List with the generated tables (prediction and/or detection).
+    """
+    
+    n = len(models)
+
+    if plot_SPE:
+        fig_spe, ax_spe = plt.subplots(n, 3, figsize = (15, 4*n))
+
+    if plot_predictions:
+        fig_pred, ax_pred = plt.subplots(n, 3, figsize = (15, 4*n))
+        
+    train_metrics = {}     
+    validation_metrics = {}        
+    test_metrics = {}        
+
+    detection_alarms = {}
+    false_detection_rates = {}
+    false_alarm_rates = {}
+
+    for i in range(len(models)):
+        
+        model = models[i]
+        
+        cond_to_plot_pred = (model.has_Y or 
+                            ((not model.has_Y) and 
+                            (X_pred_to_plot is not None)))
+
+        ######## TRAINING ########
+        
+        if fit_model:
+            model.fit(X_train, Y_train, 
+                      f_pp = f_pp_train,
+                      a_pp = a_pp_train, 
+                      f_pp_test = f_pp_test,
+                      a_pp_test = a_pp_test,
+                      lim_conf = lim_conf,
+                      redefine_limit = False)
+        
+        # TERMS FOR PREDICTION TABLE
+        
+        if metrics is not None:
+            if model.has_Y:
+                true = model.Y_train_orig
+                pred = model.Y_train_pred_orig
+            else:
+                if X_pred_to_plot is not None:
+                    true = model.X_train_orig[X_pred_to_plot]
+                    pred = model.X_train_pred_orig[X_pred_to_plot]                
+            for mr in metrics:
+                true, pred = align_dfs_by_rows(true.dropna(), pred)
+                train_metrics[model.name+': '+mr.__name__] = mr(true, pred)
+                                    
+        # PLOTTING SPE
+                
+        if plot_SPE:
+            model.plot_SPE(ax = ax_spe[i,0], logy = logy)
+            ax_spe[i,0].set_title('Training')
+
+        # PLOTTING PREDICTIONS
+            
+        if plot_predictions:
+            if cond_to_plot_pred:
+                model.plot_predictions(ax = ax_pred[i,0], 
+                                        train_or_test = 'train', 
+                                        X_pred_to_plot = X_pred_to_plot,
+                                        metrics = metrics)
+
+        ######## VALIDATION ########
+                
+        model.predict(X_validation, Y_validation, 
+                      count_window_size = count_window_size, 
+                      redefine_limit = True)
+
+        # TERMS FOR PREDICTION TABLE
+        
+        if metrics is not None:
+            if model.has_Y:
+                true = model.Y_test_orig
+                pred = model.Y_test_pred_orig
+            else:
+                if X_pred_to_plot is not None:
+                    true = model.X_test_orig[X_pred_to_plot]
+                    pred = model.X_test_pred_orig[X_pred_to_plot]                
+            for mr in metrics:
+                true, pred = align_dfs_by_rows(true.dropna(), pred)
+                validation_metrics[model.name+': '+mr.__name__]= mr(true, pred)
+
+        # PLOTTING SPE
+                
+        if plot_SPE:
+            model.plot_SPE(ax = ax_spe[i,1], train_or_test = 'test', 
+                           logy=logy)
+            ax_spe[i,1].set_title(model.name+'\n\nValidation')
+
+        # PLOTTING PREDICTIONS
+            
+        if plot_predictions:
+            if cond_to_plot_pred:
+                model.plot_predictions(ax = ax_pred[i,1], 
+                                       train_or_test = 'test', 
+                                       X_pred_to_plot = X_pred_to_plot, 
+                                       metrics = metrics)
+                ax_pred[i,1].set_title(model.name+'\n\n'+
+                                       ax_pred[i,1].get_title())
+                
+        ######## TEST ########
+                
+        model.predict(X_test, Y_test, 
+                      count_window_size = count_window_size, 
+                      count_limit = count_limit,
+                      redefine_limit = False)
+
+        # TERMS FOR PREDICTION TABLE
+        
+        if metrics is not None:
+            if model.has_Y:
+                true = model.Y_test_orig
+                pred = model.Y_test_pred_orig
+            else:
+                if X_pred_to_plot is not None:
+                    true = model.X_test_orig[X_pred_to_plot]
+                    pred = model.X_test_pred_orig[X_pred_to_plot]                
+            for mr in metrics:
+                true, pred = align_dfs_by_rows(true.dropna(), pred)
+                test_metrics[model.name+': '+mr.__name__] =  mr(true, pred)
+
+        # TERMS FOR DETECTION TABLE
+        
+        if mask is None:
+            if fault_start is not None:            
+                for key, value in model.alarms.items():
+                    if fault_end is not None:
+                        detection_alarms[model.name+': '+key] = \
+                            value[fault_start:fault_end][:-1].mean()
+                        false_detection_rates[model.name+': '+key] = \
+                            pd.concat([value[:fault_start][:-1], 
+                                    value[fault_end:]]).mean()
+                    else:
+                        detection_alarms[model.name+': '+key] = \
+                            value[fault_start:fault_end].mean()
+                        false_detection_rates[model.name+': '+key] = \
+                            value[:fault_start][:-1].mean()
+        else:
+            for key, value in model.alarms.items():
+                detection_alarms[model.name+': '+key] = \
+                    mask[mask==1].eq(value[value==1]).astype(int).mean()
+                false_detection_rates[model.name+': '+key] = \
+                    1-mask[mask==0].eq(value[value==0]).astype(int).mean()
+
+        # PLOTTING SPE
+                
+        if plot_SPE:
+
+            model.plot_SPE(ax = ax_spe[i,2], train_or_test='test',
+                           logy = logy)
+            ax_spe[i,2].set_title('Test')
+            
+            if fault_start is not None:
+                ax_spe[i,2].axvline(datetime.strptime(str(fault_start),
+                                                      '%Y-%m-%d %H:%M:%S'), 
+                                                      ls='--')
+            if fault_end is not None:
+                ax_spe[i,2].axvline(datetime.strptime(str(fault_end),
+                                                      '%Y-%m-%d %H:%M:%S'), 
+                                                      ls='--')
+
+        # PLOTTING PREDICTIONS
+                
+        if plot_predictions:
+            if cond_to_plot_pred:
+                model.plot_predictions(ax = ax_pred[i,2], 
+                                        train_or_test = 'test', 
+                                        X_pred_to_plot = X_pred_to_plot,
+                                        metrics = metrics)
+                if fault_start is not None:
+                    ax_pred[i,2].axvline(datetime.strptime(str(fault_start),
+                                                 '%Y-%m-%d %H:%M:%S'), ls='--')
+                if fault_end is not None:
+                    ax_pred[i,2].axvline(datetime.strptime(str(fault_end),
+                                                 '%Y-%m-%d %H:%M:%S'), ls='--')
+
+        if plot_SPE:            
+            fig_spe.tight_layout();
+        if plot_predictions:
+            fig_pred.tight_layout();
+            
+    ######## GENERATING FINAL TABLES ########
+        
+    return_tables = []
+        
+    # PREDICTION
+
+    if metrics is not None:
+
+        prediction_table = pd.DataFrame([train_metrics, validation_metrics,
+                                         test_metrics], 
+                                        index = ['Train',
+                                                 'Validation',
+                                                 'Test']).T
+                                                            
+        models_names = [models[i].name for i in range(len(models))]
+        metrics_names = [metrics[i].__name__ for i in range(len(metrics))]
+        
+        iterables = [models_names, metrics_names]
+
+        index = pd.MultiIndex.from_product(iterables, 
+                                           names = ['Models', 'Metrics'])
+        
+        message = ("The MultiIndex table is not of the right size. "+
+                   "This could happen when two models have the same name.")
+        
+        try:
+            prediction_table.index = index
+        except ValueError as err:
+            raise ValueError(message) from err
+        
+        return_tables.append(prediction_table.swaplevel().sort_index(axis=0))
+
+    # DETECTION     
+        
+    if fault_start is not None:
+        
+        detection_table = pd.DataFrame([detection_alarms, 
+                                        false_detection_rates],
+                                       index = ['FDR','FAR']).T
+        
+        models_names = [models[i].name for i in range(len(models))]
+        alarms_names = [list(model.alarms.keys())[i] for i in 
+                range(len(list(model.alarms.keys())))]  
+        
+        iterables = [models_names, alarms_names]
+
+        index = pd.MultiIndex.from_product(iterables, 
+                                        names = ['Models', 'Alarms'])
+        
+        detection_table.index = index
+
+        return_tables.append(detection_table.swaplevel().sort_index(axis=0))
+        
+    # COMPUTATIONAL TIMES
+        
+    if times:
+        
+        times_dict = {}
+        
+        times_dict['Train'] = [1e6*models[i].train_time/X_train.shape[0]
+                        for i in range(len(models))]
+        times_dict['Test'] = [1e6*models[i].test_time/X_test.shape[0] 
+                        for i in range(len(models))]
+        
+        times_df = pd.DataFrame(times_dict, 
+                        index=[models[i].name for i in range(len(models))])
+        
+        return_tables.append(times_df)
+        
     return return_tables
```

### Comparing `bibmon-1.0.0/bibmon/_generic_model.py` & `bibmon-1.0.1/bibmon/_generic_model.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,1032 +1,1032 @@
-import copy
-import time
-import optuna
-import numpy as np
-import pandas as pd
-import seaborn as sns
-import sklearn.model_selection
-import matplotlib.pyplot as plt
-
-from abc import ABC, abstractmethod
-
-from ._alarms import detecOutlier
-from ._preprocess import PreProcess
-from ._bibmon_tools import align_dfs_by_rows
-
-###############################################################################
-
-class GenericModel (ABC):
-    """
-    Abstract class used as a base for creating child classes with
-    specific models (PCA, sklearnRegressor, etc).
-
-    Attributes
-    ----------
-            
-        * Data sets:
-        ----------
-        X_train, X_test, Y_train, Y_test: pandas.DataFrame
-            Normalized training and testing data sets.
-            X refers to the input and Y to the output (when there is Y).
-            
-        X_train_orig, X_test_orig, 
-        Y_train_orig, Y_test_orig: pandas.DataFrame
-            Original training and testing data sets (before pre-processing). 
-            X refers to the input and Y to the output (when there is Y).       
-            
-        * Predictions:
-        ----------
-        X_train_pred, X_test_pred 
-        (or Y_train_pred, Y_test_pred): pandas.DataFrame
-            Reconstructions (or predictions) 
-            provided by the model in training and testing.
-            
-        X_train_pred_orig, X_test_pred_orig
-        (or Y_train_pred_orig, Y_test_pred_orig): pandas.DataFrame
-            Reconstructions (or predictions) 
-            provided by the model in training and testing
-            in the original units.
-        
-        * Detection, contribution and prediction metrics:
-        ----------
-        SPE_train, SPE_test: pd.Series
-            Square Prediction Error. One-dimensional vectors containing
-            the SPE values calculated at each time step in 
-            training and testing.  
-                
-        * Training parameters:
-        ----------
-        Mux, SDx, Muy, SDy: pandas.Series
-            Means and standard deviations of the variables 
-            in the training period.
-            
-        limSPE_train, SPE_mean: float
-            Limit for detection and mean of the SPE obtained in training.
-
-        limSPE: float
-            Potentially redefined detection limit in the validation stage.
-            
-        lim_conf: float
-            Confidence limit for the detection index.
-
-        train_time: float
-            Computational training time.
-            
-        index_train: pandas.DatetimeIndex
-            Indexes of the training set.
-            
-        * Testing parameters:
-        ----------            
-        count_window_size: int
-            Window sizes used in alarm calculations.
-        
-        outlier_alarm,
-        count_alarm: numpy.array
-            One-dimensional arrays that store the various alarms for each
-            time step.
-            
-        alarms: dict
-            Dictionary containing the mentioned alarms above.
-        
-        count_limit: int
-            Limit of points to be considered for the count_alarm to trigger.
-
-        test_time: float
-            Computational testing time.
-
-        has_alarm_windows: boolean
-            Indicator of testing step with or without windows for the alarms.
-            
-        * Other attributes:
-        ----------
-        preproc_X, preproc_Y: PreProcess
-            Object of the PreProcess class (defined in the _bibmon_tools.py 
-            file) that contains the preprocessing functions and arguments
-            to be applied in training and testing.
-        tags_X, tags_Y: list of str
-            tags kept in the data set, obtained in pre-training.
-        test_tags_X, test_tags_Y: list of str
-            tags used in testing.
-        has_Y: boolean
-            indicator of the existence or absence of 
-            a predicted dataset (Y) in the model.
-            
-    Methods
-    ----------
-        train_core (@abstractmethod)
-        map_from_X (@abstractmethod)
-        set_hyperparameters
-        load_model
-        pre_train
-        train
-        pre_test
-        test
-        plot_SPE
-        fit
-        predict       
-    """
-
-    ###########################################################################
-    
-    @abstractmethod
-    def train_core (self):
-        """
-        The core of the training algorithm, that is,
-        all the necessary steps between `pre_train()` and
-        the calculation of the prediction or reconstruction 
-        in training by `map_from_X()`.
-        """
-        pass
-
-    ###########################################################################
-            
-    @abstractmethod
-    def map_from_X (self, X):
-        """
-        Receives a data matrix X and returns a matrix of predicted 
-        or reconstructed values.
-
-        Parameters
-        ----------
-        X: numpy.array
-            Window X of data for prediction or reconstruction.  
-            
-        Returns
-        ----------                
-        : numpy.array
-        Reconstructed X (or predicted Y).
-        """  
-        pass
-
-    ###########################################################################
-            
-    def set_hyperparameters (self, params_dict):
-        """
-        Receives a dict with hyperparameters to be assigned in the model.
-
-        Parameters
-        ----------
-        params_dict: dict
-            Dictionary with hyperparameter values
-
-        """          
-        for key, value in params_dict.items():
-            setattr(self, key, value)
-
-    ###########################################################################
-        
-    def load_model (self, limSPE, SPE_mean, count_window_size,
-                    Mux, SDx, Muy = None, SDy = None):
-        """
-        Receives parameters from a previously trained model for
-        making predictions and tests without the need for training.
-
-        Parameters
-        ----------                     
-        limSPE: float
-            Detection limit and mean of the SPE.
-        SPE_mean: float
-            Mean of the SPE.
-        count_window_size: int
-            Window sizes used in count alarms calculation.
-        Mux: pandas.Series
-            Means of the X variables in the training period.
-        SDx: pandas.Series
-            Standard deviations of the X variables in
-            the training period.
-        Muy: pandas.Series, optional
-            Means of the Y variables in the training period.
-        SDy: pandas.Series, optional
-            Standard deviations of the Y variables in the training period.    
-        """  
-    
-        self.MuX = pd.Series(Mux)
-        self.SDX = pd.Series(SDx)
-        self.MuY = pd.Series(Muy)
-        self.SDY = pd.Series(SDy)
-        self.limSPE = limSPE
-        self.SPE_mean = SPE_mean
-        self.count_window_size = count_window_size
-
-    ###########################################################################
-
-    def pre_train (self, X_train, Y_train = None, 
-                   f_pp = ['remove_empty_variables',
-                           'ffill_nan',
-                           'remove_frozen_variables',
-                           'normalize'], 
-                   a_pp = None,
-                   f_pp_test = ['replace_nan_with_values',
-                                'normalize'], 
-                   a_pp_test = None):
-        """
-        Receives the data for model training and prepares them for training.
-
-        Parameters
-        ----------
-        X_train: pandas.DataFrame or numpy.ndarray
-            Window of X data used in training.
-        Y_train: pandas.DataFrame or numpy.ndarray, optional
-            Window of Y data used in training.
-        f_pp: list, optional
-            List containing strings with names of functions to be used 
-            in pre-processing the training data (the functions are defined
-            in the PreProcess class, in the BibMon_Tools.py file)
-        f_pp_test: list, optional
-            List containing strings with names of functions to be used 
-            in pre-processing the testing data (the functions are defined 
-            in the PreProcess class, in the BibMon_Tools.py file)
-        a_pp: dict, optional
-            Dictionary containing the parameters to be provided
-            to each function to perform pre-processing of the training data, 
-            in the format {'functionname__argname': argvalue, ...}
-        a_pp_test: dict, optional
-            Dictionary containing the parameters to be provided
-            to each function to perform pre-processing of the testing data, ]
-            in the format {'functionname__argname': argvalue, ...}
-        """
-                
-        # storing complete training set
-        
-        self.X_train = pd.DataFrame(X_train)
-        self.Y_train = pd.DataFrame(Y_train)
-
-        # data set that will keep the original units
-
-        self.X_train_orig = copy.deepcopy(self.X_train)
-        if self.has_Y:
-            self.Y_train_orig = copy.deepcopy(self.Y_train)
-
-        # defining the training medians as the default values 
-        # to replace NaNs during testing
-        
-        if f_pp_test is not None:
-            if 'replace_nan_with_values' in f_pp_test:
-                if a_pp_test is None:
-                    a_pp_test = {}
-                a_pp_test['replace_nan_with_values__val'] = \
-                    self.X_train.median()
-
-        # applying pre-processing functions
-
-        if f_pp is not None:
-            self.preproc_X = PreProcess(f_pp, a_pp)
-            self.X_train = self.preproc_X.apply(self.X_train)
-            if self.has_Y:
-                self.preproc_Y = PreProcess(f_pp,  a_pp, is_Y = True)
-                self.Y_train = self.preproc_Y.apply(self.Y_train)
-                
-        # preparing the testing pre-processing functions
-                            
-        if f_pp_test is not None:
-            self.preproc_X.f_pp = f_pp_test
-            self.preproc_X.a_pp = a_pp_test
-            if self.has_Y:
-                self.preproc_Y.f_pp = f_pp_test
-                self.preproc_Y.a_pp = a_pp_test
-                
-        # aligning the rows of X and Y, if necessary            
-        if self.has_Y:
-            self.X_train, self.Y_train = align_dfs_by_rows(self.X_train,
-                                                            self.Y_train)
-        
-        # saving the tags
-        self.tags_X = self.X_train.columns.to_list()
-        if self.has_Y:
-            self.tags_Y = self.Y_train.columns.to_list()
-          
-    ###########################################################################
-
-    def train (self, lim_conf = 0.99, delete_training_data = False):
-        """
-        Performs the model training. 
-        Must be called after the pre_train function.
-
-        Parameters
-        ----------
-        lim_conf: float, optional
-            Confidence limit for the detection index.
-        delete_training_data: boolean, optional
-            If True, the data is deleted at the end of training.
-            Useful to save memory.
-        """        
-        
-        self.lim_conf = lim_conf
-
-        start_train = time.time()
-        
-        # core of the training algorithm!
-        self.train_core()
-        
-        # predicting! (or reconstructing!)
-        train_pred = self.map_from_X (self.X_train.values)
-
-        end_train = time.time()  
-        
-        self.train_time = end_train - start_train
-        
-        # storing results and calculating SPE
-        
-        if self.has_Y:        
-            self.Y_train_pred = pd.DataFrame(train_pred,
-                                            index=self.Y_train.index,
-                                            columns = self.Y_train.columns)  
-            
-            self.SPE_train = np.sum((self.Y_train.values-
-                                    self.Y_train_pred.values)**2,
-                                    axis=1)
-        else:
-            self.X_train_pred = pd.DataFrame(train_pred,
-                                            index=self.X_train.index,
-                                            columns = self.X_train.columns) 
-
-            self.SPE_train = np.sum((self.X_train.values-
-                                    self.X_train_pred.values)**2,
-                                    axis=1)
-            
-        # calculating indices and detection limits
-
-        self.SPE_mean = self.SPE_train.mean()
-        
-        iSPE = np.sort(self.SPE_train)
-        self.limSPE = iSPE[int(lim_conf*self.X_train.shape[0])]
-        
-        self.limSPE_train = copy.deepcopy(self.limSPE)
-        
-        # denormalizing
-        
-        if self.has_Y and self.preproc_Y is not None:
-            if 'normalize' in self.preproc_Y.f_pp:
-                self.Y_train_pred_orig = \
-                    self.preproc_Y.back_to_units(self.Y_train_pred)
-            else:
-                self.Y_train_pred_orig = self.Y_train_pred
-        else:
-            if 'normalize' in self.preproc_X.f_pp:
-                self.X_train_pred_orig = \
-                    self.preproc_X.back_to_units(self.X_train_pred)
-            else:
-                self.X_train_pred_orig = self.X_train_pred
-
-        # indexes of the training set
-        self.index_train = self.X_train.index
-        
-        self.SPE_train = pd.Series(self.SPE_train, index = self.index_train)
-        
-        # deleting training data, if applicable
-        if delete_training_data:
-            del self.X_train, self.X_train_orig, \
-                self.SPE_train, self.index_train
-            if self.has_Y:
-                del self.Y_train, self.Y_train_orig, \
-                    self.Y_train_pred, self.Y_train_pred_orig
-            else:
-                del self.X_train_pred, self.X_train_pred_orig    
-    
-    ###########################################################################
-    
-    def hyperparameter_tuning (self, params, n_trials = 20, lim_conf = 0.99,
-                               percent_validation = 0.2,
-                               n_splits = None, delete_training_data = False):
-        """
-        Performs hyperparameter tuning using the Optuna library.
-
-        Parameters
-        ----------
-        params: pandas.DataFrame
-            Contains the possibilities to be tested and the types of 
-            parameters. Must be defined as: 
-            pd.DataFrame({'possibilities': [list_possibilities1, 
-                                            list_possibilities2, ...],
-                          'types': [str_type1, 
-                                    str_type2, ...]},
-                         index = [str_param1_name, str_param2_name, ...])
-        n_trials: int, optional
-            Number of trials in the optimization performed by Optuna.
-        lim_conf: float, optional
-            Confidence limit for the detection index.
-        percent_validation: float (0<value<1), optional
-            Percentage of the data to be separated for use 
-            in internal validation, if no cross-validation is performed.
-        n_splits: int, optional
-            Number of sets to be used in cross-validation.
-            If not None, the value of percent_validation is disregarded.
-        delete_training_data: boolean, optional
-            If True, the data is deleted at the end of training.
-            Useful to save memory.
-        """  
-        def objective (trial):
-
-            suggestions = {}
-            
-            for index, row in params.iterrows():
-                if row['type'] == 'uniform':
-                    sug = trial.suggest_uniform(index, 
-                                                row['possibilities'][0], 
-                                                row['possibilities'][1])                  
-                if row['type'] == 'loguniform':
-                    sug = trial.suggest_loguniform(index, 
-                                                row['possibilities'][0], 
-                                                row['possibilities'][1])  
-                if row['type'] == 'discrete_uniform':
-                    sug = trial.suggest_discrete_uniform(index, 
-                                                       row['possibilities'][0], 
-                                                       row['possibilities'][1],
-                                                       row['possibilities'][2])   
-                if row['type'] == 'int':
-                    sug = trial.suggest_int(index, 
-                                            int(row['possibilities'][0]), 
-                                            int(row['possibilities'][1]))
-                if row['type'] == 'categorical':
-                    sug = trial.suggest_categorical(index, 
-                                                    row['possibilities']) 
-                suggestions[index] = sug
-            
-            self.set_hyperparameters(suggestions)
-            
-            if n_splits is not None:
-            
-                kf = sklearn.model_selection.KFold(n_splits = n_splits)
-                            
-                SPEs = []
-                
-                for train_index, test_index in kf.split(self.X_train):
-                    autocopy = copy.deepcopy(self)
-                    autocopy.pre_train(X_train =
-                                       self.X_train.iloc[train_index,:],
-                                       Y_train = 
-                                       self.Y_train.iloc[train_index,:])
-                    autocopy.train(lim_conf, delete_training_data = True)
-                    
-                    autocopy.pre_test(X_test = self.X_train.iloc[test_index,:],
-                                      Y_test = self.Y_train.iloc[test_index,:])
-                    
-                    autocopy.test()
-                    SPEs.append(np.mean(autocopy.SPE_test))
-
-                del autocopy
-                return np.mean(SPEs)
-            
-            else:
-                
-                n = int(self.X_train.shape[0]*percent_validation)
-                
-                autocopy = copy.deepcopy(self)
-                
-                autocopy.pre_train(X_train = self.X_train.iloc[n:,:],
-                                    Y_train = self.Y_train.iloc[n:,:])
-                autocopy.train(lim_conf, delete_training_data = True)
-                autocopy.pre_test(X_test = self.X_train.iloc[:n,:],
-                                    Y_test = self.Y_train.iloc[:n,:])
-                autocopy.test()
-            
-                mean_spe = np.mean(autocopy.SPE_test)
-                del autocopy
-                return mean_spe
-        
-        self.hyperparemeter_study = optuna.create_study()
-        self.hyperparemeter_study.optimize(objective, n_trials = n_trials)
-        
-        print(self.hyperparemeter_study.best_params)
-        
-        self.set_hyperparameters(self.hyperparemeter_study.best_params)
-                   
-    ###########################################################################
-
-    def pre_test (self, X_test, Y_test = None, 
-                  count_window_size = 0, count_limit = 1,
-                  f_pp = None, a_pp = None):
-        '''   
-        Receives a window of data and prepares it for the model testing.
-        
-        Parameters
-        ----------
-        X_test: pandas.DataFrame, pandas.Series or numpy.ndarray
-            Window of data or observation X needed to perform the analysis.
-        Y_test: pandas.DataFrame, pandas.Series or numpy.ndarray, optional
-            Window of data or observation Y needed to perform the analysis.
-        count_window_size: int, optional
-            Window size used in the count alarm calculation.
-        count_limit: int, optional
-            Limit of points to be considered in the window 
-            for the count alarm to trigger. 
-        f_pp: list, optional
-            List containing strings with names of functions to be used 
-            in pre-processing (the functions are defined in the 
-            PreProcess class).
-        a_pp: dict, optional
-            Dictionary containing the parameters to be provided
-            to each function to perform pre-processing of the data, in
-            the format {'functionname__argname': argvalue, ...}
-        '''
-        
-        # window sizes for alarms:
-                        
-        self.count_limit = count_limit
-        self.count_window_size = count_window_size
-
-        # storing complete testing set
-                                
-        if (isinstance(X_test, np.ndarray) and X_test.shape == ()):
-            self.X_test = pd.DataFrame(X_test[None])
-        elif len(X_test.shape)==1 and ((isinstance(X_test, np.ndarray))):
-                self.X_test = pd.DataFrame(X_test).T
-        else:
-            self.X_test = pd.DataFrame(X_test)  
-            
-        if self.has_Y:
-            if (isinstance(Y_test, np.ndarray) and Y_test.shape == ()):
-                self.Y_test = pd.DataFrame(Y_test[None])
-            elif len(Y_test.shape)==1 and ((isinstance(Y_test, np.ndarray))):
-                    self.Y_test = pd.DataFrame(Y_test).T
-            else:
-                self.Y_test = pd.DataFrame(Y_test)
-
-        # data set that will keep the original units       
-                
-        self.X_test_orig = copy.deepcopy(self.X_test)
-        if self.has_Y:
-            self.Y_test_orig = copy.deepcopy(self.Y_test) 
-
-        # applying pre-processing functions
-
-        if f_pp is not None:
-
-            if not hasattr(self, 'preproc_X'):
-                self.preproc_X = PreProcess(f_pp, a_pp)
-            else:
-                self.preproc_X.f_pp = f_pp
-                self.preproc_X.a_pp = a_pp
-
-            if self.has_Y:
-
-                if not hasattr(self, 'preproc_Y'):
-                    self.preproc_Y = PreProcess(f_pp, a_pp, is_Y = True)
-                else:
-                    self.preproc_Y.f_pp = f_pp
-                    self.preproc_Y.a_pp = a_pp
-
-        if hasattr(self, 'preproc_X'):
-            self.X_test = self.preproc_X.apply(self.X_test, 
-                                                train_or_test = 'test')
-
-        if hasattr(self, 'preproc_Y'):
-            self.Y_test = self.preproc_Y.apply(self.Y_test, 
-                                                train_or_test = 'test')  
-
-        # aligning the rows of X and Y, if necessary
-        if self.has_Y:
-            self.X_test, self.Y_test = align_dfs_by_rows(self.X_test,
-                                                         self.Y_test)
-
-        # test tags   
-            
-        self.tags_test_X = [t for t in self.tags_X
-                            if t in self.X_test.columns.tolist()]
-        
-        self.X_test = self.X_test[self.tags_test_X]
-
-        if self.has_Y:
-
-            self.tags_test_Y = [t for t in self.tags_Y 
-                                if t in self.Y_test.columns.tolist()]
-                
-            self.Y_test = self.Y_test[self.tags_test_Y]
-                        
-    ###########################################################################
-
-    def test (self, redefine_limit = False, delete_testing_data = False):
-        """
-        Analyzes a window of data, applying a model test.
-        Must be called after the pre_test function.
-        
-        Parameters
-        ----------
-        redefine_limit: boolean, optional
-            Indicator of redefinition or not of the detection limit during
-            testing.
-        delete_testing_data: boolean, optional
-            If True, the data is deleted at the end of testing.
-            Useful to save memory.
-        """
-
-        start_test = time.time()
-        
-        # predicting!
-        test_pred = self.map_from_X(self.X_test.values)
-
-        end_test = time.time()
-        
-        self.test_time = end_test - start_test
-
-        # storing results and calculating SPE
-    
-        if self.has_Y:
-            self.Y_test_pred = pd.DataFrame(test_pred,
-                                            index=self.Y_test.index,
-                                            columns = self.Y_test.columns)
-            self.SPE_test = np.sum((self.Y_test.values-
-                                    self.Y_test_pred.values)**2,
-                                    axis=1)
-            
-        else:
-            self.X_test_pred = pd.DataFrame(test_pred,
-                                            index=self.X_test.index,
-                                            columns = self.X_test.columns)
-            self.SPE_test = np.sum((self.X_test.values-
-                                    self.X_test_pred.values)**2,
-                                    axis=1)   
-        
-        # redefining the limit, for the validation case
-        
-        if redefine_limit:
-            iSPE = np.sort(self.SPE_test)
-            self.limSPE = iSPE[int(self.lim_conf*self.X_test.shape[0])]
-        
-        # calculations of the alarms
-        
-        if self.count_window_size != 0:
-            self.alarmCount = np.zeros(len(self.SPE_test))
-
-        self.alarmOutlier = detecOutlier(self.SPE_test, 
-                                         self.limSPE)
-
-        # if more window alarms are defined in the package, 
-        # i_min must be the minumum size among them
-        i_min = self.count_window_size
-        
-        for i in range(i_min, len(self.SPE_test)):
-                        
-            if self.count_window_size != 0:
-                if i >= self.count_window_size:
-                    self.alarmCount[i] = \
-                    detecOutlier(self.SPE_test[i-self.count_window_size:(i+1)], 
-                                 self.limSPE, count = True, 
-                                 count_limit = self.count_limit)
-            
-        # adjusting the size of the prediction and denormalizing    
-        if self.has_Y:
-            if 'normalize' in self.preproc_Y.f_pp:
-                self.Y_test_pred_orig = \
-                    self.preproc_Y.back_to_units(self.Y_test_pred)
-            else:
-                self.Y_test_pred_orig = self.Y_test_pred
-        else:
-            if 'normalize' in self.preproc_X.f_pp:
-                self.X_test_pred_orig = \
-                    self.preproc_X.back_to_units(self.X_test_pred)
-            else:
-                self.X_test_pred_orig = self.X_test_pred
-        
-        self.SPE_test = pd.Series(self.SPE_test, 
-                                index = self.X_test.index)
-
-        self.alarms = {}
-
-        self.alarmOutlier = pd.Series(self.alarmOutlier,
-                                    index = self.X_test.index)
-        self.alarms['alarmOutlier'] = self.alarmOutlier
-        if self.count_window_size != 0:
-            self.alarmCount = pd.Series(self.alarmCount,
-                                        index = self.X_test.index)
-            str_count = f'alarmCount WS={self.count_window_size}, '\
-                    f'limCount = {self.count_limit}'
-            self.alarms[str_count] = self.alarmCount
-
-        # deleting testing data, if applicable
-        if delete_testing_data:
-            del self.X_test, self.X_test_orig, \
-                self.SPE_test, self.alarms, self.alarmOutlier
-            if self.has_Y:
-                del self.Y_test, self.Y_test_orig, \
-                    self.Y_test_pred, self.Y_test_pred_orig
-            else:
-                del self.X_test_pred, self.X_test_pred_orig
-            if hasattr(self, 'alarmCount'): del self.alarmCount
-
-    ###########################################################################
-        
-    def plot_SPE (self, ax = None, train_or_test = 'train', logy = True,
-                  legends = True, plot_alarm_outlier = True):
-        """
-        Plotting the temporal evolution of SPE.
-
-        Parameters
-        ----------
-        ax: matplotlib.axes._subplots.AxesSubplot, optional
-            Axis on which the graph will be plotted.
-        train_or_test: string, optional
-            Indicates whether to plot the graph for 'train' or 'test'.
-        logy: boolean, optional
-            Indicates whether the y-axis scale should be logarithmic (True) or 
-            linear (False).
-        legends: boolean, optional
-            If the graph should display legends.
-        plot_alarm_outlier: boolean, optional
-            If the alarmOutlier should be plotted.
-        """
-        
-        if ax is not None:
-            pass
-        else:
-            fig, ax = plt.subplots()
-            
-        if train_or_test == 'train':
-            SPE = self.SPE_train
-            limSPE = self.limSPE_train
-        elif train_or_test == 'test':
-            SPE = self.SPE_test
-            limSPE = self.limSPE
-        
-        SPE.plot(ax=ax, logy = logy, ls='',
-                marker='.', label='SPE')
-        
-        if train_or_test == 'test':
-            for label, alarm in self.alarms.items():
-                if not plot_alarm_outlier and label=='alarmOutlier':
-                    continue
-                (ax.get_ylim()[1]*alarm).replace(0, np.nan).plot(ax = ax, 
-                                                                logy = logy, 
-                                                                ls = '',
-                                                                marker = '.', 
-                                                                alpha = 0.5,
-                                                                label = label)
-                    
-        ax.axhline(limSPE, color='red', ls = '--',
-                label='%.0f%% Confidence Limit' %(self.lim_conf*100))
-        
-        if legends:
-            ax.legend(fontsize=12);
-                        
-    ###########################################################################
-
-    def plot_predictions (self, ax = None, train_or_test = 'train', 
-                          X_pred_to_plot = None, metrics = None):
-        """
-        Plotting the temporal evolution of the predictions along with the
-        respective true values.
-
-        Parameters
-        ----------
-        ax: matplotlib.axes._subplots.AxesSubplot, optional
-            Axis on which the graph will be plotted.
-        train_or_test: string, optional
-            Indicates whether to plot the graph for 'train' or 'test'.
-        X_pred_to_plot: string, optional
-            In case the model is a reconstruction model 
-            (i.e., self.has_Y = False), indicates which column of X to plot 
-            along with the prediction.
-        metrics: list of functions, optional
-            Functions for calculating metrics to be displayed in the title of 
-            the graph.
-        """ 
-
-        if ax is not None:
-            pass
-        else:
-            fig, ax = plt.subplots()
-        
-        if self.has_Y:
-        
-            if train_or_test=='train':
-                true = self.Y_train_orig
-                pred = self.Y_train_pred_orig
-            elif train_or_test=='test':
-                true = self.Y_test_orig
-                pred = self.Y_test_pred_orig
-            
-            regression_or_reconstruction = 'Regression'
-            
-        else:
-            
-            if X_pred_to_plot is not None:
-
-                if train_or_test=='train':
-                    true = self.X_train_orig[X_pred_to_plot]
-                    pred = self.X_train_pred_orig[X_pred_to_plot]
-                elif train_or_test=='test':
-                    true = self.X_test_orig[X_pred_to_plot]
-                    pred = self.X_test_pred_orig[X_pred_to_plot]
-                
-                regression_or_reconstruction = 'Reconstruction'
-                
-            else:
-
-                raise RuntimeError('The model has no Y. \
-                                Specify which variable in X should be plotted')
-                
-        true.plot(ax=ax)
-        pred.plot(ax=ax,ls='--')
-        
-        ax.legend(['Measurement',regression_or_reconstruction])
-        
-        tags = pd.DataFrame(true).columns.to_list()
-                
-        title = str(tags)
-        
-        if metrics is not None:
-            
-            if not isinstance(metrics, list): 
-                metrics = [metrics]
-                                
-            true, pred = align_dfs_by_rows(true.dropna(), pred)
-            
-            for metric in metrics:
-                title = (title+
-                        f'\n{metric.__name__}: {metric(true, pred):.2f}')
-        
-        ax.set_title(title)
-    
-    ###########################################################################
-
-    def fit (self, X_train, Y_train = None,
-             f_pp = ['remove_empty_variables',
-                     'ffill_nan',
-                     'remove_frozen_variables',
-                     'normalize'],
-             a_pp = None,
-             f_pp_test = ['replace_nan_with_values',
-                          'normalize'],
-             a_pp_test = None,
-             lim_conf = 0.99,
-             delete_training_data = False,
-             redefine_limit = False,
-             frac_val = 0.15,
-             tune = False,
-             params = None,
-             params_types = None,
-             params_possibilities = None,
-             n_trials = 20):
-        """
-        Performs the complete pipeline of model training,
-        sequentially executing the 'pre_train' and 'train' methods.
-
-        Parameters
-        ----------
-        X_train: pandas.DataFrame or numpy.ndarray
-            Window of X data used in training.
-        Y_train: pandas.DataFrame or numpy.ndarray, optional
-            Window of Y data used in training.
-        f_pp: list, optional
-            List containing strings with names of functions to be used 
-            in pre-processing the training data (the functions are defined
-            in the PreProcess class, in the BibMon_Tools.py file).
-        f_pp_test: list, optional
-            List containing strings with names of functions to be used 
-            in pre-processing the testing data (the functions are defined 
-            in the PreProcess class, in the BibMon_Tools.py file).
-        a_pp: dict, optional
-            Dictionary containing the parameters to be provided
-            to each function to perform pre-processing of the training data, in
-            the format {'functionname__argname': argvalue, ...}.
-        a_pp_test: dict, optional
-            Dictionary containing the parameters to be provided
-            to each function to perform pre-processing of the testing data, in
-            the format {'functionname__argname': argvalue, ...}.
-        lim_conf: float, optional
-            Confidence limit for the detection index.
-        delete_training_data: boolean, optional
-            If True, the data is deleted at the end of training.
-            Useful to save memory.
-        redefine_limit: boolean, optional
-            Indicator of redefinition or not of the detection limit using
-            a validation period taken from the training data itself.
-        frac_val: float, optional
-            Fraction of the data used for validation. 
-            0<frac_val<1.
-            Only used if redefine_limit==True.
-        tune: boolean, optional
-            Indicator of automatic hyperparameter tuning.
-        params: string or list of strings, optional
-            Name(s) of the parameter(s) to be tuned.
-        params_types:  string or list of strings
-            Type(s) of the parameter(s) to be tuned.
-        params_possibilities: list, optional
-            Possibilities to be tested for each parameter.
-            It must be a list containing the possibilities 
-            (in case of only one parameter), or a list containing the lists
-            for each possibility.
-            Possibilities must be provided according to the type of
-            the parameter, as specified in the Optuna library API.
-        n_trials: int, optional
-            Number of iterations in the hyperparameter search optimization.
-        """
-
-        X_train = pd.DataFrame(X_train)
-        Y_train = pd.DataFrame(Y_train)
-
-        if redefine_limit:
-            
-            n_trn =  int(X_train.shape[0]*(1-frac_val))
-            X_val = X_train.iloc[n_trn:]
-            X_train = X_train.iloc[:n_trn]
-            
-            if Y_train is not None:
-
-                Y_val = Y_train.iloc[n_trn:]
-                Y_train = Y_train.iloc[:n_trn]
-            
-            else:
-                
-                Y_val = None
-            
-        if tune:
-            self.pre_train(X_train, Y_train, 
-                f_pp = f_pp,
-                a_pp = a_pp,
-                f_pp_test = f_pp_test,
-                a_pp_test  = a_pp_test)
-            if not isinstance(params, list):
-                params = [params]
-            if not isinstance(params_types, list):
-                params_types = [params_types]
-            if not isinstance(params_possibilities, list):
-                print('params_possibilities must be a list!')
-            else:
-                if not isinstance(params_possibilities[0], list):
-                    params_possibilities = [params_possibilities]
-            params_df = pd.DataFrame({'possibilities': params_possibilities,
-                                      'type': params_types},
-                                     index = params) 
-            self.tuning(n_trials = n_trials, params = params_df, 
-                        lim_conf = lim_conf, 
-                        delete_training_data = delete_training_data)
-            
-        self.pre_train(X_train, Y_train, 
-                        f_pp = f_pp,
-                        a_pp = a_pp,
-                        f_pp_test = f_pp_test,
-                        a_pp_test  = a_pp_test)
-
-        self.train(lim_conf = lim_conf, 
-                   delete_training_data = delete_training_data)
-
-        if redefine_limit:
-            self.pre_test(X_val, Y_val)
-            self.test(redefine_limit = True)
-        if f_pp_test:   
-            # save value for use in predict if necessary
-            self.f_pp_test = f_pp_test 
-        if a_pp_test:  
-             # save value for use in predict if necessary
-            self.a_pp_test = a_pp_test
-
-    ###########################################################################
-        
-    def predict (self, 
-                 X_test, 
-                 Y_test = None,  
-                 count_window_size = 0, 
-                 count_limit = 1, 
-                 f_pp = 'fit', 
-                 a_pp = 'fit', 
-                 delete_testing_data = False,
-                 redefine_limit = False):
-        '''   
-        Performs the complete pipeline of model prediction (testing), 
-        sequentially executing the 'pre_test' and 'test' methods.
-        
-        Parameters
-        ----------
-        X_test: pandas.DataFrame, pandas.Series or numpy.ndarray
-            Window of data or observation X needed to perform the analysis.
-        Y_test: pandas.DataFrame, pandas.Series or numpy.ndarray, optional
-            Window of data or observation Y needed to perform the analysis.
-        count_window_size: int, optional
-            Window size used in count alarm calculation. 
-        count_limit: int, optional
-            Limit of points to be considered in the window 
-            for the count alarm to trigger.            
-        f_pp: list, optional
-            List containing strings with names of functions to be used 
-            in pre-processing (the functions are defined in the 
-            PreProcess class).
-        a_pp: dict, optional
-            Dictionary containing the parameters to be provided
-            to each function to perform pre-processing of the data, in
-            the format {'functionname__argname': argvalue, ...}
-        delete_testing_data: boolean, optional
-            If True, the data is deleted at the end of testing.
-            Useful to save memory.   
-        redefine_limit: boolean, optional
-            Indicator of redefinition or not of the detection limit during
-            testing.
-        '''
-        
-        if f_pp == 'fit':
-            if hasattr(self,'f_pp_test'):
-                f_pp = self.f_pp_test
-            else:
-                f_pp = None
-        if a_pp == 'fit':
-            if hasattr(self,'a_pp_test'):
-                a_pp = self.a_pp_test
-            else:
-                a_pp = None
-            
-        self.pre_test(X_test, Y_test, count_limit = count_limit, 
-                      count_window_size = count_window_size, 
-                      f_pp = f_pp, a_pp = a_pp)
-        self.test(redefine_limit = redefine_limit,
-                  delete_testing_data = delete_testing_data)
+import copy
+import time
+import optuna
+import numpy as np
+import pandas as pd
+import seaborn as sns
+import sklearn.model_selection
+import matplotlib.pyplot as plt
+
+from abc import ABC, abstractmethod
+
+from ._alarms import detecOutlier
+from ._preprocess import PreProcess
+from ._bibmon_tools import align_dfs_by_rows
+
+###############################################################################
+
+class GenericModel (ABC):
+    """
+    Abstract class used as a base for creating child classes with
+    specific models (PCA, sklearnRegressor, etc).
+
+    Attributes
+    ----------
+            
+        * Data sets:
+        ----------
+        X_train, X_test, Y_train, Y_test: pandas.DataFrame
+            Normalized training and testing data sets.
+            X refers to the input and Y to the output (when there is Y).
+            
+        X_train_orig, X_test_orig, 
+        Y_train_orig, Y_test_orig: pandas.DataFrame
+            Original training and testing data sets (before pre-processing). 
+            X refers to the input and Y to the output (when there is Y).       
+            
+        * Predictions:
+        ----------
+        X_train_pred, X_test_pred 
+        (or Y_train_pred, Y_test_pred): pandas.DataFrame
+            Reconstructions (or predictions) 
+            provided by the model in training and testing.
+            
+        X_train_pred_orig, X_test_pred_orig
+        (or Y_train_pred_orig, Y_test_pred_orig): pandas.DataFrame
+            Reconstructions (or predictions) 
+            provided by the model in training and testing
+            in the original units.
+        
+        * Detection, contribution and prediction metrics:
+        ----------
+        SPE_train, SPE_test: pd.Series
+            Square Prediction Error. One-dimensional vectors containing
+            the SPE values calculated at each time step in 
+            training and testing.  
+                
+        * Training parameters:
+        ----------
+        Mux, SDx, Muy, SDy: pandas.Series
+            Means and standard deviations of the variables 
+            in the training period.
+            
+        limSPE_train, SPE_mean: float
+            Limit for detection and mean of the SPE obtained in training.
+
+        limSPE: float
+            Potentially redefined detection limit in the validation stage.
+            
+        lim_conf: float
+            Confidence limit for the detection index.
+
+        train_time: float
+            Computational training time.
+            
+        index_train: pandas.DatetimeIndex
+            Indexes of the training set.
+            
+        * Testing parameters:
+        ----------            
+        count_window_size: int
+            Window sizes used in alarm calculations.
+        
+        outlier_alarm,
+        count_alarm: numpy.array
+            One-dimensional arrays that store the various alarms for each
+            time step.
+            
+        alarms: dict
+            Dictionary containing the mentioned alarms above.
+        
+        count_limit: int
+            Limit of points to be considered for the count_alarm to trigger.
+
+        test_time: float
+            Computational testing time.
+
+        has_alarm_windows: boolean
+            Indicator of testing step with or without windows for the alarms.
+            
+        * Other attributes:
+        ----------
+        preproc_X, preproc_Y: PreProcess
+            Object of the PreProcess class (defined in the _bibmon_tools.py 
+            file) that contains the preprocessing functions and arguments
+            to be applied in training and testing.
+        tags_X, tags_Y: list of str
+            tags kept in the data set, obtained in pre-training.
+        test_tags_X, test_tags_Y: list of str
+            tags used in testing.
+        has_Y: boolean
+            indicator of the existence or absence of 
+            a predicted dataset (Y) in the model.
+            
+    Methods
+    ----------
+        train_core (@abstractmethod)
+        map_from_X (@abstractmethod)
+        set_hyperparameters
+        load_model
+        pre_train
+        train
+        pre_test
+        test
+        plot_SPE
+        fit
+        predict       
+    """
+
+    ###########################################################################
+    
+    @abstractmethod
+    def train_core (self):
+        """
+        The core of the training algorithm, that is,
+        all the necessary steps between `pre_train()` and
+        the calculation of the prediction or reconstruction 
+        in training by `map_from_X()`.
+        """
+        pass
+
+    ###########################################################################
+            
+    @abstractmethod
+    def map_from_X (self, X):
+        """
+        Receives a data matrix X and returns a matrix of predicted 
+        or reconstructed values.
+
+        Parameters
+        ----------
+        X: numpy.array
+            Window X of data for prediction or reconstruction.  
+            
+        Returns
+        ----------                
+        : numpy.array
+        Reconstructed X (or predicted Y).
+        """  
+        pass
+
+    ###########################################################################
+            
+    def set_hyperparameters (self, params_dict):
+        """
+        Receives a dict with hyperparameters to be assigned in the model.
+
+        Parameters
+        ----------
+        params_dict: dict
+            Dictionary with hyperparameter values
+
+        """          
+        for key, value in params_dict.items():
+            setattr(self, key, value)
+
+    ###########################################################################
+        
+    def load_model (self, limSPE, SPE_mean, count_window_size,
+                    Mux, SDx, Muy = None, SDy = None):
+        """
+        Receives parameters from a previously trained model for
+        making predictions and tests without the need for training.
+
+        Parameters
+        ----------                     
+        limSPE: float
+            Detection limit and mean of the SPE.
+        SPE_mean: float
+            Mean of the SPE.
+        count_window_size: int
+            Window sizes used in count alarms calculation.
+        Mux: pandas.Series
+            Means of the X variables in the training period.
+        SDx: pandas.Series
+            Standard deviations of the X variables in
+            the training period.
+        Muy: pandas.Series, optional
+            Means of the Y variables in the training period.
+        SDy: pandas.Series, optional
+            Standard deviations of the Y variables in the training period.    
+        """  
+    
+        self.MuX = pd.Series(Mux)
+        self.SDX = pd.Series(SDx)
+        self.MuY = pd.Series(Muy)
+        self.SDY = pd.Series(SDy)
+        self.limSPE = limSPE
+        self.SPE_mean = SPE_mean
+        self.count_window_size = count_window_size
+
+    ###########################################################################
+
+    def pre_train (self, X_train, Y_train = None, 
+                   f_pp = ['remove_empty_variables',
+                           'ffill_nan',
+                           'remove_frozen_variables',
+                           'normalize'], 
+                   a_pp = None,
+                   f_pp_test = ['replace_nan_with_values',
+                                'normalize'], 
+                   a_pp_test = None):
+        """
+        Receives the data for model training and prepares them for training.
+
+        Parameters
+        ----------
+        X_train: pandas.DataFrame or numpy.ndarray
+            Window of X data used in training.
+        Y_train: pandas.DataFrame or numpy.ndarray, optional
+            Window of Y data used in training.
+        f_pp: list, optional
+            List containing strings with names of functions to be used 
+            in pre-processing the training data (the functions are defined
+            in the PreProcess class, in the BibMon_Tools.py file)
+        f_pp_test: list, optional
+            List containing strings with names of functions to be used 
+            in pre-processing the testing data (the functions are defined 
+            in the PreProcess class, in the BibMon_Tools.py file)
+        a_pp: dict, optional
+            Dictionary containing the parameters to be provided
+            to each function to perform pre-processing of the training data, 
+            in the format {'functionname__argname': argvalue, ...}
+        a_pp_test: dict, optional
+            Dictionary containing the parameters to be provided
+            to each function to perform pre-processing of the testing data, ]
+            in the format {'functionname__argname': argvalue, ...}
+        """
+                
+        # storing complete training set
+        
+        self.X_train = pd.DataFrame(X_train)
+        self.Y_train = pd.DataFrame(Y_train)
+
+        # data set that will keep the original units
+
+        self.X_train_orig = copy.deepcopy(self.X_train)
+        if self.has_Y:
+            self.Y_train_orig = copy.deepcopy(self.Y_train)
+
+        # defining the training medians as the default values 
+        # to replace NaNs during testing
+        
+        if f_pp_test is not None:
+            if 'replace_nan_with_values' in f_pp_test:
+                if a_pp_test is None:
+                    a_pp_test = {}
+                a_pp_test['replace_nan_with_values__val'] = \
+                    self.X_train.median()
+
+        # applying pre-processing functions
+
+        if f_pp is not None:
+            self.preproc_X = PreProcess(f_pp, a_pp)
+            self.X_train = self.preproc_X.apply(self.X_train)
+            if self.has_Y:
+                self.preproc_Y = PreProcess(f_pp,  a_pp, is_Y = True)
+                self.Y_train = self.preproc_Y.apply(self.Y_train)
+                
+        # preparing the testing pre-processing functions
+                            
+        if f_pp_test is not None:
+            self.preproc_X.f_pp = f_pp_test
+            self.preproc_X.a_pp = a_pp_test
+            if self.has_Y:
+                self.preproc_Y.f_pp = f_pp_test
+                self.preproc_Y.a_pp = a_pp_test
+                
+        # aligning the rows of X and Y, if necessary            
+        if self.has_Y:
+            self.X_train, self.Y_train = align_dfs_by_rows(self.X_train,
+                                                            self.Y_train)
+        
+        # saving the tags
+        self.tags_X = self.X_train.columns.to_list()
+        if self.has_Y:
+            self.tags_Y = self.Y_train.columns.to_list()
+          
+    ###########################################################################
+
+    def train (self, lim_conf = 0.99, delete_training_data = False):
+        """
+        Performs the model training. 
+        Must be called after the pre_train function.
+
+        Parameters
+        ----------
+        lim_conf: float, optional
+            Confidence limit for the detection index.
+        delete_training_data: boolean, optional
+            If True, the data is deleted at the end of training.
+            Useful to save memory.
+        """        
+        
+        self.lim_conf = lim_conf
+
+        start_train = time.time()
+        
+        # core of the training algorithm!
+        self.train_core()
+        
+        # predicting! (or reconstructing!)
+        train_pred = self.map_from_X (self.X_train.values)
+
+        end_train = time.time()  
+        
+        self.train_time = end_train - start_train
+        
+        # storing results and calculating SPE
+        
+        if self.has_Y:        
+            self.Y_train_pred = pd.DataFrame(train_pred,
+                                            index=self.Y_train.index,
+                                            columns = self.Y_train.columns)  
+            
+            self.SPE_train = np.sum((self.Y_train.values-
+                                    self.Y_train_pred.values)**2,
+                                    axis=1)
+        else:
+            self.X_train_pred = pd.DataFrame(train_pred,
+                                            index=self.X_train.index,
+                                            columns = self.X_train.columns) 
+
+            self.SPE_train = np.sum((self.X_train.values-
+                                    self.X_train_pred.values)**2,
+                                    axis=1)
+            
+        # calculating indices and detection limits
+
+        self.SPE_mean = self.SPE_train.mean()
+        
+        iSPE = np.sort(self.SPE_train)
+        self.limSPE = iSPE[int(lim_conf*self.X_train.shape[0])]
+        
+        self.limSPE_train = copy.deepcopy(self.limSPE)
+        
+        # denormalizing
+        
+        if self.has_Y and self.preproc_Y is not None:
+            if 'normalize' in self.preproc_Y.f_pp:
+                self.Y_train_pred_orig = \
+                    self.preproc_Y.back_to_units(self.Y_train_pred)
+            else:
+                self.Y_train_pred_orig = self.Y_train_pred
+        else:
+            if 'normalize' in self.preproc_X.f_pp:
+                self.X_train_pred_orig = \
+                    self.preproc_X.back_to_units(self.X_train_pred)
+            else:
+                self.X_train_pred_orig = self.X_train_pred
+
+        # indexes of the training set
+        self.index_train = self.X_train.index
+        
+        self.SPE_train = pd.Series(self.SPE_train, index = self.index_train)
+        
+        # deleting training data, if applicable
+        if delete_training_data:
+            del self.X_train, self.X_train_orig, \
+                self.SPE_train, self.index_train
+            if self.has_Y:
+                del self.Y_train, self.Y_train_orig, \
+                    self.Y_train_pred, self.Y_train_pred_orig
+            else:
+                del self.X_train_pred, self.X_train_pred_orig    
+    
+    ###########################################################################
+    
+    def hyperparameter_tuning (self, params, n_trials = 20, lim_conf = 0.99,
+                               percent_validation = 0.2,
+                               n_splits = None, delete_training_data = False):
+        """
+        Performs hyperparameter tuning using the Optuna library.
+
+        Parameters
+        ----------
+        params: pandas.DataFrame
+            Contains the possibilities to be tested and the types of 
+            parameters. Must be defined as: 
+            pd.DataFrame({'possibilities': [list_possibilities1, 
+                                            list_possibilities2, ...],
+                          'types': [str_type1, 
+                                    str_type2, ...]},
+                         index = [str_param1_name, str_param2_name, ...])
+        n_trials: int, optional
+            Number of trials in the optimization performed by Optuna.
+        lim_conf: float, optional
+            Confidence limit for the detection index.
+        percent_validation: float (0<value<1), optional
+            Percentage of the data to be separated for use 
+            in internal validation, if no cross-validation is performed.
+        n_splits: int, optional
+            Number of sets to be used in cross-validation.
+            If not None, the value of percent_validation is disregarded.
+        delete_training_data: boolean, optional
+            If True, the data is deleted at the end of training.
+            Useful to save memory.
+        """  
+        def objective (trial):
+
+            suggestions = {}
+            
+            for index, row in params.iterrows():
+                if row['type'] == 'uniform':
+                    sug = trial.suggest_uniform(index, 
+                                                row['possibilities'][0], 
+                                                row['possibilities'][1])                  
+                if row['type'] == 'loguniform':
+                    sug = trial.suggest_loguniform(index, 
+                                                row['possibilities'][0], 
+                                                row['possibilities'][1])  
+                if row['type'] == 'discrete_uniform':
+                    sug = trial.suggest_discrete_uniform(index, 
+                                                       row['possibilities'][0], 
+                                                       row['possibilities'][1],
+                                                       row['possibilities'][2])   
+                if row['type'] == 'int':
+                    sug = trial.suggest_int(index, 
+                                            int(row['possibilities'][0]), 
+                                            int(row['possibilities'][1]))
+                if row['type'] == 'categorical':
+                    sug = trial.suggest_categorical(index, 
+                                                    row['possibilities']) 
+                suggestions[index] = sug
+            
+            self.set_hyperparameters(suggestions)
+            
+            if n_splits is not None:
+            
+                kf = sklearn.model_selection.KFold(n_splits = n_splits)
+                            
+                SPEs = []
+                
+                for train_index, test_index in kf.split(self.X_train):
+                    autocopy = copy.deepcopy(self)
+                    autocopy.pre_train(X_train =
+                                       self.X_train.iloc[train_index,:],
+                                       Y_train = 
+                                       self.Y_train.iloc[train_index,:])
+                    autocopy.train(lim_conf, delete_training_data = True)
+                    
+                    autocopy.pre_test(X_test = self.X_train.iloc[test_index,:],
+                                      Y_test = self.Y_train.iloc[test_index,:])
+                    
+                    autocopy.test()
+                    SPEs.append(np.mean(autocopy.SPE_test))
+
+                del autocopy
+                return np.mean(SPEs)
+            
+            else:
+                
+                n = int(self.X_train.shape[0]*percent_validation)
+                
+                autocopy = copy.deepcopy(self)
+                
+                autocopy.pre_train(X_train = self.X_train.iloc[n:,:],
+                                    Y_train = self.Y_train.iloc[n:,:])
+                autocopy.train(lim_conf, delete_training_data = True)
+                autocopy.pre_test(X_test = self.X_train.iloc[:n,:],
+                                    Y_test = self.Y_train.iloc[:n,:])
+                autocopy.test()
+            
+                mean_spe = np.mean(autocopy.SPE_test)
+                del autocopy
+                return mean_spe
+        
+        self.hyperparemeter_study = optuna.create_study()
+        self.hyperparemeter_study.optimize(objective, n_trials = n_trials)
+        
+        print(self.hyperparemeter_study.best_params)
+        
+        self.set_hyperparameters(self.hyperparemeter_study.best_params)
+                   
+    ###########################################################################
+
+    def pre_test (self, X_test, Y_test = None, 
+                  count_window_size = 0, count_limit = 1,
+                  f_pp = None, a_pp = None):
+        '''   
+        Receives a window of data and prepares it for the model testing.
+        
+        Parameters
+        ----------
+        X_test: pandas.DataFrame, pandas.Series or numpy.ndarray
+            Window of data or observation X needed to perform the analysis.
+        Y_test: pandas.DataFrame, pandas.Series or numpy.ndarray, optional
+            Window of data or observation Y needed to perform the analysis.
+        count_window_size: int, optional
+            Window size used in the count alarm calculation.
+        count_limit: int, optional
+            Limit of points to be considered in the window 
+            for the count alarm to trigger. 
+        f_pp: list, optional
+            List containing strings with names of functions to be used 
+            in pre-processing (the functions are defined in the 
+            PreProcess class).
+        a_pp: dict, optional
+            Dictionary containing the parameters to be provided
+            to each function to perform pre-processing of the data, in
+            the format {'functionname__argname': argvalue, ...}
+        '''
+        
+        # window sizes for alarms:
+                        
+        self.count_limit = count_limit
+        self.count_window_size = count_window_size
+
+        # storing complete testing set
+                                
+        if (isinstance(X_test, np.ndarray) and X_test.shape == ()):
+            self.X_test = pd.DataFrame(X_test[None])
+        elif len(X_test.shape)==1 and ((isinstance(X_test, np.ndarray))):
+                self.X_test = pd.DataFrame(X_test).T
+        else:
+            self.X_test = pd.DataFrame(X_test)  
+            
+        if self.has_Y:
+            if (isinstance(Y_test, np.ndarray) and Y_test.shape == ()):
+                self.Y_test = pd.DataFrame(Y_test[None])
+            elif len(Y_test.shape)==1 and ((isinstance(Y_test, np.ndarray))):
+                    self.Y_test = pd.DataFrame(Y_test).T
+            else:
+                self.Y_test = pd.DataFrame(Y_test)
+
+        # data set that will keep the original units       
+                
+        self.X_test_orig = copy.deepcopy(self.X_test)
+        if self.has_Y:
+            self.Y_test_orig = copy.deepcopy(self.Y_test) 
+
+        # applying pre-processing functions
+
+        if f_pp is not None:
+
+            if not hasattr(self, 'preproc_X'):
+                self.preproc_X = PreProcess(f_pp, a_pp)
+            else:
+                self.preproc_X.f_pp = f_pp
+                self.preproc_X.a_pp = a_pp
+
+            if self.has_Y:
+
+                if not hasattr(self, 'preproc_Y'):
+                    self.preproc_Y = PreProcess(f_pp, a_pp, is_Y = True)
+                else:
+                    self.preproc_Y.f_pp = f_pp
+                    self.preproc_Y.a_pp = a_pp
+
+        if hasattr(self, 'preproc_X'):
+            self.X_test = self.preproc_X.apply(self.X_test, 
+                                                train_or_test = 'test')
+
+        if hasattr(self, 'preproc_Y'):
+            self.Y_test = self.preproc_Y.apply(self.Y_test, 
+                                                train_or_test = 'test')  
+
+        # aligning the rows of X and Y, if necessary
+        if self.has_Y:
+            self.X_test, self.Y_test = align_dfs_by_rows(self.X_test,
+                                                         self.Y_test)
+
+        # test tags   
+            
+        self.tags_test_X = [t for t in self.tags_X
+                            if t in self.X_test.columns.tolist()]
+        
+        self.X_test = self.X_test[self.tags_test_X]
+
+        if self.has_Y:
+
+            self.tags_test_Y = [t for t in self.tags_Y 
+                                if t in self.Y_test.columns.tolist()]
+                
+            self.Y_test = self.Y_test[self.tags_test_Y]
+                        
+    ###########################################################################
+
+    def test (self, redefine_limit = False, delete_testing_data = False):
+        """
+        Analyzes a window of data, applying a model test.
+        Must be called after the pre_test function.
+        
+        Parameters
+        ----------
+        redefine_limit: boolean, optional
+            Indicator of redefinition or not of the detection limit during
+            testing.
+        delete_testing_data: boolean, optional
+            If True, the data is deleted at the end of testing.
+            Useful to save memory.
+        """
+
+        start_test = time.time()
+        
+        # predicting!
+        test_pred = self.map_from_X(self.X_test.values)
+
+        end_test = time.time()
+        
+        self.test_time = end_test - start_test
+
+        # storing results and calculating SPE
+    
+        if self.has_Y:
+            self.Y_test_pred = pd.DataFrame(test_pred,
+                                            index=self.Y_test.index,
+                                            columns = self.Y_test.columns)
+            self.SPE_test = np.sum((self.Y_test.values-
+                                    self.Y_test_pred.values)**2,
+                                    axis=1)
+            
+        else:
+            self.X_test_pred = pd.DataFrame(test_pred,
+                                            index=self.X_test.index,
+                                            columns = self.X_test.columns)
+            self.SPE_test = np.sum((self.X_test.values-
+                                    self.X_test_pred.values)**2,
+                                    axis=1)   
+        
+        # redefining the limit, for the validation case
+        
+        if redefine_limit:
+            iSPE = np.sort(self.SPE_test)
+            self.limSPE = iSPE[int(self.lim_conf*self.X_test.shape[0])]
+        
+        # calculations of the alarms
+        
+        if self.count_window_size != 0:
+            self.alarmCount = np.zeros(len(self.SPE_test))
+
+        self.alarmOutlier = detecOutlier(self.SPE_test, 
+                                         self.limSPE)
+
+        # if more window alarms are defined in the package, 
+        # i_min must be the minumum size among them
+        i_min = self.count_window_size
+        
+        for i in range(i_min, len(self.SPE_test)):
+                        
+            if self.count_window_size != 0:
+                if i >= self.count_window_size:
+                    self.alarmCount[i] = \
+                    detecOutlier(self.SPE_test[i-self.count_window_size:(i+1)], 
+                                 self.limSPE, count = True, 
+                                 count_limit = self.count_limit)
+            
+        # adjusting the size of the prediction and denormalizing    
+        if self.has_Y:
+            if 'normalize' in self.preproc_Y.f_pp:
+                self.Y_test_pred_orig = \
+                    self.preproc_Y.back_to_units(self.Y_test_pred)
+            else:
+                self.Y_test_pred_orig = self.Y_test_pred
+        else:
+            if 'normalize' in self.preproc_X.f_pp:
+                self.X_test_pred_orig = \
+                    self.preproc_X.back_to_units(self.X_test_pred)
+            else:
+                self.X_test_pred_orig = self.X_test_pred
+        
+        self.SPE_test = pd.Series(self.SPE_test, 
+                                index = self.X_test.index)
+
+        self.alarms = {}
+
+        self.alarmOutlier = pd.Series(self.alarmOutlier,
+                                    index = self.X_test.index)
+        self.alarms['alarmOutlier'] = self.alarmOutlier
+        if self.count_window_size != 0:
+            self.alarmCount = pd.Series(self.alarmCount,
+                                        index = self.X_test.index)
+            str_count = f'alarmCount WS={self.count_window_size}, '\
+                    f'limCount = {self.count_limit}'
+            self.alarms[str_count] = self.alarmCount
+
+        # deleting testing data, if applicable
+        if delete_testing_data:
+            del self.X_test, self.X_test_orig, \
+                self.SPE_test, self.alarms, self.alarmOutlier
+            if self.has_Y:
+                del self.Y_test, self.Y_test_orig, \
+                    self.Y_test_pred, self.Y_test_pred_orig
+            else:
+                del self.X_test_pred, self.X_test_pred_orig
+            if hasattr(self, 'alarmCount'): del self.alarmCount
+
+    ###########################################################################
+        
+    def plot_SPE (self, ax = None, train_or_test = 'train', logy = True,
+                  legends = True, plot_alarm_outlier = True):
+        """
+        Plotting the temporal evolution of SPE.
+
+        Parameters
+        ----------
+        ax: matplotlib.axes._subplots.AxesSubplot, optional
+            Axis on which the graph will be plotted.
+        train_or_test: string, optional
+            Indicates whether to plot the graph for 'train' or 'test'.
+        logy: boolean, optional
+            Indicates whether the y-axis scale should be logarithmic (True) or 
+            linear (False).
+        legends: boolean, optional
+            If the graph should display legends.
+        plot_alarm_outlier: boolean, optional
+            If the alarmOutlier should be plotted.
+        """
+        
+        if ax is not None:
+            pass
+        else:
+            fig, ax = plt.subplots()
+            
+        if train_or_test == 'train':
+            SPE = self.SPE_train
+            limSPE = self.limSPE_train
+        elif train_or_test == 'test':
+            SPE = self.SPE_test
+            limSPE = self.limSPE
+        
+        SPE.plot(ax=ax, logy = logy, ls='',
+                marker='.', label='SPE')
+        
+        if train_or_test == 'test':
+            for label, alarm in self.alarms.items():
+                if not plot_alarm_outlier and label=='alarmOutlier':
+                    continue
+                (ax.get_ylim()[1]*alarm).replace(0, np.nan).plot(ax = ax, 
+                                                                logy = logy, 
+                                                                ls = '',
+                                                                marker = '.', 
+                                                                alpha = 0.5,
+                                                                label = label)
+                    
+        ax.axhline(limSPE, color='red', ls = '--',
+                label='%.0f%% Confidence Limit' %(self.lim_conf*100))
+        
+        if legends:
+            ax.legend(fontsize=12);
+                        
+    ###########################################################################
+
+    def plot_predictions (self, ax = None, train_or_test = 'train', 
+                          X_pred_to_plot = None, metrics = None):
+        """
+        Plotting the temporal evolution of the predictions along with the
+        respective true values.
+
+        Parameters
+        ----------
+        ax: matplotlib.axes._subplots.AxesSubplot, optional
+            Axis on which the graph will be plotted.
+        train_or_test: string, optional
+            Indicates whether to plot the graph for 'train' or 'test'.
+        X_pred_to_plot: string, optional
+            In case the model is a reconstruction model 
+            (i.e., self.has_Y = False), indicates which column of X to plot 
+            along with the prediction.
+        metrics: list of functions, optional
+            Functions for calculating metrics to be displayed in the title of 
+            the graph.
+        """ 
+
+        if ax is not None:
+            pass
+        else:
+            fig, ax = plt.subplots()
+        
+        if self.has_Y:
+        
+            if train_or_test=='train':
+                true = self.Y_train_orig
+                pred = self.Y_train_pred_orig
+            elif train_or_test=='test':
+                true = self.Y_test_orig
+                pred = self.Y_test_pred_orig
+            
+            regression_or_reconstruction = 'Regression'
+            
+        else:
+            
+            if X_pred_to_plot is not None:
+
+                if train_or_test=='train':
+                    true = self.X_train_orig[X_pred_to_plot]
+                    pred = self.X_train_pred_orig[X_pred_to_plot]
+                elif train_or_test=='test':
+                    true = self.X_test_orig[X_pred_to_plot]
+                    pred = self.X_test_pred_orig[X_pred_to_plot]
+                
+                regression_or_reconstruction = 'Reconstruction'
+                
+            else:
+
+                raise RuntimeError('The model has no Y. \
+                                Specify which variable in X should be plotted')
+                
+        true.plot(ax=ax)
+        pred.plot(ax=ax,ls='--')
+        
+        ax.legend(['Measurement',regression_or_reconstruction])
+        
+        tags = pd.DataFrame(true).columns.to_list()
+                
+        title = str(tags)
+        
+        if metrics is not None:
+            
+            if not isinstance(metrics, list): 
+                metrics = [metrics]
+                                
+            true, pred = align_dfs_by_rows(true.dropna(), pred)
+            
+            for metric in metrics:
+                title = (title+
+                        f'\n{metric.__name__}: {metric(true, pred):.2f}')
+        
+        ax.set_title(title)
+    
+    ###########################################################################
+
+    def fit (self, X_train, Y_train = None,
+             f_pp = ['remove_empty_variables',
+                     'ffill_nan',
+                     'remove_frozen_variables',
+                     'normalize'],
+             a_pp = None,
+             f_pp_test = ['replace_nan_with_values',
+                          'normalize'],
+             a_pp_test = None,
+             lim_conf = 0.99,
+             delete_training_data = False,
+             redefine_limit = False,
+             frac_val = 0.15,
+             tune = False,
+             params = None,
+             params_types = None,
+             params_possibilities = None,
+             n_trials = 20):
+        """
+        Performs the complete pipeline of model training,
+        sequentially executing the 'pre_train' and 'train' methods.
+
+        Parameters
+        ----------
+        X_train: pandas.DataFrame or numpy.ndarray
+            Window of X data used in training.
+        Y_train: pandas.DataFrame or numpy.ndarray, optional
+            Window of Y data used in training.
+        f_pp: list, optional
+            List containing strings with names of functions to be used 
+            in pre-processing the training data (the functions are defined
+            in the PreProcess class, in the BibMon_Tools.py file).
+        f_pp_test: list, optional
+            List containing strings with names of functions to be used 
+            in pre-processing the testing data (the functions are defined 
+            in the PreProcess class, in the BibMon_Tools.py file).
+        a_pp: dict, optional
+            Dictionary containing the parameters to be provided
+            to each function to perform pre-processing of the training data, in
+            the format {'functionname__argname': argvalue, ...}.
+        a_pp_test: dict, optional
+            Dictionary containing the parameters to be provided
+            to each function to perform pre-processing of the testing data, in
+            the format {'functionname__argname': argvalue, ...}.
+        lim_conf: float, optional
+            Confidence limit for the detection index.
+        delete_training_data: boolean, optional
+            If True, the data is deleted at the end of training.
+            Useful to save memory.
+        redefine_limit: boolean, optional
+            Indicator of redefinition or not of the detection limit using
+            a validation period taken from the training data itself.
+        frac_val: float, optional
+            Fraction of the data used for validation. 
+            0<frac_val<1.
+            Only used if redefine_limit==True.
+        tune: boolean, optional
+            Indicator of automatic hyperparameter tuning.
+        params: string or list of strings, optional
+            Name(s) of the parameter(s) to be tuned.
+        params_types:  string or list of strings
+            Type(s) of the parameter(s) to be tuned.
+        params_possibilities: list, optional
+            Possibilities to be tested for each parameter.
+            It must be a list containing the possibilities 
+            (in case of only one parameter), or a list containing the lists
+            for each possibility.
+            Possibilities must be provided according to the type of
+            the parameter, as specified in the Optuna library API.
+        n_trials: int, optional
+            Number of iterations in the hyperparameter search optimization.
+        """
+
+        X_train = pd.DataFrame(X_train)
+        Y_train = pd.DataFrame(Y_train)
+
+        if redefine_limit:
+            
+            n_trn =  int(X_train.shape[0]*(1-frac_val))
+            X_val = X_train.iloc[n_trn:]
+            X_train = X_train.iloc[:n_trn]
+            
+            if Y_train is not None:
+
+                Y_val = Y_train.iloc[n_trn:]
+                Y_train = Y_train.iloc[:n_trn]
+            
+            else:
+                
+                Y_val = None
+            
+        if tune:
+            self.pre_train(X_train, Y_train, 
+                f_pp = f_pp,
+                a_pp = a_pp,
+                f_pp_test = f_pp_test,
+                a_pp_test  = a_pp_test)
+            if not isinstance(params, list):
+                params = [params]
+            if not isinstance(params_types, list):
+                params_types = [params_types]
+            if not isinstance(params_possibilities, list):
+                print('params_possibilities must be a list!')
+            else:
+                if not isinstance(params_possibilities[0], list):
+                    params_possibilities = [params_possibilities]
+            params_df = pd.DataFrame({'possibilities': params_possibilities,
+                                      'type': params_types},
+                                     index = params) 
+            self.tuning(n_trials = n_trials, params = params_df, 
+                        lim_conf = lim_conf, 
+                        delete_training_data = delete_training_data)
+            
+        self.pre_train(X_train, Y_train, 
+                        f_pp = f_pp,
+                        a_pp = a_pp,
+                        f_pp_test = f_pp_test,
+                        a_pp_test  = a_pp_test)
+
+        self.train(lim_conf = lim_conf, 
+                   delete_training_data = delete_training_data)
+
+        if redefine_limit:
+            self.pre_test(X_val, Y_val)
+            self.test(redefine_limit = True)
+        if f_pp_test:   
+            # save value for use in predict if necessary
+            self.f_pp_test = f_pp_test 
+        if a_pp_test:  
+             # save value for use in predict if necessary
+            self.a_pp_test = a_pp_test
+
+    ###########################################################################
+        
+    def predict (self, 
+                 X_test, 
+                 Y_test = None,  
+                 count_window_size = 0, 
+                 count_limit = 1, 
+                 f_pp = 'fit', 
+                 a_pp = 'fit', 
+                 delete_testing_data = False,
+                 redefine_limit = False):
+        '''   
+        Performs the complete pipeline of model prediction (testing), 
+        sequentially executing the 'pre_test' and 'test' methods.
+        
+        Parameters
+        ----------
+        X_test: pandas.DataFrame, pandas.Series or numpy.ndarray
+            Window of data or observation X needed to perform the analysis.
+        Y_test: pandas.DataFrame, pandas.Series or numpy.ndarray, optional
+            Window of data or observation Y needed to perform the analysis.
+        count_window_size: int, optional
+            Window size used in count alarm calculation. 
+        count_limit: int, optional
+            Limit of points to be considered in the window 
+            for the count alarm to trigger.            
+        f_pp: list, optional
+            List containing strings with names of functions to be used 
+            in pre-processing (the functions are defined in the 
+            PreProcess class).
+        a_pp: dict, optional
+            Dictionary containing the parameters to be provided
+            to each function to perform pre-processing of the data, in
+            the format {'functionname__argname': argvalue, ...}
+        delete_testing_data: boolean, optional
+            If True, the data is deleted at the end of testing.
+            Useful to save memory.   
+        redefine_limit: boolean, optional
+            Indicator of redefinition or not of the detection limit during
+            testing.
+        '''
+        
+        if f_pp == 'fit':
+            if hasattr(self,'f_pp_test'):
+                f_pp = self.f_pp_test
+            else:
+                f_pp = None
+        if a_pp == 'fit':
+            if hasattr(self,'a_pp_test'):
+                a_pp = self.a_pp_test
+            else:
+                a_pp = None
+            
+        self.pre_test(X_test, Y_test, count_limit = count_limit, 
+                      count_window_size = count_window_size, 
+                      f_pp = f_pp, a_pp = a_pp)
+        self.test(redefine_limit = redefine_limit,
+                  delete_testing_data = delete_testing_data)
```

### Comparing `bibmon-1.0.0/bibmon/_load_data.py` & `bibmon-1.0.1/bibmon/_load_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,88 @@
-import os
-import pandas as pd
-
-from ._bibmon_tools import create_df_with_dates
-
-###############################################################################
-
-def load_tennessee_eastman (train_id = 0, test_id = 0):
-    """
-    Load the 'Tennessee Eastman Process' benchmark data.
-
-    Parameters
-    ----------
-    train_id: int, optional
-        Identifier of the training data.
-        No fault: 0. With faults: 1 to 20.
-    test_id: int, optional
-        Identifier of the test data.
-        No fault: 0. With faults: 1 to 20.
-    Returns
-    ----------                
-    train_df: pandas.DataFrame
-        Training data.
-    test_df: pandas.DataFrame
-        Test data.
-    """    
-
-    direc = os.path.dirname(__file__)
-    direc = os.path.join(direc,'tennessee_eastman')
-        
-    tags1 = ['XMEAS('+str(ii)+')' for ii in range(1,42)]
-    tags2 = ['XMV('+str(ii)+')' for ii in range(1,12)]
-    tags = tags1 + tags2
-
-    file_train = f'd{train_id}.dat'
-    file_test = f'd{test_id}_te.dat'
-
-    if len(file_train) == 6:
-        file_train = file_train[:2]+'0'+file_train[2:]
-        
-    if len(file_test) == 9:
-        file_test = file_test[:1]+'0'+file_test[1:]
-        
-    if file_train == 'd00.dat':
-        
-        tmp1 = pd.read_csv(os.path.join(direc,'d00.dat'),sep='\t',names=['0'])
-        tmp2 = pd.DataFrame([tmp1.T.iloc[0,i].strip() for 
-                             i in range(tmp1.shape[0])])
-        train_df = pd.DataFrame()
-
-        for ii in range(52):
-            train_df[tags[ii]]=[float(s) for s in tmp2[0][ii].split('  ')]
-            
-        train_df = create_df_with_dates(train_df, 
-                                        freq = '3min')
-        
-    else:
-
-        train_df = create_df_with_dates(pd.read_csv(os.path.join(direc,
-                                                                 file_train), 
-                                                    #delim_whitespace=True, 
-                                                    sep='\s+',
-                                                    names=tags),
-                                        freq = '3min')
-
-    test_df = create_df_with_dates(pd.read_csv(os.path.join(direc,
-                                                            file_test), 
-                                                #delim_whitespace=True,
-                                                sep='\s+', 
-                                                names=tags),
-                                    start = '2020-02-01 00:00:00',
-                                    freq = '3min')
-
-    return train_df, test_df
-
-###############################################################################
-
-def load_real_data ():
-    """
-    Load a sample of real process data.
-    The variables have been anonymized for availability in the library.
-    
-    Returns
-    ----------                
-    : pandas.DataFrame
-        Process data.
-    """    
-    direc = os.path.dirname(__file__)
-    direc = os.path.join(direc, 'real_process_data')
-    file = 'real_process_data.csv'
-        
-    return pd.read_csv(os.path.join(direc,file),
-                       index_col = 0, 
-                       parse_dates = True)
+import os
+import pandas as pd
+import importlib.resources as pkg_resources
+
+from ._bibmon_tools import create_df_with_dates
+from . import real_process_data, tennessee_eastman 
+
+###############################################################################
+
+def load_tennessee_eastman (train_id = 0, test_id = 0):
+    """
+    Load the 'Tennessee Eastman Process' benchmark data.
+
+    Parameters
+    ----------
+    train_id: int, optional
+        Identifier of the training data.
+        No fault: 0. With faults: 1 to 20.
+    test_id: int, optional
+        Identifier of the test data.
+        No fault: 0. With faults: 1 to 20.
+    Returns
+    ----------                
+    train_df: pandas.DataFrame
+        Training data.
+    test_df: pandas.DataFrame
+        Test data.
+    """    
+        
+    tags1 = ['XMEAS('+str(ii)+')' for ii in range(1,42)]
+    tags2 = ['XMV('+str(ii)+')' for ii in range(1,12)]
+    tags = tags1 + tags2
+    
+    file_train = f'd{train_id}.dat'
+    file_test = f'd{test_id}_te.dat'
+
+    if len(file_train) == 6:
+        file_train = file_train[:2]+'0'+file_train[2:]
+        
+    if len(file_test) == 9:
+        file_test = file_test[:1]+'0'+file_test[1:]
+
+    with pkg_resources.path(tennessee_eastman, file_train) as filepath:
+
+        if file_train == 'd00.dat':
+            
+            tmp1 = pd.read_csv(filepath,sep='\t',
+                               names=['0'])
+            tmp2 = pd.DataFrame([tmp1.T.iloc[0,i].strip() for 
+                                i in range(tmp1.shape[0])])
+            train_df = pd.DataFrame()
+
+            for ii in range(52):
+                train_df[tags[ii]]=[float(s) for s in tmp2[0][ii].split('  ')]
+                
+            train_df = create_df_with_dates(train_df, 
+                                            freq = '3min')
+            
+        else:
+
+            train_df = create_df_with_dates(filepath, sep='\s+',names=tags,
+                                            freq = '3min')
+
+    with pkg_resources.path(tennessee_eastman, file_test) as filepath:
+
+        test_df = create_df_with_dates(pd.read_csv(filepath, 
+                                                   sep = '\s+', 
+                                                   names = tags),
+                                       start = '2020-02-01 00:00:00',
+                                       freq = '3min')
+
+    return train_df, test_df
+
+###############################################################################
+
+def load_real_data ():
+    """
+    Load a sample of real process data.
+    The variables have been anonymized for availability in the library.
+    
+    Returns
+    ----------                
+    : pandas.DataFrame
+        Process data.
+    """    
+
+    with pkg_resources.path(real_process_data,'real_process_data.csv') as file:
+        return pd.read_csv(file,index_col = 0, parse_dates = True)
```

### Comparing `bibmon-1.0.0/bibmon/_pca.py` & `bibmon-1.0.1/bibmon/_pca.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-import numpy as np
-import matplotlib.pyplot as plt
-
-from ._generic_model import GenericModel
-
-###############################################################################
-
-class PCA (GenericModel):
-    """
-    Principal Component Analysis.
-    
-    For details on the technique, see https://doi.org/10.3390/pr12020251
-    
-    Parameters
-    ----------
-    ncomp: int or float
-           float: number between 0.0 and 1.0 that corresponds to the minimum 
-                  fraction of accumulated variance for component selection;
-           int: defines the number of components.
-    """
-
-    ###########################################################################
-            
-    def __init__ (self, ncomp=0.9):
-
-        self.has_Y = False
-        self.ncomp = ncomp
-        self.name = 'PCA'
-        
-    ###########################################################################
-    
-    def load_model (self,limSPE, SPE_mean, count_window_size,
-                    Mux, SDx, S, V, n):
-        
-        """
-        Receives parameters from a previously trained model to
-        perform predictions and tests without the need for training.
-    
-        Parameters
-        ----------
-        Mux: pandas.Series
-            Means of the X variables in the training period.
-        SDx: pandas.Series
-            Standard deviations of the X variables in the training period.
-        Mux: pandas.Series, optional
-            Means of the Y variables in the training period.
-        SDx: pandas.Series, optional
-            Standard deviations of the Y variables in the training period.                         
-        limSPE: float
-            Detection limit and mean of the SPE.
-        SPE_mean: float
-            Mean of the SPE.
-        count_window_size: int
-            Window sizes used in the count alarms calculation.        
-        S: numpy.array
-            Specific parameter of PCA.
-        V: numpy.array
-            Specific parameter of PCA.
-        n: int
-            Specific parameter of PCA.        
-        """            
-                
-        super().load_model (limSPE, SPE_mean,
-                            count_window_size, Mux, SDx)
-        
-        self.S = np.array(S)
-        self.V = np.array(V)
-        self.n = n
-        
-        self.pv = S/np.sum(S)
-        self.pva = np.cumsum(S)/sum(S)
-
-    ###########################################################################
-        
-    def train_core (self):
-
-        self.Sxx_train = np.cov(self.X_train, rowvar=False)
-        _, self.S, self.Vh = np.linalg.svd(self.Sxx_train)
-        self.V = self.Vh.T
-        self.pv = self.S/np.sum(self.S)
-        self.pva = np.cumsum(self.S)/sum(self.S)
-
-        if self.ncomp> 0 and self.ncomp < 1:
-            self.n = np.where(self.pva>self.ncomp)[0][0]+1
-        elif self.ncomp >= 1:
-            self.n = self.ncomp
-        else:
-            # Error: unkown self.n
-            self.n = None
-                
-    ###########################################################################
-
-    def map_from_X (self, X): 
-
-        X_train_proj = X@self.V[:,:self.n]
-        return X_train_proj@self.V[:,:self.n].T
-    
-    ###########################################################################
-        
-    def plot_cumulative_variance (self, ax = None):
-        """
-        Plots the cumulative variance.
-    
-        Parameters
-        ----------
-        ax: matplotlib.axes._subplots.AxesSubplot, optional
-            Axis on which the graph will be plotted.
-        """                
-        if ax is not None:
-            pass
-        else:
-            fig, ax = plt.subplots()
-        
-        ax.bar(np.arange(len(self.pv)), self.pv)
-        ax.plot(np.arange(len(self.pv)), self.pva)
-        ax.set_xlabel('Number of components')
+import numpy as np
+import matplotlib.pyplot as plt
+
+from ._generic_model import GenericModel
+
+###############################################################################
+
+class PCA (GenericModel):
+    """
+    Principal Component Analysis.
+    
+    For details on the technique, see https://doi.org/10.3390/pr12020251
+    
+    Parameters
+    ----------
+    ncomp: int or float
+           float: number between 0.0 and 1.0 that corresponds to the minimum 
+                  fraction of accumulated variance for component selection;
+           int: defines the number of components.
+    """
+
+    ###########################################################################
+            
+    def __init__ (self, ncomp=0.9):
+
+        self.has_Y = False
+        self.ncomp = ncomp
+        self.name = 'PCA'
+        
+    ###########################################################################
+    
+    def load_model (self,limSPE, SPE_mean, count_window_size,
+                    Mux, SDx, S, V, n):
+        
+        """
+        Receives parameters from a previously trained model to
+        perform predictions and tests without the need for training.
+    
+        Parameters
+        ----------
+        Mux: pandas.Series
+            Means of the X variables in the training period.
+        SDx: pandas.Series
+            Standard deviations of the X variables in the training period.
+        Mux: pandas.Series, optional
+            Means of the Y variables in the training period.
+        SDx: pandas.Series, optional
+            Standard deviations of the Y variables in the training period.                         
+        limSPE: float
+            Detection limit and mean of the SPE.
+        SPE_mean: float
+            Mean of the SPE.
+        count_window_size: int
+            Window sizes used in the count alarms calculation.        
+        S: numpy.array
+            Specific parameter of PCA.
+        V: numpy.array
+            Specific parameter of PCA.
+        n: int
+            Specific parameter of PCA.        
+        """            
+                
+        super().load_model (limSPE, SPE_mean,
+                            count_window_size, Mux, SDx)
+        
+        self.S = np.array(S)
+        self.V = np.array(V)
+        self.n = n
+        
+        self.pv = S/np.sum(S)
+        self.pva = np.cumsum(S)/sum(S)
+
+    ###########################################################################
+        
+    def train_core (self):
+
+        self.Sxx_train = np.cov(self.X_train, rowvar=False)
+        _, self.S, self.Vh = np.linalg.svd(self.Sxx_train)
+        self.V = self.Vh.T
+        self.pv = self.S/np.sum(self.S)
+        self.pva = np.cumsum(self.S)/sum(self.S)
+
+        if self.ncomp> 0 and self.ncomp < 1:
+            self.n = np.where(self.pva>self.ncomp)[0][0]+1
+        elif self.ncomp >= 1:
+            self.n = self.ncomp
+        else:
+            # Error: unkown self.n
+            self.n = None
+                
+    ###########################################################################
+
+    def map_from_X (self, X): 
+
+        X_train_proj = X@self.V[:,:self.n]
+        return X_train_proj@self.V[:,:self.n].T
+    
+    ###########################################################################
+        
+    def plot_cumulative_variance (self, ax = None):
+        """
+        Plots the cumulative variance.
+    
+        Parameters
+        ----------
+        ax: matplotlib.axes._subplots.AxesSubplot, optional
+            Axis on which the graph will be plotted.
+        """                
+        if ax is not None:
+            pass
+        else:
+            fig, ax = plt.subplots()
+        
+        ax.bar(np.arange(len(self.pv)), self.pv)
+        ax.plot(np.arange(len(self.pv)), self.pva)
+        ax.set_xlabel('Number of components')
         ax.set_ylabel('Data variance')
```

### Comparing `bibmon-1.0.0/bibmon/_preprocess.py` & `bibmon-1.0.1/bibmon/_preprocess.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,394 +1,394 @@
-import copy
-import pandas as pd
-import statsmodels.tsa.tsatools
-
-###############################################################################
-
-class PreProcess ():
-    """
-    Class used to encapsulate data preprocessing methods.
-    
-    Parameters
-    ----------
-            
-        f_pp: list, optional
-            List containing strings with names of methods to be used 
-            in the preprocessing of the train data. The list of methods 
-            is shown below.
-        a_pp: dict, optional
-            Dictionary containing the parameters to be provided
-            to each function to perform preprocessing of the train data, in
-            the format {'functionname__argname': argvalue, ...}
-        is_Y: boolean, optional
-            If the data being preprocessed is Y (that is, to be predicted).
-        
-    Methods:
-    
-    * Variable selection:
-        remove_empty_variables();
-        remove_frozen_variables()
-        
-    * Missing values imputation:
-        ffill()
-        remove_observations_with_nan();
-        replace_nan_with_values()
-        
-    * Normalization:
-        back_to_units();
-        normalize()
-        
-    * Adding dynamics:
-        apply_lag();
-        add_moving_average()
-        
-    * Noise treatment:
-        moving_average_filter()       
-    
-    """
-            
-    ###########################################################################
-    
-    def __init__(self, f_pp = None, a_pp = None, is_Y = False):
- 
-        self.is_Y = is_Y
-        self.f_pp = f_pp        
-        self._a_pp = a_pp     
-        if self.f_pp is not None:
-            self.params_per_func = {f: {} for f in f_pp}        
-
-    ###########################################################################
-
-    @property
-    def a_pp(self):
-        return self._a_pp
-
-    ###########################################################################
-    
-    @a_pp.setter
-    def a_pp(self, a_pp):
-
-        self._a_pp = a_pp
-        
-        if self.f_pp is not None:
-        
-            self.params_per_func = {f: {} for f in self.f_pp}
-            
-            if a_pp is not None:
-                                
-                for pname, pval in a_pp.items():
-                    func, param = pname.split('__',1)
-                    self.params_per_func[func][param] = pval
-
-    ###########################################################################
-    
-    def apply(self, df, train_or_test = 'train'):
-        """
-        Sequentially applies the preprocessing functions 
-        defined during initialization.
-    
-        Parameters
-        ----------
-        df: pandas.DataFrame
-            Data to be processed.
-        train_or_test: string, optional
-            Indicates which step the data corresponds to.
-        Returns
-        ----------                
-        : pandas.DataFrame
-           Processed data.
-        """         
-        
-        df_processed = df
-        
-        for i in range(len(self.f_pp)):
-            f = self.f_pp[i]
-            df_processed = getattr(self, f)(df_processed,
-                                            train_or_test, 
-                                            **self.params_per_func[f])
-                
-        return df_processed
-    
-    ######################### 
-    # VARIABLE SELECTION 
-    #########################
-
-    ###########################################################################
-
-    def remove_empty_variables (self, df, train_or_test = 'train'):
-        """
-        Removes variables with no values.
-    
-        Parameters
-        ----------
-        df: pandas.DataFrame
-            Data to be processed.
-        train_or_test: string, optional
-            Indicates which step the data corresponds to.
-        Returns
-        ----------                
-        : pandas.DataFrame
-           Processed data.
-        """           
-        if train_or_test == 'train':
-            return df.dropna(axis=1, how='all')
-        elif train_or_test == 'test':
-            return df
-
-    ###########################################################################
-
-    def remove_frozen_variables (self, df, train_or_test = 'train',
-                                 threshold = 1e-6): 
-        """
-        Removes variables whose variation falls below a given limit.
-    
-        Parameters
-        ----------
-        df: pandas.DataFrame
-            Data to be processed.
-        train_or_test: string, optional
-            Indicates which step the data corresponds to.
-        threshold: float, optional
-            Variance limit to consider a variable as frozen.
-        Returns
-        ----------                
-        : pandas.DataFrame
-           Processed data.
-        """                                              
-        if not self.is_Y:
-            if train_or_test == 'train':
-                return df.loc[:, df.var(ddof=1) > threshold]
-            elif train_or_test == 'test':
-                return df
-        else:
-            return df
-        
-    ################################## 
-    # MISSING VALUES IMPUTATION
-    ##################################
-        
-    ###########################################################################
-    
-    def ffill_nan (self, df, train_or_test = 'train'):
-        """
-        Fills missing (NaN) values with the last valid value.
-        Uses the next valid value if there is no last available.
-    
-        Parameters
-        ----------
-        df: pandas.DataFrame
-            Data to be processed.
-        train_or_test: string, optional
-            Indicates which step the data corresponds to.
-        Returns
-        ----------                
-        : pandas.DataFrame
-           Processed data.
-        """    
-        return df.ffill().bfill()
-
-    ###########################################################################
-    
-    def remove_observations_with_nan (self, df, train_or_test = 'train'):
-        """
-        Removes observations with missing data (NaN).
-    
-        Parameters
-        ----------
-        df: pandas.DataFrame
-            Data to be processed.
-        train_or_test: string, optional
-            Indicates which step the data corresponds to.
-        Returns
-        ----------                
-        : pandas.DataFrame
-           Processed data.
-        """    
-        return df.dropna(axis=0, how='any')
-    
-    ###########################################################################
-
-    def replace_nan_with_values (self, df, train_or_test = 'train', val = 0):
-        """
-        Replaces missing data (NaN) with a predefined value.
-
-        Parameters
-        ----------
-        df: pandas.DataFrame
-            Data to be processed.
-        train_or_test: string, optional
-            Indicates which step the data corresponds to.
-        val: int or float
-            Value to be used in the replacement.
-        Returns
-        ----------                
-        : pandas.DataFrame
-        Processed data.
-        """    
-                                    
-        return df.fillna(val)
-
-    ###############
-    # NORMALIZATION
-    ###############
-
-    ###########################################################################
-
-    def back_to_units (self, df):
-        """
-        Returns the variables to the original scale, 
-        reverting effects of a normalization.
-
-        Parameters
-        ----------
-        df: pandas.DataFrame
-            Data to be processed.
-        Returns
-        ----------                
-        : pandas.DataFrame
-        Processed data.
-        """    
-        return df*self.SD + self.Mu
-    
-    ###########################################################################
-
-    def normalize (self, df, train_or_test = 'train', mode = 'standard'):
-        """
-        Variable normalization.
-
-        Parameters
-        ----------
-        df: pandas.DataFrame
-            Data to be processed.
-        train_or_test: string, optional
-            Indicates which step the data corresponds to.
-        mode: string, optional
-            Type of normalization (standard, robust, m-robust or s-robust).
-        Returns
-        ----------                
-        : pandas.DataFrame
-        Processed data.
-        """    
-        if train_or_test == 'train':
-            
-            if mode == 'standard':
-                self.Mu = df.mean()
-                self.SD = df.std(ddof=1)
-            elif mode == 'robust':
-                self.Mu = df.median()
-                self.SD = df.mad()               
-            elif mode == 'm-robust':
-                self.Mu = df.median()
-                self.SD = df.std(ddof=1)
-            elif mode == 's-robust':
-                self.Mu = df.mean()
-                self.SD = df.mad()               
-            
-            return (df - self.Mu)/self.SD
-        
-        elif train_or_test == 'test':
-        
-            return (df - self.Mu)/self.SD
-
-    ##############################
-    # ADDING DYNAMICS
-    ##############################
-        
-    ###########################################################################
-
-    def apply_lag (self, df, train_or_test = 'train', lag = 1):
-        """
-        Generation of time-delayed variables.
-
-        Parameters
-        ----------
-        df: pandas.DataFrame
-            Data to be processed.
-        train_or_test: string, optional
-            Indicates which step the data corresponds to.
-        lag: int, optional
-            Number of delays to be considered.
-        Returns
-        ----------                
-        : pandas.DataFrame
-        Processed data.
-        """    
-                        
-        if self.is_Y:
-            return df.iloc[lag:,:]
-        else:    
-            array_lagged = statsmodels.tsa.tsatools.lagmat(df, maxlag = lag, 
-                                                           trim = "forward", 
-                                                       original = 'in')[lag:,:]   
-            new_columns = []
-            for l in range(lag):
-                new_columns.append(df.columns+' - lag '+str(l+1))
-            columns_lagged = df.columns.append(new_columns)
-            index_lagged = df.index[lag:]
-            df_lagged = pd.DataFrame(array_lagged, index = index_lagged,
-                                     columns = columns_lagged)
-            
-            return df_lagged  
-        
-    ###########################################################################
-
-    def add_moving_average (self, df, train_or_test = 'train', WS = 10):
-        """
-        Adding variables filtered by moving average.
-        Attention! Do not confuse with moving_average_filter, in which
-        the original variables are not kept in the dataset.
-
-        Parameters
-        ----------
-        df: pandas.DataFrame
-            Data to be processed.
-        train_or_test: string, optional
-            Indicates which step the data corresponds to.
-        WS: int, optional
-            Window size of the filter.
-        Returns
-        ----------                
-        : pandas.DataFrame
-        Processed data.
-        """    
-        if self.is_Y:
-            return df
-                
-        new_df = copy.deepcopy(df)
-                
-        for column in df:
-            new_df[column+' MA'] = new_df[column].rolling(WS).mean()
-        
-        return new_df.drop(df.index[:WS])
-
-    ##############################
-    # NOISE TREATMENT
-    ##############################
-
-    ###########################################################################
-
-    def moving_average_filter (self, df,  train_or_test = 'train', WS = 10):
-        """
-        Moving average noise filter.
-
-        Parameters
-        ----------
-        df: pandas.DataFrame
-            Data to be processed.
-        train_or_test: string, optional
-            Indicates which step the data corresponds to.
-        WS: int, optional
-            Window size of the filter.
-        Returns
-        ----------                
-        : pandas.DataFrame
-        Processed data.
-        """    
-        new_df = copy.deepcopy(df)
-                
-        for column in df:
-            new_df[column] = new_df[column].rolling(WS).mean()
-            
-        if hasattr(df,'name'):
-            new_df.name = df.name
-                        
+import copy
+import pandas as pd
+import statsmodels.tsa.tsatools
+
+###############################################################################
+
+class PreProcess ():
+    """
+    Class used to encapsulate data preprocessing methods.
+    
+    Parameters
+    ----------
+            
+        f_pp: list, optional
+            List containing strings with names of methods to be used 
+            in the preprocessing of the train data. The list of methods 
+            is shown below.
+        a_pp: dict, optional
+            Dictionary containing the parameters to be provided
+            to each function to perform preprocessing of the train data, in
+            the format {'functionname__argname': argvalue, ...}
+        is_Y: boolean, optional
+            If the data being preprocessed is Y (that is, to be predicted).
+        
+    Methods:
+    
+    * Variable selection:
+        remove_empty_variables();
+        remove_frozen_variables()
+        
+    * Missing values imputation:
+        ffill()
+        remove_observations_with_nan();
+        replace_nan_with_values()
+        
+    * Normalization:
+        back_to_units();
+        normalize()
+        
+    * Adding dynamics:
+        apply_lag();
+        add_moving_average()
+        
+    * Noise treatment:
+        moving_average_filter()       
+    
+    """
+            
+    ###########################################################################
+    
+    def __init__(self, f_pp = None, a_pp = None, is_Y = False):
+ 
+        self.is_Y = is_Y
+        self.f_pp = f_pp        
+        self._a_pp = a_pp     
+        if self.f_pp is not None:
+            self.params_per_func = {f: {} for f in f_pp}        
+
+    ###########################################################################
+
+    @property
+    def a_pp(self):
+        return self._a_pp
+
+    ###########################################################################
+    
+    @a_pp.setter
+    def a_pp(self, a_pp):
+
+        self._a_pp = a_pp
+        
+        if self.f_pp is not None:
+        
+            self.params_per_func = {f: {} for f in self.f_pp}
+            
+            if a_pp is not None:
+                                
+                for pname, pval in a_pp.items():
+                    func, param = pname.split('__',1)
+                    self.params_per_func[func][param] = pval
+
+    ###########################################################################
+    
+    def apply(self, df, train_or_test = 'train'):
+        """
+        Sequentially applies the preprocessing functions 
+        defined during initialization.
+    
+        Parameters
+        ----------
+        df: pandas.DataFrame
+            Data to be processed.
+        train_or_test: string, optional
+            Indicates which step the data corresponds to.
+        Returns
+        ----------                
+        : pandas.DataFrame
+           Processed data.
+        """         
+        
+        df_processed = df
+        
+        for i in range(len(self.f_pp)):
+            f = self.f_pp[i]
+            df_processed = getattr(self, f)(df_processed,
+                                            train_or_test, 
+                                            **self.params_per_func[f])
+                
+        return df_processed
+    
+    ######################### 
+    # VARIABLE SELECTION 
+    #########################
+
+    ###########################################################################
+
+    def remove_empty_variables (self, df, train_or_test = 'train'):
+        """
+        Removes variables with no values.
+    
+        Parameters
+        ----------
+        df: pandas.DataFrame
+            Data to be processed.
+        train_or_test: string, optional
+            Indicates which step the data corresponds to.
+        Returns
+        ----------                
+        : pandas.DataFrame
+           Processed data.
+        """           
+        if train_or_test == 'train':
+            return df.dropna(axis=1, how='all')
+        elif train_or_test == 'test':
+            return df
+
+    ###########################################################################
+
+    def remove_frozen_variables (self, df, train_or_test = 'train',
+                                 threshold = 1e-6): 
+        """
+        Removes variables whose variation falls below a given limit.
+    
+        Parameters
+        ----------
+        df: pandas.DataFrame
+            Data to be processed.
+        train_or_test: string, optional
+            Indicates which step the data corresponds to.
+        threshold: float, optional
+            Variance limit to consider a variable as frozen.
+        Returns
+        ----------                
+        : pandas.DataFrame
+           Processed data.
+        """                                              
+        if not self.is_Y:
+            if train_or_test == 'train':
+                return df.loc[:, df.var(ddof=1) > threshold]
+            elif train_or_test == 'test':
+                return df
+        else:
+            return df
+        
+    ################################## 
+    # MISSING VALUES IMPUTATION
+    ##################################
+        
+    ###########################################################################
+    
+    def ffill_nan (self, df, train_or_test = 'train'):
+        """
+        Fills missing (NaN) values with the last valid value.
+        Uses the next valid value if there is no last available.
+    
+        Parameters
+        ----------
+        df: pandas.DataFrame
+            Data to be processed.
+        train_or_test: string, optional
+            Indicates which step the data corresponds to.
+        Returns
+        ----------                
+        : pandas.DataFrame
+           Processed data.
+        """    
+        return df.ffill().bfill()
+
+    ###########################################################################
+    
+    def remove_observations_with_nan (self, df, train_or_test = 'train'):
+        """
+        Removes observations with missing data (NaN).
+    
+        Parameters
+        ----------
+        df: pandas.DataFrame
+            Data to be processed.
+        train_or_test: string, optional
+            Indicates which step the data corresponds to.
+        Returns
+        ----------                
+        : pandas.DataFrame
+           Processed data.
+        """    
+        return df.dropna(axis=0, how='any')
+    
+    ###########################################################################
+
+    def replace_nan_with_values (self, df, train_or_test = 'train', val = 0):
+        """
+        Replaces missing data (NaN) with a predefined value.
+
+        Parameters
+        ----------
+        df: pandas.DataFrame
+            Data to be processed.
+        train_or_test: string, optional
+            Indicates which step the data corresponds to.
+        val: int or float
+            Value to be used in the replacement.
+        Returns
+        ----------                
+        : pandas.DataFrame
+        Processed data.
+        """    
+                                    
+        return df.fillna(val)
+
+    ###############
+    # NORMALIZATION
+    ###############
+
+    ###########################################################################
+
+    def back_to_units (self, df):
+        """
+        Returns the variables to the original scale, 
+        reverting effects of a normalization.
+
+        Parameters
+        ----------
+        df: pandas.DataFrame
+            Data to be processed.
+        Returns
+        ----------                
+        : pandas.DataFrame
+        Processed data.
+        """    
+        return df*self.SD + self.Mu
+    
+    ###########################################################################
+
+    def normalize (self, df, train_or_test = 'train', mode = 'standard'):
+        """
+        Variable normalization.
+
+        Parameters
+        ----------
+        df: pandas.DataFrame
+            Data to be processed.
+        train_or_test: string, optional
+            Indicates which step the data corresponds to.
+        mode: string, optional
+            Type of normalization (standard, robust, m-robust or s-robust).
+        Returns
+        ----------                
+        : pandas.DataFrame
+        Processed data.
+        """    
+        if train_or_test == 'train':
+            
+            if mode == 'standard':
+                self.Mu = df.mean()
+                self.SD = df.std(ddof=1)
+            elif mode == 'robust':
+                self.Mu = df.median()
+                self.SD = df.mad()               
+            elif mode == 'm-robust':
+                self.Mu = df.median()
+                self.SD = df.std(ddof=1)
+            elif mode == 's-robust':
+                self.Mu = df.mean()
+                self.SD = df.mad()               
+            
+            return (df - self.Mu)/self.SD
+        
+        elif train_or_test == 'test':
+        
+            return (df - self.Mu)/self.SD
+
+    ##############################
+    # ADDING DYNAMICS
+    ##############################
+        
+    ###########################################################################
+
+    def apply_lag (self, df, train_or_test = 'train', lag = 1):
+        """
+        Generation of time-delayed variables.
+
+        Parameters
+        ----------
+        df: pandas.DataFrame
+            Data to be processed.
+        train_or_test: string, optional
+            Indicates which step the data corresponds to.
+        lag: int, optional
+            Number of delays to be considered.
+        Returns
+        ----------                
+        : pandas.DataFrame
+        Processed data.
+        """    
+                        
+        if self.is_Y:
+            return df.iloc[lag:,:]
+        else:    
+            array_lagged = statsmodels.tsa.tsatools.lagmat(df, maxlag = lag, 
+                                                           trim = "forward", 
+                                                       original = 'in')[lag:,:]   
+            new_columns = []
+            for l in range(lag):
+                new_columns.append(df.columns+' - lag '+str(l+1))
+            columns_lagged = df.columns.append(new_columns)
+            index_lagged = df.index[lag:]
+            df_lagged = pd.DataFrame(array_lagged, index = index_lagged,
+                                     columns = columns_lagged)
+            
+            return df_lagged  
+        
+    ###########################################################################
+
+    def add_moving_average (self, df, train_or_test = 'train', WS = 10):
+        """
+        Adding variables filtered by moving average.
+        Attention! Do not confuse with moving_average_filter, in which
+        the original variables are not kept in the dataset.
+
+        Parameters
+        ----------
+        df: pandas.DataFrame
+            Data to be processed.
+        train_or_test: string, optional
+            Indicates which step the data corresponds to.
+        WS: int, optional
+            Window size of the filter.
+        Returns
+        ----------                
+        : pandas.DataFrame
+        Processed data.
+        """    
+        if self.is_Y:
+            return df
+                
+        new_df = copy.deepcopy(df)
+                
+        for column in df:
+            new_df[column+' MA'] = new_df[column].rolling(WS).mean()
+        
+        return new_df.drop(df.index[:WS])
+
+    ##############################
+    # NOISE TREATMENT
+    ##############################
+
+    ###########################################################################
+
+    def moving_average_filter (self, df,  train_or_test = 'train', WS = 10):
+        """
+        Moving average noise filter.
+
+        Parameters
+        ----------
+        df: pandas.DataFrame
+            Data to be processed.
+        train_or_test: string, optional
+            Indicates which step the data corresponds to.
+        WS: int, optional
+            Window size of the filter.
+        Returns
+        ----------                
+        : pandas.DataFrame
+        Processed data.
+        """    
+        new_df = copy.deepcopy(df)
+                
+        for column in df:
+            new_df[column] = new_df[column].rolling(WS).mean()
+            
+        if hasattr(df,'name'):
+            new_df.name = df.name
+                        
         return new_df.drop(df.index[:WS])
```

### Comparing `bibmon-1.0.0/bibmon/_template_generic_model_childs.py` & `bibmon-1.0.1/bibmon/_template_generic_model_childs.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-from .generic_model import GenericModel
-
-class NewModel (GenericModel):
-    
-    ###########################################################################
-            
-    def __init__ (self):
-        """
-        Constructor.
-
-        Here, the variable has_Y should be specified.
-        This variable indicates whether the model has a 
-        separate set of prediction variables Y or not.
-
-        It is recommended to inform model initialization parameters here.
-        """
-        self.has_Y = False # or True!
-        
-    ###########################################################################
-    
-    def load_model (self,
-                         limSPE, SPE_mean, lagX, count_window_size,
-                         Mux, SDx, Muy = None, SDy = None,
-                         # potential additional parameters,
-                         ):
-        
-        super().load_model (limSPE, SPE_mean, count_window_size, 
-                            Mux, SDx, Muy, SDy)
-        
-        """
-        Receives parameters from a previously trained model for
-        making predictions and tests without the need for training.
-        
-        !!
-        Below, you should store additional parameters as attributes 
-        of the class; if there are no additional parameters, 
-        this method can be deleted.
-        !!
-    
-        Parameters:
-        ----------
-        Mux: pandas.Series
-            Means of the X variables in the training period.
-        SDx: pandas.Series
-            Standard deviations of the X variables in
-            the training period.
-        Muy: pandas.Series, optional
-            Means of the Y variables in the training period.
-        SDy: pandas.Series, optional
-            Standard deviations of the Y variables in the training period.                         
-        limSPE: float
-            Detection limit and mean of the SPE.
-        SPE_mean: float
-            Mean of the SPE.
-        count_window_size: int
-            Window sizes used in count alarms calculation.
-        """
-
-    ###########################################################################
-        
-    def train_core (self):
-        """
-        The core of the training algorithm, that is,
-        all the necessary steps between pre_train() and
-        the calculation of the prediction in training.
-        """
-
-    ###########################################################################
-
-    def map_from_X (self, X): 
-        """
-        Receives a data matrix X and returns a matrix of predicted 
-        or reconstructed values.
-
-        Parameters
-        ----------
-        X: numpy.array
-            Window X of data for prediction or reconstruction.  
-            
-        Returns
-        ----------                
-        : numpy.array
-            Reconstructed X (or predicted Y).
+from .generic_model import GenericModel
+
+class NewModel (GenericModel):
+    
+    ###########################################################################
+            
+    def __init__ (self):
+        """
+        Constructor.
+
+        Here, the variable has_Y should be specified.
+        This variable indicates whether the model has a 
+        separate set of prediction variables Y or not.
+
+        It is recommended to inform model initialization parameters here.
+        """
+        self.has_Y = False # or True!
+        
+    ###########################################################################
+    
+    def load_model (self,
+                         limSPE, SPE_mean, lagX, count_window_size,
+                         Mux, SDx, Muy = None, SDy = None,
+                         # potential additional parameters,
+                         ):
+        
+        super().load_model (limSPE, SPE_mean, count_window_size, 
+                            Mux, SDx, Muy, SDy)
+        
+        """
+        Receives parameters from a previously trained model for
+        making predictions and tests without the need for training.
+        
+        !!
+        Below, you should store additional parameters as attributes 
+        of the class; if there are no additional parameters, 
+        this method can be deleted.
+        !!
+    
+        Parameters:
+        ----------
+        Mux: pandas.Series
+            Means of the X variables in the training period.
+        SDx: pandas.Series
+            Standard deviations of the X variables in
+            the training period.
+        Muy: pandas.Series, optional
+            Means of the Y variables in the training period.
+        SDy: pandas.Series, optional
+            Standard deviations of the Y variables in the training period.                         
+        limSPE: float
+            Detection limit and mean of the SPE.
+        SPE_mean: float
+            Mean of the SPE.
+        count_window_size: int
+            Window sizes used in count alarms calculation.
+        """
+
+    ###########################################################################
+        
+    def train_core (self):
+        """
+        The core of the training algorithm, that is,
+        all the necessary steps between pre_train() and
+        the calculation of the prediction in training.
+        """
+
+    ###########################################################################
+
+    def map_from_X (self, X): 
+        """
+        Receives a data matrix X and returns a matrix of predicted 
+        or reconstructed values.
+
+        Parameters
+        ----------
+        X: numpy.array
+            Window X of data for prediction or reconstruction.  
+            
+        Returns
+        ----------                
+        : numpy.array
+            Reconstructed X (or predicted Y).
         """
```

### Comparing `bibmon-1.0.0/bibmon.egg-info/PKG-INFO` & `bibmon-1.0.1/bibmon.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibmon
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library with routines for data-driven process monitoring.
 Home-page: https://github.com/petrobras/bibmon
 Author: BibMon developers
 Author-email: cc-bibmon@petrobras.com.br
 License: Apache 2.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -21,17 +21,17 @@
 # BibMon
 
 `BibMon` (from the Portuguese ***Bib**lioteca de **Mon**itoramento de Processos*, or Process Monitoring Library) is a Python package that provides deviation-based predictive models for fault detection, soft sensing, and process condition monitoring.
 
 Installation
 ----------------------
 
-`BibMon` can be installed locally using `pip`. In the root directory of the package, which contains the `setup.py` file, type the following command:
+`BibMon` can be installed using `pip`:
 
-    pip install -e .
+    pip install bibmon
 
 Available Models
 ----------------------
 
 * PCA (Principal Component Analysis);
 * any regressor that uses the `scikit-learn` interface.
```

### Comparing `bibmon-1.0.0/test/test_models.py` & `bibmon-1.0.1/test/test_models.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,229 +1,229 @@
-#%%
-import bibmon
-import pandas as pd
-import numpy as np
-
-#%%
-
-def test_models_with_df_inputs():
-
-    # load data
-    data = bibmon.load_real_data()
-    data = data.apply(pd.to_numeric, errors='coerce')
-    
-    # preprocessing pipeline
-    f_pp_tr = ['remove_empty_variables',
-               'ffill_nan',
-               'remove_frozen_variables',
-               'normalize']
-    
-    f_pp_ts = ['ffill_nan','normalize']
-    
-    # define training set
-    (X_train, X_validation, 
-     X_test, Y_train, 
-     Y_validation, Y_test) = bibmon.train_val_test_split(data, 
-                                           start_train = '2017-12-24T12:00', 
-                                           end_train = '2018-01-01T00:00', 
-                                           end_validation = '2018-01-02T00:00', 
-                                           end_test = '2018-01-04T00:00',
-                                           tags_Y = 'tag100')
-    
-    # running the unit tests
-                                                             
-    for attr in bibmon.__all__:             
-        a = getattr(bibmon,attr)     
-        if isinstance(a, type):         
-            if a.__base__ == bibmon._generic_model.GenericModel:   
-                if a == bibmon.sklearnRegressor:                 
-                    from sklearn.linear_model import LinearRegression
-                    m = a(LinearRegression())
-                else:                    
-                    m = a()        
-                              
-                # TRAINING
-                    
-                if m.has_Y:    
-                    # X DF with one column
-                    m.fit(X_train.loc[:,['tag102']], Y_train, 
-                          f_pp = f_pp_tr,
-                          delete_training_data = False)
-                    
-                    # X series with one column
-                    m.fit(X_train.loc[:,['tag102']].T.squeeze(), Y_train, 
-                          f_pp = f_pp_tr,
-                          delete_training_data = False)
-                    
-                # X complete DF
-                m.fit(X_train, Y_train, 
-                      f_pp = f_pp_tr,
-                      delete_training_data = False)
-                                            
-                dfs_train = [m.X_train, m.X_train_orig]
-                series_train = [m.SPE_train]                
-
-                if m.has_Y:
-                    dfs_train.extend([m.Y_train_pred, m.Y_train_pred_orig])
-                else:
-                    dfs_train.extend([m.X_train_pred, m.X_train_pred_orig])
-                       
-                if m.has_Y:
-                    dfs_train.extend([m.Y_train, m.Y_train_orig])
-                
-                for df in dfs_train:
-                    assert(isinstance(df, pd.DataFrame))
-                    
-                for s in series_train:
-                    assert(isinstance(s, pd.Series))
-                    
-                assert(isinstance(m.limSPE, float))
-
-                # PREDICTION 1 - VALIDATION AND REDEFINITION OF LIMIT
-                
-                m.predict(X_validation, Y_validation, redefine_limit = True,
-                          f_pp = f_pp_ts)
-                
-                dfs_val = [m.X_test, m.X_test_orig]
-                series_val = [m.SPE_test]                
-
-                if m.has_Y:
-                    dfs_val.extend([m.Y_test_pred, m.Y_test_pred_orig])
-                else:
-                    dfs_val.extend([m.X_test_pred, m.X_test_pred_orig])
-                       
-                if m.has_Y:
-                    dfs_val.extend([m.Y_test, m.Y_test_orig])
-                
-                for df in dfs_val:
-                    assert(isinstance(df, pd.DataFrame))
-                    
-                for s in series_val:
-                    assert(isinstance(s, pd.Series))
-                
-                # PREDICTION 2 - TEST WITH WINDOWS FOR ALARMS
-                    
-                m.predict(X_test, Y_test,                           
-                          count_window_size = 10,
-                          redefine_limit = False, count_limit = 5, 
-                          f_pp = f_pp_ts)        
-                                
-                series_alarms = [m.alarmOutlier, m.alarmCount]
-
-                for s in series_alarms:
-                    assert(isinstance(s, pd.Series))
-                    
-                # PREDICTION 3 - TEST WITH A POINT (SERIES AND DF)
-
-                f_pp_ts =['replace_nan_with_values']
-                a_pp_ts = {'replace_nan_with_values__val': X_train.median()}
-        
-                # SERIES
-                m.predict(X_test.iloc[0:1], Y_test.iloc[0:1],
-                          f_pp = f_pp_ts,
-                          a_pp = a_pp_ts)
-                
-                # DF
-                m.predict(X_test.iloc[0:1], Y_test.iloc[0:1],
-                          f_pp = f_pp_ts,
-                          a_pp = a_pp_ts)               
-
-#%%
-                
-def test_models_with_np_array_inputs():
-
-    # load data
-    train_df, test_df = bibmon.load_tennessee_eastman(train_id = 0, 
-                                                      test_id = 1)
-    
-    X_train = train_df.drop('XMEAS(35)',axis=1)
-    Y_train = train_df['XMEAS(35)']
-
-    X_test = test_df.drop('XMEAS(35)',axis=1)
-    Y_test = test_df['XMEAS(35)']
-
-    # preprocessing pipeline    
-    f_pp = ['normalize']
-    
-    for attr in bibmon.__all__:             
-        a = getattr(bibmon,attr)     
-        if isinstance(a, type):         
-            if a.__base__ == bibmon._generic_model.GenericModel:   
-                if a == bibmon.sklearnRegressor:                 
-                    from sklearn.linear_model import LinearRegression
-                    m = a(LinearRegression())
-                else:                    
-                    m = a()        
-                              
-                # TRAINING
-
-                if m.has_Y:    
-                    # X with one column
-                    m.fit(np.array(X_train.iloc[:,0]), np.array(Y_train), 
-                          f_pp = f_pp,
-                          delete_training_data = False)
-                    
-                # complete X
-                m.fit(np.array(X_train), np.array(Y_train), 
-                      f_pp = f_pp,
-                      delete_training_data = False)
-    
-                dfs_train = [m.X_train, m.X_train_orig]
-                series_train = [m.SPE_train]                
-
-                if m.has_Y:
-                    dfs_train.extend([m.Y_train_pred, m.Y_train_pred_orig])
-                else:
-                    dfs_train.extend([m.X_train_pred, m.X_train_pred_orig])
-                       
-                if m.has_Y:
-                    dfs_train.extend([m.Y_train, m.Y_train_orig])
-                
-                for df in dfs_train:
-                    assert(isinstance(df, pd.DataFrame))
-                    
-                for s in series_train:
-                    assert(isinstance(s, pd.Series))
-                    
-                assert(isinstance(m.limSPE, float))  
-                
-                if isinstance(m, bibmon.PCA):
-                    m.plot_cumulative_variance()
-                
-                # TEST
-                
-                m.predict(np.array(X_test), np.array(Y_test), 
-                          f_pp = f_pp)
-                
-                dfs_val = [m.X_test, m.X_test_orig]
-                series_val = [m.SPE_test]                
-
-                if m.has_Y:
-                    dfs_val.extend([m.Y_test_pred, m.Y_test_pred_orig])
-                else:
-                    dfs_val.extend([m.X_test_pred, m.X_test_pred_orig])
-                       
-                if m.has_Y:
-                    dfs_val.extend([m.Y_test, m.Y_test_orig])
-                
-                for df in dfs_val:
-                    assert(isinstance(df, pd.DataFrame))
-                    
-                for s in series_val:
-                    assert(isinstance(s, pd.Series))
-                    
-                # PREDICTION 3 - TEST WITH A POINT (SERIES AND DF)
-
-                f_pp_ts =['normalize','replace_nan_with_values']
-                a_pp_ts = {'replace_nan_with_values__val': X_train.median()}
-        
-                # SERIES
-                m.predict(np.array(X_test.iloc[0]), np.array(Y_test.iloc[0]),
-                          f_pp = f_pp_ts,
-                          a_pp = a_pp_ts)
-                
-                # DF
-                m.predict(np.array(X_test.iloc[0:1]), 
-                          np.array(Y_test.iloc[0:1]),
-                          f_pp = f_pp_ts,
-                          a_pp = a_pp_ts)           
+#%%
+import bibmon
+import pandas as pd
+import numpy as np
+
+#%%
+
+def test_models_with_df_inputs():
+
+    # load data
+    data = bibmon.load_real_data()
+    data = data.apply(pd.to_numeric, errors='coerce')
+    
+    # preprocessing pipeline
+    f_pp_tr = ['remove_empty_variables',
+               'ffill_nan',
+               'remove_frozen_variables',
+               'normalize']
+    
+    f_pp_ts = ['ffill_nan','normalize']
+    
+    # define training set
+    (X_train, X_validation, 
+     X_test, Y_train, 
+     Y_validation, Y_test) = bibmon.train_val_test_split(data, 
+                                           start_train = '2017-12-24T12:00', 
+                                           end_train = '2018-01-01T00:00', 
+                                           end_validation = '2018-01-02T00:00', 
+                                           end_test = '2018-01-04T00:00',
+                                           tags_Y = 'tag100')
+    
+    # running the unit tests
+                                                             
+    for attr in bibmon.__all__:             
+        a = getattr(bibmon,attr)     
+        if isinstance(a, type):         
+            if a.__base__ == bibmon._generic_model.GenericModel:   
+                if a == bibmon.sklearnRegressor:                 
+                    from sklearn.linear_model import LinearRegression
+                    m = a(LinearRegression())
+                else:                    
+                    m = a()        
+                              
+                # TRAINING
+                    
+                if m.has_Y:    
+                    # X DF with one column
+                    m.fit(X_train.loc[:,['tag102']], Y_train, 
+                          f_pp = f_pp_tr,
+                          delete_training_data = False)
+                    
+                    # X series with one column
+                    m.fit(X_train.loc[:,['tag102']].T.squeeze(), Y_train, 
+                          f_pp = f_pp_tr,
+                          delete_training_data = False)
+                    
+                # X complete DF
+                m.fit(X_train, Y_train, 
+                      f_pp = f_pp_tr,
+                      delete_training_data = False)
+                                            
+                dfs_train = [m.X_train, m.X_train_orig]
+                series_train = [m.SPE_train]                
+
+                if m.has_Y:
+                    dfs_train.extend([m.Y_train_pred, m.Y_train_pred_orig])
+                else:
+                    dfs_train.extend([m.X_train_pred, m.X_train_pred_orig])
+                       
+                if m.has_Y:
+                    dfs_train.extend([m.Y_train, m.Y_train_orig])
+                
+                for df in dfs_train:
+                    assert(isinstance(df, pd.DataFrame))
+                    
+                for s in series_train:
+                    assert(isinstance(s, pd.Series))
+                    
+                assert(isinstance(m.limSPE, float))
+
+                # PREDICTION 1 - VALIDATION AND REDEFINITION OF LIMIT
+                
+                m.predict(X_validation, Y_validation, redefine_limit = True,
+                          f_pp = f_pp_ts)
+                
+                dfs_val = [m.X_test, m.X_test_orig]
+                series_val = [m.SPE_test]                
+
+                if m.has_Y:
+                    dfs_val.extend([m.Y_test_pred, m.Y_test_pred_orig])
+                else:
+                    dfs_val.extend([m.X_test_pred, m.X_test_pred_orig])
+                       
+                if m.has_Y:
+                    dfs_val.extend([m.Y_test, m.Y_test_orig])
+                
+                for df in dfs_val:
+                    assert(isinstance(df, pd.DataFrame))
+                    
+                for s in series_val:
+                    assert(isinstance(s, pd.Series))
+                
+                # PREDICTION 2 - TEST WITH WINDOWS FOR ALARMS
+                    
+                m.predict(X_test, Y_test,                           
+                          count_window_size = 10,
+                          redefine_limit = False, count_limit = 5, 
+                          f_pp = f_pp_ts)        
+                                
+                series_alarms = [m.alarmOutlier, m.alarmCount]
+
+                for s in series_alarms:
+                    assert(isinstance(s, pd.Series))
+                    
+                # PREDICTION 3 - TEST WITH A POINT (SERIES AND DF)
+
+                f_pp_ts =['replace_nan_with_values']
+                a_pp_ts = {'replace_nan_with_values__val': X_train.median()}
+        
+                # SERIES
+                m.predict(X_test.iloc[0:1], Y_test.iloc[0:1],
+                          f_pp = f_pp_ts,
+                          a_pp = a_pp_ts)
+                
+                # DF
+                m.predict(X_test.iloc[0:1], Y_test.iloc[0:1],
+                          f_pp = f_pp_ts,
+                          a_pp = a_pp_ts)               
+
+#%%
+                
+def test_models_with_np_array_inputs():
+
+    # load data
+    train_df, test_df = bibmon.load_tennessee_eastman(train_id = 0, 
+                                                      test_id = 1)
+    
+    X_train = train_df.drop('XMEAS(35)',axis=1)
+    Y_train = train_df['XMEAS(35)']
+
+    X_test = test_df.drop('XMEAS(35)',axis=1)
+    Y_test = test_df['XMEAS(35)']
+
+    # preprocessing pipeline    
+    f_pp = ['normalize']
+    
+    for attr in bibmon.__all__:             
+        a = getattr(bibmon,attr)     
+        if isinstance(a, type):         
+            if a.__base__ == bibmon._generic_model.GenericModel:   
+                if a == bibmon.sklearnRegressor:                 
+                    from sklearn.linear_model import LinearRegression
+                    m = a(LinearRegression())
+                else:                    
+                    m = a()        
+                              
+                # TRAINING
+
+                if m.has_Y:    
+                    # X with one column
+                    m.fit(np.array(X_train.iloc[:,0]), np.array(Y_train), 
+                          f_pp = f_pp,
+                          delete_training_data = False)
+                    
+                # complete X
+                m.fit(np.array(X_train), np.array(Y_train), 
+                      f_pp = f_pp,
+                      delete_training_data = False)
+    
+                dfs_train = [m.X_train, m.X_train_orig]
+                series_train = [m.SPE_train]                
+
+                if m.has_Y:
+                    dfs_train.extend([m.Y_train_pred, m.Y_train_pred_orig])
+                else:
+                    dfs_train.extend([m.X_train_pred, m.X_train_pred_orig])
+                       
+                if m.has_Y:
+                    dfs_train.extend([m.Y_train, m.Y_train_orig])
+                
+                for df in dfs_train:
+                    assert(isinstance(df, pd.DataFrame))
+                    
+                for s in series_train:
+                    assert(isinstance(s, pd.Series))
+                    
+                assert(isinstance(m.limSPE, float))  
+                
+                if isinstance(m, bibmon.PCA):
+                    m.plot_cumulative_variance()
+                
+                # TEST
+                
+                m.predict(np.array(X_test), np.array(Y_test), 
+                          f_pp = f_pp)
+                
+                dfs_val = [m.X_test, m.X_test_orig]
+                series_val = [m.SPE_test]                
+
+                if m.has_Y:
+                    dfs_val.extend([m.Y_test_pred, m.Y_test_pred_orig])
+                else:
+                    dfs_val.extend([m.X_test_pred, m.X_test_pred_orig])
+                       
+                if m.has_Y:
+                    dfs_val.extend([m.Y_test, m.Y_test_orig])
+                
+                for df in dfs_val:
+                    assert(isinstance(df, pd.DataFrame))
+                    
+                for s in series_val:
+                    assert(isinstance(s, pd.Series))
+                    
+                # PREDICTION 3 - TEST WITH A POINT (SERIES AND DF)
+
+                f_pp_ts =['normalize','replace_nan_with_values']
+                a_pp_ts = {'replace_nan_with_values__val': X_train.median()}
+        
+                # SERIES
+                m.predict(np.array(X_test.iloc[0]), np.array(Y_test.iloc[0]),
+                          f_pp = f_pp_ts,
+                          a_pp = a_pp_ts)
+                
+                # DF
+                m.predict(np.array(X_test.iloc[0:1]), 
+                          np.array(Y_test.iloc[0:1]),
+                          f_pp = f_pp_ts,
+                          a_pp = a_pp_ts)
```

### Comparing `bibmon-1.0.0/test/test_preprocess.py` & `bibmon-1.0.1/test/test_preprocess.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Fri Sep  4 00:04:38 2020
-
-@author: afranio
-"""
-
-import pandas as pd
-import bibmon
-
-#%%
-def test_preprocess():
-
-    # load data
-    data = bibmon.load_real_data()
-    data = data.apply(pd.to_numeric, errors='coerce')
-    
-    # define functions to be tested
-    
-    pp = bibmon.PreProcess()
-    
-    funcs = [f for f in dir(pp) if (f[0] != '_' and callable(getattr(pp,f)))]
-    funcs = [f for f in funcs if f not in ['apply','back_to_units']]
-    
-    # define training and test sets
-        
-    (X_train, _, 
-     X_test, Y_train, 
-     _, Y_test) = bibmon.train_val_test_split(data, 
-                                           start_train = '2017-12-24T12:00', 
-                                           end_train = '2018-01-01T00:00', 
-                                           end_validation = '2018-01-02T00:00', 
-                                           end_test = '2018-01-04T00:00',
-                                           tags_Y = 'tag100')
-                                                         
-    for f in funcs:
-        
-        print(f)
-        
-        ppX = bibmon.PreProcess(f_pp = [f])
-        ppY = bibmon.PreProcess(f_pp = [f], is_Y = True)
-
-        X_train_proc = ppX.apply(X_train, train_or_test = 'train')
-        Y_train_proc = ppY.apply(Y_train, train_or_test = 'train')
-
-        assert(isinstance(X_train_proc, pd.DataFrame))
-        assert(isinstance(Y_train_proc, pd.DataFrame))
-        assert(Y_train_proc.columns == Y_train.columns)
-        
-        X_test_proc = ppX.apply(X_test, train_or_test = 'test')
-        Y_test_proc = ppY.apply(Y_test, train_or_test = 'test')
-      
-        assert(isinstance(X_test_proc, pd.DataFrame))
-        assert(isinstance(Y_test_proc, pd.DataFrame))
-        assert(Y_test_proc.columns == Y_test.columns)
-        
-        if 'nan' in f:
-            assert(X_train_proc.isnull().sum().sum()==0)
-            assert(Y_train_proc.isnull().sum().sum()==0)
-            assert(X_test_proc.isnull().sum().sum()==0)
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Created on Fri Sep  4 00:04:38 2020
+
+@author: afranio
+"""
+
+import pandas as pd
+import bibmon
+
+#%%
+def test_preprocess():
+
+    # load data
+    data = bibmon.load_real_data()
+    data = data.apply(pd.to_numeric, errors='coerce')
+    
+    # define functions to be tested
+    
+    pp = bibmon.PreProcess()
+    
+    funcs = [f for f in dir(pp) if (f[0] != '_' and callable(getattr(pp,f)))]
+    funcs = [f for f in funcs if f not in ['apply','back_to_units']]
+    
+    # define training and test sets
+        
+    (X_train, _, 
+     X_test, Y_train, 
+     _, Y_test) = bibmon.train_val_test_split(data, 
+                                           start_train = '2017-12-24T12:00', 
+                                           end_train = '2018-01-01T00:00', 
+                                           end_validation = '2018-01-02T00:00', 
+                                           end_test = '2018-01-04T00:00',
+                                           tags_Y = 'tag100')
+                                                         
+    for f in funcs:
+        
+        print(f)
+        
+        ppX = bibmon.PreProcess(f_pp = [f])
+        ppY = bibmon.PreProcess(f_pp = [f], is_Y = True)
+
+        X_train_proc = ppX.apply(X_train, train_or_test = 'train')
+        Y_train_proc = ppY.apply(Y_train, train_or_test = 'train')
+
+        assert(isinstance(X_train_proc, pd.DataFrame))
+        assert(isinstance(Y_train_proc, pd.DataFrame))
+        assert(Y_train_proc.columns == Y_train.columns)
+        
+        X_test_proc = ppX.apply(X_test, train_or_test = 'test')
+        Y_test_proc = ppY.apply(Y_test, train_or_test = 'test')
+      
+        assert(isinstance(X_test_proc, pd.DataFrame))
+        assert(isinstance(Y_test_proc, pd.DataFrame))
+        assert(Y_test_proc.columns == Y_test.columns)
+        
+        if 'nan' in f:
+            assert(X_train_proc.isnull().sum().sum()==0)
+            assert(Y_train_proc.isnull().sum().sum()==0)
+            assert(X_test_proc.isnull().sum().sum()==0)
             assert(Y_test_proc.isnull().sum().sum()==0)
```

### Comparing `bibmon-1.0.0/test/test_tools.py` & `bibmon-1.0.1/test/test_tools.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Thu Sep  3 23:38:16 2020
-
-@author: afranio
-"""
-
-import bibmon
-import pandas as pd
-
-def test_complete_analysis():
-    
-    # load data
-    data = bibmon.load_real_data()
-    data = data.apply(pd.to_numeric, errors='coerce')
-    
-    # preprocessing pipeline
-    
-    preproc_tr = ['remove_empty_variables',
-                  'ffill_nan',
-                  'remove_frozen_variables',
-                  'normalize']
-    
-    preproc_ts = ['ffill_nan','normalize']
-    
-    # define training set
-        
-    (X_train, X_validation, 
-     X_test, Y_train, 
-     Y_validation, Y_test) = bibmon.train_val_test_split(data, 
-                                            start_train = '2017-12-24T12:00', 
-                                            end_train = '2018-01-01T00:00', 
-                                           end_validation = '2018-01-02T00:00', 
-                                            end_test = '2018-01-04T00:00',
-                                            tags_Y = 'tag100')
-                                                         
-    # define the model
-                                                         
-    from sklearn.linear_model import LinearRegression
-    reg = LinearRegression()
-    
-    model = bibmon.sklearnRegressor(reg)                                                          
-
-    # define regression metrics
-                                                         
-    from sklearn.metrics import r2_score
-    from sklearn.metrics import mean_absolute_error
-    
-    mtr = [r2_score, mean_absolute_error]
-                           
-    # complete analysis!
-                              
-    bibmon.complete_analysis(model, X_train, X_validation, X_test, 
-                            Y_train, Y_validation, Y_test,
-                            f_pp_train = preproc_tr,
-                            f_pp_test = preproc_ts,
-                            metrics = mtr, 
-                            count_window_size = 3, count_limit = 2,
-                            fault_start = '2018-01-02 06:00:00',
-                            fault_end = '2018-01-02 09:00:00') 
-    
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Created on Thu Sep  3 23:38:16 2020
+
+@author: afranio
+"""
+
+import bibmon
+import pandas as pd
+
+def test_complete_analysis():
+    
+    # load data
+    data = bibmon.load_real_data()
+    data = data.apply(pd.to_numeric, errors='coerce')
+    
+    # preprocessing pipeline
+    
+    preproc_tr = ['remove_empty_variables',
+                  'ffill_nan',
+                  'remove_frozen_variables',
+                  'normalize']
+    
+    preproc_ts = ['ffill_nan','normalize']
+    
+    # define training set
+        
+    (X_train, X_validation, 
+     X_test, Y_train, 
+     Y_validation, Y_test) = bibmon.train_val_test_split(data, 
+                                            start_train = '2017-12-24T12:00', 
+                                            end_train = '2018-01-01T00:00', 
+                                           end_validation = '2018-01-02T00:00', 
+                                            end_test = '2018-01-04T00:00',
+                                            tags_Y = 'tag100')
+                                                         
+    # define the model
+                                                         
+    from sklearn.linear_model import LinearRegression
+    reg = LinearRegression()
+    
+    model = bibmon.sklearnRegressor(reg)                                                          
+
+    # define regression metrics
+                                                         
+    from sklearn.metrics import r2_score
+    from sklearn.metrics import mean_absolute_error
+    
+    mtr = [r2_score, mean_absolute_error]
+                           
+    # complete analysis!
+                              
+    bibmon.complete_analysis(model, X_train, X_validation, X_test, 
+                            Y_train, Y_validation, Y_test,
+                            f_pp_train = preproc_tr,
+                            f_pp_test = preproc_ts,
+                            metrics = mtr, 
+                            count_window_size = 3, count_limit = 2,
+                            fault_start = '2018-01-02 06:00:00',
+                            fault_end = '2018-01-02 09:00:00') 
+    
     model.plot_importances()
```

