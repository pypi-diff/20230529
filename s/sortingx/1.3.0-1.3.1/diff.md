# Comparing `tmp/sortingx-1.3.0.tar.gz` & `tmp/sortingx-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortingx-1.3.0.tar", last modified: Sun Mar 26 09:15:12 2023, max compression
+gzip compressed data, was "sortingx-1.3.1.tar", last modified: Mon May 29 12:21:37 2023, max compression
```

## Comparing `sortingx-1.3.0.tar` & `sortingx-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-03-26 09:15:12.397112 sortingx-1.3.0/
--rw-rw-rw-   0        0        0    11558 2022-03-25 06:43:14.000000 sortingx-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     8077 2023-03-26 09:15:12.396113 sortingx-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     6833 2023-03-26 08:01:18.000000 sortingx-1.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-03-26 09:15:12.397112 sortingx-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2673 2023-02-16 08:48:18.000000 sortingx-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-26 09:15:12.372848 sortingx-1.3.0/sortingx/
--rw-rw-rw-   0        0        0      741 2023-03-26 07:00:50.000000 sortingx-1.3.0/sortingx/__init__.py
--rw-rw-rw-   0        0        0     1153 2022-11-29 05:22:16.000000 sortingx-1.3.0/sortingx/_typing.py
--rw-rw-rw-   0        0        0     2084 2023-03-26 07:36:05.000000 sortingx-1.3.0/sortingx/_utils.py
--rw-rw-rw-   0        0        0    10783 2023-03-26 09:02:49.000000 sortingx-1.3.0/sortingx/sorting.py
-drwxrwxrwx   0        0        0        0 2023-03-26 09:15:12.394103 sortingx-1.3.0/sortingx.egg-info/
--rw-rw-rw-   0        0        0     8077 2023-03-26 09:15:11.000000 sortingx-1.3.0/sortingx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-03-26 09:15:12.000000 sortingx-1.3.0/sortingx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-26 09:15:12.000000 sortingx-1.3.0/sortingx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-26 09:14:47.000000 sortingx-1.3.0/sortingx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       28 2023-03-26 09:15:12.000000 sortingx-1.3.0/sortingx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-26 09:15:12.000000 sortingx-1.3.0/sortingx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 12:21:37.889490 sortingx-1.3.1/
+-rw-rw-rw-   0        0        0    11357 2023-04-14 13:10:05.000000 sortingx-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0     8404 2023-05-29 12:21:37.887490 sortingx-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7054 2023-05-29 12:19:34.000000 sortingx-1.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-29 12:21:37.890494 sortingx-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     2599 2023-04-14 13:10:05.000000 sortingx-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 12:21:37.858494 sortingx-1.3.1/sortingx/
+-rw-rw-rw-   0        0        0      721 2023-05-29 12:00:56.000000 sortingx-1.3.1/sortingx/__init__.py
+-rw-rw-rw-   0        0        0     1114 2023-04-14 13:10:05.000000 sortingx-1.3.1/sortingx/_typing.py
+-rw-rw-rw-   0        0        0     1891 2023-05-29 12:00:27.000000 sortingx-1.3.1/sortingx/_utils.py
+-rw-rw-rw-   0        0        0    10547 2023-04-14 13:10:05.000000 sortingx-1.3.1/sortingx/sorting.py
+drwxrwxrwx   0        0        0        0 2023-05-29 12:21:37.877494 sortingx-1.3.1/sortingx.egg-info/
+-rw-rw-rw-   0        0        0     8404 2023-05-29 12:21:37.000000 sortingx-1.3.1/sortingx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-05-29 12:21:37.000000 sortingx-1.3.1/sortingx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 12:21:37.000000 sortingx-1.3.1/sortingx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-29 12:21:37.000000 sortingx-1.3.1/sortingx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       28 2023-05-29 12:21:37.000000 sortingx-1.3.1/sortingx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-29 12:21:37.000000 sortingx-1.3.1/sortingx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 12:21:37.884492 sortingx-1.3.1/tests/
+-rw-rw-rw-   0        0        0      313 2023-04-14 13:10:05.000000 sortingx-1.3.1/tests/test_.py
+-rw-rw-rw-   0        0        0      390 2023-04-14 13:10:05.000000 sortingx-1.3.1/tests/test_equal.py
```

### Comparing `sortingx-1.3.0/LICENSE` & `sortingx-1.3.1/LICENSE`

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

### Comparing `sortingx-1.3.0/PKG-INFO` & `sortingx-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sortingx
-Version: 1.3.0
+Version: 1.3.1
 Summary: The powerful package designed for sorting.
 Home-page: https://github.com/linjing-lab/sorting-algorithms
 Download-URL: https://github.com/linjing-lab/sorting-algorithms/tags
 Author: 林景
 Author-email: linjing010729@163.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/linjing-lab/sorting-algorithms/tree/main/sortingx
@@ -30,15 +30,15 @@
 Theory analysis and code implementation of common array sorting algorithms.
 
 ## 📍 start from galley
 
 First, You need to click the [`fork`](https://github.com/linjing-lab/sorting-algorithms/fork) button to create your own sub repository, or use the following command to synchronize the repository to the local folder:
 
 ```git
-git clone https://github.com/linjing-lab/sorting-algorithms
+git clone https://github.com/linjing-lab/sorting-algorithms.git
 ```
 
 Second, I have put different implemented versions of various sorting algorithms in the [`galley`](./docs/galley/) folder, everyone can import it with the underlying command:
 
 ```python
 import galley as ge
 ```
@@ -121,11 +121,14 @@
 - [sortingx-1.2.1](https://github.com/linjing-lab/sorting-algorithms/tree/v1.2.1) is the portable version that comparison is faster than ever, the generate is more portable.
 
 By the way, I didn't complete all the iterative data types, in order to develop a more targeted scenario. If you are **interested** in other iterative data types, please add them in the `convert` function of the `_utils.py` file, for example: bytes, bytearray, range, zip. If you need to deal with `dict_keys`, `dict_values`, `dict_items`, please use `list()` to convert the variables of these data types before using any method of sortingx.
 
 - [sortingx-1.2.2](https://github.com/linjing-lab/sorting-algorithms/tree/v1.2.2) is the package that support `range`, `zip`, `dict_keys`, `dict_values`, `dict_items` additionally, you can choose what suitable data you want to input.
 - [sortingx-1.2.3](https://github.com/linjing-lab/sorting-algorithms/tree/v1.2.3) is the package that corrected the situation where elements are equal in `compare`, support more input data, like data as `[['Jack', (98, 100)], ['Bob', (98, 99)], ['Jessi', (98, 97)]]` and key as `lambda x: x[1][0]`.
 - [sortingx-1.3.0](https://github.com/linjing-lab/sorting-algorithms/tree/v1.3.0) is the final version that fully aligned with the `sorted`', reduces redundant data exchanging. like data as `[('Alex', 97, 90, 98, 95), ('Jack', 97, 88, 98, 92), ('Peter', 92, 95, 92, 96), ('Li', 97, 89, 98, 92)]` and key as `key=lambda x: x[1]`.
+- [sortingx-1.3.1](https://github.com/linjing-lab/sorting-algorithms/tree/v1.3.1) is the improved version from v1.3.0, and pre-operations from `_utils` are more conise to reduce shallow copy in Runtime.
+
+refer to [this](https://github.com/linjing-lab/sorting-algorithms/blob/main/README_release.md) for downloaded info.
 
 ## LICENSE
 
 [Apache 2.0](./LICENSE)
```

### Comparing `sortingx-1.3.0/README.md` & `sortingx-1.3.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,104 +1,107 @@
-# sorting-algorithms🎢
-
-Theory analysis and code implementation of common array sorting algorithms.
-
-## 📍 start from galley
-
-First, You need to click the [`fork`](https://github.com/linjing-lab/sorting-algorithms/fork) button to create your own sub repository, or use the following command to synchronize the repository to the local folder:
-
-```git
-git clone https://github.com/linjing-lab/sorting-algorithms
-```
-
-Second, I have put different implemented versions of various sorting algorithms in the [`galley`](./docs/galley/) folder, everyone can import it with the underlying command:
-
-```python
-import galley as ge
-```
-
-For example, If I use the `bubble` sorting algorithm to sort a real data in reverse, use the following commands:
-
-```python
-import random 
-data = [random.randint(0, 100) for _ in range(10000)]
-ge.bubble.flag(data, reverse=True)
-print(data)
-```
-
-Lastly, many algorithms are *in-place* sorting, and a few are *out-place*, you should pay attention to it during the study, so that you can distinguish between `print(data)` and `print(method)`. I mainly use `if... else...` to implement the reverse order of sorting algorithms in gallery and the partition of some algorithms.
-
-## 📊 sorting complexity
-
-<div align="center">
-
-|Algorithm||Time Complexity||Space Complexity|
-|--|--|--|--|--|
-|---|Best|Average|Worst|Worst|
-|[Quicksort](./docs/Quicksort.md)|$\Omega(n \log(n))$|$\Theta(n \log(n))$|$O(n^2)$|$O(\log(n))$|
-|[Mergesort](./docs/Mergesort.md)|$\Omega(n \log(n))$|$\Theta(n \log(n))$|$O(n \log(n))$|$O(n)$|
-|[Timsort](./docs/Timsort.md)|$\Omega(n)$|$\Theta(n \log(n))$|$O(n \log(n))$|$O(n)$|
-|[Heapsort](./docs/Heapsort.md)|$\Omega(n \log(n))$|$\Theta(n \log(n))$|$O(n \log(n))$|$O(1)$|
-|[Bubble Sort](./docs/Bubblesort.md)|$\Omega(n)$|$\Theta(n^2)$|$O(n^2)$|$O(1)$|
-|[Insertion Sort](./docs/Insertionsort.md)|$\Omega(n)$|$\Theta(n^2)$|$O(n^2)$|$O(1)$|
-|[Selection Sort](./docs/Selectionsort.md)|$\Omega(n^2)$|$\Theta(n^2)$|$O(n^2)$|$O(1)$|
-|[Tree Sort](./docs/Treesort.md)|$\Omega(n \log(n))$|$\Theta(n \log(n))$|$O(n^2)$|$O(n)$|
-|[Shell Sort](./docs/Shellsort.md)|$\Omega(n \log (n))$|$\Theta(n(\log (n))^2)$|$O(n(\log (n))^2)$|$O(1)$|
-|[Bucket Sort](./docs/Bucketsort.md)|$\Omega(n + k)$|$\Theta(n + k)$|$O(n^2)$|$O(n)$|
-|[Radix Sort](./docs/Radixsort.md)|$\Omega(nk)$|$\Theta(nk)$|$O(nk)$|$O(n+k)$|
-|[Counting Sort](./docs/Countingsort.md)|$\Omega(n + k)$|$\Theta(n + k)$|$O(n + k)$|$O(k)$|
-|Cubesort|$\Omega(n)$|$\Theta(n \log(n))$|$O(n \log(n))$|$O(n)$|
-
-</div>
-
-## 🙋 test description
-
-I test the performance of the sorting algorithm after adding the [*keyword*](./keyword_sorting.py) sorting in the [*test_key*](./test_key.py) file (The [*utils*](./utils.py) file stores the most core function for keyword sorting), test the time accumulation of the sorting algorithm with respect to the large data set in the [*test_time*](./test_time.py) file, and test whether the reverse parameter of the sorting algorithms is designed correctly in the [*test_reverse*](./test_reverse.py) file, including the robustness of these.
-
-The design of reverse sorting of all methods is completely correct, and the design of keyword sorting is feasible, which is consistent with the usage of *sorted* parameter officially released by Python.
-
-The example of keyword sorting are underlying:
-
-```python
-data = [('Alex', 100, 90, 98, 95), ('Jack', 97, 88, 98, 92), ('Peter', 92, 95, 92, 96), ('Li', 97, 89, 98, 92)]
-insertion_sort(data, key=lambda x: (x[1], x[2]), reverse=False)
-# sorted(data, key=lambda x: (x[1], x[2]), reverse=False)
-print(data)
-
-'''
-reverse=False: 
-[('Peter', 92, 95, 92, 96), ('Jack', 97, 88, 98, 92), ('Li', 97, 89, 98, 92), ('Alex', 100, 90, 98, 95)]
-
-reverse=True: 
-[('Alex', 100, 90, 98, 95), ('Li', 97, 89, 98, 92), ('Jack', 97, 88, 98, 92), ('Peter', 92, 95, 92, 96)]
-'''
-```
-
-you can see more 5 methods in [*keyword_sorting*](./keyword_sorting.py) file.
-
-## 🎒 pip install
-
-As you can see, I create a core function to drive keyword sorting just by opening up an array with the size of k (k = nums of keyword), and the type of sorting implemented by Python officially released is Timsort, which is more complicated than the other algorithms in my released packages in the future.
-
-```python
-!pip install sortingx # in jupyter
-pip install sortingx # in cmd
-```
-sortingx can do whatever `list.sort()` do, and support more methods and more data types.
-
-explain:
-- [sortingx-1.1.0](https://github.com/linjing-lab/sorting-algorithms/tree/v1.1.0) is the first version aligned with the `list.sort()` usage method.
-- [sortingx-1.1.1](https://github.com/linjing-lab/sorting-algorithms/tree/v1.1.1) is the first stable version accelerated with typing_extensions.
-- [sortingx-1.1.2](https://github.com/linjing-lab/sorting-algorithms/tree/v1.1.2) is the first stable version that has a return value and extends the iterable data types.
-- [sortingx-1.1.3](https://github.com/linjing-lab/sorting-algorithms/tree/v1.1.3) is the version that complete the typing of local variables and align with `sorted()` usage method.
-- [sortingx-1.2.0](https://github.com/linjing-lab/sorting-algorithms/tree/v1.2.0) is the end version of sorting series, which optimize the kernel of generate.
-- [sortingx-1.2.1](https://github.com/linjing-lab/sorting-algorithms/tree/v1.2.1) is the portable version that comparison is faster than ever, the generate is more portable.
-
-By the way, I didn't complete all the iterative data types, in order to develop a more targeted scenario. If you are **interested** in other iterative data types, please add them in the `convert` function of the `_utils.py` file, for example: bytes, bytearray, range, zip. If you need to deal with `dict_keys`, `dict_values`, `dict_items`, please use `list()` to convert the variables of these data types before using any method of sortingx.
-
-- [sortingx-1.2.2](https://github.com/linjing-lab/sorting-algorithms/tree/v1.2.2) is the package that support `range`, `zip`, `dict_keys`, `dict_values`, `dict_items` additionally, you can choose what suitable data you want to input.
-- [sortingx-1.2.3](https://github.com/linjing-lab/sorting-algorithms/tree/v1.2.3) is the package that corrected the situation where elements are equal in `compare`, support more input data, like data as `[['Jack', (98, 100)], ['Bob', (98, 99)], ['Jessi', (98, 97)]]` and key as `lambda x: x[1][0]`.
-- [sortingx-1.3.0](https://github.com/linjing-lab/sorting-algorithms/tree/v1.3.0) is the final version that fully aligned with the `sorted`', reduces redundant data exchanging. like data as `[('Alex', 97, 90, 98, 95), ('Jack', 97, 88, 98, 92), ('Peter', 92, 95, 92, 96), ('Li', 97, 89, 98, 92)]` and key as `key=lambda x: x[1]`.
-
-## LICENSE
-
+# sorting-algorithms🎢
+
+Theory analysis and code implementation of common array sorting algorithms.
+
+## 📍 start from galley
+
+First, You need to click the [`fork`](https://github.com/linjing-lab/sorting-algorithms/fork) button to create your own sub repository, or use the following command to synchronize the repository to the local folder:
+
+```git
+git clone https://github.com/linjing-lab/sorting-algorithms.git
+```
+
+Second, I have put different implemented versions of various sorting algorithms in the [`galley`](./docs/galley/) folder, everyone can import it with the underlying command:
+
+```python
+import galley as ge
+```
+
+For example, If I use the `bubble` sorting algorithm to sort a real data in reverse, use the following commands:
+
+```python
+import random 
+data = [random.randint(0, 100) for _ in range(10000)]
+ge.bubble.flag(data, reverse=True)
+print(data)
+```
+
+Lastly, many algorithms are *in-place* sorting, and a few are *out-place*, you should pay attention to it during the study, so that you can distinguish between `print(data)` and `print(method)`. I mainly use `if... else...` to implement the reverse order of sorting algorithms in gallery and the partition of some algorithms.
+
+## 📊 sorting complexity
+
+<div align="center">
+
+|Algorithm||Time Complexity||Space Complexity|
+|--|--|--|--|--|
+|---|Best|Average|Worst|Worst|
+|[Quicksort](./docs/Quicksort.md)|$\Omega(n \log(n))$|$\Theta(n \log(n))$|$O(n^2)$|$O(\log(n))$|
+|[Mergesort](./docs/Mergesort.md)|$\Omega(n \log(n))$|$\Theta(n \log(n))$|$O(n \log(n))$|$O(n)$|
+|[Timsort](./docs/Timsort.md)|$\Omega(n)$|$\Theta(n \log(n))$|$O(n \log(n))$|$O(n)$|
+|[Heapsort](./docs/Heapsort.md)|$\Omega(n \log(n))$|$\Theta(n \log(n))$|$O(n \log(n))$|$O(1)$|
+|[Bubble Sort](./docs/Bubblesort.md)|$\Omega(n)$|$\Theta(n^2)$|$O(n^2)$|$O(1)$|
+|[Insertion Sort](./docs/Insertionsort.md)|$\Omega(n)$|$\Theta(n^2)$|$O(n^2)$|$O(1)$|
+|[Selection Sort](./docs/Selectionsort.md)|$\Omega(n^2)$|$\Theta(n^2)$|$O(n^2)$|$O(1)$|
+|[Tree Sort](./docs/Treesort.md)|$\Omega(n \log(n))$|$\Theta(n \log(n))$|$O(n^2)$|$O(n)$|
+|[Shell Sort](./docs/Shellsort.md)|$\Omega(n \log (n))$|$\Theta(n(\log (n))^2)$|$O(n(\log (n))^2)$|$O(1)$|
+|[Bucket Sort](./docs/Bucketsort.md)|$\Omega(n + k)$|$\Theta(n + k)$|$O(n^2)$|$O(n)$|
+|[Radix Sort](./docs/Radixsort.md)|$\Omega(nk)$|$\Theta(nk)$|$O(nk)$|$O(n+k)$|
+|[Counting Sort](./docs/Countingsort.md)|$\Omega(n + k)$|$\Theta(n + k)$|$O(n + k)$|$O(k)$|
+|Cubesort|$\Omega(n)$|$\Theta(n \log(n))$|$O(n \log(n))$|$O(n)$|
+
+</div>
+
+## 🙋 test description
+
+I test the performance of the sorting algorithm after adding the [*keyword*](./keyword_sorting.py) sorting in the [*test_key*](./test_key.py) file (The [*utils*](./utils.py) file stores the most core function for keyword sorting), test the time accumulation of the sorting algorithm with respect to the large data set in the [*test_time*](./test_time.py) file, and test whether the reverse parameter of the sorting algorithms is designed correctly in the [*test_reverse*](./test_reverse.py) file, including the robustness of these.
+
+The design of reverse sorting of all methods is completely correct, and the design of keyword sorting is feasible, which is consistent with the usage of *sorted* parameter officially released by Python.
+
+The example of keyword sorting are underlying:
+
+```python
+data = [('Alex', 100, 90, 98, 95), ('Jack', 97, 88, 98, 92), ('Peter', 92, 95, 92, 96), ('Li', 97, 89, 98, 92)]
+insertion_sort(data, key=lambda x: (x[1], x[2]), reverse=False)
+# sorted(data, key=lambda x: (x[1], x[2]), reverse=False)
+print(data)
+
+'''
+reverse=False: 
+[('Peter', 92, 95, 92, 96), ('Jack', 97, 88, 98, 92), ('Li', 97, 89, 98, 92), ('Alex', 100, 90, 98, 95)]
+
+reverse=True: 
+[('Alex', 100, 90, 98, 95), ('Li', 97, 89, 98, 92), ('Jack', 97, 88, 98, 92), ('Peter', 92, 95, 92, 96)]
+'''
+```
+
+you can see more 5 methods in [*keyword_sorting*](./keyword_sorting.py) file.
+
+## 🎒 pip install
+
+As you can see, I create a core function to drive keyword sorting just by opening up an array with the size of k (k = nums of keyword), and the type of sorting implemented by Python officially released is Timsort, which is more complicated than the other algorithms in my released packages in the future.
+
+```python
+!pip install sortingx # in jupyter
+pip install sortingx # in cmd
+```
+sortingx can do whatever `list.sort()` do, and support more methods and more data types.
+
+explain:
+- [sortingx-1.1.0](https://github.com/linjing-lab/sorting-algorithms/tree/v1.1.0) is the first version aligned with the `list.sort()` usage method.
+- [sortingx-1.1.1](https://github.com/linjing-lab/sorting-algorithms/tree/v1.1.1) is the first stable version accelerated with typing_extensions.
+- [sortingx-1.1.2](https://github.com/linjing-lab/sorting-algorithms/tree/v1.1.2) is the first stable version that has a return value and extends the iterable data types.
+- [sortingx-1.1.3](https://github.com/linjing-lab/sorting-algorithms/tree/v1.1.3) is the version that complete the typing of local variables and align with `sorted()` usage method.
+- [sortingx-1.2.0](https://github.com/linjing-lab/sorting-algorithms/tree/v1.2.0) is the end version of sorting series, which optimize the kernel of generate.
+- [sortingx-1.2.1](https://github.com/linjing-lab/sorting-algorithms/tree/v1.2.1) is the portable version that comparison is faster than ever, the generate is more portable.
+
+By the way, I didn't complete all the iterative data types, in order to develop a more targeted scenario. If you are **interested** in other iterative data types, please add them in the `convert` function of the `_utils.py` file, for example: bytes, bytearray, range, zip. If you need to deal with `dict_keys`, `dict_values`, `dict_items`, please use `list()` to convert the variables of these data types before using any method of sortingx.
+
+- [sortingx-1.2.2](https://github.com/linjing-lab/sorting-algorithms/tree/v1.2.2) is the package that support `range`, `zip`, `dict_keys`, `dict_values`, `dict_items` additionally, you can choose what suitable data you want to input.
+- [sortingx-1.2.3](https://github.com/linjing-lab/sorting-algorithms/tree/v1.2.3) is the package that corrected the situation where elements are equal in `compare`, support more input data, like data as `[['Jack', (98, 100)], ['Bob', (98, 99)], ['Jessi', (98, 97)]]` and key as `lambda x: x[1][0]`.
+- [sortingx-1.3.0](https://github.com/linjing-lab/sorting-algorithms/tree/v1.3.0) is the final version that fully aligned with the `sorted`', reduces redundant data exchanging. like data as `[('Alex', 97, 90, 98, 95), ('Jack', 97, 88, 98, 92), ('Peter', 92, 95, 92, 96), ('Li', 97, 89, 98, 92)]` and key as `key=lambda x: x[1]`.
+- [sortingx-1.3.1](https://github.com/linjing-lab/sorting-algorithms/tree/v1.3.1) is the improved version from v1.3.0, and pre-operations from `_utils` are more conise to reduce shallow copy in Runtime.
+
+refer to [this](https://github.com/linjing-lab/sorting-algorithms/blob/main/README_release.md) for downloaded info.
+
+## LICENSE
+
 [Apache 2.0](./LICENSE)
```

### Comparing `sortingx-1.3.0/setup.py` & `sortingx-1.3.1/setup.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-import os
-import sys
-
-from setuptools import setup
-
-if sys.version_info < (3, 7, 0):
-    raise OSError(f'sortingx requires Python >=3.7, but yours is {sys.version}')
-
-if (3, 7, 0) <= sys.version_info < (3, 8, 0):
-    # https://github.com/pypa/setuptools/issues/926#issuecomment-294369342
-    try:
-        import fastentrypoints
-    except ImportError:
-        try:
-            import pkg_resources
-            from setuptools.command import easy_install
-
-            easy_install.main(['fastentrypoints'])
-            pkg_resources.require('fastentrypoints')
-        except:
-            pass
-
-try:
-    pkg_name = 'sortingx'
-    libinfo_py = os.path.join(pkg_name, '__init__.py')
-    libinfo_content = open(libinfo_py, 'r', encoding='utf-8').readlines()
-    version_line = [l.strip() for l in libinfo_content if l.startswith('__version__')][0]
-    exec(version_line) # gives __version
-except FileNotFoundError:
-    __version__ = '0.0.0'
-
-try:
-    with open('README.md', 'r', encoding='utf-8') as fp:
-        _long_description = fp.read()
-except FileNotFoundError:
-    _long_description = ''
-
-setup(
-    name=pkg_name,
-    packages=['sortingx',],
-    version=__version__,
-    description='The powerful package designed for sorting.',
-    author='林景',
-    author_email='linjing010729@163.com',
-    license='Apache 2.0',
-    url='https://github.com/linjing-lab/sorting-algorithms',
-    download_url='https://github.com/linjing-lab/sorting-algorithms/tags',
-    long_description=_long_description,
-    long_description_content_type='text/markdown',
-    zip_safe=False,
-    setup_requires=['setuptools>=18.0', 'wheel'],
-    project_urls={
-        'Source': 'https://github.com/linjing-lab/sorting-algorithms/tree/main/sortingx',
-        'Tracker': 'https://github.com/linjing-lab/sorting-algorithms/issues',
-    },
-    classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'Intended Audience :: Education',
-        'Intended Audience :: Science/Research',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'License :: OSI Approved :: Apache Software License',
-        'Topic :: Software Development',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-    ],
-    install_requires = [
-        'typing_extensions>=3.10.0.2'
-    ]
-    # extras_require = []
+import os
+import sys
+
+from setuptools import setup
+
+if sys.version_info < (3, 7, 0):
+    raise OSError(f'sortingx requires Python >=3.7, but yours is {sys.version}')
+
+if (3, 7, 0) <= sys.version_info < (3, 8, 0):
+    # https://github.com/pypa/setuptools/issues/926#issuecomment-294369342
+    try:
+        import fastentrypoints
+    except ImportError:
+        try:
+            import pkg_resources
+            from setuptools.command import easy_install
+
+            easy_install.main(['fastentrypoints'])
+            pkg_resources.require('fastentrypoints')
+        except:
+            pass
+
+try:
+    pkg_name = 'sortingx'
+    libinfo_py = os.path.join(pkg_name, '__init__.py')
+    libinfo_content = open(libinfo_py, 'r', encoding='utf-8').readlines()
+    version_line = [l.strip() for l in libinfo_content if l.startswith('__version__')][0]
+    exec(version_line) # gives __version
+except FileNotFoundError:
+    __version__ = '0.0.0'
+
+try:
+    with open('README.md', 'r', encoding='utf-8') as fp:
+        _long_description = fp.read()
+except FileNotFoundError:
+    _long_description = ''
+
+setup(
+    name=pkg_name,
+    packages=['sortingx',],
+    version=__version__,
+    description='The powerful package designed for sorting.',
+    author='林景',
+    author_email='linjing010729@163.com',
+    license='Apache 2.0',
+    url='https://github.com/linjing-lab/sorting-algorithms',
+    download_url='https://github.com/linjing-lab/sorting-algorithms/tags',
+    long_description=_long_description,
+    long_description_content_type='text/markdown',
+    zip_safe=False,
+    setup_requires=['setuptools>=18.0', 'wheel'],
+    project_urls={
+        'Source': 'https://github.com/linjing-lab/sorting-algorithms/tree/main/sortingx',
+        'Tracker': 'https://github.com/linjing-lab/sorting-algorithms/issues',
+    },
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'Intended Audience :: Developers',
+        'Intended Audience :: Education',
+        'Intended Audience :: Science/Research',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'License :: OSI Approved :: Apache Software License',
+        'Topic :: Software Development',
+        'Topic :: Software Development :: Libraries',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+    ],
+    install_requires = [
+        'typing_extensions>=3.10.0.2'
+    ]
+    # extras_require = []
 )
```

### Comparing `sortingx-1.3.0/sortingx/__init__.py` & `sortingx-1.3.1/sortingx/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Copyright 2022 linjing-lab
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     https://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import sys
-
-from .sorting import bubble, insert, shell, heap, quick, merge, __all__
-
-__version__ = '1.3.0'
-
+# Copyright 2022 linjing-lab
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import sys
+
+from .sorting import bubble, insert, shell, heap, quick, merge, __all__
+
+__version__ = '1.3.1'
+
 assert sys.version_info >= (3, 7, 0)
```

### Comparing `sortingx-1.3.0/sortingx/_utils.py` & `sortingx-1.3.1/sortingx/_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,43 @@
-# Copyright 2022 linjing-lab
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     https://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from ._typing import Iterable, List, Callable, Optional, _T, SupportsRichComparison
-
-# Data Generated by Mapping.
-def generate(__iterable: List[_T], key: Optional[Callable[[_T], SupportsRichComparison]]=None) -> List[_T]:
-    '''
-    :param __iterable: iterable data, mainly refers to `list`, `tuple`, `set`, `dict`, `str`, `zip`, `range`.
-    :param key: callable function, for example: key=lambda x: x[1], key=lambda x: (x[0], x[1]), key=str.lower.
-
-    :return: data generated by map.
-    '''
-    compare: List[_T] = list(map(key, __iterable)) if key != None else __iterable
-    return compare
-
-# Verify Elements Are Equal before Comparison.
-def verify(compare: List[_T]) -> bool:
-    '''
-    :param compare: List[_T], list generated by `generate` with builtin api named `map`.
-
-    :return: bool value indicated whether to enter comparison.
-    '''
-    return compare.count(compare[0]) == len(compare)
-
-# Uniformly Convert `Iterable` into `List`: Facilitate the Execution of Sorting Algorithms.
-def convert(__iterable: Iterable[_T]) -> List[_T]:
-    '''
-    :param __iterable: iterable data, mainly refers to `list`, `tuple`, `set`, `dict`, `str`, `zip`, `range`.
-
-    :return: converted result in a list.
-    '''
-    if isinstance(__iterable, list): # represents unifying data as list, not refer to allowing some input that is not suitable for sorting.
-        return __iterable
-    return list(__iterable) # iterable data (except list) are convert to list.
+# Copyright 2022 linjing-lab
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from ._typing import Iterable, List, Callable, Optional, _T, SupportsRichComparison
+
+# Data Generated by Mapping.
+def generate(__iterable: List[_T], key: Optional[Callable[[_T], SupportsRichComparison]]=None) -> List[_T]:
+    '''
+    :param __iterable: iterable data, mainly refers to `list`, `tuple`, `set`, `dict`, `str`, `zip`, `range`.
+    :param key: callable function, for example: key=lambda x: x[1], key=lambda x: (x[0], x[1]), key=str.lower.
+
+    :return: data generated by map.
+    '''
+    return list(map(key, __iterable)) if key != None else __iterable
+
+# Verify Elements Are Equal before Comparison.
+def verify(compare: List[_T]) -> bool:
+    '''
+    :param compare: List[_T], list generated by `generate` with builtin api named `map`.
+
+    :return: bool value indicated whether to enter comparison.
+    '''
+    return compare.count(compare[0]) == len(compare)
+
+# Uniformly Convert `Iterable` into `List`: Facilitate the Execution of Sorting Algorithms.
+def convert(__iterable: Iterable[_T]) -> List[_T]:
+    '''
+    :param __iterable: iterable data, mainly refers to `list`, `tuple`, `set`, `dict`, `str`, `zip`, `range`.
+
+    :return: converted result in a list.
+    '''
+    return __iterable if isinstance(__iterable, list) else list(__iterable) # iterable data (except list) are converted to list.
```

### Comparing `sortingx-1.3.0/sortingx/sorting.py` & `sortingx-1.3.1/sortingx/sorting.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,237 +1,237 @@
-# Copyright 2022 linjing-lab
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     https://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from ._utils import generate, convert, verify
-from ._typing import Iterable, Callable, Optional, _T, SupportsRichComparison, List
-
-__all__ = ["bubble", "insert", "shell", "heap", "quick", "merge"]
-
-def bubble(__iterable: Iterable[_T], key: Optional[Callable[[_T], SupportsRichComparison]]=None, reverse: bool=False) -> List[_T]:
-    '''
-    :param __iterable: iterable data, mainly refers to `list`, `tuple`, `set`, `dict`, `str`, `zip`, `range`.
-    :param key: callable function, for example: key=lambda x: x[1], key=lambda x: (x[0], x[1]), key=str.lower.
-    :param reverse: whether to use descending order. The default is ascending order.
-
-    :return: bubble's sorted result in a list.
-    '''
-    __iterable: List[_T] = convert(__iterable)
-    compare: List[_T] = generate(__iterable, key)
-    if compare and not verify(compare):
-        for i in range(len(__iterable) - 1):
-            flag: bool = False # early stop by adding a bool value named flag
-            for j in range(len(__iterable) - i - 1):
-                if (compare[j] < compare[j + 1] if reverse else compare[j] > compare[j+1]):
-                    __iterable[j], __iterable[j + 1] = __iterable[j + 1], __iterable[j]
-                    if key != None:
-                        compare[j], compare[j + 1] = compare[j + 1], compare[j]
-                    flag: bool = True
-            if not flag:
-                break
-    return __iterable
-
-def insert(__iterable: Iterable[_T], key: Optional[Callable[[_T], SupportsRichComparison]]=None, reverse: bool=False) -> List[_T]:
-    '''
-    :param __iterable: iterable data, mainly refers to `list`, `tuple`, `set`, `dict`, `str`, `zip`, `range`.
-    :param key: callable function, for example: key=lambda x: x[1], key=lambda x: (x[0], x[1]), key=str.lower.
-    :param reverse: whether to use descending order. The default is ascending order.
-
-    :return: insert's sorted result in a list.
-    '''
-    __iterable: List[_T] = convert(__iterable)
-    compare: List[_T] = generate(__iterable, key)
-    if compare and not verify(compare):
-        for index in range(1, len(__iterable)):
-            keyc: _T = compare[index]
-            keya: _T = __iterable[index]
-            low : int = 0
-            high: int = index - 1
-            while low <= high: # sequence conforming to monotonicity
-                mid: int = (low + high) // 2
-                if (keyc <= compare[mid] if reverse else keyc >= compare[mid]):
-                    low: int = mid + 1
-                else:
-                    high: int = mid - 1
-            for pre in range(index, low, -1): # from back to front
-                __iterable[pre] = __iterable[pre - 1]
-                if key != None:
-                    compare[pre] = compare[pre - 1]
-            __iterable[low] = keya
-            if key != None:
-                compare[low] = keyc
-    return __iterable
-
-def shell(__iterable: Iterable[_T], key: Optional[Callable[[_T], SupportsRichComparison]]=None, reverse: bool=False) -> List[_T]:
-    '''
-    :param __iterable: iterable data, mainly refers to `list`, `tuple`, `set`, `dict`, `str`, `zip`, `range`.
-    :param key: callable function, for example: key=lambda x: x[1], key=lambda x: (x[0], x[1]), key=str.lower.
-    :param reverse: whether to use descending order. The default is ascending order.
-
-    :return: shell's sorted result in a list.
-    '''
-    __iterable: List[_T] = convert(__iterable)
-    compare: List[_T] = generate(__iterable, key)
-    if compare and not verify(compare):
-        length: int = len(__iterable)
-        gap: int = 1
-        while gap < length / 3:
-            gap: int = int(3 * gap + 1)
-        while gap >= 1:
-            for index in range(gap, length):
-                next: int = index
-                while next >= gap and (compare[next - gap] < compare[next] if reverse else compare[next - gap] > compare[next]):
-                    __iterable[next], __iterable[next - gap] = __iterable[next - gap], __iterable[next]
-                    if key != None:
-                        compare[next], compare[next - gap] = compare[next - gap], compare[next]
-                    next -= gap
-            gap: int = int(gap / 3)
-    return __iterable
-    
-def heap(__iterable: Iterable[_T], key: Optional[Callable[[_T], SupportsRichComparison]]=None, reverse: bool=False) -> List[_T]:
-    '''
-    :param __iterable: iterable data, mainly refers to `list`, `tuple`, `set`, `dict`, `str`, `zip`, `range`.
-    :param key: callable function, for example: key=lambda x: x[1], key=lambda x: (x[0], x[1]), key=str.lower.
-    :param reverse: whether to use descending order. The default is ascending order.
-
-    :return: heap's sorted result in a list.
-    '''
-    __iterable: List[_T] = convert(__iterable)
-    compare: List[_T] = generate(__iterable, key)
-    def build(root: int, end: int) -> None:
-        '''
-        :param root: cursor indicating the root node (int).
-        :param end: cursor indicating the end of the __iterable (int).
-        '''
-        piv: int = root
-        left: int = 2 * root + 1
-        right: int = 2 * root + 2
-        if left < end and (compare[left] < compare[root] if reverse else compare[left] > compare[root]):
-            piv: int = left
-        if right < end and (compare[right] < compare[piv] if reverse else compare[right] > compare[piv]):
-            piv: int = right
-        if piv != root:
-            __iterable[root], __iterable[piv] = __iterable[piv], __iterable[root]
-            if key != None:
-                compare[root], compare[piv] = compare[piv], compare[root]
-            build(piv, end)
-    if compare and not verify(compare):
-        length: int = len(__iterable)
-        for root in range(length // 2 - 1 , -1, -1):
-            build(root, length)
-        for end in range(length - 1, 0, -1):
-            if compare[0] != compare[end]:
-                __iterable[0], __iterable[end] = __iterable[end], __iterable[0]
-                if key != None:
-                    compare[0], compare[end] = compare[end], compare[0]
-            build(0, end)
-    return __iterable
-
-def quick(__iterable: Iterable[_T], key: Optional[Callable[[_T], SupportsRichComparison]]=None, reverse: bool=False) -> List[_T]:
-    '''
-    :param __iterable: iterable data, mainly refers to `list`, `tuple`, `set`, `dict`, `str`, `zip`, `range`.
-    :param key: callable function, for example: key=lambda x: x[1], key=lambda x: (x[0], x[1]), key=str.lower.
-    :param reverse: whether to use descending order. The default is ascending order.
-
-    :return: quick's sorted result in a list.
-    '''
-    __iterable: List[_T] = convert(__iterable)
-    compare: List[_T] = generate(__iterable, key)
-    def solve(l: int, r: int) -> None:
-        '''
-        main
-        '''
-        if l < r:
-            mid: int = partition(l, r)
-            solve(l, mid - 1)
-            solve(mid + 1, r)
-
-    def partition(l: int, r: int) -> int:
-        '''
-        :param l: The left cursor of __iterable (int).
-        :param r: The right cursor of __iterable (int).
-        '''
-        val: _T = compare[r]
-        index: int = l - 1
-        for ind in range(l, r):
-            if (val < compare[ind] if reverse else val > compare[ind]):
-                index += 1
-                if compare[index] != compare[ind]:
-                    __iterable[index], __iterable[ind] = __iterable[ind], __iterable[index]
-                    if key != None:
-                        compare[index], compare[ind] = compare[ind], compare[index]
-        if compare[index + 1] != compare[r]:
-            __iterable[index + 1], __iterable[r] = __iterable[r], __iterable[index + 1]
-            if key != None:
-                compare[index + 1], compare[r] = compare[r], compare[index + 1]
-        return index + 1
-    if compare and not verify(compare):
-        solve(0, len(__iterable) - 1)
-    return __iterable
-
-def merge(__iterable: Iterable[_T], key: Optional[Callable[[_T], SupportsRichComparison]]=None, reverse: bool=False) -> List[_T]:
-    '''
-    :param __iterable: iterable data, mainly refers to `list`, `tuple`, `set`, `dict`, `str`, `zip`, `range`.
-    :param key: callable function, for example: key=lambda x: x[1], key=lambda x: (x[0], x[1]), key=str.lower.
-    :param reverse: whether to use descending order. The default is ascending order.
-
-    :return: merge's sorted result in a list.
-    '''
-    __iterable: List[_T] = convert(__iterable)
-    compare: List[_T] = generate(__iterable, key)
-    def merg(low: int, mid: int, high: int) -> None:
-        '''
-        :param low: The low cursor of __iterable (int).
-        :param mid: The middle cursor of __iterable (int).
-        :param high: The high cursor of __iterable (int).
-        '''
-        left: List[_T] = __iterable[low: mid]
-        lc: List[_T] = compare[low: mid]
-        right: List[_T] = __iterable[mid: high]
-        rc: List[_T] = compare[mid: high]
-        i: int = 0
-        j: int = 0
-        result: List[_T] = []
-        store: List[_T] = []
-        while i < len(left) and j < len(right):
-            if (rc[j] <= lc[i] if reverse else rc[j] >= lc[i]):
-                result.append(left[i])
-                store.append(lc[i])
-                i += 1
-            else:
-                result.append(right[j])
-                store.append(rc[j])
-                j += 1
-        result += left[i:]
-        store += lc[i:]
-        result += right[j:]
-        store += rc[j:]
-        __iterable[low: high]: List[_T] = result
-        compare[low: high]: List[_T] = store
-
-    def solve() -> None:
-        '''
-        main
-        '''
-        i: int = 1
-        while i < len(__iterable):
-            low: int = 0
-            while low < len(__iterable):
-                mid: int = low + i
-                high: int = min(low + 2 * i, len(__iterable))
-                if mid < high:
-                    merg(low, mid, high)
-                low += 2 * i
-            i *= 2
-    if compare and not verify(compare):
-        solve()
+# Copyright 2022 linjing-lab
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from ._utils import generate, convert, verify
+from ._typing import Iterable, Callable, Optional, _T, SupportsRichComparison, List
+
+__all__ = ["bubble", "insert", "shell", "heap", "quick", "merge"]
+
+def bubble(__iterable: Iterable[_T], key: Optional[Callable[[_T], SupportsRichComparison]]=None, reverse: bool=False) -> List[_T]:
+    '''
+    :param __iterable: iterable data, mainly refers to `list`, `tuple`, `set`, `dict`, `str`, `zip`, `range`.
+    :param key: callable function, for example: key=lambda x: x[1], key=lambda x: (x[0], x[1]), key=str.lower.
+    :param reverse: whether to use descending order. The default is ascending order.
+
+    :return: bubble's sorted result in a list.
+    '''
+    __iterable: List[_T] = convert(__iterable)
+    compare: List[_T] = generate(__iterable, key)
+    if compare and not verify(compare):
+        for i in range(len(__iterable) - 1):
+            flag: bool = False # early stop by adding a bool value named flag
+            for j in range(len(__iterable) - i - 1):
+                if (compare[j] < compare[j + 1] if reverse else compare[j] > compare[j+1]):
+                    __iterable[j], __iterable[j + 1] = __iterable[j + 1], __iterable[j]
+                    if key != None:
+                        compare[j], compare[j + 1] = compare[j + 1], compare[j]
+                    flag: bool = True
+            if not flag:
+                break
+    return __iterable
+
+def insert(__iterable: Iterable[_T], key: Optional[Callable[[_T], SupportsRichComparison]]=None, reverse: bool=False) -> List[_T]:
+    '''
+    :param __iterable: iterable data, mainly refers to `list`, `tuple`, `set`, `dict`, `str`, `zip`, `range`.
+    :param key: callable function, for example: key=lambda x: x[1], key=lambda x: (x[0], x[1]), key=str.lower.
+    :param reverse: whether to use descending order. The default is ascending order.
+
+    :return: insert's sorted result in a list.
+    '''
+    __iterable: List[_T] = convert(__iterable)
+    compare: List[_T] = generate(__iterable, key)
+    if compare and not verify(compare):
+        for index in range(1, len(__iterable)):
+            keyc: _T = compare[index]
+            keya: _T = __iterable[index]
+            low : int = 0
+            high: int = index - 1
+            while low <= high: # sequence conforming to monotonicity
+                mid: int = (low + high) // 2
+                if (keyc <= compare[mid] if reverse else keyc >= compare[mid]):
+                    low: int = mid + 1
+                else:
+                    high: int = mid - 1
+            for pre in range(index, low, -1): # from back to front
+                __iterable[pre] = __iterable[pre - 1]
+                if key != None:
+                    compare[pre] = compare[pre - 1]
+            __iterable[low] = keya
+            if key != None:
+                compare[low] = keyc
+    return __iterable
+
+def shell(__iterable: Iterable[_T], key: Optional[Callable[[_T], SupportsRichComparison]]=None, reverse: bool=False) -> List[_T]:
+    '''
+    :param __iterable: iterable data, mainly refers to `list`, `tuple`, `set`, `dict`, `str`, `zip`, `range`.
+    :param key: callable function, for example: key=lambda x: x[1], key=lambda x: (x[0], x[1]), key=str.lower.
+    :param reverse: whether to use descending order. The default is ascending order.
+
+    :return: shell's sorted result in a list.
+    '''
+    __iterable: List[_T] = convert(__iterable)
+    compare: List[_T] = generate(__iterable, key)
+    if compare and not verify(compare):
+        length: int = len(__iterable)
+        gap: int = 1
+        while gap < length / 3:
+            gap: int = int(3 * gap + 1)
+        while gap >= 1:
+            for index in range(gap, length):
+                next: int = index
+                while next >= gap and (compare[next - gap] < compare[next] if reverse else compare[next - gap] > compare[next]):
+                    __iterable[next], __iterable[next - gap] = __iterable[next - gap], __iterable[next]
+                    if key != None:
+                        compare[next], compare[next - gap] = compare[next - gap], compare[next]
+                    next -= gap
+            gap: int = int(gap / 3)
+    return __iterable
+    
+def heap(__iterable: Iterable[_T], key: Optional[Callable[[_T], SupportsRichComparison]]=None, reverse: bool=False) -> List[_T]:
+    '''
+    :param __iterable: iterable data, mainly refers to `list`, `tuple`, `set`, `dict`, `str`, `zip`, `range`.
+    :param key: callable function, for example: key=lambda x: x[1], key=lambda x: (x[0], x[1]), key=str.lower.
+    :param reverse: whether to use descending order. The default is ascending order.
+
+    :return: heap's sorted result in a list.
+    '''
+    __iterable: List[_T] = convert(__iterable)
+    compare: List[_T] = generate(__iterable, key)
+    def build(root: int, end: int) -> None:
+        '''
+        :param root: cursor indicating the root node (int).
+        :param end: cursor indicating the end of the __iterable (int).
+        '''
+        piv: int = root
+        left: int = 2 * root + 1
+        right: int = 2 * root + 2
+        if left < end and (compare[left] < compare[root] if reverse else compare[left] > compare[root]):
+            piv: int = left
+        if right < end and (compare[right] < compare[piv] if reverse else compare[right] > compare[piv]):
+            piv: int = right
+        if piv != root:
+            __iterable[root], __iterable[piv] = __iterable[piv], __iterable[root]
+            if key != None:
+                compare[root], compare[piv] = compare[piv], compare[root]
+            build(piv, end)
+    if compare and not verify(compare):
+        length: int = len(__iterable)
+        for root in range(length // 2 - 1 , -1, -1):
+            build(root, length)
+        for end in range(length - 1, 0, -1):
+            if compare[0] != compare[end]:
+                __iterable[0], __iterable[end] = __iterable[end], __iterable[0]
+                if key != None:
+                    compare[0], compare[end] = compare[end], compare[0]
+            build(0, end)
+    return __iterable
+
+def quick(__iterable: Iterable[_T], key: Optional[Callable[[_T], SupportsRichComparison]]=None, reverse: bool=False) -> List[_T]:
+    '''
+    :param __iterable: iterable data, mainly refers to `list`, `tuple`, `set`, `dict`, `str`, `zip`, `range`.
+    :param key: callable function, for example: key=lambda x: x[1], key=lambda x: (x[0], x[1]), key=str.lower.
+    :param reverse: whether to use descending order. The default is ascending order.
+
+    :return: quick's sorted result in a list.
+    '''
+    __iterable: List[_T] = convert(__iterable)
+    compare: List[_T] = generate(__iterable, key)
+    def solve(l: int, r: int) -> None:
+        '''
+        main
+        '''
+        if l < r:
+            mid: int = partition(l, r)
+            solve(l, mid - 1)
+            solve(mid + 1, r)
+
+    def partition(l: int, r: int) -> int:
+        '''
+        :param l: The left cursor of __iterable (int).
+        :param r: The right cursor of __iterable (int).
+        '''
+        val: _T = compare[r]
+        index: int = l - 1
+        for ind in range(l, r):
+            if (val < compare[ind] if reverse else val > compare[ind]):
+                index += 1
+                if compare[index] != compare[ind]:
+                    __iterable[index], __iterable[ind] = __iterable[ind], __iterable[index]
+                    if key != None:
+                        compare[index], compare[ind] = compare[ind], compare[index]
+        if compare[index + 1] != compare[r]:
+            __iterable[index + 1], __iterable[r] = __iterable[r], __iterable[index + 1]
+            if key != None:
+                compare[index + 1], compare[r] = compare[r], compare[index + 1]
+        return index + 1
+    if compare and not verify(compare):
+        solve(0, len(__iterable) - 1)
+    return __iterable
+
+def merge(__iterable: Iterable[_T], key: Optional[Callable[[_T], SupportsRichComparison]]=None, reverse: bool=False) -> List[_T]:
+    '''
+    :param __iterable: iterable data, mainly refers to `list`, `tuple`, `set`, `dict`, `str`, `zip`, `range`.
+    :param key: callable function, for example: key=lambda x: x[1], key=lambda x: (x[0], x[1]), key=str.lower.
+    :param reverse: whether to use descending order. The default is ascending order.
+
+    :return: merge's sorted result in a list.
+    '''
+    __iterable: List[_T] = convert(__iterable)
+    compare: List[_T] = generate(__iterable, key)
+    def merg(low: int, mid: int, high: int) -> None:
+        '''
+        :param low: The low cursor of __iterable (int).
+        :param mid: The middle cursor of __iterable (int).
+        :param high: The high cursor of __iterable (int).
+        '''
+        left: List[_T] = __iterable[low: mid]
+        lc: List[_T] = compare[low: mid]
+        right: List[_T] = __iterable[mid: high]
+        rc: List[_T] = compare[mid: high]
+        i: int = 0
+        j: int = 0
+        result: List[_T] = []
+        store: List[_T] = []
+        while i < len(left) and j < len(right):
+            if (rc[j] <= lc[i] if reverse else rc[j] >= lc[i]):
+                result.append(left[i])
+                store.append(lc[i])
+                i += 1
+            else:
+                result.append(right[j])
+                store.append(rc[j])
+                j += 1
+        result += left[i:]
+        store += lc[i:]
+        result += right[j:]
+        store += rc[j:]
+        __iterable[low: high]: List[_T] = result
+        compare[low: high]: List[_T] = store
+
+    def solve() -> None:
+        '''
+        main
+        '''
+        i: int = 1
+        while i < len(__iterable):
+            low: int = 0
+            while low < len(__iterable):
+                mid: int = low + i
+                high: int = min(low + 2 * i, len(__iterable))
+                if mid < high:
+                    merg(low, mid, high)
+                low += 2 * i
+            i *= 2
+    if compare and not verify(compare):
+        solve()
     return __iterable
```

### Comparing `sortingx-1.3.0/sortingx.egg-info/PKG-INFO` & `sortingx-1.3.1/sortingx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sortingx
-Version: 1.3.0
+Version: 1.3.1
 Summary: The powerful package designed for sorting.
 Home-page: https://github.com/linjing-lab/sorting-algorithms
 Download-URL: https://github.com/linjing-lab/sorting-algorithms/tags
 Author: 林景
 Author-email: linjing010729@163.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/linjing-lab/sorting-algorithms/tree/main/sortingx
@@ -30,15 +30,15 @@
 Theory analysis and code implementation of common array sorting algorithms.
 
 ## 📍 start from galley
 
 First, You need to click the [`fork`](https://github.com/linjing-lab/sorting-algorithms/fork) button to create your own sub repository, or use the following command to synchronize the repository to the local folder:
 
 ```git
-git clone https://github.com/linjing-lab/sorting-algorithms
+git clone https://github.com/linjing-lab/sorting-algorithms.git
 ```
 
 Second, I have put different implemented versions of various sorting algorithms in the [`galley`](./docs/galley/) folder, everyone can import it with the underlying command:
 
 ```python
 import galley as ge
 ```
@@ -121,11 +121,14 @@
 - [sortingx-1.2.1](https://github.com/linjing-lab/sorting-algorithms/tree/v1.2.1) is the portable version that comparison is faster than ever, the generate is more portable.
 
 By the way, I didn't complete all the iterative data types, in order to develop a more targeted scenario. If you are **interested** in other iterative data types, please add them in the `convert` function of the `_utils.py` file, for example: bytes, bytearray, range, zip. If you need to deal with `dict_keys`, `dict_values`, `dict_items`, please use `list()` to convert the variables of these data types before using any method of sortingx.
 
 - [sortingx-1.2.2](https://github.com/linjing-lab/sorting-algorithms/tree/v1.2.2) is the package that support `range`, `zip`, `dict_keys`, `dict_values`, `dict_items` additionally, you can choose what suitable data you want to input.
 - [sortingx-1.2.3](https://github.com/linjing-lab/sorting-algorithms/tree/v1.2.3) is the package that corrected the situation where elements are equal in `compare`, support more input data, like data as `[['Jack', (98, 100)], ['Bob', (98, 99)], ['Jessi', (98, 97)]]` and key as `lambda x: x[1][0]`.
 - [sortingx-1.3.0](https://github.com/linjing-lab/sorting-algorithms/tree/v1.3.0) is the final version that fully aligned with the `sorted`', reduces redundant data exchanging. like data as `[('Alex', 97, 90, 98, 95), ('Jack', 97, 88, 98, 92), ('Peter', 92, 95, 92, 96), ('Li', 97, 89, 98, 92)]` and key as `key=lambda x: x[1]`.
+- [sortingx-1.3.1](https://github.com/linjing-lab/sorting-algorithms/tree/v1.3.1) is the improved version from v1.3.0, and pre-operations from `_utils` are more conise to reduce shallow copy in Runtime.
+
+refer to [this](https://github.com/linjing-lab/sorting-algorithms/blob/main/README_release.md) for downloaded info.
 
 ## LICENSE
 
 [Apache 2.0](./LICENSE)
```

