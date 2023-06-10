# Comparing `tmp/custom_diffusion-0.0.7.tar.gz` & `tmp/custom_diffusion-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_diffusion-0.0.7.tar", last modified: Fri Jun  9 22:30:32 2023, max compression
+gzip compressed data, was "custom_diffusion-0.1.0.tar", last modified: Sat Jun 10 13:20:54 2023, max compression
```

## Comparing `custom_diffusion-0.0.7.tar` & `custom_diffusion-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 22:30:32.674478 custom_diffusion-0.0.7/
--rw-rw-rw-   0        0        0    11357 2023-06-09 21:50:57.000000 custom_diffusion-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       24 2023-06-09 21:50:57.000000 custom_diffusion-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1354 2023-06-09 22:30:32.674478 custom_diffusion-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-06-09 21:50:57.000000 custom_diffusion-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 22:30:32.636227 custom_diffusion-0.0.7/custom_diffusion/
--rw-rw-rw-   0        0        0       22 2023-06-09 22:30:25.000000 custom_diffusion-0.0.7/custom_diffusion/__init__.py
--rw-rw-rw-   0        0        0      859 2023-06-09 22:29:27.000000 custom_diffusion-0.0.7/custom_diffusion/demo.py
-drwxrwxrwx   0        0        0        0 2023-06-09 22:30:32.665478 custom_diffusion-0.0.7/custom_diffusion/pipelines/
--rw-rw-rw-   0        0        0        0 2023-06-09 22:04:46.000000 custom_diffusion-0.0.7/custom_diffusion/pipelines/__init__.py
--rw-rw-rw-   0        0        0     6684 2023-06-09 21:50:57.000000 custom_diffusion-0.0.7/custom_diffusion/pipelines/controlnet_inpaint_pipeline.py
--rw-rw-rw-   0        0        0     6759 2023-06-09 22:29:37.000000 custom_diffusion-0.0.7/custom_diffusion/pipelines/controlnet_pipeline.py
--rw-rw-rw-   0        0        0     8952 2023-06-09 21:50:57.000000 custom_diffusion-0.0.7/custom_diffusion/preprocces.py
-drwxrwxrwx   0        0        0        0 2023-06-09 22:30:32.672478 custom_diffusion-0.0.7/custom_diffusion/utils/
--rw-rw-rw-   0        0        0        0 2023-06-09 21:50:57.000000 custom_diffusion-0.0.7/custom_diffusion/utils/__init__.py
--rw-rw-rw-   0        0        0     2242 2023-06-09 21:50:57.000000 custom_diffusion-0.0.7/custom_diffusion/utils/data_utils.py
--rw-rw-rw-   0        0        0     1338 2023-06-09 21:50:57.000000 custom_diffusion-0.0.7/custom_diffusion/utils/downloads.py
--rw-rw-rw-   0        0        0     1268 2023-06-09 22:29:52.000000 custom_diffusion-0.0.7/custom_diffusion/utils/scheduler_utils.py
--rw-rw-rw-   0        0        0     3517 2023-06-09 21:50:57.000000 custom_diffusion-0.0.7/custom_diffusion/utils/video_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 22:30:32.660231 custom_diffusion-0.0.7/custom_diffusion.egg-info/
--rw-rw-rw-   0        0        0     1354 2023-06-09 22:30:31.000000 custom_diffusion-0.0.7/custom_diffusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      699 2023-06-09 22:30:32.000000 custom_diffusion-0.0.7/custom_diffusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 22:30:32.000000 custom_diffusion-0.0.7/custom_diffusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      175 2023-06-09 22:30:32.000000 custom_diffusion-0.0.7/custom_diffusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-09 22:30:32.000000 custom_diffusion-0.0.7/custom_diffusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       80 2023-06-09 21:50:57.000000 custom_diffusion-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      113 2023-06-09 22:23:40.000000 custom_diffusion-0.0.7/requirements.txt
--rw-rw-rw-   0        0        0      375 2023-06-09 22:30:32.681480 custom_diffusion-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2151 2023-06-09 21:50:57.000000 custom_diffusion-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:20:54.259650 custom_diffusion-0.1.0/
+-rw-rw-rw-   0        0        0    11558 2023-06-07 17:52:13.000000 custom_diffusion-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-06-09 11:29:48.000000 custom_diffusion-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2598 2023-06-10 13:20:54.259650 custom_diffusion-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1431 2023-06-10 13:17:02.000000 custom_diffusion-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 13:20:54.230750 custom_diffusion-0.1.0/custom_diffusion/
+-rw-rw-rw-   0        0        0       23 2023-06-10 13:19:54.000000 custom_diffusion-0.1.0/custom_diffusion/__init__.py
+-rw-rw-rw-   0        0        0     1618 2023-06-10 13:11:21.000000 custom_diffusion-0.1.0/custom_diffusion/demo.py
+-rw-rw-rw-   0        0        0     9310 2023-06-10 12:22:15.000000 custom_diffusion-0.1.0/custom_diffusion/preprocces.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:20:54.257654 custom_diffusion-0.1.0/custom_diffusion/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-09 11:02:04.000000 custom_diffusion-0.1.0/custom_diffusion/utils/__init__.py
+-rw-rw-rw-   0        0        0     2242 2023-06-09 11:02:04.000000 custom_diffusion-0.1.0/custom_diffusion/utils/data_utils.py
+-rw-rw-rw-   0        0        0     1375 2023-06-09 11:02:04.000000 custom_diffusion-0.1.0/custom_diffusion/utils/downloads.py
+-rw-rw-rw-   0        0        0     1307 2023-06-10 12:22:15.000000 custom_diffusion-0.1.0/custom_diffusion/utils/scheduler_utils.py
+-rw-rw-rw-   0        0        0     3637 2023-06-09 11:02:04.000000 custom_diffusion-0.1.0/custom_diffusion/utils/video_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:20:54.246686 custom_diffusion-0.1.0/custom_diffusion.egg-info/
+-rw-rw-rw-   0        0        0     2598 2023-06-10 13:20:54.000000 custom_diffusion-0.1.0/custom_diffusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2023-06-10 13:20:54.000000 custom_diffusion-0.1.0/custom_diffusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 13:20:54.000000 custom_diffusion-0.1.0/custom_diffusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      175 2023-06-10 13:20:54.000000 custom_diffusion-0.1.0/custom_diffusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-10 13:20:54.000000 custom_diffusion-0.1.0/custom_diffusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-06-09 11:02:04.000000 custom_diffusion-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      123 2023-06-10 12:22:15.000000 custom_diffusion-0.1.0/requirements.txt
+-rw-rw-rw-   0        0        0      375 2023-06-10 13:20:54.262643 custom_diffusion-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2218 2023-06-09 11:29:48.000000 custom_diffusion-0.1.0/setup.py
```

### Comparing `custom_diffusion-0.0.7/LICENSE` & `custom_diffusion-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

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
-   Copyright [yyyy] [name of copyright owner]
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
+   Copyright [yyyy] [name of copyright owner]
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

### Comparing `custom_diffusion-0.0.7/custom_diffusion/utils/data_utils.py` & `custom_diffusion-0.1.0/custom_diffusion/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.7/custom_diffusion/utils/downloads.py` & `custom_diffusion-0.1.0/custom_diffusion/utils/downloads.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-def download_video(
-    video_url: str = "https://www.youtube.com/watch?v=8QRG4vzbdE0",
-    output_path: str = "output_videos",
-    quality: str = "720p",
-    filename: str = "downloaded_video.mp4",
-):
-    """
-    This function downloads a video and corresponding audio from YouTube and saves it in the designated output folder.
-
-    Args:
-    video_url (str): URL of the YouTube video to be downloaded.
-    output_path (str): Directory path where the downloaded video will be saved.
-    quality (str): Desired quality of the video to be downloaded. It can be '144p', '240p', '360p', '480p', '720p', '1080p', '1440p' (for 2K), or '2160p' (for 4K).
-    filename (str): Desired filename of the downloaded video.
-
-    Returns:
-    None
-    """
-    import os
-
-    from pytube import YouTube
-
-    # Create a YouTube object
-    yt = YouTube(video_url)
-
-    # Find the stream with the desired quality that also contains audio
-    video_stream = yt.streams.filter(progressive=True, file_extension="mp4", res=quality).first()
-
-    if video_stream is not None:
-        # Download the stream
-        video_stream.download(output_path, filename=filename)
-        print("Video downloaded successfully!")
-    else:
-        print(f"No video stream found for {quality} quality.")
-
-    save_path = os.path.join(output_path, filename)
-    return save_path
+def download_video(
+    video_url: str = "https://www.youtube.com/watch?v=8QRG4vzbdE0",
+    output_path: str = "output_videos",
+    quality: str = "720p",
+    filename: str = "downloaded_video.mp4",
+):
+    """
+    This function downloads a video and corresponding audio from YouTube and saves it in the designated output folder.
+
+    Args:
+    video_url (str): URL of the YouTube video to be downloaded.
+    output_path (str): Directory path where the downloaded video will be saved.
+    quality (str): Desired quality of the video to be downloaded. It can be '144p', '240p', '360p', '480p', '720p', '1080p', '1440p' (for 2K), or '2160p' (for 4K).
+    filename (str): Desired filename of the downloaded video.
+
+    Returns:
+    None
+    """
+    import os
+
+    from pytube import YouTube
+
+    # Create a YouTube object
+    yt = YouTube(video_url)
+
+    # Find the stream with the desired quality that also contains audio
+    video_stream = yt.streams.filter(progressive=True, file_extension="mp4", res=quality).first()
+
+    if video_stream is not None:
+        # Download the stream
+        video_stream.download(output_path, filename=filename)
+        print("Video downloaded successfully!")
+    else:
+        print(f"No video stream found for {quality} quality.")
+
+    save_path = os.path.join(output_path, filename)
+    return save_path
```

### Comparing `custom_diffusion-0.0.7/custom_diffusion/utils/video_utils.py` & `custom_diffusion-0.1.0/custom_diffusion/utils/video_utils.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-def video_to_frames(video_path, output_path, frame_rate=1):
-    """
-    This function takes a video file, separates it into frames,
-    and saves them in the designated output folder.
-
-    Args:
-    video_path (str): Path to the video file to be dissected.
-    output_path (str): Directory path where the dissected frames will be saved.
-    frame_rate (int): Determines the frequency of frames to be saved, every 'frame_rate' frame will be saved.
-
-    Returns:
-    None
-    """
-    import os
-
-    import cv2
-
-    # Create VideoCapture object
-    vidcap = cv2.VideoCapture(video_path)
-
-    # Check if output directory exists, if not, create it.
-    if not os.path.exists(output_path):
-        os.makedirs(output_path)
-
-    count = 0
-    success = True
-    frame_id = 0
-
-    while success:
-        # Read frame
-        success, image = vidcap.read()
-
-        if success:
-            # Only save frame if it is the right id (based on frame_rate)
-            if frame_id % frame_rate == 0:
-                # Save frame to specified output path with zero-padded file name
-                cv2.imwrite(os.path.join(output_path, f"{str(count).zfill(5)}.jpg"), image)
-                count += 1
-
-            frame_id += 1
-
-    print("Video frames saved successfully!")
-
-    return output_path
-
-
-def trim_video(video_path: str, output_path: str, start_time: int, end_time: int):
-    """
-    This function trims a video clip from the given start time to the end time.
-
-    Args:
-    video_path (str): Path to the input video file.
-    output_path (str): Path to save the output trimmed video file.
-    start_time (int): The start time of the clip in seconds.
-    end_time (int): The end time of the clip in seconds.
-
-    Returns:
-    None
-    """
-    from moviepy.editor import VideoFileClip
-
-    # Load the video
-    clip = VideoFileClip(video_path)
-
-    # Trim the video
-    trimmed_clip = clip.subclip(start_time, end_time)
-
-    # Write the result to a file (without processing audio)
-    trimmed_clip.write_videofile(output_path, audio=True)
-
-    print("Video trimmed successfully!")
-
-    return output_path
-
-
-def frames_to_video(folder_path, output_folder, output_video_name="output.avi", duration=10):
-    """
-    This function takes a folder with image files, orders them, and creates a video file from them.
-    The video is then saved in the designated output folder.
-
-    Args:
-    folder_path (str): Path to the folder with image files.
-    output_folder (str): Directory path where the video will be saved.
-    output_video_name (str): The name of the output video file.
-    duration (int): The desired duration of the output video in seconds.
-
-    Returns:
-    None
-    """
-    import glob
-    import os
-
-    import cv2
-
-    # Get the list of images
-    img_array = []
-    for filename in sorted(glob.glob(os.path.join(folder_path, "*.jpg"))):
-        img = cv2.imread(filename)
-        height, width, layers = img.shape
-        size = (width, height)
-        img_array.append(img)
-
-    # Calculate fps based on the desired duration
-    fps = len(img_array) / duration
-
-    # Check if output directory exists, if not, create it.
-    if not os.path.exists(output_folder):
-        os.makedirs(output_folder)
-
-    # Create a VideoWriter object
-    out = cv2.VideoWriter(os.path.join(output_folder, output_video_name), cv2.VideoWriter_fourcc(*"DIVX"), fps, size)
-
-    for i in range(len(img_array)):
-        out.write(img_array[i])
-
-    out.release()
-
-    print("Video created successfully!")
-
-    return output_folder
+def video_to_frames(video_path, output_path, frame_rate=1):
+    """
+    This function takes a video file, separates it into frames,
+    and saves them in the designated output folder.
+
+    Args:
+    video_path (str): Path to the video file to be dissected.
+    output_path (str): Directory path where the dissected frames will be saved.
+    frame_rate (int): Determines the frequency of frames to be saved, every 'frame_rate' frame will be saved.
+
+    Returns:
+    None
+    """
+    import os
+
+    import cv2
+
+    # Create VideoCapture object
+    vidcap = cv2.VideoCapture(video_path)
+
+    # Check if output directory exists, if not, create it.
+    if not os.path.exists(output_path):
+        os.makedirs(output_path)
+
+    count = 0
+    success = True
+    frame_id = 0
+
+    while success:
+        # Read frame
+        success, image = vidcap.read()
+
+        if success:
+            # Only save frame if it is the right id (based on frame_rate)
+            if frame_id % frame_rate == 0:
+                # Save frame to specified output path with zero-padded file name
+                cv2.imwrite(os.path.join(output_path, f"{str(count).zfill(5)}.jpg"), image)
+                count += 1
+
+            frame_id += 1
+
+    print("Video frames saved successfully!")
+
+    return output_path
+
+
+def trim_video(video_path: str, output_path: str, start_time: int, end_time: int):
+    """
+    This function trims a video clip from the given start time to the end time.
+
+    Args:
+    video_path (str): Path to the input video file.
+    output_path (str): Path to save the output trimmed video file.
+    start_time (int): The start time of the clip in seconds.
+    end_time (int): The end time of the clip in seconds.
+
+    Returns:
+    None
+    """
+    from moviepy.editor import VideoFileClip
+
+    # Load the video
+    clip = VideoFileClip(video_path)
+
+    # Trim the video
+    trimmed_clip = clip.subclip(start_time, end_time)
+
+    # Write the result to a file (without processing audio)
+    trimmed_clip.write_videofile(output_path, audio=True)
+
+    print("Video trimmed successfully!")
+
+    return output_path
+
+
+def frames_to_video(folder_path, output_folder, output_video_name="output.avi", duration=10):
+    """
+    This function takes a folder with image files, orders them, and creates a video file from them.
+    The video is then saved in the designated output folder.
+
+    Args:
+    folder_path (str): Path to the folder with image files.
+    output_folder (str): Directory path where the video will be saved.
+    output_video_name (str): The name of the output video file.
+    duration (int): The desired duration of the output video in seconds.
+
+    Returns:
+    None
+    """
+    import glob
+    import os
+
+    import cv2
+
+    # Get the list of images
+    img_array = []
+    for filename in sorted(glob.glob(os.path.join(folder_path, "*.jpg"))):
+        img = cv2.imread(filename)
+        height, width, layers = img.shape
+        size = (width, height)
+        img_array.append(img)
+
+    # Calculate fps based on the desired duration
+    fps = len(img_array) / duration
+
+    # Check if output directory exists, if not, create it.
+    if not os.path.exists(output_folder):
+        os.makedirs(output_folder)
+
+    # Create a VideoWriter object
+    out = cv2.VideoWriter(os.path.join(output_folder, output_video_name), cv2.VideoWriter_fourcc(*"DIVX"), fps, size)
+
+    for i in range(len(img_array)):
+        out.write(img_array[i])
+
+    out.release()
+
+    print("Video created successfully!")
+
+    return output_folder
```

### Comparing `custom_diffusion-0.0.7/custom_diffusion.egg-info/SOURCES.txt` & `custom_diffusion-0.1.0/custom_diffusion.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,12 @@
 custom_diffusion/demo.py
 custom_diffusion/preprocces.py
 custom_diffusion.egg-info/PKG-INFO
 custom_diffusion.egg-info/SOURCES.txt
 custom_diffusion.egg-info/dependency_links.txt
 custom_diffusion.egg-info/requires.txt
 custom_diffusion.egg-info/top_level.txt
-custom_diffusion/pipelines/__init__.py
-custom_diffusion/pipelines/controlnet_inpaint_pipeline.py
-custom_diffusion/pipelines/controlnet_pipeline.py
 custom_diffusion/utils/__init__.py
 custom_diffusion/utils/data_utils.py
 custom_diffusion/utils/downloads.py
 custom_diffusion/utils/scheduler_utils.py
 custom_diffusion/utils/video_utils.py
```

### Comparing `custom_diffusion-0.0.7/setup.py` & `custom_diffusion-0.1.0/setup.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-import io
-import os
-import re
-
-import setuptools
-
-
-def get_long_description():
-    base_dir = os.path.abspath(os.path.dirname(__file__))
-    with io.open(os.path.join(base_dir, "README.md"), encoding="utf-8") as f:
-        return f.read()
-
-
-def get_requirements():
-    with open("requirements.txt") as f:
-        return f.read().splitlines()
-
-
-def get_version():
-    current_dir = os.path.abspath(os.path.dirname(__file__))
-    version_file = os.path.join(current_dir, "custom_diffusion", "__init__.py")
-    with io.open(version_file, encoding="utf-8") as f:
-        return re.search(r'^__version__ = [\'"]([^\'"]*)[\'"]', f.read(), re.M).group(1)
-
-
-_DEV_REQUIREMENTS = [
-    "black==21.7b0",
-    "flake8==3.9.2",
-    "isort==5.9.2",
-    "click==8.0.4",
-]
-
-
-extras = {"dev": _DEV_REQUIREMENTS}
-
-
-setuptools.setup(
-    name="custom_diffusion",
-    version=get_version(),
-    author="kadirnar",
-    license="Apache License 2.0",
-    description="Custom Diffusion: Creating Video from Frame Using Multiple Diffusion",
-    long_description=get_long_description(),
-    long_description_content_type="text/markdown",
-    url="https://github.com/kadirnar/Custom-Diffusion",
-    packages=setuptools.find_packages(exclude=["tests"]),
-    extras_require=extras,
-    include_package_data=True,
-    python_requires=">=3.6",
-    install_requires=get_requirements(),
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Operating System :: OS Independent",
-        "Intended Audience :: Developers",
-        "Intended Audience :: Science/Research",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Topic :: Software Development :: Libraries",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-        "Topic :: Education",
-        "Topic :: Scientific/Engineering",
-        "Topic :: Scientific/Engineering :: Artificial Intelligence",
-    ],
-    keywords="machine-learning, deep-learning, pytorch, diffusion, diffusion models, controlnet,stable diffusion",
-)
+import io
+import os
+import re
+
+import setuptools
+
+
+def get_long_description():
+    base_dir = os.path.abspath(os.path.dirname(__file__))
+    with io.open(os.path.join(base_dir, "README.md"), encoding="utf-8") as f:
+        return f.read()
+
+
+def get_requirements():
+    with open("requirements.txt") as f:
+        return f.read().splitlines()
+
+
+def get_version():
+    current_dir = os.path.abspath(os.path.dirname(__file__))
+    version_file = os.path.join(current_dir, "custom_diffusion", "__init__.py")
+    with io.open(version_file, encoding="utf-8") as f:
+        return re.search(r'^__version__ = [\'"]([^\'"]*)[\'"]', f.read(), re.M).group(1)
+
+
+_DEV_REQUIREMENTS = [
+    "black==21.7b0",
+    "flake8==3.9.2",
+    "isort==5.9.2",
+    "click==8.0.4",
+]
+
+
+extras = {"dev": _DEV_REQUIREMENTS}
+
+
+setuptools.setup(
+    name="custom_diffusion",
+    version=get_version(),
+    author="kadirnar",
+    license="Apache License 2.0",
+    description="Custom Diffusion: Creating Video from Frame Using Multiple Diffusion",
+    long_description=get_long_description(),
+    long_description_content_type="text/markdown",
+    url="https://github.com/kadirnar/Custom-Diffusion",
+    packages=setuptools.find_packages(exclude=["tests"]),
+    extras_require=extras,
+    include_package_data=True,
+    python_requires=">=3.6",
+    install_requires=get_requirements(),
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Operating System :: OS Independent",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Science/Research",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Topic :: Education",
+        "Topic :: Scientific/Engineering",
+        "Topic :: Scientific/Engineering :: Artificial Intelligence",
+    ],
+    keywords="machine-learning, deep-learning, pytorch, diffusion, diffusion models, controlnet,stable diffusion",
+)
```

