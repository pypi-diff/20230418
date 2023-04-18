# Comparing `tmp/eaxml2code-0.7.tar.gz` & `tmp/eaxml2code-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\eaxml2code-0.7.tar", last modified: Tue Apr  4 18:24:32 2023, max compression
+gzip compressed data, was "dist/eaxml2code-0.8.tar", last modified: Tue Apr 18 12:24:29 2023, max compression
```

## Comparing `eaxml2code-0.7.tar` & `eaxml2code-0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 18:24:32.000000 eaxml2code-0.7/
--rw-rw-rw-   0        0        0    11558 2023-03-21 17:42:37.000000 eaxml2code-0.7/LICENSE
--rw-rw-rw-   0        0        0      754 2023-04-04 18:24:32.000000 eaxml2code-0.7/PKG-INFO
--rw-rw-rw-   0        0        0      104 2023-03-21 17:42:37.000000 eaxml2code-0.7/README.md
--rw-rw-rw-   0        0        0      933 2023-04-04 18:24:32.000000 eaxml2code-0.7/setup.cfg
--rw-rw-rw-   0        0        0      228 2023-03-26 20:06:17.000000 eaxml2code-0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:24:32.000000 eaxml2code-0.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-04 18:24:32.000000 eaxml2code-0.7/src/eaxml2code/
--rw-rw-rw-   0        0        0       21 2023-04-04 18:20:33.000000 eaxml2code-0.7/src/eaxml2code/__init__.py
--rw-rw-rw-   0        0        0      643 2023-03-21 18:34:44.000000 eaxml2code-0.7/src/eaxml2code/__main__.py
--rw-rw-rw-   0        0        0     4936 2023-04-04 17:52:07.000000 eaxml2code-0.7/src/eaxml2code/main.py
--rw-rw-rw-   0        0        0    24396 2023-04-04 18:08:34.000000 eaxml2code-0.7/src/eaxml2code/modelbuilder.py
--rw-rw-rw-   0        0        0     1916 2023-03-21 20:20:55.000000 eaxml2code-0.7/src/eaxml2code/xmlprocessor.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:24:32.000000 eaxml2code-0.7/src/eaxml2code.egg-info/
--rw-rw-rw-   0        0        0      754 2023-04-04 18:24:32.000000 eaxml2code-0.7/src/eaxml2code.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-04-04 18:24:32.000000 eaxml2code-0.7/src/eaxml2code.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 18:24:32.000000 eaxml2code-0.7/src/eaxml2code.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-04-04 18:24:32.000000 eaxml2code-0.7/src/eaxml2code.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2023-04-04 18:24:32.000000 eaxml2code-0.7/src/eaxml2code.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-04 18:24:32.000000 eaxml2code-0.7/src/eaxml2code.egg-info/top_level.txt
+drwxrwxr-x   0 art       (1000) art       (1000)        0 2023-04-18 12:24:29.000000 eaxml2code-0.8/
+-rw-rw-r--   0 art       (1000) art       (1000)      742 2023-04-18 12:24:29.000000 eaxml2code-0.8/PKG-INFO
+-rw-rw-r--   0 art       (1000) art       (1000)      102 2023-03-27 13:49:00.000000 eaxml2code-0.8/README.md
+-rw-rw-r--   0 art       (1000) art       (1000)    11357 2023-03-27 13:49:00.000000 eaxml2code-0.8/LICENSE
+-rw-rw-r--   0 art       (1000) art       (1000)      901 2023-04-18 12:24:29.000000 eaxml2code-0.8/setup.cfg
+drwxrwxr-x   0 art       (1000) art       (1000)        0 2023-04-18 12:24:29.000000 eaxml2code-0.8/src/
+drwxrwxr-x   0 art       (1000) art       (1000)        0 2023-04-18 12:24:29.000000 eaxml2code-0.8/src/eaxml2code.egg-info/
+-rw-rw-r--   0 art       (1000) art       (1000)        1 2023-04-18 12:24:29.000000 eaxml2code-0.8/src/eaxml2code.egg-info/dependency_links.txt
+-rw-rw-r--   0 art       (1000) art       (1000)      742 2023-04-18 12:24:29.000000 eaxml2code-0.8/src/eaxml2code.egg-info/PKG-INFO
+-rw-rw-r--   0 art       (1000) art       (1000)       12 2023-04-18 12:24:29.000000 eaxml2code-0.8/src/eaxml2code.egg-info/requires.txt
+-rw-rw-r--   0 art       (1000) art       (1000)       11 2023-04-18 12:24:29.000000 eaxml2code-0.8/src/eaxml2code.egg-info/top_level.txt
+-rw-rw-r--   0 art       (1000) art       (1000)      405 2023-04-18 12:24:29.000000 eaxml2code-0.8/src/eaxml2code.egg-info/SOURCES.txt
+-rw-rw-r--   0 art       (1000) art       (1000)       53 2023-04-18 12:24:29.000000 eaxml2code-0.8/src/eaxml2code.egg-info/entry_points.txt
+drwxrwxr-x   0 art       (1000) art       (1000)        0 2023-04-18 12:24:29.000000 eaxml2code-0.8/src/eaxml2code/
+-rw-rw-r--   0 art       (1000) art       (1000)     4808 2023-03-28 07:28:42.000000 eaxml2code-0.8/src/eaxml2code/main.py
+-rw-rw-r--   0 art       (1000) art       (1000)       20 2023-04-18 09:24:39.000000 eaxml2code-0.8/src/eaxml2code/__init__.py
+-rw-rw-r--   0 art       (1000) art       (1000)      623 2023-03-27 13:49:00.000000 eaxml2code-0.8/src/eaxml2code/__main__.py
+-rw-rw-r--   0 art       (1000) art       (1000)     1856 2023-03-27 13:49:00.000000 eaxml2code-0.8/src/eaxml2code/xmlprocessor.py
+-rw-rw-r--   0 art       (1000) art       (1000)    24334 2023-04-18 09:22:35.000000 eaxml2code-0.8/src/eaxml2code/modelbuilder.py
+-rw-rw-r--   0 art       (1000) art       (1000)      218 2023-04-05 08:11:52.000000 eaxml2code-0.8/setup.py
```

### Comparing `eaxml2code-0.7/LICENSE` & `eaxml2code-0.8/LICENSE`

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

### Comparing `eaxml2code-0.7/PKG-INFO` & `eaxml2code-0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-Metadata-Version: 2.1
-Name: eaxml2code
-Version: 0.7
-Summary: Generate C headers from SW component design in Enterprise Architect XMI file.
-Home-page: https://github.com/cimplart/eaxml2code
-Author: CimplArt
-Author-email: artwisz@gmail.com
-License: Apache License, Version 2.0
-Keywords: Enterprise Architect,code generation
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# eaxml2code
-Generate C header files from SW interface definition exported from Enterprise Architect 
-
-
+Metadata-Version: 2.1
+Name: eaxml2code
+Version: 0.8
+Summary: Generate C headers from SW component design in Enterprise Architect XMI file.
+Home-page: https://github.com/cimplart/eaxml2code
+Author: CimplArt
+Author-email: artwisz@gmail.com
+License: Apache License, Version 2.0
+Description: # eaxml2code
+        Generate C header files from SW interface definition exported from Enterprise Architect 
+        
+Keywords: Enterprise Architect,code generation
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Requires-Python: <3.11,>3.6
+Description-Content-Type: text/markdown
```

### Comparing `eaxml2code-0.7/setup.cfg` & `eaxml2code-0.8/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,57 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2065 6178 6d6c 3263 6f64 650d 0a76   = eaxml2code..v
-00000020: 6572 7369 6f6e 203d 2061 7474 723a 2065  ersion = attr: e
-00000030: 6178 6d6c 3263 6f64 652e 5f5f 7665 7273  axml2code.__vers
-00000040: 696f 6e5f 5f0d 0a64 6573 6372 6970 7469  ion__..descripti
-00000050: 6f6e 203d 2047 656e 6572 6174 6520 4320  on = Generate C 
-00000060: 6865 6164 6572 7320 6672 6f6d 2053 5720  headers from SW 
-00000070: 636f 6d70 6f6e 656e 7420 6465 7369 676e  component design
-00000080: 2069 6e20 456e 7465 7270 7269 7365 2041   in Enterprise A
-00000090: 7263 6869 7465 6374 2058 4d49 2066 696c  rchitect XMI fil
-000000a0: 652e 0d0a 6c6f 6e67 5f64 6573 6372 6970  e...long_descrip
-000000b0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
-000000c0: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
-000000d0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
-000000e0: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
-000000f0: 6b64 6f77 6e0d 0a75 726c 203d 2068 7474  kdown..url = htt
-00000100: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000110: 6369 6d70 6c61 7274 2f65 6178 6d6c 3263  cimplart/eaxml2c
-00000120: 6f64 650d 0a6b 6579 776f 7264 7320 3d20  ode..keywords = 
-00000130: 456e 7465 7270 7269 7365 2041 7263 6869  Enterprise Archi
-00000140: 7465 6374 2c20 636f 6465 2067 656e 6572  tect, code gener
-00000150: 6174 696f 6e0d 0a6c 6963 656e 7365 203d  ation..license =
-00000160: 2041 7061 6368 6520 4c69 6365 6e73 652c   Apache License,
-00000170: 2056 6572 7369 6f6e 2032 2e30 0d0a 6175   Version 2.0..au
-00000180: 7468 6f72 203d 2043 696d 706c 4172 740d  thor = CimplArt.
-00000190: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
-000001a0: 6172 7477 6973 7a40 676d 6169 6c2e 636f  artwisz@gmail.co
-000001b0: 6d0d 0a63 6c61 7373 6966 6965 7273 203d  m..classifiers =
-000001c0: 200d 0a09 4c69 6365 6e73 6520 3a3a 204f   ...License :: O
-000001d0: 5349 2041 7070 726f 7665 6420 3a3a 2041  SI Approved :: A
-000001e0: 7061 6368 6520 536f 6674 7761 7265 204c  pache Software L
-000001f0: 6963 656e 7365 0d0a 0950 726f 6772 616d  icense...Program
-00000200: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000210: 2050 7974 686f 6e20 3a3a 2033 0d0a 0949   Python :: 3...I
-00000220: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
-00000230: 203a 3a20 4465 7665 6c6f 7065 7273 0d0a   :: Developers..
-00000240: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
-00000250: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-00000260: 656e 740d 0a0d 0a5b 6f70 7469 6f6e 735d  ent....[options]
-00000270: 0d0a 696e 636c 7564 655f 7061 636b 6167  ..include_packag
-00000280: 655f 6461 7461 203d 2054 7275 650d 0a70  e_data = True..p
-00000290: 6163 6b61 6765 5f64 6972 203d 203d 2073  ackage_dir = = s
-000002a0: 7263 0d0a 7061 636b 6167 6573 203d 2066  rc..packages = f
-000002b0: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
-000002c0: 7569 7265 7320 3d20 3e3d 2033 2e36 0d0a  uires = >= 3.6..
-000002d0: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-000002e0: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
-000002f0: 203d 2073 7263 0d0a 0d0a 5b6f 7074 696f   = src....[optio
-00000300: 6e73 2e70 6163 6b61 6765 5f64 6174 615d  ns.package_data]
-00000310: 0d0a 2a20 3d20 2a2e 786d 6c20 2a2e 6820  ..* = *.xml *.h 
-00000320: 2a2e 7165 610d 0a0d 0a5b 6f70 7469 6f6e  *.qea....[option
-00000330: 732e 656e 7472 795f 706f 696e 7473 5d0d  s.entry_points].
-00000340: 0a63 6f6e 736f 6c65 5f73 6372 6970 7473  .console_scripts
-00000350: 203d 200d 0a09 6561 786d 6c32 636f 6465   = ...eaxml2code
-00000360: 203d 2065 6178 6d6c 3263 6f64 652e 6d61   = eaxml2code.ma
-00000370: 696e 3a6d 6169 6e0d 0a0d 0a5b 6567 675f  in:main....[egg_
-00000380: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-00000390: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-000003a0: 300d 0a0d 0a                             0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6561 786d 6c32 636f 6465 0a76 6572  = eaxml2code.ver
+00000020: 7369 6f6e 203d 2061 7474 723a 2065 6178  sion = attr: eax
+00000030: 6d6c 3263 6f64 652e 5f5f 7665 7273 696f  ml2code.__versio
+00000040: 6e5f 5f0a 6465 7363 7269 7074 696f 6e20  n__.description 
+00000050: 3d20 4765 6e65 7261 7465 2043 2068 6561  = Generate C hea
+00000060: 6465 7273 2066 726f 6d20 5357 2063 6f6d  ders from SW com
+00000070: 706f 6e65 6e74 2064 6573 6967 6e20 696e  ponent design in
+00000080: 2045 6e74 6572 7072 6973 6520 4172 6368   Enterprise Arch
+00000090: 6974 6563 7420 584d 4920 6669 6c65 2e0a  itect XMI file..
+000000a0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000b0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
+000000c0: 6d64 0a6c 6f6e 675f 6465 7363 7269 7074  md.long_descript
+000000d0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
+000000e0: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
+000000f0: 0a75 726c 203d 2068 7474 7073 3a2f 2f67  .url = https://g
+00000100: 6974 6875 622e 636f 6d2f 6369 6d70 6c61  ithub.com/cimpla
+00000110: 7274 2f65 6178 6d6c 3263 6f64 650a 6b65  rt/eaxml2code.ke
+00000120: 7977 6f72 6473 203d 2045 6e74 6572 7072  ywords = Enterpr
+00000130: 6973 6520 4172 6368 6974 6563 742c 2063  ise Architect, c
+00000140: 6f64 6520 6765 6e65 7261 7469 6f6e 0a6c  ode generation.l
+00000150: 6963 656e 7365 203d 2041 7061 6368 6520  icense = Apache 
+00000160: 4c69 6365 6e73 652c 2056 6572 7369 6f6e  License, Version
+00000170: 2032 2e30 0a61 7574 686f 7220 3d20 4369   2.0.author = Ci
+00000180: 6d70 6c41 7274 0a61 7574 686f 725f 656d  mplArt.author_em
+00000190: 6169 6c20 3d20 6172 7477 6973 7a40 676d  ail = artwisz@gm
+000001a0: 6169 6c2e 636f 6d0a 636c 6173 7369 6669  ail.com.classifi
+000001b0: 6572 7320 3d20 0a09 4c69 6365 6e73 6520  ers = ..License 
+000001c0: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+000001d0: 3a3a 2041 7061 6368 6520 536f 6674 7761  :: Apache Softwa
+000001e0: 7265 204c 6963 656e 7365 0a09 5072 6f67  re License..Prog
+000001f0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000200: 203a 3a20 5079 7468 6f6e 203a 3a20 330a   :: Python :: 3.
+00000210: 0949 6e74 656e 6465 6420 4175 6469 656e  .Intended Audien
+00000220: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
+00000230: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
+00000240: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+00000250: 6465 6e74 0a0a 5b6f 7074 696f 6e73 5d0a  dent..[options].
+00000260: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
+00000270: 6461 7461 203d 2054 7275 650a 7061 636b  data = True.pack
+00000280: 6167 655f 6469 7220 3d20 3d20 7372 630a  age_dir = = src.
+00000290: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
+000002a0: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
+000002b0: 203d 203e 332e 362c 203c 332e 3131 0a0a   = >3.6, <3.11..
+000002c0: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+000002d0: 732e 6669 6e64 5d0a 7768 6572 6520 3d20  s.find].where = 
+000002e0: 7372 630a 0a5b 6f70 7469 6f6e 732e 7061  src..[options.pa
+000002f0: 636b 6167 655f 6461 7461 5d0a 2a20 3d20  ckage_data].* = 
+00000300: 2a2e 786d 6c20 2a2e 6820 2a2e 7165 610a  *.xml *.h *.qea.
+00000310: 0a5b 6f70 7469 6f6e 732e 656e 7472 795f  .[options.entry_
+00000320: 706f 696e 7473 5d0a 636f 6e73 6f6c 655f  points].console_
+00000330: 7363 7269 7074 7320 3d20 0a09 6561 786d  scripts = ..eaxm
+00000340: 6c32 636f 6465 203d 2065 6178 6d6c 3263  l2code = eaxml2c
+00000350: 6f64 652e 6d61 696e 3a6d 6169 6e0a 0a5b  ode.main:main..[
+00000360: 6567 675f 696e 666f 5d0a 7461 675f 6275  egg_info].tag_bu
+00000370: 696c 6420 3d20 0a74 6167 5f64 6174 6520  ild = .tag_date 
+00000380: 3d20 300a 0a                             = 0..
```

### Comparing `eaxml2code-0.7/src/eaxml2code/__main__.py` & `eaxml2code-0.8/src/eaxml2code/__main__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-#
-# eaxml2code
-#
-# Copyright 2023 Artur Wisz
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from .main import main
-
-main()
+#
+# eaxml2code
+#
+# Copyright 2023 Artur Wisz
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from .main import main
+
+main()
```

### Comparing `eaxml2code-0.7/src/eaxml2code/main.py` & `eaxml2code-0.8/src/eaxml2code/main.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-#
-# eaxml2code
-#
-# Copyright 2023 Artur Wisz
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from argparse import ArgumentParser
-import json
-from mako.template import Template
-from mako.runtime import Context
-from mako import exceptions
-from io import StringIO
-import pkg_resources
-import os
-import xml.sax
-
-try:
-    from .xmlprocessor import XmlProcessor
-    from .modelbuilder import ModelBuilder
-    from .__init__ import __version__
-except:
-    from xmlprocessor import XmlProcessor
-    from modelbuilder import ModelBuilder
-    from __init__ import __version__
-
-
-def main():
-    try:
-        version = pkg_resources.get_distribution('eaxml2code').version
-    except pkg_resources.DistributionNotFound as e:
-        version = __version__
-    print("eaxml2code version ", version)
-    parser = ArgumentParser()
-    parser.add_argument("-i", "--input", dest="input", help="xml input file", metavar="INPUT-FILE", required=True, nargs='+')
-    parser.add_argument("-e", "--encoding", dest="encoding", help="XML encoding", required=False, default="windows-1252")
-    parser.add_argument("-t", "--template", dest="templ", help="header template", metavar="TEMPLATE", required=True)
-    parser.add_argument("-o", "--odir", dest="odir", help="output folder", metavar="OUTPUT-DIR", required=True)
-    parser.add_argument("-d", "--dump", dest="dump", help="dump content dictionary", default=False, required=False, action='store_true')
-    parser.add_argument("-v", "--verbose", dest="verbose", help="Be more verbose about what is going on",
-                        default=False, required=False, action='store_true')
-
-    args = vars(parser.parse_args())
-
-    with open(args['templ'], 'r') as f:
-        templ_str = f.read()
-
-    if args['verbose']:
-        print("Analyzing code template...")
-    try:
-        header_templ = Template(templ_str)
-    except:
-        print(exceptions.text_error_template().render())
-        raise
-
-    builder = ModelBuilder(args['verbose'])
-
-    for input in args['input']:
-        with open(input, 'r', encoding=args['encoding']) as f:
-            text = f.read()
-            if args['verbose']:
-                print("Parsing input file...")
-            handler = XmlProcessor()
-            xml.sax.parse(input, handler)
-            root = handler.current_element
-
-            if not os.path.exists(args['odir']):
-                if args['verbose']:
-                    print("Creating output directory...")
-                os.mkdir(args['odir'])
-            elif not os.path.isdir(args['odir']):
-                print("ERROR: ", args['odir'], " is not a directory")
-
-            if args['verbose']:
-                print("Dumping raw model dict...")
-                js = json.dumps(root, indent=3)
-                with open(args['odir'] + os.sep + os.path.basename(input) + '_rawmodeldump.json', 'w') as fdump:
-                    fdump.write(js)
-
-            builder.walk_raw_model_subtree(root)
-
-    if args['verbose']:
-        print("Dumping model dict...")
-        js = json.dumps(builder._model, indent=3)
-        with open(args['odir'] + os.sep + 'modeldump.json', 'w') as fdump:
-            fdump.write(js)
-
-    builder.post_process()
-
-    print("Generated headers:")
-    for header in builder._headers:
-        if builder._headers[header]['generated']:
-            print('   ' + header)
-
-    for header in builder._headers:
-        try:
-            if args['dump']:
-                print('------ Dump content for header: ', header, ' ------')
-                dump = json.dumps(builder._headers[header], indent=3)
-                print(dump)
-            if builder._headers[header]['generated']:
-                buf = StringIO()
-                ctx = Context(buf, file=header, content=builder._headers[header])
-                header_templ.render_context(ctx)
-                if args['verbose']:
-                    print("Writing ", header)
-                with open(args['odir'] + '/' + header, "w") as outf:
-                    outf.write(buf.getvalue())
-            else:
-                if args['verbose']:
-                    print("Skip writing ", header)
-        except:
-            print('Exception while rendering ' + header + ': ' + exceptions.text_error_template().render())
-
-    if args['verbose']:
-        print("Done.")
-
-if __name__ == "__main__":
+#
+# eaxml2code
+#
+# Copyright 2023 Artur Wisz
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from argparse import ArgumentParser
+import json
+from mako.template import Template
+from mako.runtime import Context
+from mako import exceptions
+from io import StringIO
+import pkg_resources
+import os
+import xml.sax
+
+try:
+    from .xmlprocessor import XmlProcessor
+    from .modelbuilder import ModelBuilder
+    from .__init__ import __version__
+except:
+    from xmlprocessor import XmlProcessor
+    from modelbuilder import ModelBuilder
+    from __init__ import __version__
+
+
+def main():
+    try:
+        version = pkg_resources.get_distribution('eaxml2code').version
+    except pkg_resources.DistributionNotFound as e:
+        version = __version__
+    print("eaxml2code version ", version)
+    parser = ArgumentParser()
+    parser.add_argument("-i", "--input", dest="input", help="xml input file", metavar="INPUT-FILE", required=True, nargs='+')
+    parser.add_argument("-e", "--encoding", dest="encoding", help="XML encoding", required=False, default="windows-1252")
+    parser.add_argument("-t", "--template", dest="templ", help="header template", metavar="TEMPLATE", required=True)
+    parser.add_argument("-o", "--odir", dest="odir", help="output folder", metavar="OUTPUT-DIR", required=True)
+    parser.add_argument("-d", "--dump", dest="dump", help="dump content dictionary", default=False, required=False, action='store_true')
+    parser.add_argument("-v", "--verbose", dest="verbose", help="Be more verbose about what is going on",
+                        default=False, required=False, action='store_true')
+
+    args = vars(parser.parse_args())
+
+    with open(args['templ'], 'r') as f:
+        templ_str = f.read()
+
+    if args['verbose']:
+        print("Analyzing code template...")
+    try:
+        header_templ = Template(templ_str)
+    except:
+        print(exceptions.text_error_template().render())
+        raise
+
+    builder = ModelBuilder(args['verbose'])
+
+    for input in args['input']:
+        with open(input, 'r', encoding=args['encoding']) as f:
+            text = f.read()
+            if args['verbose']:
+                print("Parsing input file...")
+            handler = XmlProcessor()
+            xml.sax.parse(input, handler)
+            root = handler.current_element
+
+            if not os.path.exists(args['odir']):
+                if args['verbose']:
+                    print("Creating output directory...")
+                os.mkdir(args['odir'])
+            elif not os.path.isdir(args['odir']):
+                print("ERROR: ", args['odir'], " is not a directory")
+
+            if args['verbose']:
+                print("Dumping raw model dict...")
+                js = json.dumps(root, indent=3)
+                with open(args['odir'] + os.sep + os.path.basename(input) + '_rawmodeldump.json', 'w') as fdump:
+                    fdump.write(js)
+
+            builder.walk_raw_model_subtree(root)
+
+    if args['verbose']:
+        print("Dumping model dict...")
+        js = json.dumps(builder._model, indent=3)
+        with open(args['odir'] + os.sep + 'modeldump.json', 'w') as fdump:
+            fdump.write(js)
+
+    builder.post_process()
+
+    print("Generated headers:")
+    for header in builder._headers:
+        if builder._headers[header]['generated']:
+            print('   ' + header)
+
+    for header in builder._headers:
+        try:
+            if args['dump']:
+                print('------ Dump content for header: ', header, ' ------')
+                dump = json.dumps(builder._headers[header], indent=3)
+                print(dump)
+            if builder._headers[header]['generated']:
+                buf = StringIO()
+                ctx = Context(buf, file=header, content=builder._headers[header])
+                header_templ.render_context(ctx)
+                if args['verbose']:
+                    print("Writing ", header)
+                with open(args['odir'] + '/' + header, "w") as outf:
+                    outf.write(buf.getvalue())
+            else:
+                if args['verbose']:
+                    print("Skip writing ", header)
+        except:
+            print('Exception while rendering ' + header + ': ' + exceptions.text_error_template().render())
+
+    if args['verbose']:
+        print("Done.")
+
+if __name__ == "__main__":
     main()
```

### Comparing `eaxml2code-0.7/src/eaxml2code/modelbuilder.py` & `eaxml2code-0.8/src/eaxml2code/modelbuilder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,562 +1,569 @@
-#
-# eaxml2code
-#
-# Copyright 2023 Artur Wisz
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from copy import deepcopy
-import sys
-
-class ModelBuilder:
-
-    def __init__(self, verbose=False):
-        self._model = {}    #intermediate model
-        self._id_map = {}
-        self._model['elements'] = []
-        self._model['dependencies'] = []
-        self._model['attributes'] = []
-        self._model['operations'] = []
-        self._model['literals'] = []
-        self._model['component'] = ''
-
-        self._headers = {}  #main entry point to final model
-
-    @property
-    def current_element(self):
-        if self._model['elements']:
-            return self._model['elements'][-1]
-        else:
-            return None
-
-    def walk_raw_model_subtree(self, node: dict):
-        '''
-        node is from a raw model converted from xml.
-        '''
-        method_map = {
-            'packagedElement': self.visit_packaged_element,
-            'ownedAttribute': self.visit_owned_attribute,
-            'ownedOperation': self.visit_owned_operation,
-            'ownedLiteral': self.visit_owned_literal,
-            'element': self.visit_ea_element,
-            'connector': self.visit_ea_connector,
-            'attribute': self.visit_ea_attribute,
-            'operation': self.visit_ea_operation
-        }
-
-        skip_nodes = [ 'diagrams' ]
-
-        if node['name'] in method_map.keys():
-            if "attributes" in node:
-                attr = node["attributes"]
-                if "xmi:type" in attr:
-                    method_map[node['name']](node, attr['xmi:type'])
-                else:
-                    method_map[node['name']](node)
-            else:
-                print(f"WARNING: {node['name']} without attributes, ignored")
-                return
-
-        if node['name'] in skip_nodes:
-            return
-
-        if "children" in node:
-            for ch in node["children"]:
-                self.walk_raw_model_subtree(ch)
-
-
-    def visit_packaged_element(self, node: dict, xmi_type: str):
-
-        if xmi_type == 'uml:Package' and node['attributes']['xmi:id'].startswith('EAPK_'):
-            if not 'component' in self._model:
-                self._model['component'] = node['attributes']['name']
-        elif xmi_type in [ 'uml:Class', 'uml:Interface', 'uml:Artifact', 'uml:Enumeration', 'uml:Component' ]:
-            model_el = {
-                'name': node['attributes']['name'],
-                'xmi:type': xmi_type,
-                'xmi:id': node['attributes']['xmi:id']
-            }
-            self._model['elements'] += [ model_el ]
-            self._id_map[model_el['xmi:id']] = self._model['elements'][-1]
-        elif xmi_type in [ 'uml:Dependency' ]:
-            model_el = {
-                'xmi:type': xmi_type,
-                'xmi:id': node['attributes']['xmi:id'],
-                'supplier': node['attributes']['supplier'],
-                'client': node['attributes']['client']
-            }
-            self._model['dependencies'] += [ model_el ]
-            self._id_map[model_el['xmi:id']] = self._model['dependencies'][-1]
-
-    def visit_owned_attribute(self, node: dict, xmi_type: str):
-        model_el = {
-            'name': node['attributes'].get('name', ''),
-            'xmi:id': node['attributes']['xmi:id'],
-            'owner': self.current_element['xmi:id']
-        }
-        self._model['attributes'] += [ model_el ]
-        self._id_map[model_el['xmi:id']] = self._model['attributes'][-1]
-
-    def visit_owned_operation(self, node: dict):
-        model_el = {
-            'name': node['attributes']['name'],
-            'xmi:id': node['attributes']['xmi:id'],
-            'owner': self.current_element['xmi:id'],
-            'parameters': []
-        }
-
-        for c in node['children']:
-            assert c['name'] == 'ownedParameter'
-            param_el = {
-                'name': c['attributes']['name'],
-                'xmi:id': c['attributes']['xmi:id'],
-                'direction': c['attributes']['direction']
-            }
-            # 'return' is not really a parameter, just ignore it
-            if param_el['name'] != 'return':
-                model_el['parameters'] += [ param_el ]
-                self._id_map[param_el['xmi:id']] = model_el['parameters'][-1]
-
-        self._model['operations'] += [ model_el ]
-        self._id_map[model_el['xmi:id']] = self._model['operations'][-1]
-
-    def visit_owned_literal(self, node: dict, xmi_type: str):
-        model_el = {
-            'name': node['attributes']['name'],
-            'xmi:id': node['attributes']['xmi:id'],
-            'owner': self.current_element['xmi:id']
-        }
-        self._model['literals'] += [ model_el ]
-        self._id_map[model_el['xmi:id']] = self._model['literals'][-1]
-
-    def visit_ea_element(self, node: dict, xmi_type: str):
-        if xmi_type not in [ 'uml:Class', 'uml:Interface', 'uml:Artifact', 'uml:Enumeration' ]:
-            print('Ignore node ' + xmi_type)
-            return
-
-        try:
-            found = self._id_map[node['attributes']['xmi:idref']]
-        except KeyError as e:
-            return
-        for c in node['children']:
-            if c['name'] == 'properties' and "attributes" in c:
-                if 'documentation' in c['attributes']:
-                    found['description'] = self._clear_formatting(c['attributes']['documentation'])
-                    if xmi_type != 'uml:Artifact':
-                        found['header'] = self._extract_header(found['name'], found['description'])
-                    else:
-                        found['generated'] = self._extract_generated(found['name'], found['description'])
-                if 'stereotype' in c['attributes']:
-                    found['stereotype'] = c['attributes']['stereotype']
-            elif c['name'] == 'links' and found.get('stereotype', '') == 'typedef':
-                for cc in c['children']:
-                    if cc['name'] == 'Generalization':
-                        found['base:id'] = cc['attributes']['end']
-
-    def _extract_header(self, el_name, notes):
-        for line in notes.split('\n'):
-            if 'Declared in:' in line:
-                return line.replace('Declared in:', '').strip()
-        else:
-            raise Exception(f"Missing 'Declared in:' in notes of {el_name}")
-
-    def _extract_generated(self, el_name, notes):
-        for line in notes.split('\n'):
-            if 'Generated:' in line:
-                return 'Yes' in line or 'YES' in line or 'yes' in line
-        else:
-            raise Exception(f"Missing 'Generated:' in notes of {el_name}")
-
-    def visit_ea_attribute(self, node:dict):
-        found = self._id_map[node['attributes']['xmi:idref']]
-        assert found['name'] == node['attributes']['name']
-
-        for c in node['children']:
-            if c['name'] == 'initial':
-                found.setdefault('initial', '')
-                if "attributes" in c:
-                    found['initial'] = c["attributes"]['body']
-            elif c['name'] == 'documentation':
-                found.setdefault('description', '')
-                if "attributes" in c:
-                    found['description'] = self._clear_formatting(c['attributes']['value'])
-            elif c['name'] == 'properties' and 'attributes' in c:
-                found['type'] = c['attributes'].get('type', '')
-                found['static'] = 'static' if c['attributes'].get('static', '') == '1' else ''
-
-
-    def visit_ea_operation(self, node:dict):
-        found = self._id_map[node['attributes']['xmi:idref']]
-        assert found['name'] == node['attributes']['name']
-
-        for c in node['children']:
-            if c['name'] == 'stereotype' and 'attributes' in c:
-                found['stereotype'] = c['attributes']['stereotype']
-            elif c['name'] == 'type':
-                found['static'] = c['attributes']["static"]
-                found.setdefault('return-value', {})
-                found['return-value'].setdefault('description', '')
-                if "type" in c['attributes']:
-                    found['return-value']['type'] = c['attributes']['type']
-                else:
-                    found['return-value']['type'] = 'void'
-            elif c['name'] == 'documentation':
-                if 'attributes' in c:
-                    found['description'] = self._clear_formatting(c['attributes']['value'])
-                    if found['return-value']['type'] != 'void':
-                        found['return-value']['description'] = self._extract_return_value_description(found['name'], found['description'])
-                elif found.get('return-value', {}).get('type', 'void') != 'void':
-                    print(f"WARNING: operation {found['name']} returning non-void is missing return value description")
-            elif c['name'] == 'parameters':
-                self._collect_parameters(c, found['parameters'])
-
-    def _extract_return_value_description(self, op_name, description):
-        for line in description.split('\n'):
-            if 'Return value:' in line:
-                return line.replace('Return value:', '').strip()
-        print(f"WARNING: return value of {op_name} is missing description")
-        return ''
-
-    def _collect_parameters(self, node:dict, params: list):
-        for c in node['children']:
-            assert c['name'] == 'parameter'
-            assert "attributes" in c
-            if c['attributes']['xmi:idref'].startswith('EAID_RETURNID_'):
-                #Skip return parameters
-                continue
-            for p in params:
-                if p['xmi:id'] == c['attributes']['xmi:idref']:
-                    found_param = p
-                    break
-            else:
-                print(f"WARNING: parameter {c['attributes']['xmi:idref']} was not found")
-                found_param = None
-                continue
-            found_param.setdefault('description', '')
-            for cc in c['children']:
-                if cc['name'] == 'properties':
-                    found_param['type'] = cc['attributes'].get('type', '')
-                    found_param['position'] = cc['attributes']['pos']
-                    found_param['const'] = cc['attributes']['const']
-                elif cc['name'] == 'documentation' and 'attributes' in cc:
-                    found_param['description'] = self._clear_formatting(cc['attributes']['value'])
-
-    def visit_ea_connector(self, node:dict):
-        found = self._id_map.get(node['attributes']['xmi:idref'], None)
-        if found is None:
-            return
-
-        for c in node['children']:
-            if c['name'] == 'properties':
-                found['stereotype'] = c['attributes'].get('stereotype', '')
-                found['type'] = c['attributes']['ea_type']
-
-    _default_header_content = {
-        'functions': list(),
-        'types': list(),
-        'variables': list(),
-        'macro-constants': list(),
-        'includes': list(),
-        'file-name': '',
-        'description': '',
-        'generated': False
-    }
-
-    #Create the final model for use in the code template.
-    def post_process(self):
-        self._create_headers()
-        self._arrange_function_groups()
-        self._arrange_types()
-        self._arrange_variables()
-        self._arrange_macro_constants()
-
-    def _create_headers(self):
-        for el in self._model['elements']:
-            if el['xmi:type'] == 'uml:Artifact':
-                if not 'stereotype' in el:
-                    print(f"WARNING: artifact {el['name']} has no stereotype, ignoring")
-                elif el['stereotype'] == 'header':
-                    self._headers.setdefault(el['name'], deepcopy(self._default_header_content))
-                    header_ref = self._headers[el['name']]
-                    header_ref['file-name'] = el['name']
-                    if not 'description' in el:
-                        print(f"WARNING: artifact {el['name']} is missing description")
-                    header_ref['description'] = self._clean_el_description(el.get('description', ''))
-                    header_ref['generated'] = el.get('generated', False)
-                    header_ref['component'] = self._model['component']
-                    header_ref['includes'] = []
-                    self._get_includes(el, header_ref)
-
-    def _get_includes(self, artifact, header_ref):
-        for dep in self._model['dependencies']:
-            if dep['client'] == artifact['xmi:id'] and dep.get('stereotype', 'include'):
-                if dep['supplier'] in self._id_map:
-                    supplier_el = self._id_map[dep['supplier']]
-                    header_ref['includes'] += [ supplier_el['name'] ]
-                else:
-                    print(f"WARNING: artifact {dep['supplier']} not found in the model, ignoring")
-
-    def _get_brief(self, descr: str):
-        p_dot = descr.find('.')
-        p_newl = descr.find('\n')
-        if p_dot < 0:
-            p_dot = sys.maxsize
-        if p_newl < 0:
-            p_newl = sys.maxsize
-        cut_point = min([ p_dot, p_newl ])
-        if cut_point < sys.maxsize:
-            return descr[:cut_point]
-        else:
-            return "GO FIX THIS DESCRIPTION"
-
-    #
-    # Post-process operations
-    #
-    def _arrange_function_groups(self):
-        for el in self._model['elements']:
-            if el['xmi:type'] == 'uml:Interface':
-                functions_group = {
-                    'functions-group': el['name'],
-                    'functions': [ ]
-                }
-                self._headers[el['header']]['functions'] += [ functions_group ]
-                #add functions for this owner
-                for f in self._model['operations']:
-                    if f['owner'] == el['xmi:id']:
-                        functions_group['functions'] += [ f ]
-                        #supplement missing keys
-                        f.setdefault('in-params', [])
-                        f.setdefault('out-params', [])
-                        f.setdefault('inout-params', [])
-                        f.setdefault('return-value', { 'type': 'void', 'description': '' })
-                        f['description'] = self._clean_el_description(f.get('description', ''))
-                        f['brief'] = self._get_brief(f['description'])
-
-                        self._set_func_params(f)
-                        if 'stereotype' in f and f['stereotype'] == "macro":
-                            f['is-macro'] = True
-                            self._set_func_macro_syntax(f)
-                            self._set_func_macro_definition(f)
-                        else:
-                            f['is-macro'] = False
-                            self._set_func_syntax(f)
-
-    def _set_func_syntax(self, func):
-        syntax = ''
-        if func['static'] == 'true':
-            syntax = 'static '
-        syntax += func['return-value']['type'] + ' ' + func['name'] + '('
-        for p in func['parameters']:
-            if p['name'] == "...":
-                syntax += p['name'] + ', '
-            else:
-                type = p['type']
-                if p['const'] == 'true' and not type.startswith('const'):
-                    type = 'const ' + type
-                syntax += type + ' ' + p['name'] + ', '
-        if syntax.endswith(', '):
-            syntax = syntax[:-2]
-        syntax += ')'
-        func['syntax'] = syntax
-
-    def _set_func_params(self, func):
-        for p in func['parameters']:
-            key = p['direction'] + '-params'
-            func[key] += [
-                {
-                    'name': p['name'],
-                    'description': p['description']
-                }
-            ]
-
-    def _set_func_macro_syntax(self, func):
-        syntax = func['name'] + '('
-        for p in func['parameters']:
-            syntax += p['name'] + ', '
-        if syntax.endswith(', '):
-            syntax = syntax[:-2]
-        syntax += ')'
-        func['syntax'] = syntax
-
-    def _set_func_macro_definition(self, func):
-        code = ''
-        descr = ''
-        add_to_code = False
-        leading_spaces = None
-        for line in func['description'].split('\n'):
-            if add_to_code:
-                if line.strip():
-                    if leading_spaces is None:
-                        leading_spaces = len(line) - len(line.lstrip(' '))
-                    code += line[leading_spaces:] + '\n'
-            elif 'Definition:' in line:
-                add_to_code = True
-            else:
-                descr += line.strip() + '\n'
-        func['definition'] = code.replace('&amp;', '&').replace('&lt;', '<').replace('&gt;', '>')
-        # Remove Definition: from description.
-        func['description'] = descr.strip()
-
-    #
-    # Post-process types
-    #
-    def _arrange_types(self):
-        for el in self._model['elements']:
-            if el['xmi:type'] == 'uml:Class' and el.get('stereotype', '') == 'struct':
-                type = {
-                    'brief': self._get_brief(el['description']),
-                    'description': self._clean_el_description(el['description']),
-                    'kind': 'Structure',
-                    'type-name': el['name'],
-                    'elements': []
-                }
-                self._add_struct_fields(el, type)
-                self._headers[el['header']]['types'] += [ type ]
-            elif el['xmi:type'] == 'uml:Enumeration' and not 'stereotype' in el:
-                type = {
-                    'brief': self._get_brief(el['description']),
-                    'description': self._clean_el_description(el['description']),
-                    'kind': 'Enumeration',
-                    'type-name': el['name'],
-                    'constants': []
-                }
-                self._add_enums(el, type)
-                self._headers[el['header']]['types'] += [ type ]
-            elif el['xmi:type'] == 'uml:Class' and el.get('stereotype', '') == 'typedef':
-                #Generalization has priority over containment.
-                if 'base:id' in el:
-                    found_base_type_el = self._id_map.get(el['base:id'], None)
-                    declaration = self._make_typedef_from_base(el, found_base_type_el)
-                else:
-                    found_feature = self._find_typedef_feature(el['xmi:id'])
-                    if found_feature != None:
-                        declaration = self._make_typedef_from_feature(el, found_feature)
-                    else:
-                        print(f"WARNING: insufficient information for typedef declaration of {el['name']}, ignoring")
-                        return
-                type = {
-                    'brief': self._get_brief(el['description']),
-                    'description': self._clean_el_description(el['description']),
-                    'kind': 'Typedef',
-                    'type-name': el['name'],
-                    'declaration': declaration
-                }
-                self._headers[el['header']]['types'] += [ type ]
-
-    def _find_typedef_feature(self, owner):
-        for attr in self._model['attributes']:
-            if attr['owner'] == owner:
-                return attr
-        for op in self._model['operations']:
-            if op['owner'] == owner:
-                return op
-        return None
-
-    def _make_typedef_from_feature(self, el, feat):
-        if 'parameters' in feat and 'return-value' in feat:
-            if not feat['name'].startswith('(*') or not feat['name'].endswith(')'):
-                print(f"WARNING: invalid declaration information for typedef f{el['name']} - expecting pointer to function")
-                return ''
-            decl = 'typedef ' + feat['return-value']['type'] + ' ' + feat['name'] + '('
-            if len(feat['parameters']):
-                for p in feat['parameters']:
-                    decl += p['type'] + ', '
-                decl = decl[:-2]
-            decl += ')'
-        else:
-            if not 'type' in feat or not feat['type']:
-                print("WARNING: missing or invalid type for typedef declaration")
-            decl = 'typedef ' + feat['type'] + ' ' + el['name']
-        return decl
-
-    def _make_typedef_from_base(self, el, base):
-        return 'typedef ' + base['name'] + ' ' + el['name']
-
-    def _clear_formatting(self, descr):
-        cleaned = ''
-        for line in descr.split('\n'):
-            l = line.replace('<b>', '').replace('</b>', '').replace('<i>', '').replace('</i>', '')
-            cleaned += l + '\n'
-        return cleaned.strip()
-
-
-    def _clean_el_description(self, descr):
-        unformatted = self._clear_formatting(descr)
-        cleaned = ''
-        for line in unformatted.split('\n'):
-            if 'Declared in:' not in line and 'Generated:' not in line:
-                cleaned += line + '\n'
-        return cleaned.strip()
-
-    def _add_struct_fields(self, el, type):
-        for a in self._model['attributes']:
-            if a['owner'] == el['xmi:id']:
-                struct_el = {
-                    'description': a['description'],
-                    'type': a['type'],
-                    'field': a['name']
-                }
-                type['elements'].append(struct_el)
-
-    def _add_enums(self, el, type):
-        for l in self._model['literals']:
-            if l['owner'] == el['xmi:id']:
-                constant = {
-                    'name': l['name'],
-                    'description': l['description'],
-                    'value': l["initial"]
-                }
-                type['constants'].append(constant)
-
-    #
-    # Post-process variables
-    #
-    def _arrange_variables(self):
-        for el in self._model['elements']:
-            if el['xmi:type'] == 'uml:Class' and el.get('stereotype', '') == 'variables':
-                variables_group = {
-                    'variables-group': el['name'],
-                    'variables':  [ ]
-                }
-                self._headers[el['header']]['variables'] += [ variables_group ]
-                #add attributes for this owner
-                for a in self._model['attributes']:
-                    if a['owner'] == el['xmi:id']:
-                        variables_group['variables'] += [ a ]
-                        # description is already set
-                        a['syntax'] = a['static'] + bool(a['static']) * ' ' + a['type'] + ' ' + a['name']
-                        if a['initial']:
-                            a['syntax'] += ' = ' + a['initial']
-
-    #
-    # Post-process macro constants
-    #
-    def _arrange_macro_constants(self):
-        for el in self._model['elements']:
-            if el['xmi:type'] == 'uml:Enumeration' and el.get('stereotype', '') == 'macros':
-                macro_constants_group = {
-                    'constants-group': el['name'],
-                    'constants': []
-                }
-                self._headers[el['header']]['macro-constants'] += [ macro_constants_group ]
-                #add constants for this owner
-                for c in self._model['literals']:
-                    if c['owner'] == el['xmi:id']:
-                        macro_constants_group['constants'] += [ c ]
-                        # name and description are already set
-                        if not c['initial'] and 'Definition:' in c['description']:
-                            self._set_func_macro_definition(c)
-                        else:
-                            c['value'] = c['initial']
-
-
+#
+# eaxml2code
+#
+# Copyright 2023 Artur Wisz
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from copy import deepcopy
+import sys
+
+class ModelBuilder:
+
+    def __init__(self, verbose=False):
+        self._model = {}    #intermediate model
+        self._id_map = {}
+        self._model['elements'] = []
+        self._model['dependencies'] = []
+        self._model['attributes'] = []
+        self._model['operations'] = []
+        self._model['literals'] = []
+        self._model['component'] = ''
+
+        self._headers = {}  #main entry point to final model
+
+    @property
+    def current_element(self):
+        if self._model['elements']:
+            return self._model['elements'][-1]
+        else:
+            return None
+
+    def walk_raw_model_subtree(self, node: dict):
+        '''
+        node is from a raw model converted from xml.
+        '''
+        method_map = {
+            'packagedElement': self.visit_packaged_element,
+            'ownedAttribute': self.visit_owned_attribute,
+            'ownedOperation': self.visit_owned_operation,
+            'ownedLiteral': self.visit_owned_literal,
+            'element': self.visit_ea_element,
+            'connector': self.visit_ea_connector,
+            'attribute': self.visit_ea_attribute,
+            'operation': self.visit_ea_operation
+        }
+
+        skip_nodes = [ 'diagrams' ]
+
+        if node['name'] in method_map.keys():
+            if "attributes" in node:
+                attr = node["attributes"]
+                if "xmi:type" in attr:
+                    method_map[node['name']](node, attr['xmi:type'])
+                else:
+                    method_map[node['name']](node)
+            else:
+                print(f"WARNING: {node['name']} without attributes, ignored")
+                return
+
+        if node['name'] in skip_nodes:
+            return
+
+        if "children" in node:
+            for ch in node["children"]:
+                self.walk_raw_model_subtree(ch)
+
+
+    def visit_packaged_element(self, node: dict, xmi_type: str):
+
+        if xmi_type == 'uml:Package' and node['attributes']['xmi:id'].startswith('EAPK_'):
+            if not 'component' in self._model:
+                self._model['component'] = node['attributes']['name']
+        elif xmi_type in [ 'uml:Class', 'uml:Interface', 'uml:Artifact', 'uml:Enumeration', 'uml:Component' ]:
+            model_el = {
+                'name': node['attributes']['name'],
+                'xmi:type': xmi_type,
+                'xmi:id': node['attributes']['xmi:id']
+            }
+            self._model['elements'] += [ model_el ]
+            self._id_map[model_el['xmi:id']] = self._model['elements'][-1]
+        elif xmi_type in [ 'uml:Dependency' ]:
+            model_el = {
+                'xmi:type': xmi_type,
+                'xmi:id': node['attributes']['xmi:id'],
+                'supplier': node['attributes']['supplier'],
+                'client': node['attributes']['client']
+            }
+            self._model['dependencies'] += [ model_el ]
+            self._id_map[model_el['xmi:id']] = self._model['dependencies'][-1]
+
+    def visit_owned_attribute(self, node: dict, xmi_type: str):
+        model_el = {
+            'name': node['attributes'].get('name', ''),
+            'xmi:id': node['attributes']['xmi:id'],
+            'owner': self.current_element['xmi:id']
+        }
+        self._model['attributes'] += [ model_el ]
+        self._id_map[model_el['xmi:id']] = self._model['attributes'][-1]
+
+    def visit_owned_operation(self, node: dict):
+        model_el = {
+            'name': node['attributes']['name'],
+            'xmi:id': node['attributes']['xmi:id'],
+            'owner': self.current_element['xmi:id'],
+            'parameters': []
+        }
+
+        for c in node['children']:
+            assert c['name'] == 'ownedParameter'
+            param_el = {
+                'name': c['attributes']['name'],
+                'xmi:id': c['attributes']['xmi:id'],
+                'direction': c['attributes']['direction']
+            }
+            # 'return' is not really a parameter, just ignore it
+            if param_el['name'] != 'return':
+                model_el['parameters'] += [ param_el ]
+                self._id_map[param_el['xmi:id']] = model_el['parameters'][-1]
+
+        self._model['operations'] += [ model_el ]
+        self._id_map[model_el['xmi:id']] = self._model['operations'][-1]
+
+    def visit_owned_literal(self, node: dict, xmi_type: str):
+        model_el = {
+            'name': node['attributes']['name'],
+            'xmi:id': node['attributes']['xmi:id'],
+            'owner': self.current_element['xmi:id']
+        }
+        self._model['literals'] += [ model_el ]
+        self._id_map[model_el['xmi:id']] = self._model['literals'][-1]
+
+    def visit_ea_element(self, node: dict, xmi_type: str):
+        if xmi_type not in [ 'uml:Class', 'uml:Interface', 'uml:Artifact', 'uml:Enumeration' ]:
+            print('Ignore node ' + xmi_type)
+            return
+
+        try:
+            found = self._id_map[node['attributes']['xmi:idref']]
+        except KeyError as e:
+            return
+        for c in node['children']:
+            if c['name'] == 'properties' and "attributes" in c:
+                if 'documentation' in c['attributes']:
+                    found['description'] = self._clear_formatting(c['attributes']['documentation'])
+                    if xmi_type != 'uml:Artifact':
+                        found['header'] = self._extract_header(found['name'], found['description'])
+                    else:
+                        found['generated'] = self._extract_generated(found['name'], found['description'])
+                if 'stereotype' in c['attributes']:
+                    found['stereotype'] = c['attributes']['stereotype']
+            elif c['name'] == 'links' and found.get('stereotype', '') == 'typedef':
+                for cc in c['children']:
+                    #Only consider outgoing links.
+                    if cc['name'] == 'Generalization' and cc['attributes']['end'] != found['xmi:id']:
+                        found['base:id'] = cc['attributes']['end']
+
+    def _extract_header(self, el_name, notes):
+        for line in notes.split('\n'):
+            if 'Declared in:' in line:
+                return line.replace('Declared in:', '').strip()
+        else:
+            raise Exception(f"Missing 'Declared in:' in notes of {el_name}")
+
+    def _extract_generated(self, el_name, notes):
+        for line in notes.split('\n'):
+            if 'Generated:' in line:
+                return 'Yes' in line or 'YES' in line or 'yes' in line
+        else:
+            raise Exception(f"Missing 'Generated:' in notes of {el_name}")
+
+    def visit_ea_attribute(self, node:dict):
+        found = self._id_map[node['attributes']['xmi:idref']]
+        assert found['name'] == node['attributes']['name']
+
+        for c in node['children']:
+            if c['name'] == 'initial':
+                found.setdefault('initial', '')
+                if "attributes" in c:
+                    found['initial'] = c["attributes"]['body']
+            elif c['name'] == 'documentation':
+                found.setdefault('description', '')
+                if "attributes" in c:
+                    found['description'] = self._clear_formatting(c['attributes']['value'])
+            elif c['name'] == 'properties' and 'attributes' in c:
+                found['type'] = c['attributes'].get('type', '')
+                found['static'] = 'static' if c['attributes'].get('static', '') == '1' else ''
+
+
+    def visit_ea_operation(self, node:dict):
+        found = self._id_map[node['attributes']['xmi:idref']]
+        assert found['name'] == node['attributes']['name']
+
+        for c in node['children']:
+            if c['name'] == 'stereotype' and 'attributes' in c:
+                found['stereotype'] = c['attributes']['stereotype']
+            elif c['name'] == 'type':
+                found['static'] = c['attributes']["static"]
+                found.setdefault('return-value', {})
+                found['return-value'].setdefault('description', '')
+                if "type" in c['attributes']:
+                    found['return-value']['type'] = c['attributes']['type']
+                else:
+                    found['return-value']['type'] = 'void'
+            elif c['name'] == 'documentation':
+                if 'attributes' in c:
+                    found['description'] = self._clear_formatting(c['attributes']['value'])
+                    if found['return-value']['type'] != 'void':
+                        found['return-value']['description'] = self._extract_return_value_description(found['name'], found['description'])
+                elif found.get('return-value', {}).get('type', 'void') != 'void':
+                    print(f"WARNING: operation {found['name']} returning non-void is missing return value description")
+            elif c['name'] == 'parameters':
+                self._collect_parameters(c, found['parameters'])
+
+    def _extract_return_value_description(self, op_name, description):
+        for line in description.split('\n'):
+            if 'Return value:' in line:
+                return line.replace('Return value:', '').strip()
+        print(f"WARNING: return value of {op_name} is missing description")
+        return ''
+
+    def _collect_parameters(self, node:dict, params: list):
+        for c in node['children']:
+            assert c['name'] == 'parameter'
+            assert "attributes" in c
+            if c['attributes']['xmi:idref'].startswith('EAID_RETURNID_'):
+                #Skip return parameters
+                continue
+            for p in params:
+                if p['xmi:id'] == c['attributes']['xmi:idref']:
+                    found_param = p
+                    break
+            else:
+                print(f"WARNING: parameter {c['attributes']['xmi:idref']} was not found")
+                found_param = None
+                continue
+            found_param.setdefault('description', '')
+            for cc in c['children']:
+                if cc['name'] == 'properties':
+                    found_param['type'] = cc['attributes'].get('type', '')
+                    found_param['position'] = cc['attributes']['pos']
+                    found_param['const'] = cc['attributes']['const']
+                elif cc['name'] == 'documentation' and 'attributes' in cc:
+                    found_param['description'] = self._clear_formatting(cc['attributes']['value'])
+
+    def visit_ea_connector(self, node:dict):
+        found = self._id_map.get(node['attributes']['xmi:idref'], None)
+        if found is None:
+            return
+
+        for c in node['children']:
+            if c['name'] == 'properties':
+                found['stereotype'] = c['attributes'].get('stereotype', '')
+                found['type'] = c['attributes']['ea_type']
+
+    _default_header_content = {
+        'functions': list(),
+        'types': list(),
+        'variables': list(),
+        'macro-constants': list(),
+        'includes': list(),
+        'file-name': '',
+        'description': '',
+        'generated': False
+    }
+
+    #Create the final model for use in the code template.
+    def post_process(self):
+        self._create_headers()
+        self._arrange_function_groups()
+        self._arrange_types()
+        self._arrange_variables()
+        self._arrange_macro_constants()
+
+    def _create_headers(self):
+        for el in self._model['elements']:
+            if el['xmi:type'] == 'uml:Artifact':
+                if not 'stereotype' in el:
+                    print(f"WARNING: artifact {el['name']} has no stereotype, ignoring")
+                elif el['stereotype'] == 'header':
+                    self._headers.setdefault(el['name'], deepcopy(self._default_header_content))
+                    header_ref = self._headers[el['name']]
+                    header_ref['file-name'] = el['name']
+                    if not 'description' in el:
+                        print(f"WARNING: artifact {el['name']} is missing description")
+                    header_ref['description'] = self._clean_el_description(el.get('description', ''))
+                    header_ref['generated'] = el.get('generated', False)
+                    header_ref['component'] = self._model['component']
+                    header_ref['includes'] = []
+                    self._get_includes(el, header_ref)
+
+    def _get_includes(self, artifact, header_ref):
+        for dep in self._model['dependencies']:
+            if dep['client'] == artifact['xmi:id'] and dep.get('stereotype', 'include'):
+                if dep['supplier'] in self._id_map:
+                    supplier_el = self._id_map[dep['supplier']]
+                    header_ref['includes'] += [ supplier_el['name'] ]
+                else:
+                    print(f"WARNING: artifact {dep['supplier']} not found in the model, ignoring")
+
+    def _get_brief(self, descr: str):
+        p_dot = descr.find('.')
+        p_newl = descr.find('\n')
+        if p_dot < 0:
+            p_dot = sys.maxsize
+        if p_newl < 0:
+            p_newl = sys.maxsize
+        cut_point = min([ p_dot, p_newl ])
+        if cut_point < sys.maxsize:
+            return descr[:cut_point]
+        else:
+            return "GO FIX THIS DESCRIPTION"
+
+    #
+    # Post-process operations
+    #
+    def _arrange_function_groups(self):
+        for el in self._model['elements']:
+            if el['xmi:type'] == 'uml:Interface':
+                functions_group = {
+                    'functions-group': el['name'],
+                    'functions': [ ]
+                }
+                if 'header' not in el:
+                    print(f"WARNING: interface {el['name']} not assigned to any header file, will not be generated")
+                    continue
+                if el['header'] not in self._headers:
+                    print(f"WARNING: interface {el['name']} assigned to undefined header file {el['header']}, will not be generated")
+                    continue
+                self._headers[el['header']]['functions'] += [ functions_group ]
+                #add functions for this owner
+                for f in self._model['operations']:
+                    if f['owner'] == el['xmi:id']:
+                        functions_group['functions'] += [ f ]
+                        #supplement missing keys
+                        f.setdefault('in-params', [])
+                        f.setdefault('out-params', [])
+                        f.setdefault('inout-params', [])
+                        f.setdefault('return-value', { 'type': 'void', 'description': '' })
+                        f['description'] = self._clean_el_description(f.get('description', ''))
+                        f['brief'] = self._get_brief(f['description'])
+
+                        self._set_func_params(f)
+                        if 'stereotype' in f and f['stereotype'] == "macro":
+                            f['is-macro'] = True
+                            self._set_func_macro_syntax(f)
+                            self._set_func_macro_definition(f)
+                        else:
+                            f['is-macro'] = False
+                            self._set_func_syntax(f)
+
+    def _set_func_syntax(self, func):
+        syntax = ''
+        if func['static'] == 'true':
+            syntax = 'static '
+        syntax += func['return-value']['type'] + ' ' + func['name'] + '('
+        for p in func['parameters']:
+            if p['name'] == "...":
+                syntax += p['name'] + ', '
+            else:
+                type = p['type']
+                if p['const'] == 'true' and not type.startswith('const'):
+                    type = 'const ' + type
+                syntax += type + ' ' + p['name'] + ', '
+        if syntax.endswith(', '):
+            syntax = syntax[:-2]
+        syntax += ')'
+        func['syntax'] = syntax
+
+    def _set_func_params(self, func):
+        for p in func['parameters']:
+            key = p['direction'] + '-params'
+            func[key] += [
+                {
+                    'name': p['name'],
+                    'description': p['description']
+                }
+            ]
+
+    def _set_func_macro_syntax(self, func):
+        syntax = func['name'] + '('
+        for p in func['parameters']:
+            syntax += p['name'] + ', '
+        if syntax.endswith(', '):
+            syntax = syntax[:-2]
+        syntax += ')'
+        func['syntax'] = syntax
+
+    def _set_func_macro_definition(self, func):
+        code = ''
+        descr = ''
+        add_to_code = False
+        leading_spaces = None
+        for line in func['description'].split('\n'):
+            if add_to_code:
+                if line.strip():
+                    if leading_spaces is None:
+                        leading_spaces = len(line) - len(line.lstrip(' '))
+                    code += line[leading_spaces:] + '\n'
+            elif 'Definition:' in line:
+                add_to_code = True
+            else:
+                descr += line.strip() + '\n'
+        func['definition'] = code.replace('&amp;', '&').replace('&lt;', '<').replace('&gt;', '>')
+        # Remove Definition: from description.
+        func['description'] = descr.strip()
+
+    #
+    # Post-process types
+    #
+    def _arrange_types(self):
+        for el in self._model['elements']:
+            if el['xmi:type'] == 'uml:Class' and el.get('stereotype', '') == 'struct':
+                type = {
+                    'brief': self._get_brief(el['description']),
+                    'description': self._clean_el_description(el['description']),
+                    'kind': 'Structure',
+                    'type-name': el['name'],
+                    'elements': []
+                }
+                self._add_struct_fields(el, type)
+                self._headers[el['header']]['types'] += [ type ]
+            elif el['xmi:type'] == 'uml:Enumeration' and not 'stereotype' in el:
+                type = {
+                    'brief': self._get_brief(el['description']),
+                    'description': self._clean_el_description(el['description']),
+                    'kind': 'Enumeration',
+                    'type-name': el['name'],
+                    'constants': []
+                }
+                self._add_enums(el, type)
+                self._headers[el['header']]['types'] += [ type ]
+            elif el['xmi:type'] == 'uml:Class' and el.get('stereotype', '') == 'typedef':
+                #Generalization has priority over containment.
+                if 'base:id' in el:
+                    found_base_type_el = self._id_map.get(el['base:id'], None)
+                    declaration = self._make_typedef_from_base(el, found_base_type_el)
+                else:
+                    found_feature = self._find_typedef_feature(el['xmi:id'])
+                    if found_feature != None:
+                        declaration = self._make_typedef_from_feature(el, found_feature)
+                    else:
+                        print(f"WARNING: insufficient information for typedef declaration of {el['name']}, ignoring")
+                        return
+                type = {
+                    'brief': self._get_brief(el['description']),
+                    'description': self._clean_el_description(el['description']),
+                    'kind': 'Typedef',
+                    'type-name': el['name'],
+                    'declaration': declaration
+                }
+                self._headers[el['header']]['types'] += [ type ]
+
+    def _find_typedef_feature(self, owner):
+        for attr in self._model['attributes']:
+            if attr['owner'] == owner:
+                return attr
+        for op in self._model['operations']:
+            if op['owner'] == owner:
+                return op
+        return None
+
+    def _make_typedef_from_feature(self, el, feat):
+        if 'parameters' in feat and 'return-value' in feat:
+            if not feat['name'].startswith('(*') or not feat['name'].endswith(')'):
+                print(f"WARNING: invalid declaration information for typedef f{el['name']} - expecting pointer to function")
+                return ''
+            decl = 'typedef ' + feat['return-value']['type'] + ' ' + feat['name'] + '('
+            if len(feat['parameters']):
+                for p in feat['parameters']:
+                    decl += p['type'] + ', '
+                decl = decl[:-2]
+            decl += ')'
+        else:
+            if not 'type' in feat or not feat['type']:
+                print("WARNING: missing or invalid type for typedef declaration")
+            decl = 'typedef ' + feat['type'] + ' ' + el['name']
+        return decl
+
+    def _make_typedef_from_base(self, el, base):
+        return 'typedef ' + base['name'] + ' ' + el['name']
+
+    def _clear_formatting(self, descr):
+        cleaned = ''
+        for line in descr.split('\n'):
+            l = line.replace('<b>', '').replace('</b>', '').replace('<i>', '').replace('</i>', '')
+            cleaned += l + '\n'
+        return cleaned.strip()
+
+
+    def _clean_el_description(self, descr):
+        unformatted = self._clear_formatting(descr)
+        cleaned = ''
+        for line in unformatted.split('\n'):
+            if 'Declared in:' not in line and 'Generated:' not in line:
+                cleaned += line + '\n'
+        return cleaned.strip()
+
+    def _add_struct_fields(self, el, type):
+        for a in self._model['attributes']:
+            if a['owner'] == el['xmi:id']:
+                struct_el = {
+                    'description': a['description'],
+                    'type': a['type'],
+                    'field': a['name']
+                }
+                type['elements'].append(struct_el)
+
+    def _add_enums(self, el, type):
+        for l in self._model['literals']:
+            if l['owner'] == el['xmi:id']:
+                constant = {
+                    'name': l['name'],
+                    'description': l['description'],
+                    'value': l["initial"]
+                }
+                type['constants'].append(constant)
+
+    #
+    # Post-process variables
+    #
+    def _arrange_variables(self):
+        for el in self._model['elements']:
+            if el['xmi:type'] == 'uml:Class' and el.get('stereotype', '') == 'variables':
+                variables_group = {
+                    'variables-group': el['name'],
+                    'variables':  [ ]
+                }
+                self._headers[el['header']]['variables'] += [ variables_group ]
+                #add attributes for this owner
+                for a in self._model['attributes']:
+                    if a['owner'] == el['xmi:id']:
+                        variables_group['variables'] += [ a ]
+                        # description is already set
+                        a['syntax'] = a['static'] + bool(a['static']) * ' ' + a['type'] + ' ' + a['name']
+                        if a['initial']:
+                            a['syntax'] += ' = ' + a['initial']
+
+    #
+    # Post-process macro constants
+    #
+    def _arrange_macro_constants(self):
+        for el in self._model['elements']:
+            if el['xmi:type'] == 'uml:Enumeration' and el.get('stereotype', '') == 'macros':
+                macro_constants_group = {
+                    'constants-group': el['name'],
+                    'constants': []
+                }
+                self._headers[el['header']]['macro-constants'] += [ macro_constants_group ]
+                #add constants for this owner
+                for c in self._model['literals']:
+                    if c['owner'] == el['xmi:id']:
+                        macro_constants_group['constants'] += [ c ]
+                        # name and description are already set
+                        if not c['initial'] and 'Definition:' in c['description']:
+                            self._set_func_macro_definition(c)
+                        else:
+                            c['value'] = c['initial']
+
+
```

### Comparing `eaxml2code-0.7/src/eaxml2code/xmlprocessor.py` & `eaxml2code-0.8/src/eaxml2code/xmlprocessor.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-#
-# eaxml2code
-#
-# Copyright 2023 Artur Wisz
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from xml.sax.handler import ContentHandler
-import json
-
-'''
-The class converts the visited XML elements into a dictionary tree.
-'''
-class XmlProcessor(ContentHandler):
-
-    def __init__(self) -> None:
-        super().__init__()
-        self._element_stack = []
-
-    @property
-    def current_element(self):
-        return self._element_stack[-1]
-
-    def endDocument(self):
-        print("end of document")
-
-    def startElement(self, name, attrs):
-        #print(f"BEGIN: <{name}>, {attrs.keys()}")
-        self._element_stack.append({
-            "name": name,
-            "attributes": dict(attrs),
-            "children": [],
-            "value": ""
-        })
-
-    def endElement(self, name):
-        #print(f"END: </{name}>")
-        self._clear_element(self.current_element)
-        if len(self._element_stack) > 1:
-            child = self._element_stack.pop()
-            self.current_element["children"].append(child)
-
-    def characters(self, content):
-        if content.strip() != "":
-            self.current_element["value"] += content
-
-    def _clear_element(self, element):
-        element["value"] = element["value"].strip()
-        for key in ("attributes", "children", "value"):
-            if not element[key]:
+#
+# eaxml2code
+#
+# Copyright 2023 Artur Wisz
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from xml.sax.handler import ContentHandler
+import json
+
+'''
+The class converts the visited XML elements into a dictionary tree.
+'''
+class XmlProcessor(ContentHandler):
+
+    def __init__(self) -> None:
+        super().__init__()
+        self._element_stack = []
+
+    @property
+    def current_element(self):
+        return self._element_stack[-1]
+
+    def endDocument(self):
+        print("end of document")
+
+    def startElement(self, name, attrs):
+        #print(f"BEGIN: <{name}>, {attrs.keys()}")
+        self._element_stack.append({
+            "name": name,
+            "attributes": dict(attrs),
+            "children": [],
+            "value": ""
+        })
+
+    def endElement(self, name):
+        #print(f"END: </{name}>")
+        self._clear_element(self.current_element)
+        if len(self._element_stack) > 1:
+            child = self._element_stack.pop()
+            self.current_element["children"].append(child)
+
+    def characters(self, content):
+        if content.strip() != "":
+            self.current_element["value"] += content
+
+    def _clear_element(self, element):
+        element["value"] = element["value"].strip()
+        for key in ("attributes", "children", "value"):
+            if not element[key]:
                 del element[key]
```

### Comparing `eaxml2code-0.7/src/eaxml2code.egg-info/PKG-INFO` & `eaxml2code-0.8/src/eaxml2code.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-Metadata-Version: 2.1
-Name: eaxml2code
-Version: 0.7
-Summary: Generate C headers from SW component design in Enterprise Architect XMI file.
-Home-page: https://github.com/cimplart/eaxml2code
-Author: CimplArt
-Author-email: artwisz@gmail.com
-License: Apache License, Version 2.0
-Keywords: Enterprise Architect,code generation
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# eaxml2code
-Generate C header files from SW interface definition exported from Enterprise Architect 
-
-
+Metadata-Version: 2.1
+Name: eaxml2code
+Version: 0.8
+Summary: Generate C headers from SW component design in Enterprise Architect XMI file.
+Home-page: https://github.com/cimplart/eaxml2code
+Author: CimplArt
+Author-email: artwisz@gmail.com
+License: Apache License, Version 2.0
+Description: # eaxml2code
+        Generate C header files from SW interface definition exported from Enterprise Architect 
+        
+Keywords: Enterprise Architect,code generation
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Requires-Python: <3.11,>3.6
+Description-Content-Type: text/markdown
```

