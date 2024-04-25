# Comparing `tmp/sqlx-exec-2.3.7.tar.gz` & `tmp/sqlx-exec-2.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-2.3.7.tar", last modified: Mon Apr 22 02:19:26 2024, max compression
+gzip compressed data, was "sqlx-exec-2.3.8.tar", last modified: Thu Apr 25 08:14:12 2024, max compression
```

## Comparing `sqlx-exec-2.3.7.tar` & `sqlx-exec-2.3.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 02:19:26.000000 sqlx-exec-2.3.7/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-2.3.7/LICENSE
--rw-rw-rw-   0        0        0     7693 2024-04-22 02:19:26.000000 sqlx-exec-2.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     7158 2024-04-21 13:24:48.000000 sqlx-exec-2.3.7/README.rst
--rw-rw-rw-   0        0        0       42 2024-04-22 02:19:26.000000 sqlx-exec-2.3.7/setup.cfg
--rw-rw-rw-   0        0        0     1335 2024-04-22 02:14:37.000000 sqlx-exec-2.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 02:19:26.000000 sqlx-exec-2.3.7/sqlexec/
--rw-rw-rw-   0        0        0      655 2024-03-26 02:35:08.000000 sqlx-exec-2.3.7/sqlexec/constant.py
--rw-rw-rw-   0        0        0     8236 2024-04-21 13:24:48.000000 sqlx-exec-2.3.7/sqlexec/dialect.py
--rw-rw-rw-   0        0        0    14270 2024-04-21 13:24:48.000000 sqlx-exec-2.3.7/sqlexec/exec.py
--rw-rw-rw-   0        0        0     1998 2024-04-21 13:38:06.000000 sqlx-exec-2.3.7/sqlexec/loader.py
--rw-rw-rw-   0        0        0      838 2024-03-26 05:20:53.000000 sqlx-exec-2.3.7/sqlexec/log_support.py
--rw-rw-rw-   0        0        0     1983 2024-03-26 13:46:42.000000 sqlx-exec-2.3.7/sqlexec/page_exec.py
--rw-rw-rw-   0        0        0    12439 2024-03-26 06:05:25.000000 sqlx-exec-2.3.7/sqlexec/sql_exec.py
--rw-rw-rw-   0        0        0     3164 2024-04-21 13:24:48.000000 sqlx-exec-2.3.7/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0    18946 2024-04-21 13:24:48.000000 sqlx-exec-2.3.7/sqlexec/table_exec.py
--rw-rw-rw-   0        0        0     1891 2024-04-22 02:13:46.000000 sqlx-exec-2.3.7/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 02:19:26.000000 sqlx-exec-2.3.7/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2024-04-22 02:19:26.000000 sqlx-exec-2.3.7/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-27 04:01:32.000000 sqlx-exec-2.3.7/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     7693 2024-04-22 02:19:26.000000 sqlx-exec-2.3.7/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       21 2024-04-22 02:19:26.000000 sqlx-exec-2.3.7/sqlx_exec.egg-info/requires.txt
--rw-rw-rw-   0        0        0      438 2024-04-22 02:19:26.000000 sqlx-exec-2.3.7/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2024-04-22 02:19:26.000000 sqlx-exec-2.3.7/sqlx_exec.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-22 02:19:26.000000 sqlx-exec-2.3.7/test/
--rw-rw-rw-   0        0        0     1234 2024-04-21 13:24:48.000000 sqlx-exec-2.3.7/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-25 08:14:12.760810 sqlx-exec-2.3.8/
+-rw-r--r--   0 summy      (501) staff       (20)    11357 2024-01-23 07:49:56.000000 sqlx-exec-2.3.8/LICENSE
+-rw-r--r--   0 summy      (501) staff       (20)     7493 2024-04-25 08:14:12.759953 sqlx-exec-2.3.8/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)     6974 2024-03-29 02:19:13.000000 sqlx-exec-2.3.8/README.rst
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-04-25 08:14:12.761638 sqlx-exec-2.3.8/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1299 2024-04-25 08:13:55.000000 sqlx-exec-2.3.8/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-25 08:14:12.745543 sqlx-exec-2.3.8/sqlexec/
+-rw-r--r--   0 summy      (501) staff       (20)     1833 2024-04-25 08:03:09.000000 sqlx-exec-2.3.8/sqlexec/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)      637 2024-03-27 13:46:01.000000 sqlx-exec-2.3.8/sqlexec/constant.py
+-rw-r--r--   0 summy      (501) staff       (20)     8518 2024-04-25 07:59:15.000000 sqlx-exec-2.3.8/sqlexec/dialect.py
+-rw-r--r--   0 summy      (501) staff       (20)    14101 2024-04-25 08:07:19.000000 sqlx-exec-2.3.8/sqlexec/exec.py
+-rw-r--r--   0 summy      (501) staff       (20)     1936 2024-04-25 04:18:32.000000 sqlx-exec-2.3.8/sqlexec/loader.py
+-rw-r--r--   0 summy      (501) staff       (20)      816 2024-03-27 08:41:08.000000 sqlx-exec-2.3.8/sqlexec/log_support.py
+-rw-r--r--   0 summy      (501) staff       (20)     1933 2024-03-27 08:41:08.000000 sqlx-exec-2.3.8/sqlexec/page_exec.py
+-rw-r--r--   0 summy      (501) staff       (20)    12121 2024-03-27 08:41:08.000000 sqlx-exec-2.3.8/sqlexec/sql_exec.py
+-rw-r--r--   0 summy      (501) staff       (20)     3068 2024-04-08 10:27:42.000000 sqlx-exec-2.3.8/sqlexec/sql_support.py
+-rw-r--r--   0 summy      (501) staff       (20)    18422 2024-04-08 12:17:35.000000 sqlx-exec-2.3.8/sqlexec/table_exec.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-25 08:14:12.755070 sqlx-exec-2.3.8/sqlx_exec.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     7493 2024-04-25 08:14:12.000000 sqlx-exec-2.3.8/sqlx_exec.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      438 2024-04-25 08:14:12.000000 sqlx-exec-2.3.8/sqlx_exec.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-25 08:14:12.000000 sqlx-exec-2.3.8/sqlx_exec.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-03-27 09:08:34.000000 sqlx-exec-2.3.8/sqlx_exec.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       21 2024-04-25 08:14:12.000000 sqlx-exec-2.3.8/sqlx_exec.egg-info/requires.txt
+-rw-r--r--   0 summy      (501) staff       (20)        8 2024-04-25 08:14:12.000000 sqlx-exec-2.3.8/sqlx_exec.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-25 08:14:12.757132 sqlx-exec-2.3.8/test/
+-rw-r--r--   0 summy      (501) staff       (20)     1192 2024-04-08 10:07:10.000000 sqlx-exec-2.3.8/test/test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sqlx-exec-2.3.7/LICENSE` & `sqlx-exec-2.3.8/LICENSE`

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

### Comparing `sqlx-exec-2.3.7/PKG-INFO` & `sqlx-exec-2.3.8/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,200 +1,184 @@
-Metadata-Version: 2.1
-Name: sqlx-exec
-Version: 2.3.7
-Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions. Support MySQL, PostgreSQL, SQLite etc.
-Home-page: https://gitee.com/summry/sqlx-exec
-Author: summy
-Author-email: xiazhongbiao@126.com
-License: UNKNOWN
-Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python,RDB
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-Usage Sample
-''''''''''''
-
-.. code:: python
-
-       import sqlexec as db
-
-       if __name__ == '__main__':
-           db.init('test.db', driver='sqlite3', show_sql=True, debug=True)
-
-           # or
-           db.init("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
-
-           # or
-           db.init(host='127.0.0.1', port='5432', user='xxx', password='xxx', database='testdb', show_sql=True, driver='psycopg2')
-
-           effected_rowcount = db.insert(table='person', name='zhangsan', age=15)
-
-           # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
-           select_key = "SELECT currval('person_id_seq')"
-
-           id = db.save(select_key=select_key, table='person', name='lisi', age=26)
-
-           id = db.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(?,?)', 'wangwu', 38)
-
-           id = db.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(:name, :age)', name='zhaoliu', age=45)
-
-           count = db.get('select count(1) from person')
-           # result: 4
-
-           count = db.sql('select count(1) from person').get()
-           # result: 4
-
-           persons = db.select('select id, name, age from person')
-           # result:
-           # (3, 'zhangsan', 15)
-           # (4, 'lisi', 26)
-           # (5, 'wangwu', 38)
-           # (6, 'zhaoliu', 45)
-
-           persons = db.sql('select id, name, age from person').select()
-           # result:
-           # (3, 'zhangsan', 15)
-           # (4, 'lisi', 26)
-           # (5, 'wangwu', 38)
-           # (6, 'zhaoliu', 45)
-
-           persons = db.table('person').select('id', 'name', 'age')
-           # result:
-           # (3, 'zhangsan', 15)
-           # (4, 'lisi', 26)
-           # (5, 'wangwu', 38)
-           # (6, 'zhaoliu', 45)
-
-           persons = db.select_one('select id, name, age from person where name = ?', 'zhangsan')
-           # result:
-           # (3, 'zhangsan', 15)
-
-           persons = db.sql('select id, name, age from person where name = ?').select_one('zhangsan')
-           # result:
-           # (3, 'zhangsan', 15)
-
-           persons = db.select('select id, name, age from person where name = :name', name='zhangsan')
-           # result:
-           # [(3, 'zhangsan', 15)]
-
-           persons = db.sql('select id, name, age from person where name = :name').select(name='zhangsan')
-           # result:
-           # [(3, 'zhangsan', 15)]
-
-           persons = db.sql('select id, name, age from person where name = :name').param(name='zhangsan').select()
-           # result:
-           # [(3, 'zhangsan', 15)]
-
-           persons = db.table('person').where(name__eq='zhangsan').select('id', 'name', 'age')
-           # result:
-           # [(3, 'zhangsan', 15)]
-
-           persons = db.query('select id, name, age from person')
-           # result:
-           # {'id': 3, 'name': 'zhangsan', 'age': 15}
-           # {'id': 4, 'name': 'lisi', 'age': 26}
-           # {'id': 5, 'name': 'wangwu', 'age': 38}
-           # {'id': 6, 'name': 'zhaoliu', 'age': 45}
-
-           persons = db.sql('select id, name, age from person').query()
-           # result:
-           # {'id': 3, 'name': 'zhangsan', 'age': 15}
-           # {'id': 4, 'name': 'lisi', 'age': 26}
-           # {'id': 5, 'name': 'wangwu', 'age': 38}
-           # {'id': 6, 'name': 'zhaoliu', 'age': 45}
-
-           persons = db.query_one('select id, name, age from person where name = ?', 'zhangsan')
-           # result:
-           # {'id': 3, 'name': 'zhangsan', 'age': 15}
-
-           persons = db.sql('select id, name, age from person where name = ?').query_one('zhangsan')
-           # result:
-           # {'id': 3, 'name': 'zhangsan', 'age': 15}
-
-           persons = db.query('select id, name, age from person where name = :name', name='zhangsan')
-           # result:
-           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
-
-           persons = db.sql('select id, name, age from person where name = :name').query(name='zhangsan')
-           # result:
-           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
-
-           persons = db.sql('select id, name, age from person where name = :name').param(name='zhangsan').query()
-           # result:
-           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
-
-           persons = db.table('person').columns('id', 'name', 'age').where(name='zhangsan').query()
-           # result:
-           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
-
-           effected_rowcount = db.table('person').where(name='zhangsan').update(name='xxx', age=45)
-
-           effected_rowcount = db.table('person').where(id=6).delete()
-           count = db.table('person').count())
-           # result: 3
-
-           effected_rowcount = db.execute('delete from person where id = :id', id=5)
-           count = db.get('select count(1) from person')
-           # result: 2
-
-           effected_rowcount = db.sql('delete from person where id = ?').execute(4)
-           count = db.sql('select count(1) from person').get()
-           # result: 1
-
-           effected_rowcount = db.sql('delete from person where id = :id').execute(id=3)
-           count = db.sql('select count(1) from person').get()
-           # result: 0
-
-           # select data save as csv
-           db.sql('select name, age from person WHERE name = ?').load('张三').to_csv('test.csv')
-
-           db.sql('select name, age from person WHERE name = ?').param('张三').to_csv('test.csv')
-
-           # insert from csv
-           db.table('person').insert_from_csv('test.csv')
-
-           # select data transform to DataFrame of pandas
-           df = db.sql('select name, age from person WHERE name = :name').load(name='张三').to_df()
-
-           df = db.sql('select name, age from person WHERE name = :name').param(name='张三').to_df()
-
-           # insert from DataFrame of pandas
-           db.table('person').insert_from_df(dataframe)
-
-           # select data save as json
-           db.sql('select name, age from person WHERE name = ?').load('张三').to_json('test.json')
-
-           db.sql('select name, age from person WHERE name = ?').param('张三').to_json('test.json')
-
-           # insert from json
-           db.table('person').insert_from_json('test.json')
-
-           db.close()
-
-Transaction
-'''''''''''
-
-.. code:: python
-
-       from sqlexec import with_transaction, transaction
-
-       @with_transaction
-       def test_transaction():
-           insert_func(....)
-           update_func(....)
-
-
-       def test_transaction2():
-           with transaction():
-               insert_func(....)
-               update_func(....)
-
-
-If you want to operate MySQL database like Mybatis, may be you need MySqlx: https://pypi.org/project/mysqlx
-
-If you want to operate PostgreSQL database like Mybatis, may be you need PgSqlx: https://pypi.org/project/pgsqlx
-
-If you want to execute SQL like Mybatis, may be you need sqlx-batis: https://pypi.org/project/sqlx-batis
-
-
+Usage Sample
+''''''''''''
+
+.. code:: python
+
+       import sqlexec as db
+
+       if __name__ == '__main__':
+           db.init('test.db', driver='sqlite3', show_sql=True, debug=True)
+
+           # or
+           db.init("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
+
+           # or
+           db.init(host='127.0.0.1', port='5432', user='xxx', password='xxx', database='testdb', show_sql=True, driver='psycopg2')
+
+           effected_rowcount = db.insert(table='person', name='zhangsan', age=15)
+
+           # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
+           select_key = "SELECT currval('person_id_seq')"
+
+           id = db.save(select_key=select_key, table='person', name='lisi', age=26)
+
+           id = db.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(?,?)', 'wangwu', 38)
+
+           id = db.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(:name, :age)', name='zhaoliu', age=45)
+
+           count = db.get('select count(1) from person')
+           # result: 4
+
+           count = db.sql('select count(1) from person').get()
+           # result: 4
+
+           persons = db.select('select id, name, age from person')
+           # result:
+           # (3, 'zhangsan', 15)
+           # (4, 'lisi', 26)
+           # (5, 'wangwu', 38)
+           # (6, 'zhaoliu', 45)
+
+           persons = db.sql('select id, name, age from person').select()
+           # result:
+           # (3, 'zhangsan', 15)
+           # (4, 'lisi', 26)
+           # (5, 'wangwu', 38)
+           # (6, 'zhaoliu', 45)
+
+           persons = db.table('person').select('id', 'name', 'age')
+           # result:
+           # (3, 'zhangsan', 15)
+           # (4, 'lisi', 26)
+           # (5, 'wangwu', 38)
+           # (6, 'zhaoliu', 45)
+
+           persons = db.select_one('select id, name, age from person where name = ?', 'zhangsan')
+           # result:
+           # (3, 'zhangsan', 15)
+
+           persons = db.sql('select id, name, age from person where name = ?').select_one('zhangsan')
+           # result:
+           # (3, 'zhangsan', 15)
+
+           persons = db.select('select id, name, age from person where name = :name', name='zhangsan')
+           # result:
+           # [(3, 'zhangsan', 15)]
+
+           persons = db.sql('select id, name, age from person where name = :name').select(name='zhangsan')
+           # result:
+           # [(3, 'zhangsan', 15)]
+
+           persons = db.sql('select id, name, age from person where name = :name').param(name='zhangsan').select()
+           # result:
+           # [(3, 'zhangsan', 15)]
+
+           persons = db.table('person').where(name__eq='zhangsan').select('id', 'name', 'age')
+           # result:
+           # [(3, 'zhangsan', 15)]
+
+           persons = db.query('select id, name, age from person')
+           # result:
+           # {'id': 3, 'name': 'zhangsan', 'age': 15}
+           # {'id': 4, 'name': 'lisi', 'age': 26}
+           # {'id': 5, 'name': 'wangwu', 'age': 38}
+           # {'id': 6, 'name': 'zhaoliu', 'age': 45}
+
+           persons = db.sql('select id, name, age from person').query()
+           # result:
+           # {'id': 3, 'name': 'zhangsan', 'age': 15}
+           # {'id': 4, 'name': 'lisi', 'age': 26}
+           # {'id': 5, 'name': 'wangwu', 'age': 38}
+           # {'id': 6, 'name': 'zhaoliu', 'age': 45}
+
+           persons = db.query_one('select id, name, age from person where name = ?', 'zhangsan')
+           # result:
+           # {'id': 3, 'name': 'zhangsan', 'age': 15}
+
+           persons = db.sql('select id, name, age from person where name = ?').query_one('zhangsan')
+           # result:
+           # {'id': 3, 'name': 'zhangsan', 'age': 15}
+
+           persons = db.query('select id, name, age from person where name = :name', name='zhangsan')
+           # result:
+           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+
+           persons = db.sql('select id, name, age from person where name = :name').query(name='zhangsan')
+           # result:
+           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+
+           persons = db.sql('select id, name, age from person where name = :name').param(name='zhangsan').query()
+           # result:
+           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+
+           persons = db.table('person').columns('id', 'name', 'age').where(name='zhangsan').query()
+           # result:
+           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+
+           effected_rowcount = db.table('person').where(name='zhangsan').update(name='xxx', age=45)
+
+           effected_rowcount = db.table('person').where(id=6).delete()
+           count = db.table('person').count())
+           # result: 3
+
+           effected_rowcount = db.execute('delete from person where id = :id', id=5)
+           count = db.get('select count(1) from person')
+           # result: 2
+
+           effected_rowcount = db.sql('delete from person where id = ?').execute(4)
+           count = db.sql('select count(1) from person').get()
+           # result: 1
+
+           effected_rowcount = db.sql('delete from person where id = :id').execute(id=3)
+           count = db.sql('select count(1) from person').get()
+           # result: 0
+
+           # select data save as csv
+           db.sql('select name, age from person WHERE name = ?').load('张三').to_csv('test.csv')
+
+           db.sql('select name, age from person WHERE name = ?').param('张三').to_csv('test.csv')
+
+           # insert from csv
+           db.table('person').insert_from_csv('test.csv')
+
+           # select data transform to DataFrame of pandas
+           df = db.sql('select name, age from person WHERE name = :name').load(name='张三').to_df()
+
+           df = db.sql('select name, age from person WHERE name = :name').param(name='张三').to_df()
+
+           # insert from DataFrame of pandas
+           db.table('person').insert_from_df(dataframe)
+
+           # select data save as json
+           db.sql('select name, age from person WHERE name = ?').load('张三').to_json('test.json')
+
+           db.sql('select name, age from person WHERE name = ?').param('张三').to_json('test.json')
+
+           # insert from json
+           db.table('person').insert_from_json('test.json')
+
+           db.close()
+
+Transaction
+'''''''''''
+
+.. code:: python
+
+       from sqlexec import with_transaction, transaction
+
+       @with_transaction
+       def test_transaction():
+           insert_func(....)
+           update_func(....)
+
+
+       def test_transaction2():
+           with transaction():
+               insert_func(....)
+               update_func(....)
+
+
+If you want to operate MySQL database like Mybatis, may be you need MySqlx: https://pypi.org/project/mysqlx
+
+If you want to operate PostgreSQL database like Mybatis, may be you need PgSqlx: https://pypi.org/project/pgsqlx
+
+If you want to execute SQL like Mybatis, may be you need sqlx-batis: https://pypi.org/project/sqlx-batis
```

### Comparing `sqlx-exec-2.3.7/setup.py` & `sqlx-exec-2.3.8/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import os
-from setuptools import setup
-
-# INSTALL_PACKAGES = open(path.join(DIR, 'requirements.txt')).read().splitlines()
-def read(rel_path: str) -> str:
-    here = os.path.abspath(os.path.dirname(__file__))
-    # intentionally *not* adding an encoding option to open, See:
-    #   https://github.com/pypa/virtualenv/issues/201#issuecomment-3145690
-    with open(os.path.join(here, rel_path), 'r', encoding='UTF-8') as fp:
-        return fp.read()
-
-long_description = read("README.rst")
-
-setup(
-    name='sqlx-exec',
-    packages=['sqlexec'],
-    description="A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions. Support MySQL, PostgreSQL, SQLite etc.",
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    version='2.3.7',
-    install_requires=[
-        'sqlx-executor>=1.1.1',
-    ],
-    url='https://gitee.com/summry/sqlx-exec',
-    author='summy',
-    author_email='xiazhongbiao@126.com',
-    keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Oracle', 'SQL Server', 'Database', 'Python', 'RDB'],
-    package_data={
-        # include json and txt files
-        '': ['*.rst', '*.dtd', '*.tpl'],
-    },
-    include_package_data=True,
-    python_requires='>=3.6',
-    zip_safe=False
-)
-
+import os
+from setuptools import setup
+
+# INSTALL_PACKAGES = open(path.join(DIR, 'requirements.txt')).read().splitlines()
+def read(rel_path: str) -> str:
+    here = os.path.abspath(os.path.dirname(__file__))
+    # intentionally *not* adding an encoding option to open, See:
+    #   https://github.com/pypa/virtualenv/issues/201#issuecomment-3145690
+    with open(os.path.join(here, rel_path), 'r', encoding='UTF-8') as fp:
+        return fp.read()
+
+long_description = read("README.rst")
+
+setup(
+    name='sqlx-exec',
+    packages=['sqlexec'],
+    description="A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions. Support MySQL, PostgreSQL, SQLite etc.",
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    version='2.3.8',
+    install_requires=[
+        'sqlx-executor>=1.1.1',
+    ],
+    url='https://gitee.com/summry/sqlx-exec',
+    author='summy',
+    author_email='xiazhongbiao@126.com',
+    keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Oracle', 'SQL Server', 'Database', 'Python', 'RDB'],
+    package_data={
+        # include json and txt files
+        '': ['*.rst', '*.dtd', '*.tpl'],
+    },
+    include_package_data=True,
+    python_requires='>=3.6',
+    zip_safe=False
+)
+
```

### Comparing `sqlx-exec-2.3.7/sqlexec/constant.py` & `sqlx-exec-2.3.8/sqlexec/constant.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-LIMIT_1 = 1
-
-CACHE_SIZE = 256
-
-SELECT_COUNT = 'count(1)'
-
-NAMED_REGEX = r':[\w|\d]*'
-
-DEFAULT_KEY_FIELD = 'id'
-
-MYSQL_SELECT_KEY = "SELECT LAST_INSERT_ID()"
-
-SQLITE_SELECT_KEY = 'SELECT last_insert_rowid()'
-
-MYSQL_COLUMN_SQL = '''SELECT GROUP_CONCAT(CONCAT("`",column_name,"`") SEPARATOR ",") 
-                        FROM `information_schema`.`columns` WHERE `table_schema` = (SELECT DATABASE()) AND `table_name` = ? LIMIT ?'''
-
-POSTGRES_COLUMN_SQL = '''SELECT array_to_string(array_agg(column_name),',') as column_name FROM information_schema.columns 
+LIMIT_1 = 1
+
+CACHE_SIZE = 256
+
+SELECT_COUNT = 'count(1)'
+
+NAMED_REGEX = r':[\w|\d]*'
+
+DEFAULT_KEY_FIELD = 'id'
+
+MYSQL_SELECT_KEY = "SELECT LAST_INSERT_ID()"
+
+SQLITE_SELECT_KEY = 'SELECT last_insert_rowid()'
+
+MYSQL_COLUMN_SQL = '''SELECT GROUP_CONCAT(CONCAT("`",column_name,"`") SEPARATOR ",") 
+                        FROM `information_schema`.`columns` WHERE `table_schema` = (SELECT DATABASE()) AND `table_name` = ? LIMIT ?'''
+
+POSTGRES_COLUMN_SQL = '''SELECT array_to_string(array_agg(column_name),',') as column_name FROM information_schema.columns 
                           WHERE table_schema='public' and table_name = ? LIMIT ?'''
```

### Comparing `sqlx-exec-2.3.7/sqlexec/exec.py` & `sqlx-exec-2.3.8/sqlexec/exec.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,392 +1,398 @@
-from .dialect import Dialect
-from .loader import Loader
-from . import sql_support
-from executor import DBError
-from typing import Collection, Iterable
-from .log_support import logger, insert_log, save_log
-from executor import execute as _execute, select as _select, select_one as _select_one, do_select as _do_select,\
-    save as _save, batch_execute as _batch_execute, get as _get, query as _query, query_one as _query_one
-
-
-def execute(sql: str, *args, **kwargs):
-    """
-    Execute sql return effect rowcount
-
-    sql: INSERT INTO person(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
-         INSERT INTO person(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
-    """
-    sql, args = sql_support.try_mapping('sqlexec.execute', sql, *args, **kwargs)
-    return do_execute(sql, *args)
-
-
-def insert(table_name: str, **kwargs):
-    """
-    Insert data into table, return effect rowcount.
-
-    :param table_name: table name
-    :param kwargs: {name='张三', age=20}
-    return: Effect rowcount
-    """
-    insert_log('insert', table_name, **kwargs)
-    sql, args = sql_support.insert_sql_args(table_name.strip(), **kwargs)
-    return do_execute(sql, *args)
-
-
-def save(table_name: str, **kwargs):
-    """
-    Insert data into table, return primary key.
-    """
-    try:
-        select_key = Dialect.get_select_key(table_name=table_name)
-    except NotImplementedError:
-        raise DBError(f"Expect 'select_key' but not. you may should use 'save_select_key' func with 'select_key'.")
-    return save_select_key(select_key, table_name, **kwargs)
-
-
-def save_sql(sql: str, *args, **kwargs):
-    """
-    Insert data into table, return primary key.
-    """
-    try:
-        select_key = Dialect.get_select_key(sql=sql)
-    except NotImplementedError:
-        raise DBError(f"Expect 'select_key' but not. you may should use 'save_sql_select_key' func with 'select_key'.")
-    return save_sql_select_key(select_key, sql, *args, **kwargs)
-
-
-def save_select_key(select_key: str, table_name: str, **kwargs):
-    """
-    Insert data into table, return primary key.
-
-    :param select_key: sql for select primary key
-    :param table_name: table name
-    :param kwargs: {name='张三', age=20}
-    :return: Primary key
-    """
-    save_log('save_select_key', select_key, table_name, **kwargs)
-    sql, args = sql_support.insert_sql_args(table_name.strip(), **kwargs)
-    return save_sql_select_key(select_key, sql, *args)
-
-
-def save_sql_select_key(select_key: str, sql: str, *args, **kwargs):
-    """
-    Insert data into table, return primary key.
-
-    sql: INSERT INTO person(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
-         INSERT INTO person(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
-
-    :param select_key: sql for select primary key
-    :param sql: SQL
-    :return: Primary key
-    """
-    logger.debug("Exec func 'sqlexec.%s', 'select_key': %s \n\t sql: %s \n\t args: %s \n\t kwargs: %s" % ('save_sql', select_key, sql, args, kwargs))
-    sql, args = sql_support.get_mapping_sql_args(sql, *args, **kwargs)
-    return do_save_sql_select_key(select_key, sql, *args)
-
-
-def get(sql: str, *args, **kwargs):
-    """
-    Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
-
-    MultiColumnsError: Expect only one column.
-    sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
-         SELECT count(1) FROM person WHERE name=:name and age=:age limit 1  --> kwargs: {'name': '张三', 'age': 20}
-    """
-    sql, args = sql_support.try_mapping('sqlexec.get', sql, *args, **kwargs)
-    return do_get(sql, *args)
-
-
-def select(sql: str, *args, **kwargs):
-    """
-    execute select SQL and return unique result or list results(tuple).
-
-    sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
-         SELECT * FROM person WHERE name=:name and age=:age --> kwargs: {'name': '张三', 'age': 20}
-    """
-    sql, args = sql_support.try_mapping('sqlexec.select', sql, *args, **kwargs)
-    return do_select(sql, *args)
-
-
-def select_one(sql: str, *args, **kwargs):
-    """
-    Execute select SQL and return unique result(tuple), SQL contain 'limit'.
-
-    sql: SELECT * FROM person WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
-         SELECT * FROM person WHERE name=:name and age=:age limit 1 --> kwargs: {'name': '张三', 'age': 20}
-    """
-    sql, args = sql_support.try_mapping('sqlexec.select_one', sql, *args, **kwargs)
-    return do_select_one(sql, *args)
-
-
-def query(sql: str, *args, **kwargs):
-    """
-    Execute select SQL and return list results(dict).
-    sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
-         SELECT * FROM person WHERE name=:name and age=:age --> kwargs: {'name': '张三', 'age': 20}
-    """
-    sql, args = sql_support.try_mapping('sqlexec.query', sql, *args, **kwargs)
-    return do_query(sql, *args)
-
-
-def query_one(sql: str, *args, **kwargs):
-    """
-    execute select SQL and return unique result(dict), SQL contain 'limit'.
-
-    sql: SELECT * FROM person WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
-         SELECT * FROM person WHERE name=:name and age=:age limit 1 --> kwargs: {'name': '张三', 'age': 20}
-    """
-    sql, args = sql_support.try_mapping('sqlexec.query_one', sql, *args, **kwargs)
-    return do_query_one(sql, *args)
-
-
-def do_execute(sql: str, *args):
-    """
-    Execute sql return effect rowcount
-
-    sql: insert into person(name, age) values(?, ?)  -->  args: ('张三', 20)
-    """
-    sql = Dialect.before_execute(sql)
-    return _execute(sql, *args)
-
-
-def do_save_sql(sql: str, *args):
-    """
-    Insert data into table, return primary key.
-
-    :param select_key: sql for select primary key
-    :param sql: SQL
-    :param args:
-    :return: Primary key
-    """
-    try:
-        select_key = Dialect.get_select_key(sql=sql)
-    except NotImplementedError:
-        raise DBError(f"Expect 'select_key' but not. you may should use 'save_sql_select_key' func with 'select_key'.")
-    return do_save_sql_select_key(select_key, sql, *args)
-
-
-def do_save_sql_select_key(select_key: str, sql: str, *args):
-    """
-    Insert data into table, return primary key.
-
-    :param select_key: sql for select primary key
-    :param sql: SQL
-    :param args:
-    :return: Primary key
-    """
-    sql = Dialect.before_execute(sql)
-    return _save(select_key, sql, *args)
-
-
-def do_get(sql: str, *args):
-    """
-    Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
-    MultiColumnsError: Expect only one column.
-
-    sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
-    """
-    sql, args = sql_support.limit_one_sql_args(sql, *args)
-    sql = Dialect.before_execute(sql)
-    return _get(sql, *args)
-
-
-def do_select(sql: str, *args):
-    """
-    execute select SQL and return unique result or list results(tuple).
-    sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
-    """
-    sql = Dialect.before_execute(sql)
-    return _select(sql, *args)
-
-
-def do_select_one(sql: str, *args):
-    """
-    Execute select SQL and return unique result(tuple), SQL contain 'limit'.
-    sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
-    """
-    sql, args = sql_support.limit_one_sql_args(sql, *args)
-    sql = Dialect.before_execute(sql)
-    return _select_one(sql, *args)
-
-
-def do_query(sql: str, *args):
-    """
-    Execute select SQL and return list results(dict).
-    sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
-    """
-    sql = Dialect.before_execute(sql)
-    return _query(sql, *args)
-
-
-def do_query_one(sql: str, *args):
-    """
-    execute select SQL and return unique result(dict), SQL contain 'limit'.
-    sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
-    """
-    sql, args = sql_support.limit_one_sql_args(sql, *args)
-    sql = Dialect.before_execute(sql)
-    return _query_one(sql, *args)
-
-
-def select_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
-    """
-    Execute select SQL and return list(tuple) or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
-    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-         SELECT * FROM user WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
-    """
-    sql, args = sql_support.try_mapping('select_page', sql, *args, **kwargs)
-    return do_select_page(sql, page_num, page_size, *args)
-
-
-def query_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
-    """
-    Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
-    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-         SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
-    """
-    sql, args = sql_support.try_mapping('query_page', sql, *args, **kwargs)
-    return do_query_page(sql, page_num, page_size, *args)
-
-
-def do_select_page(sql: str, page_num=1, page_size=10, *args):
-    """
-    Execute select SQL and return list results(dict).
-    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-    """
-    sql, args = Dialect.get_page_sql_args(sql, page_num, page_size, *args)
-    return do_select(sql, *args)
-
-
-def do_query_page(sql: str, page_num=1, page_size=10, *args):
-    """
-    Execute select SQL and return list results(dict).
-    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-    """
-    sql, args = Dialect.get_page_sql_args(sql, page_num, page_size, *args)
-    return do_query(sql, *args)
-
-
-def batch_execute(sql: str, *args):
-    """
-    Batch execute
-    :param sql: insert into person(name, age) values(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
-    :param args: All number must have same size.
-    :return: Effect row count
-    """
-    assert args, "*args must not be empty."
-    if isinstance(args[0], dict):
-        sql, args = sql_support.batch_named_sql_args(sql, *args)
-    sql = Dialect.before_execute(sql)
-    args = sql_support.get_batch_args(*args)
-    return _batch_execute(sql, *args)
-
-
-def batch_insert(table_name: str, *args):
-    """
-    Batch insert
-    :param table_name: table name
-    :param args: All number must have same key. [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
-    :return: Effect row count
-    """
-    logger.debug("Exec func 'sqlexec.%s' \n\t Table: '%s', args: %s" % ('batch_insert', table_name, args))
-    sql, args = sql_support.batch_insert_sql_args(table_name, *args)
-    return batch_execute(sql, *args)
-
-
-def load(sql: str, *args, **kwargs) -> Loader:
-    """
-    Execute select SQL and save a csv
-
-    sqlexec.load('select id, name, age from person WHERE name=:name', name='张三')
-
-    :param sql: SELECT * FROM person WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
-                SELECT * FROM person WHERE name=:name and age=:age limit 1 --> kwargs: {'name': '张三', 'age': 20}
-    :return: Loader
-    """
-    sql, args = sql_support.try_mapping('sqlexec.csv', sql, *args, **kwargs)
-    return do_load(sql, *args)
-
-
-def do_load(sql: str, *args) -> Loader:
-    """
-    Execute select SQL and save a csv
-
-    sqlexec.do_load('select id, name, age from person WHERE name = ?', '张三')
-
-    :param sql: SELECT * FROM person WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
-    :return: Loader
-    """
-    sql = Dialect.before_execute(sql)
-    return Loader(*_do_select(sql, *args))
-
-
-def insert_from_csv(file_name: str, table_name: str, delimiter=',', header=True, columns: Collection[str] = None, encoding='utf-8') -> int:
-    """
-    sqlexec.insert_from_csv('test.csv', 'person')
-    """
-    import csv
-    sql = None
-    if columns and len(columns) > 0:
-        sql = sql_support.insert_sql(table_name.strip(), columns)
-    elif not header:
-        raise ValueError("Expected one of 'header' and 'columns'.")
-
-    with open(file_name, newline='', encoding=encoding) as f:
-        lines = csv.reader(f, delimiter=delimiter)
-        lines = [line for line in lines]
-
-    if len(lines) == 0:
-        return 0
-
-    if header:
-        if len(lines) == 1:
-            return 0
-
-        if sql is None:
-            sql = sql_support.insert_sql(table_name.strip(), lines[0])
-        lines = lines[1:]
-
-    return batch_execute(sql, lines)
-
-
-def insert_from_df(df, table_name: str, columns: Collection[str] = None) -> int:
-    """
-    sqlexec.insert_from_df(df, 'person')
-    """
-    columns = columns if columns and len(columns) > 0 else df.columns.tolist()
-    sql = sql_support.insert_sql(table_name.strip(), columns)
-    return batch_execute(sql, df.values.tolist())
-
-
-def insert_from_json(file_name: str, table_name: str, encoding='utf-8') -> int:
-    """
-    sqlexec.insert_from_json('test.json', 'person')
-
-    many rows json file example:
-    [{"id": 1, "name": "张三", "age": 55}, ...]
-
-    one row json file example:
-    {"id": 1, "name": "张三", "age": 55}
-    """
-    import json
-
-    with open(file_name, encoding=encoding) as f:
-        data = json.load(f)
-
-    if isinstance(data, dict):
-        return insert(table_name, **data)
-    elif isinstance(data, Iterable):
-        return batch_insert(table_name, data)
-    else:
-        logger.info("Exec func 'sqlexec.%s' \n\t Table: '%s' insert 0 rows." % ('insert_from_json', table_name))
-        return 0
-
-
-def truncate_table(table_name: str) -> int:
-    """ sqlexec.truncate('person') """
-    return _execute(Dialect.get_truncate_sql(table_name))
-
-
-def drop_table(table_name: str) -> int:
-    """ sqlexec.drop('person') """
-    return _execute('DROP TABLE %s' % Dialect.get_dialect_str(table_name))
+from executor import DBError
+from typing import Collection, Iterable
+from .loader import Loader
+from .dialect import Dialect, Engine
+from . import sql_support
+from .log_support import logger, insert_log, save_log
+from executor import execute as _execute, select as _select, select_one as _select_one, do_select as _do_select,\
+    save as _save, batch_execute as _batch_execute, get as _get, query as _query, query_one as _query_one
+
+
+def execute(sql: str, *args, **kwargs):
+    """
+    Execute sql return effect rowcount
+
+    sql: INSERT INTO person(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
+         INSERT INTO person(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
+    """
+    sql, args = sql_support.try_mapping('sqlexec.execute', sql, *args, **kwargs)
+    return do_execute(sql, *args)
+
+
+def insert(table_name: str, **kwargs):
+    """
+    Insert data into table, return effect rowcount.
+
+    :param table_name: table name
+    :param kwargs: {name='张三', age=20}
+    return: Effect rowcount
+    """
+    insert_log('insert', table_name, **kwargs)
+    sql, args = sql_support.insert_sql_args(table_name.strip(), **kwargs)
+    return do_execute(sql, *args)
+
+
+def save(table_name: str, **kwargs):
+    """
+    Insert data into table, return primary key.
+    """
+    try:
+        select_key = Dialect.get_select_key(table_name=table_name)
+    except NotImplementedError:
+        raise DBError(f"Expect 'select_key' but not. you may should use 'save_select_key' func with 'select_key'.")
+    return save_select_key(select_key, table_name, **kwargs)
+
+
+def save_sql(sql: str, *args, **kwargs):
+    """
+    Insert data into table, return primary key.
+    """
+    try:
+        select_key = Dialect.get_select_key(sql=sql)
+    except NotImplementedError:
+        raise DBError(f"Expect 'select_key' but not. you may should use 'save_sql_select_key' func with 'select_key'.")
+    return save_sql_select_key(select_key, sql, *args, **kwargs)
+
+
+def save_select_key(select_key: str, table_name: str, **kwargs):
+    """
+    Insert data into table, return primary key.
+
+    :param select_key: sql for select primary key
+    :param table_name: table name
+    :param kwargs: {name='张三', age=20}
+    :return: Primary key
+    """
+    save_log('save_select_key', select_key, table_name, **kwargs)
+    sql, args = sql_support.insert_sql_args(table_name.strip(), **kwargs)
+    return save_sql_select_key(select_key, sql, *args)
+
+
+def save_sql_select_key(select_key: str, sql: str, *args, **kwargs):
+    """
+    Insert data into table, return primary key.
+
+    sql: INSERT INTO person(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
+         INSERT INTO person(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
+
+    :param select_key: sql for select primary key
+    :param sql: SQL
+    :return: Primary key
+    """
+    logger.debug("Exec func 'sqlexec.%s', 'select_key': %s \n\t sql: %s \n\t args: %s \n\t kwargs: %s" % ('save_sql', select_key, sql, args, kwargs))
+    sql, args = sql_support.get_mapping_sql_args(sql, *args, **kwargs)
+    return do_save_sql_select_key(select_key, sql, *args)
+
+
+def get(sql: str, *args, **kwargs):
+    """
+    Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
+
+    MultiColumnsError: Expect only one column.
+    sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+         SELECT count(1) FROM person WHERE name=:name and age=:age limit 1  --> kwargs: {'name': '张三', 'age': 20}
+    """
+    sql, args = sql_support.try_mapping('sqlexec.get', sql, *args, **kwargs)
+    return do_get(sql, *args)
+
+
+def select(sql: str, *args, **kwargs):
+    """
+    execute select SQL and return unique result or list results(tuple).
+
+    sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
+         SELECT * FROM person WHERE name=:name and age=:age --> kwargs: {'name': '张三', 'age': 20}
+    """
+    sql, args = sql_support.try_mapping('sqlexec.select', sql, *args, **kwargs)
+    return do_select(sql, *args)
+
+
+def select_one(sql: str, *args, **kwargs):
+    """
+    Execute select SQL and return unique result(tuple), SQL contain 'limit'.
+
+    sql: SELECT * FROM person WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
+         SELECT * FROM person WHERE name=:name and age=:age limit 1 --> kwargs: {'name': '张三', 'age': 20}
+    """
+    sql, args = sql_support.try_mapping('sqlexec.select_one', sql, *args, **kwargs)
+    return do_select_one(sql, *args)
+
+
+def query(sql: str, *args, **kwargs):
+    """
+    Execute select SQL and return list results(dict).
+    sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
+         SELECT * FROM person WHERE name=:name and age=:age --> kwargs: {'name': '张三', 'age': 20}
+    """
+    sql, args = sql_support.try_mapping('sqlexec.query', sql, *args, **kwargs)
+    return do_query(sql, *args)
+
+
+def query_one(sql: str, *args, **kwargs):
+    """
+    execute select SQL and return unique result(dict), SQL contain 'limit'.
+
+    sql: SELECT * FROM person WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
+         SELECT * FROM person WHERE name=:name and age=:age limit 1 --> kwargs: {'name': '张三', 'age': 20}
+    """
+    sql, args = sql_support.try_mapping('sqlexec.query_one', sql, *args, **kwargs)
+    return do_query_one(sql, *args)
+
+
+def do_execute(sql: str, *args):
+    """
+    Execute sql return effect rowcount
+
+    sql: insert into person(name, age) values(?, ?)  -->  args: ('张三', 20)
+    """
+    sql = Dialect.before_execute(sql)
+    return _execute(sql, *args)
+
+
+def do_save_sql(sql: str, *args):
+    """
+    Insert data into table, return primary key.
+
+    :param select_key: sql for select primary key
+    :param sql: SQL
+    :param args:
+    :return: Primary key
+    """
+    try:
+        select_key = Dialect.get_select_key(sql=sql)
+    except NotImplementedError:
+        raise DBError(f"Expect 'select_key' but not. you may should use 'save_sql_select_key' func with 'select_key'.")
+    return do_save_sql_select_key(select_key, sql, *args)
+
+
+def do_save_sql_select_key(select_key: str, sql: str, *args):
+    """
+    Insert data into table, return primary key.
+
+    :param select_key: sql for select primary key
+    :param sql: SQL
+    :param args:
+    :return: Primary key
+    """
+    sql = Dialect.before_execute(sql)
+    return _save(select_key, sql, *args)
+
+
+def do_get(sql: str, *args):
+    """
+    Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
+    MultiColumnsError: Expect only one column.
+
+    sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+    """
+    sql, args = sql_support.limit_one_sql_args(sql, *args)
+    sql = Dialect.before_execute(sql)
+    return _get(sql, *args)
+
+
+def do_select(sql: str, *args):
+    """
+    execute select SQL and return unique result or list results(tuple).
+    sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
+    """
+    sql = Dialect.before_execute(sql)
+    return _select(sql, *args)
+
+
+def do_select_one(sql: str, *args):
+    """
+    Execute select SQL and return unique result(tuple), SQL contain 'limit'.
+    sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+    """
+    sql, args = sql_support.limit_one_sql_args(sql, *args)
+    sql = Dialect.before_execute(sql)
+    return _select_one(sql, *args)
+
+
+def do_query(sql: str, *args):
+    """
+    Execute select SQL and return list results(dict).
+    sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
+    """
+    sql = Dialect.before_execute(sql)
+    return _query(sql, *args)
+
+
+def do_query_one(sql: str, *args):
+    """
+    execute select SQL and return unique result(dict), SQL contain 'limit'.
+    sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+    """
+    sql, args = sql_support.limit_one_sql_args(sql, *args)
+    sql = Dialect.before_execute(sql)
+    return _query_one(sql, *args)
+
+
+def select_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
+    """
+    Execute select SQL and return list(tuple) or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
+    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+         SELECT * FROM user WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+    """
+    sql, args = sql_support.try_mapping('select_page', sql, *args, **kwargs)
+    return do_select_page(sql, page_num, page_size, *args)
+
+
+def query_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
+    """
+    Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
+    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+         SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+    """
+    sql, args = sql_support.try_mapping('query_page', sql, *args, **kwargs)
+    return do_query_page(sql, page_num, page_size, *args)
+
+
+def do_select_page(sql: str, page_num=1, page_size=10, *args):
+    """
+    Execute select SQL and return list results(dict).
+    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+    """
+    sql, args = Dialect.get_page_sql_args(sql, page_num, page_size, *args)
+    return do_select(sql, *args)
+
+
+def do_query_page(sql: str, page_num=1, page_size=10, *args):
+    """
+    Execute select SQL and return list results(dict).
+    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+    """
+    sql, args = Dialect.get_page_sql_args(sql, page_num, page_size, *args)
+    return do_query(sql, *args)
+
+
+def batch_execute(sql: str, *args):
+    """
+    Batch execute
+    :param sql: insert into person(name, age) values(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
+    :param args: All number must have same size.
+    :return: Effect row count
+    """
+    assert args, "*args must not be empty."
+    if isinstance(args[0], dict):
+        sql, args = sql_support.batch_named_sql_args(sql, *args)
+    sql = Dialect.before_execute(sql)
+    args = sql_support.get_batch_args(*args)
+    return _batch_execute(sql, *args)
+
+
+def batch_insert(table_name: str, *args):
+    """
+    Batch insert
+    :param table_name: table name
+    :param args: All number must have same key. [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
+    :return: Effect row count
+    """
+    logger.debug("Exec func 'sqlexec.%s' \n\t Table: '%s', args: %s" % ('batch_insert', table_name, args))
+    sql, args = sql_support.batch_insert_sql_args(table_name, *args)
+    return batch_execute(sql, *args)
+
+
+def load(sql: str, *args, **kwargs) -> Loader:
+    """
+    Execute select SQL and save a csv
+
+    sqlexec.load('select id, name, age from person WHERE name=:name', name='张三')
+
+    :param sql: SELECT * FROM person WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
+                SELECT * FROM person WHERE name=:name and age=:age limit 1 --> kwargs: {'name': '张三', 'age': 20}
+    :return: Loader
+    """
+    sql, args = sql_support.try_mapping('sqlexec.csv', sql, *args, **kwargs)
+    return do_load(sql, *args)
+
+
+def do_load(sql: str, *args) -> Loader:
+    """
+    Execute select SQL and save a csv
+
+    sqlexec.do_load('select id, name, age from person WHERE name = ?', '张三')
+
+    :param sql: SELECT * FROM person WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
+    :return: Loader
+    """
+    sql = Dialect.before_execute(sql)
+    return Loader(*_do_select(sql, *args))
+
+
+def insert_from_csv(file_name: str, table_name: str, delimiter=',', header=True, columns: Collection[str] = None, encoding='utf-8') -> int:
+    """
+    sqlexec.insert_from_csv('test.csv', 'person')
+    """
+    import csv
+    sql = None
+    if columns and len(columns) > 0:
+        sql = sql_support.insert_sql(table_name.strip(), columns)
+    elif not header:
+        raise ValueError("Expected one of 'header' and 'columns'.")
+
+    with open(file_name, newline='', encoding=encoding) as f:
+        lines = csv.reader(f, delimiter=delimiter)
+        lines = [line for line in lines]
+
+    if len(lines) == 0:
+        return 0
+
+    if header:
+        if len(lines) == 1:
+            return 0
+
+        if sql is None:
+            sql = sql_support.insert_sql(table_name.strip(), lines[0])
+        lines = lines[1:]
+
+    return batch_execute(sql, lines)
+
+
+def insert_from_df(df, table_name: str, columns: Collection[str] = None) -> int:
+    """
+    sqlexec.insert_from_df(df, 'person')
+    """
+    columns = columns if columns and len(columns) > 0 else df.columns.tolist()
+    sql = sql_support.insert_sql(table_name.strip(), columns)
+    return batch_execute(sql, df.values.tolist())
+
+
+def insert_from_json(file_name: str, table_name: str, encoding='utf-8') -> int:
+    """
+    sqlexec.insert_from_json('test.json', 'person')
+
+    many rows json file example:
+    [{"id": 1, "name": "张三", "age": 55}, ...]
+
+    one row json file example:
+    {"id": 1, "name": "张三", "age": 55}
+    """
+    import json
+
+    with open(file_name, encoding=encoding) as f:
+        data = json.load(f)
+
+    if isinstance(data, dict):
+        return insert(table_name, **data)
+    elif isinstance(data, Iterable):
+        return batch_insert(table_name, data)
+    else:
+        logger.info("Exec func 'sqlexec.%s' \n\t Table: '%s' insert 0 rows." % ('insert_from_json', table_name))
+        return 0
+
+
+def truncate_table(table_name: str) -> int:
+    """ sqlexec.truncate_table('person') """
+    return _execute(Dialect.get_truncate_sql(table_name))
+
+
+def drop_table(table_name: str) -> int:
+    """ sqlexec.drop_table('person') """
+    return _execute('DROP TABLE %s' % Dialect.get_dialect_str(table_name))
+
+
+def show_tables(schema: str = None):
+    if schema and Dialect.curr_engine() != Engine.SQLITE:
+        _execute('use %s' % schema)
+    return [table[0] for table in _select(Dialect.show_tables_sql())]
```

### Comparing `sqlx-exec-2.3.7/sqlexec/loader.py` & `sqlx-exec-2.3.8/sqlexec/loader.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-# !/usr/bin/env python3
-# -*- coding:utf-8 -*-
-
-from datetime import datetime, date
-
-
-class Loader:
-
-    def __init__(self, data, description):
-        self.data = data
-        self.description = description
-
-    def to_csv(self, file_name: str, delimiter=',', header=True, encoding='utf-8'):
-        """
-        Save as csv
-        :param file_name
-        :param delimiter
-        :param header bool, include header or not
-        :param encoding default utf-8
-        """
-        import csv
-        with open(file_name, 'w', newline='', encoding=encoding) as f:
-            writer = csv.writer(f, delimiter=delimiter)
-            if header and self.description:
-                description = [x[0] for x in self.description]
-                writer.writerow(description)
-            writer.writerows(self.data)
-
-    def to_df(self):
-        """
-        transform to DataFrame of pandas.
-        :return DataFrame of pandas
-        """
-        try:
-            import pandas as pd
-        except:
-            raise ModuleNotFoundError("No module named 'pandas', please install it use 'pip install pandas'")
-
-        if self.description:
-            description = [x[0] for x in self.description]
-            return pd.DataFrame(data=self.data, columns=description)
-        return pd.DataFrame(data=self.data)
-
-    def to_json(self, file_name: str, encoding='utf-8'):
-        """
-        Save as json
-        :param file_name
-        :param encoding default utf-8
-        """
-        import json
-        from executor import Dict
-
-        if self.data and self.description:
-            names = [x[0] for x in self.description]
-            data = list(map(lambda x: Dict(names, x), self.data))
-            with open(file_name, 'w', encoding=encoding) as f:
-                json.dump(data, f, default=_datetime_handler)
-
-
-def _datetime_handler(obj):
-    if isinstance(obj, datetime) or isinstance(obj, date):
-        return obj.__str__()
+# !/usr/bin/env python3
+# -*- coding:utf-8 -*-
+
+from datetime import datetime, date
+
+
+class Loader:
+
+    def __init__(self, data, description):
+        self.data = data
+        self.description = description
+
+    def to_csv(self, file_name: str, delimiter=',', header=True, encoding='utf-8'):
+        """
+        Save as csv
+        :param file_name
+        :param delimiter
+        :param header bool, include header or not
+        :param encoding default utf-8
+        """
+        import csv
+        with open(file_name, 'w', newline='', encoding=encoding) as f:
+            writer = csv.writer(f, delimiter=delimiter)
+            if header and self.description:
+                description = [x[0] for x in self.description]
+                writer.writerow(description)
+            writer.writerows(self.data)
+
+    def to_df(self):
+        """
+        transform to DataFrame of pandas.
+        :return DataFrame of pandas
+        """
+        try:
+            import pandas as pd
+        except:
+            raise ModuleNotFoundError("No module named 'pandas', please install it use 'pip install pandas'")
+
+        if self.description:
+            description = [x[0] for x in self.description]
+            return pd.DataFrame(data=self.data, columns=description)
+        return pd.DataFrame(data=self.data)
+
+    def to_json(self, file_name: str, encoding='utf-8'):
+        """
+        Save as json
+        :param file_name
+        :param encoding default utf-8
+        """
+        import json
+        from executor import Dict
+
+        if self.data and self.description:
+            names = [x[0] for x in self.description]
+            data = list(map(lambda x: Dict(names, x), self.data))
+            with open(file_name, 'w', encoding=encoding) as f:
+                json.dump(data, f, default=_datetime_handler)
+
+
+def _datetime_handler(obj):
+    if isinstance(obj, datetime) or isinstance(obj, date):
+        return obj.__str__()
```

### Comparing `sqlx-exec-2.3.7/sqlexec/log_support.py` & `sqlx-exec-2.3.8/sqlexec/log_support.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from executor.log_support import logger
-
-
-def insert_log(function: str, table: str, **kwargs):
-    logger.debug("Exec func 'sqlexec.%s' \n\t Table: '%s', kwargs: %s" % (function, table, kwargs))
-
-
-def save_log(function: str, select_key: str, table: str, **kwargs):
-    logger.debug("Exec func 'sqlexec.%s', 'select_key': %s \n\t Table: '%s', kwargs: %s" % (function, select_key, table, kwargs))
-
-
-def sql_log(function: str, sql: str, *args, **kwargs):
-    logger.debug("Exec func '%s' \n\tsql: %s \n\targs: %s \n\tkwargs: %s" % (function, sql.strip(), args, kwargs))
-
-
-def do_sql_log(function: str, sql: str, *args):
-    logger.debug("Exec func '%s' \n\t sql: %s \n\t args: %s" % (function, sql, args))
-
-
-def db_ctx_log(action, connection):
-    logger.debug("%s connection <%s>..." % (action, hex(id(connection))))
-
+from executor.log_support import logger
+
+
+def insert_log(function: str, table: str, **kwargs):
+    logger.debug("Exec func 'sqlexec.%s' \n\t Table: '%s', kwargs: %s" % (function, table, kwargs))
+
+
+def save_log(function: str, select_key: str, table: str, **kwargs):
+    logger.debug("Exec func 'sqlexec.%s', 'select_key': %s \n\t Table: '%s', kwargs: %s" % (function, select_key, table, kwargs))
+
+
+def sql_log(function: str, sql: str, *args, **kwargs):
+    logger.debug("Exec func '%s' \n\tsql: %s \n\targs: %s \n\tkwargs: %s" % (function, sql.strip(), args, kwargs))
+
+
+def do_sql_log(function: str, sql: str, *args):
+    logger.debug("Exec func '%s' \n\t sql: %s \n\t args: %s" % (function, sql, args))
+
+
+def db_ctx_log(action, connection):
+    logger.debug("%s connection <%s>..." % (action, hex(id(connection))))
+
```

### Comparing `sqlx-exec-2.3.7/sqlexec/page_exec.py` & `sqlx-exec-2.3.8/sqlexec/page_exec.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-# !/usr/bin/env python3
-# -*- coding:utf-8 -*-
-
-from . import exec
-
-
-class PageExec:
-
-    def __init__(self, _exec, page_num, page_size):
-        self.exec = _exec
-        self.page_num = page_num
-        self.page_size = page_size
-
-    def query(self, sql: str, *args, **kwargs):
-        """
-        Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
-        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-             SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
-        """
-        return self.exec.query_page(sql, self.page_num, self.page_size, *args, **kwargs)
-
-    def select(self, sql: str, *args, **kwargs):
-        """
-        Execute select SQL and return list(tuple) or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
-        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-             SELECT * FROM user WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
-        """
-        return self.exec.select_page(sql, self.page_num, self.page_size, *args, **kwargs)
-
-    def do_query(self, sql: str, *args):
-        """
-        Execute select SQL and return list results(dict).
-        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-        """
-        return self.exec.do_query_page(sql, self.page_num, self.page_size, *args)
-
-    def do_select(self, sql: str, *args):
-        """
-        Execute select SQL and return list results(dict).
-        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-        """
-        return self.exec.do_select_page(sql, self.page_num, self.page_size, *args)
-
-
-def page(page_num=1, page_size=10) -> PageExec:
-    return PageExec(exec, page_num, page_size)
-
-
-
-
+# !/usr/bin/env python3
+# -*- coding:utf-8 -*-
+
+from . import exec
+
+
+class PageExec:
+
+    def __init__(self, _exec, page_num, page_size):
+        self.exec = _exec
+        self.page_num = page_num
+        self.page_size = page_size
+
+    def query(self, sql: str, *args, **kwargs):
+        """
+        Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
+        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+             SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        """
+        return self.exec.query_page(sql, self.page_num, self.page_size, *args, **kwargs)
+
+    def select(self, sql: str, *args, **kwargs):
+        """
+        Execute select SQL and return list(tuple) or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
+        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+             SELECT * FROM user WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        """
+        return self.exec.select_page(sql, self.page_num, self.page_size, *args, **kwargs)
+
+    def do_query(self, sql: str, *args):
+        """
+        Execute select SQL and return list results(dict).
+        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+        """
+        return self.exec.do_query_page(sql, self.page_num, self.page_size, *args)
+
+    def do_select(self, sql: str, *args):
+        """
+        Execute select SQL and return list results(dict).
+        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+        """
+        return self.exec.do_select_page(sql, self.page_num, self.page_size, *args)
+
+
+def page(page_num=1, page_size=10) -> PageExec:
+    return PageExec(exec, page_num, page_size)
+
+
+
+
```

### Comparing `sqlx-exec-2.3.7/sqlexec/sql_exec.py` & `sqlx-exec-2.3.8/sqlexec/sql_exec.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,318 +1,318 @@
-# !/usr/bin/env python3
-# -*- coding:utf-8 -*-
-
-from . import exec
-from .loader import Loader
-from .page_exec import PageExec
-
-
-class SqlPageExec:
-
-    def __init__(self, sql: str, page_exec: PageExec):
-        self.sql = sql
-        self.page_exec = page_exec
-
-    def query(self, *args, **kwargs):
-        """
-        Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
-        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-             SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
-        """
-        return self.page_exec.query(self.sql, *args, **kwargs)
-
-    def select(self, *args, **kwargs):
-        """
-        Execute select SQL and return list(tuple) or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
-        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-             SELECT * FROM user WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
-        """
-        return self.page_exec.select(self.sql, *args, **kwargs)
-
-    def do_query(self, *args):
-        """
-        Execute select SQL and return list results(dict).
-        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-        """
-        return self.page_exec.do_query(self.sql, *args)
-
-    def do_select(self, *args):
-        """
-        Execute select SQL and return list results(dict).
-        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-        """
-        return self.page_exec.do_select(self.sql, *args)
-
-
-class ParamPageExec:
-
-    def __init__(self, sql_page_exec: SqlPageExec, *args, **kwargs):
-        self.sql_page_exec = sql_page_exec
-        self.args = args
-        self.kwargs = kwargs
-
-    def query(self):
-        return self.sql_page_exec.query(*self.args, **self.kwargs)
-
-    def select(self):
-        return self.sql_page_exec.select(*self.args, **self.kwargs)
-
-
-class Param:
-
-    def __init__(self, sql_exec, *args, **kwargs):
-        self.sql_exec = sql_exec
-        self.args = args
-        self.kwargs = kwargs
-
-    def execute(self) -> int:
-        """
-        sqlexec.sql('INSERT INTO person(name, age) VALUES(?, ?)').param('张三', 18).execute()
-        """
-        return self.sql_exec.execute(*self.args, **self.kwargs)
-
-    def save(self):
-        """
-        sqlexec.sql('INSERT INTO person(name, age) VALUES(?, ?)').param('张三', 18).save('SELECT LAST_INSERT_ID()')
-        """
-        return self.sql_exec.save(*self.args, **self.kwargs)
-
-    def save_select_key(self, select_key: str):
-        """
-        sqlexec.sql('INSERT INTO person(name, age) VALUES(?, ?)').param('张三', 18).save('SELECT LAST_INSERT_ID()')
-        """
-        return self.sql_exec.save_select_key(select_key, *self.args, **self.kwargs)
-
-    def get(self):
-        """
-        sqlexec.sql('SELECT count(1) FROM person WHERE name=? and age=? limit 1').param('张三', 18).get()
-        """
-        return self.sql_exec.get(*self.args, **self.kwargs)
-
-    def select(self):
-        """
-        sqlexec.sql('SELECT * FROM person WHERE name=? and age=?').param('张三', 18).select()
-        """
-        return self.sql_exec.select(*self.args, **self.kwargs)
-
-    def select_one(self):
-        """
-        sqlexec.sql('SELECT * FROM person WHERE name=? and age=? limit 1').param('张三', 18).select_one()
-        """
-        return self.sql_exec.select_one(*self.args, **self.kwargs)
-
-    def query(self):
-        """
-        sqlexec.sql('SELECT * FROM person WHERE name=? and age=?').param('张三', 18).query()
-        """
-        return self.sql_exec.query(*self.args, **self.kwargs)
-
-    def query_one(self):
-        """
-        sqlexec.sql('SELECT * FROM person WHERE name=? and age=? limit 1').param('张三', 18).query_one()
-        """
-        return self.sql_exec.query_one(*self.args, **self.kwargs)
-
-    def to_csv(self, file_name: str, delimiter=',', header=True, encoding='utf-8'):
-        """
-        sqlexec.sql('SELECT * FROM person WHERE name=? and age=?').param('张三', 18).to_csv('test.csv')
-        """
-        self.sql_exec.load(*self.args, **self.kwargs).to_csv(file_name, delimiter, header, encoding)
-
-    def to_df(self):
-        """
-        sqlexec.sql('SELECT * FROM person WHERE name=? and age=?').param('张三', 18).to_df()
-        """
-        return self.sql_exec.load(*self.args, **self.kwargs).to_df()
-
-    def to_json(self, file_name: str, encoding='utf-8'):
-        """
-        sqlexec.sql('SELECT * FROM person WHERE name=? and age=?').param('张三', 18).to_json('test.json')
-        """
-        self.sql_exec.load(*self.args, **self.kwargs).to_json(file_name, encoding)
-
-    def page(self, page_num=1, page_size=10) -> ParamPageExec:
-        return ParamPageExec(self.sql_exec.page(page_num, page_size), *self.args, **self.kwargs)
-
-
-class SqlExec:
-
-    def __init__(self, _exec, sql: str):
-        self.exec = _exec
-        self.sql = sql
-
-    def execute(self, *args, **kwargs) -> int:
-        """
-        Execute sql return effect rowcount
-
-        sql: INSERT INTO person(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
-             INSERT INTO person(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
-        """
-        return self.exec.execute(self.sql, *args, **kwargs)
-
-    def save(self, *args, **kwargs):
-        """
-        Insert data into table, return primary key.
-
-        :param select_key: sql for select primary key
-        :param args:
-        :return: Primary key
-        """
-        return self.exec.save_sql(self.sql, *args, **kwargs)
-
-    def save_select_key(self, select_key: str, *args, **kwargs):
-        """
-        Insert data into table, return primary key.
-
-        :param select_key: sql for select primary key
-        :param args:
-        :return: Primary key
-        """
-        return self.exec.save_sql_select_key(select_key, self.sql, *args, **kwargs)
-
-    def get(self, *args, **kwargs):
-        """
-        Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
-        MultiColumnsError: Expect only one column.
-
-        sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
-             SELECT count(1) FROM person WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
-        """
-        return self.exec.get(self.sql, *args, **kwargs)
-
-    def select(self, *args, **kwargs):
-        """
-        execute select SQL and return unique result or list results(tuple).
-
-        sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
-             SELECT * FROM person WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
-        """
-        return self.exec.select(self.sql, *args, **kwargs)
-
-    def select_one(self, *args, **kwargs):
-        """
-        Execute select SQL and return unique result(tuple), SQL contain 'limit'.
-
-        sql: SELECT * FROM person WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
-             SELECT * FROM person WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
-        """
-        return self.exec.select_one(self.sql, *args, **kwargs)
-
-    def query(self, *args, **kwargs):
-        """
-        Execute select SQL and return list results(dict).
-
-        sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
-             SELECT * FROM person WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
-        """
-        return self.exec.query(self.sql, *args, **kwargs)
-
-    def query_one(self, *args, **kwargs):
-        """
-        execute select SQL and return unique result(dict), SQL contain 'limit'.
-
-        sql: SELECT * FROM person WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
-             SELECT * FROM person WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
-        """
-        return self.exec.query_one(self.sql, *args, **kwargs)
-
-    def do_execute(self, *args):
-        """
-        Execute sql return effect rowcount
-
-        sql: insert into person(name, age) values(?, ?)  -->  args: ('张三', 20)
-        """
-        return self.exec.do_execute(None, self.sql, *args)
-
-    def do_save_sql(self, select_key: str, *args):
-        """
-        Insert data into table, return primary key.
-
-        :param select_key: sql for select primary key
-        :param args:
-        :return: Primary key
-        """
-        return self.exec.do_save_sql(select_key, self.sql, *args)
-
-    def do_get(self, *args):
-        """
-        Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
-        MultiColumnsError: Expect only one column.
-
-        sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
-        """
-        return self.exec.do_get(self.sql, *args)
-
-    def do_select(self, *args):
-        """
-        execute select SQL and return unique result or list results(tuple).
-
-        sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
-        """
-        return self.exec.do_select(self.sql, *args)
-
-    def do_select_one(self, *args):
-        """
-        Execute select SQL and return unique result(tuple), SQL contain 'limit'.
-
-        sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
-        """
-        return self.exec.do_select_one(self.sql, *args)
-
-    def do_query(self, *args):
-        """
-        Execute select SQL and return list results(dict).
-
-        sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
-        """
-        return self.exec.do_query(self.sql, *args)
-
-    def do_query_one(self, *args):
-        """
-        execute select SQL and return unique result(dict), SQL contain 'limit'.
-
-        sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
-        """
-        return self.exec.do_query_one(self.sql, *args)
-
-    def batch_execute(self, *args):
-        """
-        Batch execute sql return effect rowcount
-
-        sql: insert into person(name, age) values(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
-
-        :param args: All number must have same size.
-        :return: Effect rowcount
-        """
-        return self.exec.batch_execute(self.sql, *args)
-
-    def load(self, *args, **kwargs) -> Loader:
-        """
-        sqlexec.sql('select id, name, age from person WHERE name = :name').load(name='张三')
-        sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
-             SELECT * FROM person WHERE name = :name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
-        """
-        return self.exec.load(self.sql, *args, **kwargs)
-
-    def do_load(self, *args) -> Loader:
-        """
-        sqlexec.sql('select id, name, age from person WHERE name = ?').do_load('张三')
-        sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
-        """
-        return self.exec.do_load(self.sql, *args)
-
-    def param(self, *args, **kwargs) -> Param:
-        """
-        sqlexec.sql('select id, name, age from person WHERE name = :name').param(name='张三')
-        sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
-             SELECT * FROM person WHERE name = :name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
-        """
-        return Param(self, *args, **kwargs)
-
-    def page(self, page_num=1, page_size=10) -> SqlPageExec:
-        return SqlPageExec(self.sql, PageExec(self.exec, page_num=page_num, page_size=page_size))
-
-
-def sql(sql_text: str) -> SqlExec:
-    sql_text = sql_text.strip()
-    assert sql_text, "Parameter 'sql' must not be none"
-    return SqlExec(exec, sql_text)
+# !/usr/bin/env python3
+# -*- coding:utf-8 -*-
+
+from . import exec
+from .loader import Loader
+from .page_exec import PageExec
+
+
+class SqlPageExec:
+
+    def __init__(self, sql: str, page_exec: PageExec):
+        self.sql = sql
+        self.page_exec = page_exec
+
+    def query(self, *args, **kwargs):
+        """
+        Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
+        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+             SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        """
+        return self.page_exec.query(self.sql, *args, **kwargs)
+
+    def select(self, *args, **kwargs):
+        """
+        Execute select SQL and return list(tuple) or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
+        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+             SELECT * FROM user WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        """
+        return self.page_exec.select(self.sql, *args, **kwargs)
+
+    def do_query(self, *args):
+        """
+        Execute select SQL and return list results(dict).
+        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+        """
+        return self.page_exec.do_query(self.sql, *args)
+
+    def do_select(self, *args):
+        """
+        Execute select SQL and return list results(dict).
+        sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+        """
+        return self.page_exec.do_select(self.sql, *args)
+
+
+class ParamPageExec:
+
+    def __init__(self, sql_page_exec: SqlPageExec, *args, **kwargs):
+        self.sql_page_exec = sql_page_exec
+        self.args = args
+        self.kwargs = kwargs
+
+    def query(self):
+        return self.sql_page_exec.query(*self.args, **self.kwargs)
+
+    def select(self):
+        return self.sql_page_exec.select(*self.args, **self.kwargs)
+
+
+class Param:
+
+    def __init__(self, sql_exec, *args, **kwargs):
+        self.sql_exec = sql_exec
+        self.args = args
+        self.kwargs = kwargs
+
+    def execute(self) -> int:
+        """
+        sqlexec.sql('INSERT INTO person(name, age) VALUES(?, ?)').param('张三', 18).execute()
+        """
+        return self.sql_exec.execute(*self.args, **self.kwargs)
+
+    def save(self):
+        """
+        sqlexec.sql('INSERT INTO person(name, age) VALUES(?, ?)').param('张三', 18).save('SELECT LAST_INSERT_ID()')
+        """
+        return self.sql_exec.save(*self.args, **self.kwargs)
+
+    def save_select_key(self, select_key: str):
+        """
+        sqlexec.sql('INSERT INTO person(name, age) VALUES(?, ?)').param('张三', 18).save('SELECT LAST_INSERT_ID()')
+        """
+        return self.sql_exec.save_select_key(select_key, *self.args, **self.kwargs)
+
+    def get(self):
+        """
+        sqlexec.sql('SELECT count(1) FROM person WHERE name=? and age=? limit 1').param('张三', 18).get()
+        """
+        return self.sql_exec.get(*self.args, **self.kwargs)
+
+    def select(self):
+        """
+        sqlexec.sql('SELECT * FROM person WHERE name=? and age=?').param('张三', 18).select()
+        """
+        return self.sql_exec.select(*self.args, **self.kwargs)
+
+    def select_one(self):
+        """
+        sqlexec.sql('SELECT * FROM person WHERE name=? and age=? limit 1').param('张三', 18).select_one()
+        """
+        return self.sql_exec.select_one(*self.args, **self.kwargs)
+
+    def query(self):
+        """
+        sqlexec.sql('SELECT * FROM person WHERE name=? and age=?').param('张三', 18).query()
+        """
+        return self.sql_exec.query(*self.args, **self.kwargs)
+
+    def query_one(self):
+        """
+        sqlexec.sql('SELECT * FROM person WHERE name=? and age=? limit 1').param('张三', 18).query_one()
+        """
+        return self.sql_exec.query_one(*self.args, **self.kwargs)
+
+    def to_csv(self, file_name: str, delimiter=',', header=True, encoding='utf-8'):
+        """
+        sqlexec.sql('SELECT * FROM person WHERE name=? and age=?').param('张三', 18).to_csv('test.csv')
+        """
+        self.sql_exec.load(*self.args, **self.kwargs).to_csv(file_name, delimiter, header, encoding)
+
+    def to_df(self):
+        """
+        sqlexec.sql('SELECT * FROM person WHERE name=? and age=?').param('张三', 18).to_df()
+        """
+        return self.sql_exec.load(*self.args, **self.kwargs).to_df()
+
+    def to_json(self, file_name: str, encoding='utf-8'):
+        """
+        sqlexec.sql('SELECT * FROM person WHERE name=? and age=?').param('张三', 18).to_json('test.json')
+        """
+        self.sql_exec.load(*self.args, **self.kwargs).to_json(file_name, encoding)
+
+    def page(self, page_num=1, page_size=10) -> ParamPageExec:
+        return ParamPageExec(self.sql_exec.page(page_num, page_size), *self.args, **self.kwargs)
+
+
+class SqlExec:
+
+    def __init__(self, _exec, sql: str):
+        self.exec = _exec
+        self.sql = sql
+
+    def execute(self, *args, **kwargs) -> int:
+        """
+        Execute sql return effect rowcount
+
+        sql: INSERT INTO person(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
+             INSERT INTO person(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
+        """
+        return self.exec.execute(self.sql, *args, **kwargs)
+
+    def save(self, *args, **kwargs):
+        """
+        Insert data into table, return primary key.
+
+        :param select_key: sql for select primary key
+        :param args:
+        :return: Primary key
+        """
+        return self.exec.save_sql(self.sql, *args, **kwargs)
+
+    def save_select_key(self, select_key: str, *args, **kwargs):
+        """
+        Insert data into table, return primary key.
+
+        :param select_key: sql for select primary key
+        :param args:
+        :return: Primary key
+        """
+        return self.exec.save_sql_select_key(select_key, self.sql, *args, **kwargs)
+
+    def get(self, *args, **kwargs):
+        """
+        Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
+        MultiColumnsError: Expect only one column.
+
+        sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+             SELECT count(1) FROM person WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        """
+        return self.exec.get(self.sql, *args, **kwargs)
+
+    def select(self, *args, **kwargs):
+        """
+        execute select SQL and return unique result or list results(tuple).
+
+        sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
+             SELECT * FROM person WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        """
+        return self.exec.select(self.sql, *args, **kwargs)
+
+    def select_one(self, *args, **kwargs):
+        """
+        Execute select SQL and return unique result(tuple), SQL contain 'limit'.
+
+        sql: SELECT * FROM person WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
+             SELECT * FROM person WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        """
+        return self.exec.select_one(self.sql, *args, **kwargs)
+
+    def query(self, *args, **kwargs):
+        """
+        Execute select SQL and return list results(dict).
+
+        sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
+             SELECT * FROM person WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        """
+        return self.exec.query(self.sql, *args, **kwargs)
+
+    def query_one(self, *args, **kwargs):
+        """
+        execute select SQL and return unique result(dict), SQL contain 'limit'.
+
+        sql: SELECT * FROM person WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
+             SELECT * FROM person WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        """
+        return self.exec.query_one(self.sql, *args, **kwargs)
+
+    def do_execute(self, *args):
+        """
+        Execute sql return effect rowcount
+
+        sql: insert into person(name, age) values(?, ?)  -->  args: ('张三', 20)
+        """
+        return self.exec.do_execute(None, self.sql, *args)
+
+    def do_save_sql(self, select_key: str, *args):
+        """
+        Insert data into table, return primary key.
+
+        :param select_key: sql for select primary key
+        :param args:
+        :return: Primary key
+        """
+        return self.exec.do_save_sql(select_key, self.sql, *args)
+
+    def do_get(self, *args):
+        """
+        Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
+        MultiColumnsError: Expect only one column.
+
+        sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+        """
+        return self.exec.do_get(self.sql, *args)
+
+    def do_select(self, *args):
+        """
+        execute select SQL and return unique result or list results(tuple).
+
+        sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
+        """
+        return self.exec.do_select(self.sql, *args)
+
+    def do_select_one(self, *args):
+        """
+        Execute select SQL and return unique result(tuple), SQL contain 'limit'.
+
+        sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+        """
+        return self.exec.do_select_one(self.sql, *args)
+
+    def do_query(self, *args):
+        """
+        Execute select SQL and return list results(dict).
+
+        sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
+        """
+        return self.exec.do_query(self.sql, *args)
+
+    def do_query_one(self, *args):
+        """
+        execute select SQL and return unique result(dict), SQL contain 'limit'.
+
+        sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+        """
+        return self.exec.do_query_one(self.sql, *args)
+
+    def batch_execute(self, *args):
+        """
+        Batch execute sql return effect rowcount
+
+        sql: insert into person(name, age) values(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
+
+        :param args: All number must have same size.
+        :return: Effect rowcount
+        """
+        return self.exec.batch_execute(self.sql, *args)
+
+    def load(self, *args, **kwargs) -> Loader:
+        """
+        sqlexec.sql('select id, name, age from person WHERE name = :name').load(name='张三')
+        sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
+             SELECT * FROM person WHERE name = :name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        """
+        return self.exec.load(self.sql, *args, **kwargs)
+
+    def do_load(self, *args) -> Loader:
+        """
+        sqlexec.sql('select id, name, age from person WHERE name = ?').do_load('张三')
+        sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
+        """
+        return self.exec.do_load(self.sql, *args)
+
+    def param(self, *args, **kwargs) -> Param:
+        """
+        sqlexec.sql('select id, name, age from person WHERE name = :name').param(name='张三')
+        sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
+             SELECT * FROM person WHERE name = :name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+        """
+        return Param(self, *args, **kwargs)
+
+    def page(self, page_num=1, page_size=10) -> SqlPageExec:
+        return SqlPageExec(self.sql, PageExec(self.exec, page_num=page_num, page_size=page_size))
+
+
+def sql(sql_text: str) -> SqlExec:
+    sql_text = sql_text.strip()
+    assert sql_text, "Parameter 'sql' must not be none"
+    return SqlExec(exec, sql_text)
```

### Comparing `sqlx-exec-2.3.7/sqlexec/sql_support.py` & `sqlx-exec-2.3.8/sqlexec/sql_support.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-import re
-from executor import DBError
-from .dialect import Dialect
-from functools import lru_cache
-from .log_support import sql_log
-from executor.sql_support import require_limit
-from typing import Collection, Union, List, Tuple
-from .constant import CACHE_SIZE, NAMED_REGEX, LIMIT_1
-
-
-def limit_one_sql_args(sql: str, *args):
-    if require_limit(sql):
-        return '{} LIMIT ?'.format(sql), [*args, LIMIT_1]
-    return sql, args
-
-
-def insert_sql(table: str, cols: Collection[str]):
-    cols = cols if isinstance(cols, tuple) else tuple(cols)
-    return Dialect.create_insert_sql(table, cols)
-
-
-def insert_sql_args(table: str, **kwargs):
-    cols, args = zip(*kwargs.items())
-    sql = Dialect.create_insert_sql(table, cols)
-    return sql, args
-
-
-def get_batch_args(*args):
-    return args[0] if isinstance(args, tuple) and len(args) == 1 and isinstance(args[0], Collection) else args
-
-
-def batch_insert_sql_args(table: str, *args):
-    args = get_batch_args(*args)
-    args = [zip(*arg.items()) for arg in args]  # [(cols, args)]
-    cols, args = zip(*args)  # (cols), (args)
-    sql = Dialect.create_insert_sql(table, cols[0])
-    return sql, args
-
-
-def batch_named_sql_args(sql: str, *args):
-    args = get_batch_args(*args)
-    args = [get_named_args(sql, **arg) for arg in args]
-    sql = get_named_sql(sql)
-    return sql, args
-
-
-@lru_cache(maxsize=CACHE_SIZE)
-def get_named_sql(sql: str):
-    return re.sub(NAMED_REGEX, '?', sql)
-
-
-def get_named_args(sql: str, **kwargs):
-    return [kwargs[r[1:]] for r in re.findall(NAMED_REGEX, sql)]
-
-
-def get_named_sql_args(sql: str, **kwargs):
-    args = get_named_args(sql, **kwargs)
-    return get_named_sql(sql), args
-
-
-def is_mapping(sql: str):
-    return ':' in sql
-
-
-def is_placeholder(sql: str):
-    return '?' in sql
-
-
-def get_mapping_sql_args(sql: str, *args, **kwargs):
-    if is_mapping(sql):
-        assert kwargs, "Named mapping SQL expect '**kwargs' should not be empty."
-        return get_named_sql_args(sql, **kwargs)
-
-    if is_placeholder(sql) and not args:
-        raise DBError("Placeholder sql expect '*args' should not be empty.")
-
-    return sql, args
-
-
-def try_mapping(function, sql, *args, **kwargs):
-    sql_log(function, sql, *args, **kwargs)
-    return get_mapping_sql_args(sql, *args, **kwargs)
-
-
-def get_table_select_sql(table_name: str, where: str, limit: Union[int, Tuple[int], List[int]], *columns):
-    columns = Dialect.get_dialect_str(columns) if columns else Dialect.get_table_columns(table_name)
-    table_name = Dialect.get_dialect_str(table_name)
-    if limit:
-        if isinstance(limit, int):
-            return 'SELECT {} FROM {} {} LIMIT ?'.format(columns, table_name, where)
-        elif (isinstance(limit, Tuple) or isinstance(limit, List)) and len(limit) == 2:
-            return 'SELECT {} FROM {} {} LIMIT ? OFFSET ?'.format(columns, table_name, where)
-        else:
-            raise ValueError("The type of the parameter 'limit' must be 'int' or tuple, list, and it length is 2.")
-    else:
-        return 'SELECT {} FROM {} {}'.format(columns, table_name, where)
+import re
+from executor import DBError
+from .dialect import Dialect
+from functools import lru_cache
+from .log_support import sql_log
+from executor.sql_support import require_limit
+from typing import Collection, Union, List, Tuple
+from .constant import CACHE_SIZE, NAMED_REGEX, LIMIT_1
+
+
+def limit_one_sql_args(sql: str, *args):
+    if require_limit(sql):
+        return '{} LIMIT ?'.format(sql), [*args, LIMIT_1]
+    return sql, args
+
+
+def insert_sql(table: str, cols: Collection[str]):
+    cols = cols if isinstance(cols, tuple) else tuple(cols)
+    return Dialect.create_insert_sql(table, cols)
+
+
+def insert_sql_args(table: str, **kwargs):
+    cols, args = zip(*kwargs.items())
+    sql = Dialect.create_insert_sql(table, cols)
+    return sql, args
+
+
+def get_batch_args(*args):
+    return args[0] if isinstance(args, tuple) and len(args) == 1 and isinstance(args[0], Collection) else args
+
+
+def batch_insert_sql_args(table: str, *args):
+    args = get_batch_args(*args)
+    args = [zip(*arg.items()) for arg in args]  # [(cols, args)]
+    cols, args = zip(*args)  # (cols), (args)
+    sql = Dialect.create_insert_sql(table, cols[0])
+    return sql, args
+
+
+def batch_named_sql_args(sql: str, *args):
+    args = get_batch_args(*args)
+    args = [get_named_args(sql, **arg) for arg in args]
+    sql = get_named_sql(sql)
+    return sql, args
+
+
+@lru_cache(maxsize=CACHE_SIZE)
+def get_named_sql(sql: str):
+    return re.sub(NAMED_REGEX, '?', sql)
+
+
+def get_named_args(sql: str, **kwargs):
+    return [kwargs[r[1:]] for r in re.findall(NAMED_REGEX, sql)]
+
+
+def get_named_sql_args(sql: str, **kwargs):
+    args = get_named_args(sql, **kwargs)
+    return get_named_sql(sql), args
+
+
+def is_mapping(sql: str):
+    return ':' in sql
+
+
+def is_placeholder(sql: str):
+    return '?' in sql
+
+
+def get_mapping_sql_args(sql: str, *args, **kwargs):
+    if is_mapping(sql):
+        assert kwargs, "Named mapping SQL expect '**kwargs' should not be empty."
+        return get_named_sql_args(sql, **kwargs)
+
+    if is_placeholder(sql) and not args:
+        raise DBError("Placeholder sql expect '*args' should not be empty.")
+
+    return sql, args
+
+
+def try_mapping(function, sql, *args, **kwargs):
+    sql_log(function, sql, *args, **kwargs)
+    return get_mapping_sql_args(sql, *args, **kwargs)
+
+
+def get_table_select_sql(table_name: str, where: str, limit: Union[int, Tuple[int], List[int]], *columns):
+    columns = Dialect.get_dialect_str(columns) if columns else Dialect.get_table_columns(table_name)
+    table_name = Dialect.get_dialect_str(table_name)
+    if limit:
+        if isinstance(limit, int):
+            return 'SELECT {} FROM {} {} LIMIT ?'.format(columns, table_name, where)
+        elif (isinstance(limit, Tuple) or isinstance(limit, List)) and len(limit) == 2:
+            return 'SELECT {} FROM {} {} LIMIT ? OFFSET ?'.format(columns, table_name, where)
+        else:
+            raise ValueError("The type of the parameter 'limit' must be 'int' or tuple, list, and it length is 2.")
+    else:
+        return 'SELECT {} FROM {} {}'.format(columns, table_name, where)
```

### Comparing `sqlx-exec-2.3.7/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-2.3.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,200 +1,200 @@
-Metadata-Version: 2.1
-Name: sqlx-exec
-Version: 2.3.7
-Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions. Support MySQL, PostgreSQL, SQLite etc.
-Home-page: https://gitee.com/summry/sqlx-exec
-Author: summy
-Author-email: xiazhongbiao@126.com
-License: UNKNOWN
-Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python,RDB
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-Usage Sample
-''''''''''''
-
-.. code:: python
-
-       import sqlexec as db
-
-       if __name__ == '__main__':
-           db.init('test.db', driver='sqlite3', show_sql=True, debug=True)
-
-           # or
-           db.init("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
-
-           # or
-           db.init(host='127.0.0.1', port='5432', user='xxx', password='xxx', database='testdb', show_sql=True, driver='psycopg2')
-
-           effected_rowcount = db.insert(table='person', name='zhangsan', age=15)
-
-           # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
-           select_key = "SELECT currval('person_id_seq')"
-
-           id = db.save(select_key=select_key, table='person', name='lisi', age=26)
-
-           id = db.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(?,?)', 'wangwu', 38)
-
-           id = db.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(:name, :age)', name='zhaoliu', age=45)
-
-           count = db.get('select count(1) from person')
-           # result: 4
-
-           count = db.sql('select count(1) from person').get()
-           # result: 4
-
-           persons = db.select('select id, name, age from person')
-           # result:
-           # (3, 'zhangsan', 15)
-           # (4, 'lisi', 26)
-           # (5, 'wangwu', 38)
-           # (6, 'zhaoliu', 45)
-
-           persons = db.sql('select id, name, age from person').select()
-           # result:
-           # (3, 'zhangsan', 15)
-           # (4, 'lisi', 26)
-           # (5, 'wangwu', 38)
-           # (6, 'zhaoliu', 45)
-
-           persons = db.table('person').select('id', 'name', 'age')
-           # result:
-           # (3, 'zhangsan', 15)
-           # (4, 'lisi', 26)
-           # (5, 'wangwu', 38)
-           # (6, 'zhaoliu', 45)
-
-           persons = db.select_one('select id, name, age from person where name = ?', 'zhangsan')
-           # result:
-           # (3, 'zhangsan', 15)
-
-           persons = db.sql('select id, name, age from person where name = ?').select_one('zhangsan')
-           # result:
-           # (3, 'zhangsan', 15)
-
-           persons = db.select('select id, name, age from person where name = :name', name='zhangsan')
-           # result:
-           # [(3, 'zhangsan', 15)]
-
-           persons = db.sql('select id, name, age from person where name = :name').select(name='zhangsan')
-           # result:
-           # [(3, 'zhangsan', 15)]
-
-           persons = db.sql('select id, name, age from person where name = :name').param(name='zhangsan').select()
-           # result:
-           # [(3, 'zhangsan', 15)]
-
-           persons = db.table('person').where(name__eq='zhangsan').select('id', 'name', 'age')
-           # result:
-           # [(3, 'zhangsan', 15)]
-
-           persons = db.query('select id, name, age from person')
-           # result:
-           # {'id': 3, 'name': 'zhangsan', 'age': 15}
-           # {'id': 4, 'name': 'lisi', 'age': 26}
-           # {'id': 5, 'name': 'wangwu', 'age': 38}
-           # {'id': 6, 'name': 'zhaoliu', 'age': 45}
-
-           persons = db.sql('select id, name, age from person').query()
-           # result:
-           # {'id': 3, 'name': 'zhangsan', 'age': 15}
-           # {'id': 4, 'name': 'lisi', 'age': 26}
-           # {'id': 5, 'name': 'wangwu', 'age': 38}
-           # {'id': 6, 'name': 'zhaoliu', 'age': 45}
-
-           persons = db.query_one('select id, name, age from person where name = ?', 'zhangsan')
-           # result:
-           # {'id': 3, 'name': 'zhangsan', 'age': 15}
-
-           persons = db.sql('select id, name, age from person where name = ?').query_one('zhangsan')
-           # result:
-           # {'id': 3, 'name': 'zhangsan', 'age': 15}
-
-           persons = db.query('select id, name, age from person where name = :name', name='zhangsan')
-           # result:
-           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
-
-           persons = db.sql('select id, name, age from person where name = :name').query(name='zhangsan')
-           # result:
-           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
-
-           persons = db.sql('select id, name, age from person where name = :name').param(name='zhangsan').query()
-           # result:
-           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
-
-           persons = db.table('person').columns('id', 'name', 'age').where(name='zhangsan').query()
-           # result:
-           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
-
-           effected_rowcount = db.table('person').where(name='zhangsan').update(name='xxx', age=45)
-
-           effected_rowcount = db.table('person').where(id=6).delete()
-           count = db.table('person').count())
-           # result: 3
-
-           effected_rowcount = db.execute('delete from person where id = :id', id=5)
-           count = db.get('select count(1) from person')
-           # result: 2
-
-           effected_rowcount = db.sql('delete from person where id = ?').execute(4)
-           count = db.sql('select count(1) from person').get()
-           # result: 1
-
-           effected_rowcount = db.sql('delete from person where id = :id').execute(id=3)
-           count = db.sql('select count(1) from person').get()
-           # result: 0
-
-           # select data save as csv
-           db.sql('select name, age from person WHERE name = ?').load('张三').to_csv('test.csv')
-
-           db.sql('select name, age from person WHERE name = ?').param('张三').to_csv('test.csv')
-
-           # insert from csv
-           db.table('person').insert_from_csv('test.csv')
-
-           # select data transform to DataFrame of pandas
-           df = db.sql('select name, age from person WHERE name = :name').load(name='张三').to_df()
-
-           df = db.sql('select name, age from person WHERE name = :name').param(name='张三').to_df()
-
-           # insert from DataFrame of pandas
-           db.table('person').insert_from_df(dataframe)
-
-           # select data save as json
-           db.sql('select name, age from person WHERE name = ?').load('张三').to_json('test.json')
-
-           db.sql('select name, age from person WHERE name = ?').param('张三').to_json('test.json')
-
-           # insert from json
-           db.table('person').insert_from_json('test.json')
-
-           db.close()
-
-Transaction
-'''''''''''
-
-.. code:: python
-
-       from sqlexec import with_transaction, transaction
-
-       @with_transaction
-       def test_transaction():
-           insert_func(....)
-           update_func(....)
-
-
-       def test_transaction2():
-           with transaction():
-               insert_func(....)
-               update_func(....)
-
-
-If you want to operate MySQL database like Mybatis, may be you need MySqlx: https://pypi.org/project/mysqlx
-
-If you want to operate PostgreSQL database like Mybatis, may be you need PgSqlx: https://pypi.org/project/pgsqlx
-
-If you want to execute SQL like Mybatis, may be you need sqlx-batis: https://pypi.org/project/sqlx-batis
-
-
+Metadata-Version: 2.1
+Name: sqlx-exec
+Version: 2.3.8
+Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions. Support MySQL, PostgreSQL, SQLite etc.
+Home-page: https://gitee.com/summry/sqlx-exec
+Author: summy
+Author-email: xiazhongbiao@126.com
+License: UNKNOWN
+Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python,RDB
+Platform: UNKNOWN
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Usage Sample
+''''''''''''
+
+.. code:: python
+
+       import sqlexec as db
+
+       if __name__ == '__main__':
+           db.init('test.db', driver='sqlite3', show_sql=True, debug=True)
+
+           # or
+           db.init("postgres://user:password@127.0.0.1:5432/testdb", driver='psycopg2', pool_size=5, show_sql=True, debug=True)
+
+           # or
+           db.init(host='127.0.0.1', port='5432', user='xxx', password='xxx', database='testdb', show_sql=True, driver='psycopg2')
+
+           effected_rowcount = db.insert(table='person', name='zhangsan', age=15)
+
+           # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
+           select_key = "SELECT currval('person_id_seq')"
+
+           id = db.save(select_key=select_key, table='person', name='lisi', age=26)
+
+           id = db.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(?,?)', 'wangwu', 38)
+
+           id = db.save_sql(select_key, 'INSERT INTO person(name, age) VALUES(:name, :age)', name='zhaoliu', age=45)
+
+           count = db.get('select count(1) from person')
+           # result: 4
+
+           count = db.sql('select count(1) from person').get()
+           # result: 4
+
+           persons = db.select('select id, name, age from person')
+           # result:
+           # (3, 'zhangsan', 15)
+           # (4, 'lisi', 26)
+           # (5, 'wangwu', 38)
+           # (6, 'zhaoliu', 45)
+
+           persons = db.sql('select id, name, age from person').select()
+           # result:
+           # (3, 'zhangsan', 15)
+           # (4, 'lisi', 26)
+           # (5, 'wangwu', 38)
+           # (6, 'zhaoliu', 45)
+
+           persons = db.table('person').select('id', 'name', 'age')
+           # result:
+           # (3, 'zhangsan', 15)
+           # (4, 'lisi', 26)
+           # (5, 'wangwu', 38)
+           # (6, 'zhaoliu', 45)
+
+           persons = db.select_one('select id, name, age from person where name = ?', 'zhangsan')
+           # result:
+           # (3, 'zhangsan', 15)
+
+           persons = db.sql('select id, name, age from person where name = ?').select_one('zhangsan')
+           # result:
+           # (3, 'zhangsan', 15)
+
+           persons = db.select('select id, name, age from person where name = :name', name='zhangsan')
+           # result:
+           # [(3, 'zhangsan', 15)]
+
+           persons = db.sql('select id, name, age from person where name = :name').select(name='zhangsan')
+           # result:
+           # [(3, 'zhangsan', 15)]
+
+           persons = db.sql('select id, name, age from person where name = :name').param(name='zhangsan').select()
+           # result:
+           # [(3, 'zhangsan', 15)]
+
+           persons = db.table('person').where(name__eq='zhangsan').select('id', 'name', 'age')
+           # result:
+           # [(3, 'zhangsan', 15)]
+
+           persons = db.query('select id, name, age from person')
+           # result:
+           # {'id': 3, 'name': 'zhangsan', 'age': 15}
+           # {'id': 4, 'name': 'lisi', 'age': 26}
+           # {'id': 5, 'name': 'wangwu', 'age': 38}
+           # {'id': 6, 'name': 'zhaoliu', 'age': 45}
+
+           persons = db.sql('select id, name, age from person').query()
+           # result:
+           # {'id': 3, 'name': 'zhangsan', 'age': 15}
+           # {'id': 4, 'name': 'lisi', 'age': 26}
+           # {'id': 5, 'name': 'wangwu', 'age': 38}
+           # {'id': 6, 'name': 'zhaoliu', 'age': 45}
+
+           persons = db.query_one('select id, name, age from person where name = ?', 'zhangsan')
+           # result:
+           # {'id': 3, 'name': 'zhangsan', 'age': 15}
+
+           persons = db.sql('select id, name, age from person where name = ?').query_one('zhangsan')
+           # result:
+           # {'id': 3, 'name': 'zhangsan', 'age': 15}
+
+           persons = db.query('select id, name, age from person where name = :name', name='zhangsan')
+           # result:
+           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+
+           persons = db.sql('select id, name, age from person where name = :name').query(name='zhangsan')
+           # result:
+           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+
+           persons = db.sql('select id, name, age from person where name = :name').param(name='zhangsan').query()
+           # result:
+           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+
+           persons = db.table('person').columns('id', 'name', 'age').where(name='zhangsan').query()
+           # result:
+           # [{'id': 3, 'name': 'zhangsan', 'age': 15}]
+
+           effected_rowcount = db.table('person').where(name='zhangsan').update(name='xxx', age=45)
+
+           effected_rowcount = db.table('person').where(id=6).delete()
+           count = db.table('person').count())
+           # result: 3
+
+           effected_rowcount = db.execute('delete from person where id = :id', id=5)
+           count = db.get('select count(1) from person')
+           # result: 2
+
+           effected_rowcount = db.sql('delete from person where id = ?').execute(4)
+           count = db.sql('select count(1) from person').get()
+           # result: 1
+
+           effected_rowcount = db.sql('delete from person where id = :id').execute(id=3)
+           count = db.sql('select count(1) from person').get()
+           # result: 0
+
+           # select data save as csv
+           db.sql('select name, age from person WHERE name = ?').load('张三').to_csv('test.csv')
+
+           db.sql('select name, age from person WHERE name = ?').param('张三').to_csv('test.csv')
+
+           # insert from csv
+           db.table('person').insert_from_csv('test.csv')
+
+           # select data transform to DataFrame of pandas
+           df = db.sql('select name, age from person WHERE name = :name').load(name='张三').to_df()
+
+           df = db.sql('select name, age from person WHERE name = :name').param(name='张三').to_df()
+
+           # insert from DataFrame of pandas
+           db.table('person').insert_from_df(dataframe)
+
+           # select data save as json
+           db.sql('select name, age from person WHERE name = ?').load('张三').to_json('test.json')
+
+           db.sql('select name, age from person WHERE name = ?').param('张三').to_json('test.json')
+
+           # insert from json
+           db.table('person').insert_from_json('test.json')
+
+           db.close()
+
+Transaction
+'''''''''''
+
+.. code:: python
+
+       from sqlexec import with_transaction, transaction
+
+       @with_transaction
+       def test_transaction():
+           insert_func(....)
+           update_func(....)
+
+
+       def test_transaction2():
+           with transaction():
+               insert_func(....)
+               update_func(....)
+
+
+If you want to operate MySQL database like Mybatis, may be you need MySqlx: https://pypi.org/project/mysqlx
+
+If you want to operate PostgreSQL database like Mybatis, may be you need PgSqlx: https://pypi.org/project/pgsqlx
+
+If you want to execute SQL like Mybatis, may be you need sqlx-batis: https://pypi.org/project/sqlx-batis
+
+
```

### Comparing `sqlx-exec-2.3.7/test/test.py` & `sqlx-exec-2.3.8/test/test.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from typing import Collection, Sequence, Union
-
-t = ('1', '2')
-print(isinstance(t, Collection), isinstance(t, Sequence))
-# True True
-l = ['1', '2']
-print(isinstance(l, Collection), isinstance(l, Sequence))
-# True True
-s = set(l)
-print(isinstance(s, Collection), isinstance(s, Sequence))
-# True False
-s = 'hello'
-print(isinstance(s, Collection), isinstance(s, Sequence))
-# True True
-
-
-def get_dialect_str(src: Union[str, Collection[str]]):
-    return src.strip() if isinstance(src, str) else ','.join([s.strip() for s in src])
-
-
-def _dialect_str(src: str):
-    assert isinstance(src, str), 'source must be a string.'
-    if ',' in src:
-        return ','.join(['`{}`'.format(s.strip()) for s in src.split(',')])
-    elif '(' in src:
-        return src.strip()
-    else:
-        return '`{}`'.format(src.strip())
-
-
-def get_mysql_dialect_str(src: Union[str, Collection[str]]):
-    assert src, 'src string is required.'
-    if isinstance(src, str):
-        return _dialect_str(src)
-    return ','.join([_dialect_str(arg) for arg in src])
-
-
-if __name__ == '__main__':
-    # names = 'person'
-    names = ['id', 'name, age']
-    print(get_dialect_str(names))
-    print(get_mysql_dialect_str(names))
+from typing import Collection, Sequence, Union
+
+t = ('1', '2')
+print(isinstance(t, Collection), isinstance(t, Sequence))
+# True True
+l = ['1', '2']
+print(isinstance(l, Collection), isinstance(l, Sequence))
+# True True
+s = set(l)
+print(isinstance(s, Collection), isinstance(s, Sequence))
+# True False
+s = 'hello'
+print(isinstance(s, Collection), isinstance(s, Sequence))
+# True True
+
+
+def get_dialect_str(src: Union[str, Collection[str]]):
+    return src.strip() if isinstance(src, str) else ','.join([s.strip() for s in src])
+
+
+def _dialect_str(src: str):
+    assert isinstance(src, str), 'source must be a string.'
+    if ',' in src:
+        return ','.join(['`{}`'.format(s.strip()) for s in src.split(',')])
+    elif '(' in src:
+        return src.strip()
+    else:
+        return '`{}`'.format(src.strip())
+
+
+def get_mysql_dialect_str(src: Union[str, Collection[str]]):
+    assert src, 'src string is required.'
+    if isinstance(src, str):
+        return _dialect_str(src)
+    return ','.join([_dialect_str(arg) for arg in src])
+
+
+if __name__ == '__main__':
+    # names = 'person'
+    names = ['id', 'name, age']
+    print(get_dialect_str(names))
+    print(get_mysql_dialect_str(names))
```

