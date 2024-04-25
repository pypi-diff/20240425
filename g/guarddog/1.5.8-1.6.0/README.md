# Comparing `tmp/guarddog-1.5.8.tar.gz` & `tmp/guarddog-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guarddog-1.5.8.tar", max compression
+gzip compressed data, was "guarddog-1.6.0.tar", max compression
```

## Comparing `guarddog-1.5.8.tar` & `guarddog-1.6.0.tar`

### file list

```diff
@@ -1,62 +1,69 @@
--rw-r--r--   0        0        0    11377 2024-04-08 10:37:22.648802 guarddog-1.5.8/LICENSE
--rw-r--r--   0        0        0      314 2024-04-08 10:37:22.648802 guarddog-1.5.8/LICENSE-3rdparty.csv
--rw-r--r--   0        0        0      140 2024-04-08 10:37:22.648802 guarddog-1.5.8/NOTICE
--rw-r--r--   0        0        0      154 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/__init__.py
--rw-r--r--   0        0        0      246 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/__main__.py
--rw-r--r--   0        0        0        0 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/__init__.py
--rw-r--r--   0        0        0     9680 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/analyzer.py
--rw-r--r--   0        0        0      457 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/__init__.py
--rw-r--r--   0        0        0      609 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/detector.py
--rw-r--r--   0        0        0     1166 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/empty_information.py
--rw-r--r--   0        0        0      951 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/npm/__init__.py
--rw-r--r--   0        0        0     2449 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/npm/direct_url_dependency.py
--rw-r--r--   0        0        0      793 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/npm/empty_information.py
--rw-r--r--   0        0        0     4215 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py
--rw-r--r--   0        0        0     1260 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0      578 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/npm/release_zero.py
--rw-r--r--   0        0        0     1732 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/npm/typosquatting.py
--rw-r--r--   0        0        0     4153 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0      976 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/pypi/__init__.py
--rw-r--r--   0        0        0      723 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/pypi/empty_information.py
--rw-r--r--   0        0        0     1873 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py
--rw-r--r--   0        0        0      716 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/pypi/release_zero.py
--rw-r--r--   0        0        0    11635 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py
--rw-r--r--   0        0        0     1369 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/pypi/single_python_file.py
--rw-r--r--   0        0        0     3490 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/pypi/typosquatting.py
--rw-r--r--   0        0        0      438 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/release_zero.py
--rw-r--r--   0        0        0      743 2024-04-08 10:37:22.648802 guarddog-1.5.8/guarddog/analyzer/metadata/repository_integrity_mismatch.py
--rw-r--r--   0        0        0   373303 2024-04-08 10:37:22.652802 guarddog-1.5.8/guarddog/analyzer/metadata/resources/top_npm_packages.json
--rw-r--r--   0        0        0   387251 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/metadata/resources/top_pypi_packages.json
--rw-r--r--   0        0        0     5619 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/metadata/typosquatting.py
--rw-r--r--   0        0        0      889 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/__init__.py
--rw-r--r--   0        0        0      524 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/clipboard-access.yml
--rw-r--r--   0        0        0      682 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/cmd-overwrite.yml
--rw-r--r--   0        0        0     4655 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/code-execution.yml
--rw-r--r--   0        0        0     1806 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/download-executable.yml
--rw-r--r--   0        0        0     2371 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/exec-base64.yml
--rw-r--r--   0        0        0     1815 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml
--rw-r--r--   0        0        0      576 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/npm-exec-base64.yml
--rw-r--r--   0        0        0     1067 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/npm-install-script.yml
--rw-r--r--   0        0        0      835 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/npm-serialize-environment.yml
--rw-r--r--   0        0        0     3513 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml
--rw-r--r--   0        0        0      582 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/obfuscation.yml
--rw-r--r--   0        0        0     1415 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/shady-links.yml
--rw-r--r--   0        0        0      418 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/silent-process-execution.yml
--rw-r--r--   0        0        0      606 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/analyzer/sourcecode/steganography.yml
--rw-r--r--   0        0        0    13182 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/cli.py
--rw-r--r--   0        0        0      315 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/ecosystems.py
--rw-r--r--   0        0        0        0 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/reporters/__init__.py
--rw-r--r--   0        0        0     6189 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/reporters/sarif.py
--rw-r--r--   0        0        0      752 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/scanners/__init__.py
--rw-r--r--   0        0        0     1968 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/scanners/npm_package_scanner.py
--rw-r--r--   0        0        0     2243 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/scanners/npm_project_scanner.py
--rw-r--r--   0        0        0     2512 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/scanners/pypi_package_scanner.py
--rw-r--r--   0        0        0     5491 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/scanners/pypi_project_scanner.py
--rw-r--r--   0        0        0    11170 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/scanners/scanner.py
--rw-r--r--   0        0        0        0 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/utils/__init__.py
--rw-r--r--   0        0        0     1323 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/utils/archives.py
--rw-r--r--   0        0        0       54 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/utils/exceptions.py
--rw-r--r--   0        0        0      953 2024-04-08 10:37:22.656802 guarddog-1.5.8/guarddog/utils/package_info.py
--rw-r--r--   0        0        0       52 2024-04-08 10:37:22.656802 guarddog-1.5.8/pypi.rst
--rw-r--r--   0        0        0     1213 2024-04-08 10:37:32.188830 guarddog-1.5.8/pyproject.toml
--rw-r--r--   0        0        0     1270 1970-01-01 00:00:00.000000 guarddog-1.5.8/PKG-INFO
+-rw-r--r--   0        0        0    11377 2024-04-25 08:45:59.091654 guarddog-1.6.0/LICENSE
+-rw-r--r--   0        0        0      314 2024-04-25 08:45:59.091654 guarddog-1.6.0/LICENSE-3rdparty.csv
+-rw-r--r--   0        0        0      140 2024-04-25 08:45:59.091654 guarddog-1.6.0/NOTICE
+-rw-r--r--   0        0        0      154 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/__init__.py
+-rw-r--r--   0        0        0     9680 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/analyzer.py
+-rw-r--r--   0        0        0      457 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/__init__.py
+-rw-r--r--   0        0        0      609 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/detector.py
+-rw-r--r--   0        0        0     1166 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/empty_information.py
+-rw-r--r--   0        0        0     1126 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/npm/__init__.py
+-rw-r--r--   0        0        0     2449 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/npm/direct_url_dependency.py
+-rw-r--r--   0        0        0      793 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/npm/empty_information.py
+-rw-r--r--   0        0        0     4428 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py
+-rw-r--r--   0        0        0     1643 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0      578 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/npm/release_zero.py
+-rw-r--r--   0        0        0     1732 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/npm/typosquatting.py
+-rw-r--r--   0        0        0      899 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/npm/unclaimed_maintainer_email_domain.py
+-rw-r--r--   0        0        0      461 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/npm/utils.py
+-rw-r--r--   0        0        0     2806 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0     1151 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/pypi/__init__.py
+-rw-r--r--   0        0        0      723 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/pypi/empty_information.py
+-rw-r--r--   0        0        0     1679 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py
+-rw-r--r--   0        0        0      716 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/pypi/release_zero.py
+-rw-r--r--   0        0        0    11635 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py
+-rw-r--r--   0        0        0     1369 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/pypi/single_python_file.py
+-rw-r--r--   0        0        0     3490 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/pypi/typosquatting.py
+-rw-r--r--   0        0        0      406 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/pypi/unclaimed_maintainer_email_domain.py
+-rw-r--r--   0        0        0      199 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/pypi/utils.py
+-rw-r--r--   0        0        0      438 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/release_zero.py
+-rw-r--r--   0        0        0      743 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/repository_integrity_mismatch.py
+-rw-r--r--   0        0        0   373303 2024-04-25 08:45:59.095654 guarddog-1.6.0/guarddog/analyzer/metadata/resources/top_npm_packages.json
+-rw-r--r--   0        0        0   387251 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/analyzer/metadata/resources/top_pypi_packages.json
+-rw-r--r--   0        0        0     5619 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/analyzer/metadata/typosquatting.py
+-rw-r--r--   0        0        0     2367 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/analyzer/metadata/unclaimed_maintainer_email_domain.py
+-rw-r--r--   0        0        0     1603 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/analyzer/metadata/utils.py
+-rw-r--r--   0        0        0      889 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/analyzer/sourcecode/__init__.py
+-rw-r--r--   0        0        0      524 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/analyzer/sourcecode/clipboard-access.yml
+-rw-r--r--   0        0        0      682 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/analyzer/sourcecode/cmd-overwrite.yml
+-rw-r--r--   0        0        0     4655 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/analyzer/sourcecode/code-execution.yml
+-rw-r--r--   0        0        0     2855 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/analyzer/sourcecode/download-executable.yml
+-rw-r--r--   0        0        0     2371 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/analyzer/sourcecode/exec-base64.yml
+-rw-r--r--   0        0        0     1815 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml
+-rw-r--r--   0        0        0      576 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/analyzer/sourcecode/npm-exec-base64.yml
+-rw-r--r--   0        0        0     1067 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/analyzer/sourcecode/npm-install-script.yml
+-rw-r--r--   0        0        0     2100 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/analyzer/sourcecode/npm-obfuscation.yml
+-rw-r--r--   0        0        0      835 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/analyzer/sourcecode/npm-serialize-environment.yml
+-rw-r--r--   0        0        0     3513 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml
+-rw-r--r--   0        0        0      582 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/analyzer/sourcecode/obfuscation.yml
+-rw-r--r--   0        0        0     1415 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/analyzer/sourcecode/shady-links.yml
+-rw-r--r--   0        0        0      418 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/analyzer/sourcecode/silent-process-execution.yml
+-rw-r--r--   0        0        0      606 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/analyzer/sourcecode/steganography.yml
+-rw-r--r--   0        0        0    13215 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/cli.py
+-rw-r--r--   0        0        0      315 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/ecosystems.py
+-rw-r--r--   0        0        0        0 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/reporters/__init__.py
+-rw-r--r--   0        0        0     6189 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/reporters/sarif.py
+-rw-r--r--   0        0        0      752 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/scanners/__init__.py
+-rw-r--r--   0        0        0     1968 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/scanners/npm_package_scanner.py
+-rw-r--r--   0        0        0     2243 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/scanners/npm_project_scanner.py
+-rw-r--r--   0        0        0     2512 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/scanners/pypi_package_scanner.py
+-rw-r--r--   0        0        0     5491 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/scanners/pypi_project_scanner.py
+-rw-r--r--   0        0        0    11170 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/scanners/scanner.py
+-rw-r--r--   0        0        0        0 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/utils/__init__.py
+-rw-r--r--   0        0        0     1323 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/utils/archives.py
+-rw-r--r--   0        0        0       54 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/utils/exceptions.py
+-rw-r--r--   0        0        0      953 2024-04-25 08:45:59.099654 guarddog-1.6.0/guarddog/utils/package_info.py
+-rw-r--r--   0        0        0       52 2024-04-25 08:45:59.103654 guarddog-1.6.0/pypi.rst
+-rw-r--r--   0        0        0     1222 2024-04-25 08:46:08.683628 guarddog-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 guarddog-1.6.0/PKG-INFO
```

### Comparing `guarddog-1.5.8/LICENSE` & `guarddog-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/analyzer.py` & `guarddog-1.6.0/guarddog/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/metadata/detector.py` & `guarddog-1.6.0/guarddog/analyzer/metadata/detector.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/metadata/empty_information.py` & `guarddog-1.6.0/guarddog/analyzer/metadata/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/metadata/npm/__init__.py` & `guarddog-1.6.0/guarddog/analyzer/metadata/npm/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from guarddog.analyzer.metadata.npm.empty_information import NPMEmptyInfoDetector
 from guarddog.analyzer.metadata.npm.potentially_compromised_email_domain import (
     NPMPotentiallyCompromisedEmailDomainDetector,
 )
+from guarddog.analyzer.metadata.npm.unclaimed_maintainer_email_domain import (
+    NPMUnclaimedMaintainerEmailDomainDetector,
+)
 from guarddog.analyzer.metadata.npm.release_zero import NPMReleaseZeroDetector
 from guarddog.analyzer.metadata.npm.typosquatting import NPMTyposquatDetector
 from guarddog.analyzer.metadata.npm.direct_url_dependency import (
     NPMDirectURLDependencyDetector,
 )
 from guarddog.analyzer.metadata.npm.npm_metadata_mismatch import NPMMetadataMismatch
 
 NPM_METADATA_RULES = {}
 
 classes = [
     NPMEmptyInfoDetector,
     NPMReleaseZeroDetector,
     NPMPotentiallyCompromisedEmailDomainDetector,
+    NPMUnclaimedMaintainerEmailDomainDetector,
     NPMTyposquatDetector,
     NPMDirectURLDependencyDetector,
     NPMMetadataMismatch,
 ]
 
 for detectorClass in classes:
     detectorInstance = detectorClass()  # type: ignore
```

### Comparing `guarddog-1.5.8/guarddog/analyzer/metadata/npm/direct_url_dependency.py` & `guarddog-1.6.0/guarddog/analyzer/metadata/npm/direct_url_dependency.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/metadata/npm/empty_information.py` & `guarddog-1.6.0/guarddog/analyzer/metadata/npm/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py` & `guarddog-1.6.0/guarddog/analyzer/metadata/npm/npm_metadata_mismatch.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,83 +1,113 @@
-from typing import Optional, Any
+from typing import Optional, Any, Dict
 from pathlib import Path
 import json
 
 from guarddog.analyzer.metadata.detector import Detector
 
-# List of fields where mismatch between package.json and NPM can carry malicious information
-# (field, expected type)
+# List of fields where mismatch between package.json and NPM can carry malicious information.
 MANIFEST_FIELDS_CHECKLIST = {
     "dependencies": dict,
     "devDependencies": dict,
     "scripts": dict,
     "main": str,
-    "repository": dict,
-    "bugs": dict,
-    "homepage": str
 }
 
 
 class NPMMetadataMismatch(Detector):
     def __init__(self):
         super().__init__(
             name="npm_metadata_mismatch",
-            description="Identify packages which have mismatches between the npm pacakge manifest and the package info"
+            description="Identify packages which have mismatches between the npm package"
+            " manifest and the package info for some critical fields",
         )
 
-    def detect(self, package_info, path: Optional[str] = None, name: Optional[str] = None,
-               version: Optional[str] = None) -> tuple[bool, Optional[str]]:
+    def detect(
+        self,
+        package_info,
+        path: Optional[str] = None,
+        name: Optional[str] = None,
+        version: Optional[str] = None,
+    ) -> tuple[bool, Optional[str]]:
         # Get the latest version if not specified
         if not version:
             version = package_info["dist-tags"]["latest"]
 
         # Load package.json manifest
         if path is None:
             raise ValueError("path is needed to run heuristic " + self.get_name())
         package_json = Path(path) / "package" / "package.json"
-        package_manifest: dict[str, Any] = json.loads(package_json.read_text())
+        package_manifest: Dict[str, Any] = json.loads(package_json.read_text())
 
         # Get NPM manifest for version
         version_info = package_info["versions"][version]
 
-        diff: dict[str, Diff] = {
+        diff = {
             field: difference_at_key(version_info, package_manifest, field, field_type)
             for field, field_type in MANIFEST_FIELDS_CHECKLIST.items()
         }
-        number_different = sum(len(v) for k, v in diff.items())
-        diff_description = describe_diff(diff) if number_different != 0 else "No differences found"
+
+        number_different = sum(len(v) for v in diff.values())
+
+        diff_description = (
+            describe_diff(diff) if number_different != 0 else "No differences found"
+        )
+
         return number_different != 0, diff_description
 
 
 # PerItemDiff is (key, left_value, right_value)
-PerItemDiff = tuple[str, Optional[str], Optional[str]]
+PerItemDiff = tuple[str, Optional[Any], Optional[Any]]
 Diff = list[PerItemDiff]
 
 
-def diff_at_key_dict(version_at_key: dict[str, Optional[str]], manifest_at_key: dict[str, Optional[str]]) -> Diff:
+def diff_at_key_dict(
+    version_at_key: Dict[str, Optional[Any]],
+    manifest_at_key: Dict[str, Optional[Any]],
+) -> Diff:
     return [
         (key, version_at_key.get(key), manifest_at_key.get(key))
         for key in set(version_at_key.keys()).union(set(manifest_at_key.keys()))
         if version_at_key.get(key) != manifest_at_key.get(key)
     ]
 
 
-def difference_at_key(version_info: dict[str, Any], package_manifest: dict[str, Any], key: str, key_type) -> Diff:
+def difference_at_key(
+    version_info: Dict[str, Any],
+    package_manifest: Dict[str, Any],
+    key: str,
+    key_type: type,
+) -> Diff:
     version_at_key = version_info.get(key, key_type())
     manifest_at_key = package_manifest.get(key, key_type())
-    if not (isinstance(version_at_key, key_type) and isinstance(manifest_at_key, key_type)):
-        return [(f"Expected type {str(key_type)}", f"{type(version_at_key)}", f"{type(manifest_at_key)}")]
-    elif key_type == dict:
-        return diff_at_key_dict(version_at_key, manifest_at_key)
-    else:
-        # If it is not a dict do a direct comparison of the value at the key, currently the only other type is strings
-        return [(f"{key}", version_at_key, manifest_at_key)] if version_at_key != manifest_at_key else []
+
+    if not (
+        isinstance(version_at_key, key_type) and isinstance(manifest_at_key, key_type)
+    ):
+        return [
+            (
+                f"Expected type {str(key_type)}",
+                f"{type(version_at_key)}",
+                f"{type(manifest_at_key)}",
+            )
+        ]
+
+    if key_type == dict:
+        return diff_at_key_dict(version_at_key, manifest_at_key)  # type: ignore
+
+    # If it is not a dict do a direct comparison of the value at the key.
+    # Currently the only other type is strings.
+    return (
+        [(key, version_at_key, manifest_at_key)]
+        if version_at_key != manifest_at_key
+        else []
+    )
 
 
-def describe_diff(diff: dict[str, Diff]) -> str:
+def describe_diff(diff: Dict[str, Diff]) -> str:
     """
     Creates a string of the form
     Difference between manifest and package.json found:
     dependencies:
         key: Manifest("v4.0.0"), package.json("v3.0.1")
     scripts:
         key: Manifest("a"), package.json("b")
@@ -90,15 +120,17 @@
     """
     description = "Difference between manifest and package.json found: \n"
     for k, differences in diff.items():
         if differences:
             field_description = f"{k}: \n"
             if MANIFEST_FIELDS_CHECKLIST[k] == dict:
                 for d in differences:
-                    field_description += f"  {d[0]}: Manifest(\"{d[1]}\"), package.json(\"{d[2]}\") \n"
+                    field_description += (
+                        f'  {d[0]}: Manifest("{d[1]}"), package.json("{d[2]}") \n'
+                    )
             else:
                 manifest_str = "  Manifest:\n"
                 package_str = "  package.json:\n"
                 for d in differences:
                     manifest_str += f"    {d[1]}\n"
                     package_str += f"    {d[2]}\n"
                 field_description = field_description + manifest_str + package_str
```

### Comparing `guarddog-1.5.8/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py` & `guarddog-1.6.0/guarddog/analyzer/metadata/npm/potentially_compromised_email_domain.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,24 +6,34 @@
 from datetime import datetime
 from typing import Optional
 
 from dateutil import parser
 
 from guarddog.analyzer.metadata.potentially_compromised_email_domain import PotentiallyCompromisedEmailDomainDetector
 
+from .utils import NPM_API_MAINTAINER_EMAIL_WARNING, get_email_addresses
+
 
 class NPMPotentiallyCompromisedEmailDomainDetector(PotentiallyCompromisedEmailDomainDetector):
     def __init__(self):
         super().__init__("npm")
 
-    def get_email_addresses(self, package_info: dict) -> list[str]:
-        if package_info.get("maintainers"):
-            return list(map(lambda x: x["email"], package_info["maintainers"]))
-        else:
-            return []
+        self.description += "; " + NPM_API_MAINTAINER_EMAIL_WARNING
+
+    def get_email_addresses(self, package_info: dict):
+        return get_email_addresses(package_info)
+
+    def detect(self, package_info, path: Optional[str] = None, name: Optional[str] = None,
+               version: Optional[str] = None) -> tuple[bool, str]:
+        has_issues, message = super().detect(package_info, path, name, version)
+
+        if has_issues:
+            message += "\n\n" + NPM_API_MAINTAINER_EMAIL_WARNING
+
+        return has_issues, message
 
     def get_project_latest_release_date(self, package_info) -> Optional[datetime]:
         """
         Gets the most recent release date of a Python project
 
         Args:
             releases (dict): PyPI JSON API's representation field
```

### Comparing `guarddog-1.5.8/guarddog/analyzer/metadata/npm/release_zero.py` & `guarddog-1.6.0/guarddog/analyzer/metadata/npm/release_zero.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/metadata/npm/typosquatting.py` & `guarddog-1.6.0/guarddog/analyzer/metadata/npm/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/metadata/pypi/__init__.py` & `guarddog-1.6.0/guarddog/analyzer/metadata/pypi/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from guarddog.analyzer.metadata.pypi.empty_information import PypiEmptyInfoDetector
 from guarddog.analyzer.metadata.pypi.potentially_compromised_email_domain import \
     PypiPotentiallyCompromisedEmailDomainDetector
+from guarddog.analyzer.metadata.pypi.unclaimed_maintainer_email_domain import \
+    PypiUnclaimedMaintainerEmailDomainDetector
 from guarddog.analyzer.metadata.pypi.release_zero import PypiReleaseZeroDetector
 from guarddog.analyzer.metadata.pypi.repository_integrity_mismatch import PypiIntegrityMismatchDetector
 from guarddog.analyzer.metadata.pypi.single_python_file import PypiSinglePythonFileDetector
 from guarddog.analyzer.metadata.pypi.typosquatting import PypiTyposquatDetector
 
 PYPI_METADATA_RULES = {}
 
 classes = [
     PypiEmptyInfoDetector,
     PypiReleaseZeroDetector,
     PypiTyposquatDetector,
     PypiPotentiallyCompromisedEmailDomainDetector,
+    PypiUnclaimedMaintainerEmailDomainDetector,
     PypiIntegrityMismatchDetector,
     PypiSinglePythonFileDetector
 
 ]
 
 for detectorClass in classes:
     detectorInstance = detectorClass()  # type: ignore
```

### Comparing `guarddog-1.5.8/guarddog/analyzer/metadata/pypi/empty_information.py` & `guarddog-1.6.0/guarddog/analyzer/metadata/pypi/empty_information.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py` & `guarddog-1.6.0/guarddog/analyzer/metadata/pypi/potentially_compromised_email_domain.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,27 +6,23 @@
 from typing import Optional
 
 from dateutil import parser
 from packaging import version
 
 from guarddog.analyzer.metadata.potentially_compromised_email_domain import PotentiallyCompromisedEmailDomainDetector
 
+from .utils import get_email_addresses
+
 
 class PypiPotentiallyCompromisedEmailDomainDetector(PotentiallyCompromisedEmailDomainDetector):
     def __init__(self):
         super().__init__("pypi")
 
-    def get_email_addresses(self, package_info: dict) -> list[str]:
-        author_email = package_info["info"]["author_email"]
-        maintainer_email = package_info["info"]["maintainer_email"]
-        email = author_email or maintainer_email
-        if email is not None:
-            return [email]
-        else:
-            return []
+    def get_email_addresses(self, package_info: dict):
+        return get_email_addresses(package_info)
 
     def get_project_latest_release_date(self, package_info) -> Optional[datetime]:
         """
         Gets the most recent release date of a Python project
 
         Args:
             releases (dict): PyPI JSON API's representation field
```

### Comparing `guarddog-1.5.8/guarddog/analyzer/metadata/pypi/release_zero.py` & `guarddog-1.6.0/guarddog/analyzer/metadata/pypi/release_zero.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py` & `guarddog-1.6.0/guarddog/analyzer/metadata/pypi/repository_integrity_mismatch.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/metadata/pypi/single_python_file.py` & `guarddog-1.6.0/guarddog/analyzer/metadata/pypi/single_python_file.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/metadata/pypi/typosquatting.py` & `guarddog-1.6.0/guarddog/analyzer/metadata/pypi/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/metadata/repository_integrity_mismatch.py` & `guarddog-1.6.0/guarddog/analyzer/metadata/repository_integrity_mismatch.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/metadata/resources/top_npm_packages.json` & `guarddog-1.6.0/guarddog/analyzer/metadata/resources/top_npm_packages.json`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/metadata/resources/top_pypi_packages.json` & `guarddog-1.6.0/guarddog/analyzer/metadata/resources/top_pypi_packages.json`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/metadata/typosquatting.py` & `guarddog-1.6.0/guarddog/analyzer/metadata/typosquatting.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/sourcecode/__init__.py` & `guarddog-1.6.0/guarddog/analyzer/sourcecode/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/sourcecode/clipboard-access.yml` & `guarddog-1.6.0/guarddog/analyzer/sourcecode/clipboard-access.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/sourcecode/cmd-overwrite.yml` & `guarddog-1.6.0/guarddog/analyzer/sourcecode/cmd-overwrite.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/sourcecode/code-execution.yml` & `guarddog-1.6.0/guarddog/analyzer/sourcecode/code-execution.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/sourcecode/exec-base64.yml` & `guarddog-1.6.0/guarddog/analyzer/sourcecode/exec-base64.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml` & `guarddog-1.6.0/guarddog/analyzer/sourcecode/exfiltrate-sensitive-data.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/sourcecode/npm-exec-base64.yml` & `guarddog-1.6.0/guarddog/analyzer/sourcecode/npm-exec-base64.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/sourcecode/npm-install-script.yml` & `guarddog-1.6.0/guarddog/analyzer/sourcecode/npm-install-script.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/sourcecode/npm-serialize-environment.yml` & `guarddog-1.6.0/guarddog/analyzer/sourcecode/npm-serialize-environment.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml` & `guarddog-1.6.0/guarddog/analyzer/sourcecode/npm-silent-process-execution.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/sourcecode/obfuscation.yml` & `guarddog-1.6.0/guarddog/analyzer/sourcecode/obfuscation.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/sourcecode/shady-links.yml` & `guarddog-1.6.0/guarddog/analyzer/sourcecode/shady-links.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/analyzer/sourcecode/steganography.yml` & `guarddog-1.6.0/guarddog/analyzer/sourcecode/steganography.yml`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/cli.py` & `guarddog-1.6.0/guarddog/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         sarif_rules = PYPI_RULES if ecosystem == ECOSYSTEM.PYPI else NPM_RULES
         return_value = report_verify_sarif(path, list(sarif_rules), results, ecosystem)
 
     if output_format is not None:
         print(return_value)
 
     if exit_non_zero_on_finding:
-        exit_with_status_code(results)
+        exit_with_status_code([result['result'] for result in results])
 
     return return_value  # this is mostly for testing
 
 
 def is_local_target(identifier: str) -> bool:
     """
     @param identifier:  The name/path of the package as passed to "guarddog ecosystem scan"
```

### Comparing `guarddog-1.5.8/guarddog/reporters/sarif.py` & `guarddog-1.6.0/guarddog/reporters/sarif.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/scanners/__init__.py` & `guarddog-1.6.0/guarddog/scanners/__init__.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/scanners/npm_package_scanner.py` & `guarddog-1.6.0/guarddog/scanners/npm_package_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/scanners/npm_project_scanner.py` & `guarddog-1.6.0/guarddog/scanners/npm_project_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/scanners/pypi_package_scanner.py` & `guarddog-1.6.0/guarddog/scanners/pypi_package_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/scanners/pypi_project_scanner.py` & `guarddog-1.6.0/guarddog/scanners/pypi_project_scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/scanners/scanner.py` & `guarddog-1.6.0/guarddog/scanners/scanner.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/utils/archives.py` & `guarddog-1.6.0/guarddog/utils/archives.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/guarddog/utils/package_info.py` & `guarddog-1.6.0/guarddog/utils/package_info.py`

 * *Files identical despite different names*

### Comparing `guarddog-1.5.8/pyproject.toml` & `guarddog-1.6.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 [tool.poetry]
 name = "guarddog"
 description = "GuardDog is a CLI tool to Identify malicious PyPI packages"
 authors = ["Ellen Wang", "Christophe Tafani-Dereeper"]
 license = "Apache-2.0"
 readme = "pypi.rst"
 repository = "https://github.com/DataDog/guarddog"
-version = "v1.5.8"
+version = "v1.6.0"
 
 [tool.poetry.scripts]
 guarddog = "guarddog.cli:cli"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
 semgrep = "1.67.0"
 requests = "^2.29.0"
 python-dateutil = "^2.8.2"
 click = "^8.1.3"
 click-option-group = "^0.5.5"
 colorama = "^0.4.6"  # used by click
 urllib3 = "2.2.1"
-python-whois = "^0.8.0"
+python-whois = ">=0.8,<0.10"
 termcolor = "^2.1.0"
 tarsafe = "^0.0.5"
 semantic-version = "^2.10.0"
 pyyaml = "^6.0"
 # 1.12+ requires new version of libgit2 which is not avaiable in Alpine
-pygit2 = ">=1.11,<1.13"
-configparser = ">=5.3,<7.0"
+pygit2 = ">=1.11,<1.15"
+configparser = ">=5.3,<8.0"
 prettytable="^3.6.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.4.1"
 coverage = "^7.2.7"
 flake8 = ">=5.0.4,<8.0.0"
-pytest = "^7.4.0"
-setuptools = ">=65.6.3,<69.0.0"
+pytest = ">=7.4,<9.0"
+setuptools = ">=65.6.3,<70.0.0"
 pytest-mock = "^3.11.1"
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore::DeprecationWarning"
 ]
 testpaths = [
```

### Comparing `guarddog-1.5.8/PKG-INFO` & `guarddog-1.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: guarddog
-Version: 1.5.8
+Version: 1.6.0
 Summary: GuardDog is a CLI tool to Identify malicious PyPI packages
 Home-page: https://github.com/DataDog/guarddog
 License: Apache-2.0
 Author: Ellen Wang
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-option-group (>=0.5.5,<0.6.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
-Requires-Dist: configparser (>=5.3,<7.0)
+Requires-Dist: configparser (>=5.3,<8.0)
 Requires-Dist: prettytable (>=3.6.0,<4.0.0)
-Requires-Dist: pygit2 (>=1.11,<1.13)
+Requires-Dist: pygit2 (>=1.11,<1.15)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: python-whois (>=0.8.0,<0.9.0)
+Requires-Dist: python-whois (>=0.8,<0.10)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.29.0,<3.0.0)
 Requires-Dist: semantic-version (>=2.10.0,<3.0.0)
 Requires-Dist: semgrep (==1.67.0)
 Requires-Dist: tarsafe (>=0.0.5,<0.0.6)
 Requires-Dist: termcolor (>=2.1.0,<3.0.0)
 Requires-Dist: urllib3 (==2.2.1)
```

