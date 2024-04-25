# Comparing `tmp/glance_store-4.7.0.tar.gz` & `tmp/glance_store-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glance_store-4.7.0.tar", last modified: Thu Feb 22 15:29:40 2024, max compression
+gzip compressed data, was "glance_store-4.8.0.tar", last modified: Thu Apr 25 11:19:40 2024, max compression
```

## Comparing `glance_store-4.7.0.tar` & `glance_store-4.8.0.tar`

### file list

```diff
@@ -1,233 +1,235 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.349441 glance_store-4.7.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2024-02-22 15:29:07.000000 glance_store-4.7.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5681 2024-02-22 15:29:07.000000 glance_store-4.7.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6489 2024-02-22 15:29:40.000000 glance_store-4.7.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30184 2024-02-22 15:29:40.000000 glance_store-4.7.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-02-22 15:29:07.000000 glance_store-4.7.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2829 2024-02-22 15:29:40.349441 glance_store-4.7.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1396 2024-02-22 15:29:07.000000 glance_store-4.7.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.317441 glance_store-4.7.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2024-02-22 15:29:07.000000 glance_store-4.7.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.321441 glance_store-4.7.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3964 2024-02-22 15:29:07.000000 glance_store-4.7.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2024-02-22 15:29:07.000000 glance_store-4.7.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.321441 glance_store-4.7.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-02-22 15:29:07.000000 glance_store-4.7.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.321441 glance_store-4.7.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2024-02-22 15:29:07.000000 glance_store-4.7.0/doc/source/user/drivers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-02-22 15:29:07.000000 glance_store-4.7.0/doc/source/user/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.313441 glance_store-4.7.0/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.321441 glance_store-4.7.0/etc/glance/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      972 2024-02-22 15:29:07.000000 glance_store-4.7.0/etc/glance/rootwrap.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.321441 glance_store-4.7.0/etc/glance/rootwrap.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      721 2024-02-22 15:29:07.000000 glance_store-4.7.0/etc/glance/rootwrap.d/glance_cinder_store.filters
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.321441 glance_store-4.7.0/glance_store/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      761 2024-02-22 15:29:07.000000 glance_store-4.7.0/glance_store/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.321441 glance_store-4.7.0/glance_store/_drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:07.000000 glance_store-4.7.0/glance_store/_drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.325441 glance_store-4.7.0/glance_store/_drivers/cinder/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      685 2024-02-22 15:29:07.000000 glance_store-4.7.0/glance_store/_drivers/cinder/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2440 2024-02-22 15:29:07.000000 glance_store-4.7.0/glance_store/_drivers/cinder/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4101 2024-02-22 15:29:07.000000 glance_store-4.7.0/glance_store/_drivers/cinder/nfs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3074 2024-02-22 15:29:07.000000 glance_store-4.7.0/glance_store/_drivers/cinder/scaleio.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    43569 2024-02-22 15:29:07.000000 glance_store-4.7.0/glance_store/_drivers/cinder/store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31286 2024-02-22 15:29:07.000000 glance_store-4.7.0/glance_store/_drivers/filesystem.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12238 2024-02-22 15:29:07.000000 glance_store-4.7.0/glance_store/_drivers/http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28174 2024-02-22 15:29:07.000000 glance_store-4.7.0/glance_store/_drivers/rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37846 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/_drivers/s3.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.325441 glance_store-4.7.0/glance_store/_drivers/swift/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/_drivers/swift/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6698 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/_drivers/swift/buffered.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9117 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/_drivers/swift/connection_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    69799 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/_drivers/swift/store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8362 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/_drivers/swift/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32392 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/_drivers/vmware_datastore.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17462 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/backend.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5630 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/capabilities.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.325441 glance_store-4.7.0/glance_store/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9510 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/common/attachment_state_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9744 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/common/cinder_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14677 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/common/fs_mount.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4731 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11014 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5400 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1113 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.317441 glance_store-4.7.0/glance_store/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.317441 glance_store-4.7.0/glance_store/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.325441 glance_store-4.7.0/glance_store/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9042 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/locale/en_GB/LC_MESSAGES/glance_store.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.317441 glance_store-4.7.0/glance_store/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.325441 glance_store-4.7.0/glance_store/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6352 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/locale/ko_KR/LC_MESSAGES/glance_store.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8655 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/location.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22611 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/multi_backend.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.325441 glance_store-4.7.0/glance_store/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4234 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.325441 glance_store-4.7.0/glance_store/tests/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      954 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/etc/glance-swift.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      834 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.325441 glance_store-4.7.0/glance_store/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2909 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/functional/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3915 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/functional/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.325441 glance_store-4.7.0/glance_store/tests/functional/filesystem/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/functional/filesystem/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1359 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/functional/filesystem/test_functional_filesystem.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.325441 glance_store-4.7.0/glance_store/tests/functional/swift/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/functional/swift/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3228 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/functional/swift/test_functional_swift.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.333441 glance_store-4.7.0/glance_store/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.333441 glance_store-4.7.0/glance_store/tests/unit/cinder/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/cinder/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4655 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/cinder/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    41373 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/cinder/test_cinder_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6764 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/cinder/test_cinder_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12926 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/cinder/test_multistore_cinder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3933 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/cinder/test_nfs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1849 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/cinder/test_scaleio.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.333441 glance_store-4.7.0/glance_store/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4716 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/common/test_attachment_state_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7621 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/common/test_cinder_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5763 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/common/test_fs_mount.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1144 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/common/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5862 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/test_backend.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8014 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/test_connection_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16806 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2223 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/test_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35512 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/test_filesystem_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8581 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/test_http_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1204 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/test_location.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35205 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/test_multistore_filesystem.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17478 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/test_multistore_rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24725 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/test_multistore_s3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29875 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/test_multistore_vmware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5643 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/test_opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30532 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/test_rbd_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23476 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/test_s3_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3408 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/test_store_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6435 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/test_store_capabilities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   101249 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/test_swift_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    97793 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/test_swift_store_multibackend.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6319 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/test_swift_store_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1349 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/test_test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30386 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/unit/test_vmware_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3780 2024-02-22 15:29:08.000000 glance_store-4.7.0/glance_store/tests/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.321441 glance_store-4.7.0/glance_store.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2829 2024-02-22 15:29:40.000000 glance_store-4.7.0/glance_store.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8609 2024-02-22 15:29:40.000000 glance_store-4.7.0/glance_store.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-22 15:29:40.000000 glance_store-4.7.0/glance_store.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1021 2024-02-22 15:29:40.000000 glance_store-4.7.0/glance_store.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-22 15:29:40.000000 glance_store-4.7.0/glance_store.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-02-22 15:29:40.000000 glance_store-4.7.0/glance_store.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2024-02-22 15:29:40.000000 glance_store-4.7.0/glance_store.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-02-22 15:29:40.000000 glance_store-4.7.0/glance_store.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.317441 glance_store-4.7.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.345441 glance_store-4.7.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/0.29.1-notes-ded2a1d473a306c7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/Stein_final_release-c7df5838028b8c7e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/add-store-weight-d443fbea8cc8d4c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/block-creating-encrypted-nfs-volumes-d0ff370ab762042e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/bug-1620999-8b76a0ad14826197.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/bug-1820817-0ee70781918d232e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/bug-1915602-fcc807a435d8a6bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/bug-1954883-3666d63a3c0233f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/bug-2004555-4fd67fce86c07461.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/cinder-fix-nfs-sparse-vol-create-76631ce05f86257c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/cinder-nfs-block-qcow2-vol-4fed58b0afafc980.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/cinder-support-extend-in-use-volume-c6292f950ff75cca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/deprecate-rados_connect_timeout-767ed1eaa026196e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/deprecate-sheepdog-driver-1f9689c327f313d4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/deprecate-store_add_to_backend-f419e5c4210613d2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/deprecate-store_capabilities_update_min_interval-039389fa296e2494.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/deprecate-vmware-store-2f720c6074b843b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/drop-py-2-7-345cafc9c1d3f892.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/drop-python-3-6-and-3-7-41af87576c4fd7b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/fix-exception-logging-during-attach-9546e24189db83c4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/fix-interval-in-retries-471155ff34d9f0e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/fix-ip-in-connector-info-36b95d9959f10f63.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      854 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/fix-rados_connect_timeout-39e5074bc1a3b65b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/fix-rbd-lockup-3aa2bb86f7d29e19.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/fix-wait-device-resize-c282940b71a3748e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/fs-drv-chunk-sz-a1b2f6a72fad92d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/handle-sparse-image-a3ecfc4ae1c00d48.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1342 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/improved-configuration-options-3635b56aba3072c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/lock_path-cef9d6f5f52c3211.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/move-rootwrap-config-f2cf435c548aab5c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      686 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/multi-store-0c004fc8aba2a25d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/multi-tenant-store-058b67ce5b7f3bd0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/multiattach-volume-handling-1a8446a64463f2cf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/multihash-support-629e9cbc283a8b47.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2459 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/pike-relnote-9f547df14184d18c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/prevent-unauthorized-errors-ebb9cf2236595cd0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2561 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/queens-relnote-5fa2d009d9a9e458.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/rbd-trash-snapshots-158a39da4248fb0c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2096 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/release-1.0.0-7ab43e91523eb3c8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/release-1.0.1-098b1487ac8cc9a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1384 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/release-1.2.0-8d239f01cd8ff0bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/releasenote-0.17.0-efee3f557ea2096a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/remove-cinder-experimental-fbf9dea32c84dc9b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/remove-gridfs-driver-09286e27613b4353.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/remove-s3-driver-f432afa1f53ecdf8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/remove-store-cap-update-min-interval-21fea4173ed4a09b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/rethinking-filesystem-access-5ab872fd0c0d27db.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/rocky-bugfixes-adefa8f47db16a2d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/set-documented-default-directory-for-filesystem-9b417a29416d3a94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      625 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/sorted-drivers-for-configs-a905f07d3bf9c973.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/start-using-reno-73ef709807e37b74.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/support-cinder-multiple-stores-6cc8489f8f4f8ff3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/support-cinder-upload-c85849d9c88bbd7e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      443 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/support-cinder-user-domain-420c76053dd50534.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/support-s3-driver-a4158f9fa35931d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/update-stein-deprecations-3c2f6ffeab22b558.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/victoria-milestone-1-c1f9de5b90e8c326.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/vmware-store-requests-369485d2cfdb6175.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/volume-type-validation-check-011a400d7fb3b307.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/wallaby-final-release-00f0f851ff7d93ab.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/notes/xena-final-release-3c6e19dfba43b40d.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.349441 glance_store-4.7.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.349441 glance_store-4.7.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.349441 glance_store-4.7.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8972 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/liberty.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.317441 glance_store-4.7.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.317441 glance_store-4.7.0/releasenotes/source/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.349441 glance_store-4.7.0/releasenotes/source/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2551 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.317441 glance_store-4.7.0/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.349441 glance_store-4.7.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    61215 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.317441 glance_store-4.7.0/releasenotes/source/locale/zh_CN/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.349441 glance_store-4.7.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2420 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-02-22 15:29:08.000000 glance_store-4.7.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      384 2024-02-22 15:29:08.000000 glance_store-4.7.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2402 2024-02-22 15:29:40.349441 glance_store-4.7.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-02-22 15:29:08.000000 glance_store-4.7.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2024-02-22 15:29:08.000000 glance_store-4.7.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:29:40.349441 glance_store-4.7.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2024-02-22 15:29:08.000000 glance_store-4.7.0/tools/with_venv.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2098 2024-02-22 15:29:08.000000 glance_store-4.7.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.256109 glance_store-4.8.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2024-04-25 11:18:54.000000 glance_store-4.8.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5681 2024-04-25 11:18:54.000000 glance_store-4.8.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6489 2024-04-25 11:19:39.000000 glance_store-4.8.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30441 2024-04-25 11:19:39.000000 glance_store-4.8.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-04-25 11:18:54.000000 glance_store-4.8.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2829 2024-04-25 11:19:40.256109 glance_store-4.8.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1396 2024-04-25 11:18:54.000000 glance_store-4.8.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.224109 glance_store-4.8.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2024-04-25 11:18:54.000000 glance_store-4.8.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.224109 glance_store-4.8.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3964 2024-04-25 11:18:54.000000 glance_store-4.8.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2024-04-25 11:18:54.000000 glance_store-4.8.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.224109 glance_store-4.8.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-04-25 11:18:54.000000 glance_store-4.8.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.224109 glance_store-4.8.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2024-04-25 11:18:54.000000 glance_store-4.8.0/doc/source/user/drivers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-04-25 11:18:54.000000 glance_store-4.8.0/doc/source/user/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.220109 glance_store-4.8.0/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.224109 glance_store-4.8.0/etc/glance/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      972 2024-04-25 11:18:54.000000 glance_store-4.8.0/etc/glance/rootwrap.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.224109 glance_store-4.8.0/etc/glance/rootwrap.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      721 2024-04-25 11:18:54.000000 glance_store-4.8.0/etc/glance/rootwrap.d/glance_cinder_store.filters
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.228109 glance_store-4.8.0/glance_store/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      761 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.228109 glance_store-4.8.0/glance_store/_drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/_drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.228109 glance_store-4.8.0/glance_store/_drivers/cinder/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      685 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/_drivers/cinder/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2440 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/_drivers/cinder/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4101 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/_drivers/cinder/nfs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3074 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/_drivers/cinder/scaleio.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44295 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/_drivers/cinder/store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31286 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/_drivers/filesystem.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12238 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/_drivers/http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28174 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/_drivers/rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37846 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/_drivers/s3.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.232109 glance_store-4.8.0/glance_store/_drivers/swift/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/_drivers/swift/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6698 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/_drivers/swift/buffered.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9117 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/_drivers/swift/connection_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    69799 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/_drivers/swift/store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8362 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/_drivers/swift/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32392 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/_drivers/vmware_datastore.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17462 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/backend.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5630 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/capabilities.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.232109 glance_store-4.8.0/glance_store/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9510 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/common/attachment_state_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9744 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/common/cinder_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14677 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/common/fs_mount.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4731 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11014 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5400 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1113 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.220109 glance_store-4.8.0/glance_store/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.220109 glance_store-4.8.0/glance_store/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.232109 glance_store-4.8.0/glance_store/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9042 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/locale/en_GB/LC_MESSAGES/glance_store.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.220109 glance_store-4.8.0/glance_store/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.232109 glance_store-4.8.0/glance_store/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6352 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/locale/ko_KR/LC_MESSAGES/glance_store.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8655 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/location.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22611 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/multi_backend.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.232109 glance_store-4.8.0/glance_store/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4234 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.232109 glance_store-4.8.0/glance_store/tests/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      954 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/etc/glance-swift.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      834 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.232109 glance_store-4.8.0/glance_store/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2909 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/functional/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3915 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/functional/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.232109 glance_store-4.8.0/glance_store/tests/functional/filesystem/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/functional/filesystem/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1359 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/functional/filesystem/test_functional_filesystem.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.232109 glance_store-4.8.0/glance_store/tests/functional/swift/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/functional/swift/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3228 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/functional/swift/test_functional_swift.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.240109 glance_store-4.8.0/glance_store/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.240109 glance_store-4.8.0/glance_store/tests/unit/cinder/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/cinder/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4655 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/cinder/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    41373 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/cinder/test_cinder_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6764 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/cinder/test_cinder_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13795 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/cinder/test_multistore_cinder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3933 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/cinder/test_nfs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1849 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/cinder/test_scaleio.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.240109 glance_store-4.8.0/glance_store/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4716 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/common/test_attachment_state_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7621 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/common/test_cinder_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5763 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/common/test_fs_mount.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1144 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/common/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5862 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/test_backend.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8014 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/test_connection_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16806 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2223 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/test_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35512 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/test_filesystem_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8581 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/test_http_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1204 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/test_location.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35205 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/test_multistore_filesystem.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17478 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/test_multistore_rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24725 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/test_multistore_s3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29875 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/test_multistore_vmware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5643 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/test_opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30532 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/test_rbd_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23476 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/test_s3_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3408 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/test_store_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6435 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/test_store_capabilities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   101249 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/test_swift_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    97793 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/test_swift_store_multibackend.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6319 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/test_swift_store_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1349 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/test_test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30386 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/unit/test_vmware_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3780 2024-04-25 11:18:54.000000 glance_store-4.8.0/glance_store/tests/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.228109 glance_store-4.8.0/glance_store.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2829 2024-04-25 11:19:39.000000 glance_store-4.8.0/glance_store.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8705 2024-04-25 11:19:40.000000 glance_store-4.8.0/glance_store.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-25 11:19:39.000000 glance_store-4.8.0/glance_store.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1021 2024-04-25 11:19:39.000000 glance_store-4.8.0/glance_store.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-25 11:19:39.000000 glance_store-4.8.0/glance_store.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-04-25 11:19:39.000000 glance_store-4.8.0/glance_store.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2024-04-25 11:19:39.000000 glance_store-4.8.0/glance_store.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-04-25 11:19:39.000000 glance_store-4.8.0/glance_store.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.220109 glance_store-4.8.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.252109 glance_store-4.8.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/0.29.1-notes-ded2a1d473a306c7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/Stein_final_release-c7df5838028b8c7e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/add-store-weight-d443fbea8cc8d4c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/block-creating-encrypted-nfs-volumes-d0ff370ab762042e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/bug-1620999-8b76a0ad14826197.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/bug-1820817-0ee70781918d232e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/bug-1915602-fcc807a435d8a6bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/bug-1954883-3666d63a3c0233f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/bug-2004555-4fd67fce86c07461.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/cinder-fix-nfs-sparse-vol-create-76631ce05f86257c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/cinder-nfs-block-qcow2-vol-4fed58b0afafc980.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/cinder-support-extend-in-use-volume-c6292f950ff75cca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/deprecate-rados_connect_timeout-767ed1eaa026196e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/deprecate-sheepdog-driver-1f9689c327f313d4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/deprecate-store_add_to_backend-f419e5c4210613d2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/deprecate-store_capabilities_update_min_interval-039389fa296e2494.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/deprecate-vmware-store-2f720c6074b843b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/drop-py-2-7-345cafc9c1d3f892.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/drop-python-3-6-and-3-7-41af87576c4fd7b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/fix-exception-logging-during-attach-9546e24189db83c4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/fix-interval-in-retries-471155ff34d9f0e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/fix-ip-in-connector-info-36b95d9959f10f63.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/fix-legacy-image-update-49a149ec267dccb6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      854 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/fix-rados_connect_timeout-39e5074bc1a3b65b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/fix-rbd-lockup-3aa2bb86f7d29e19.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/fix-wait-device-resize-c282940b71a3748e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/fs-drv-chunk-sz-a1b2f6a72fad92d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/handle-sparse-image-a3ecfc4ae1c00d48.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1342 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/improved-configuration-options-3635b56aba3072c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/lock_path-cef9d6f5f52c3211.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/move-rootwrap-config-f2cf435c548aab5c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      686 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/multi-store-0c004fc8aba2a25d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/multi-tenant-store-058b67ce5b7f3bd0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/multiattach-volume-handling-1a8446a64463f2cf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/multihash-support-629e9cbc283a8b47.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2459 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/pike-relnote-9f547df14184d18c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/prevent-unauthorized-errors-ebb9cf2236595cd0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2561 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/queens-relnote-5fa2d009d9a9e458.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/rbd-trash-snapshots-158a39da4248fb0c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2096 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/release-1.0.0-7ab43e91523eb3c8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/release-1.0.1-098b1487ac8cc9a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1384 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/release-1.2.0-8d239f01cd8ff0bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/releasenote-0.17.0-efee3f557ea2096a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/remove-cinder-experimental-fbf9dea32c84dc9b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/remove-gridfs-driver-09286e27613b4353.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/remove-s3-driver-f432afa1f53ecdf8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/remove-store-cap-update-min-interval-21fea4173ed4a09b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/rethinking-filesystem-access-5ab872fd0c0d27db.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/rocky-bugfixes-adefa8f47db16a2d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/set-documented-default-directory-for-filesystem-9b417a29416d3a94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      625 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/sorted-drivers-for-configs-a905f07d3bf9c973.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/start-using-reno-73ef709807e37b74.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/support-cinder-multiple-stores-6cc8489f8f4f8ff3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/support-cinder-upload-c85849d9c88bbd7e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      443 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/support-cinder-user-domain-420c76053dd50534.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/support-s3-driver-a4158f9fa35931d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/update-stein-deprecations-3c2f6ffeab22b558.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/victoria-milestone-1-c1f9de5b90e8c326.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/vmware-store-requests-369485d2cfdb6175.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/volume-type-validation-check-011a400d7fb3b307.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/wallaby-final-release-00f0f851ff7d93ab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/notes/xena-final-release-3c6e19dfba43b40d.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.252109 glance_store-4.8.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/2023.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/2024.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.252109 glance_store-4.8.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.252109 glance_store-4.8.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8972 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/liberty.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.224109 glance_store-4.8.0/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.220109 glance_store-4.8.0/releasenotes/source/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.252109 glance_store-4.8.0/releasenotes/source/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2551 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.224109 glance_store-4.8.0/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.252109 glance_store-4.8.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    61215 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.224109 glance_store-4.8.0/releasenotes/source/locale/zh_CN/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.256109 glance_store-4.8.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2420 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-04-25 11:18:54.000000 glance_store-4.8.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      384 2024-04-25 11:18:54.000000 glance_store-4.8.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2402 2024-04-25 11:19:40.256109 glance_store-4.8.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-04-25 11:18:54.000000 glance_store-4.8.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2024-04-25 11:18:54.000000 glance_store-4.8.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-25 11:19:40.256109 glance_store-4.8.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2024-04-25 11:18:54.000000 glance_store-4.8.0/tools/with_venv.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2098 2024-04-25 11:18:54.000000 glance_store-4.8.0/tox.ini
```

### Comparing `glance_store-4.7.0/.zuul.yaml` & `glance_store-4.8.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/AUTHORS` & `glance_store-4.8.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/ChangeLog` & `glance_store-4.8.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 CHANGES
 =======
 
+4.8.0
+-----
+
+* Use normal credentials for legacy image update
+* reno: Update master for xena Unmaintained status
+* reno: Update master for wallaby Unmaintained status
+* reno: Update master for victoria Unmaintained status
+* Update master for stable/2024.1
+
 4.7.0
 -----
 
 * reno: Update master for yoga Unmaintained status
 * Remove \_snapshot\_has\_external\_reference from rbd driver
 * Bump hacking
 * s3: Do not log access keys
```

### Comparing `glance_store-4.7.0/LICENSE` & `glance_store-4.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/PKG-INFO` & `glance_store-4.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glance_store
-Version: 4.7.0
+Version: 4.8.0
 Summary: OpenStack Image Service Store Library
 Home-page: https://docs.openstack.org/glance_store/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `glance_store-4.7.0/README.rst` & `glance_store-4.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/doc/source/conf.py` & `glance_store-4.8.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/doc/source/index.rst` & `glance_store-4.8.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/doc/source/user/drivers.rst` & `glance_store-4.8.0/doc/source/user/drivers.rst`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/etc/glance/rootwrap.conf` & `glance_store-4.8.0/etc/glance/rootwrap.conf`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/etc/glance/rootwrap.d/glance_cinder_store.filters` & `glance_store-4.8.0/etc/glance/rootwrap.d/glance_cinder_store.filters`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/__init__.py` & `glance_store-4.8.0/glance_store/__init__.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/_drivers/cinder/__init__.py` & `glance_store-4.8.0/glance_store/_drivers/cinder/__init__.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/_drivers/cinder/base.py` & `glance_store-4.8.0/glance_store/_drivers/cinder/base.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/_drivers/cinder/nfs.py` & `glance_store-4.8.0/glance_store/_drivers/cinder/nfs.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/_drivers/cinder/scaleio.py` & `glance_store-4.8.0/glance_store/_drivers/cinder/scaleio.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/_drivers/cinder/store.py` & `glance_store-4.8.0/glance_store/_drivers/cinder/store.py`

 * *Files 0% similar despite different names*

```diff
@@ -551,18 +551,37 @@
         image against the configured stores. It returns true if the
         cinder_volume_type configured in the store matches with the volume
         type of the image-volume. When cinder_volume_type is not configured
         then the it checks it against default_volume_type set in cinder.
         If above both conditions doesn't meet, it returns false.
         """
         try:
-            cinder_client = self.get_cinderclient(context=context,
-                                                  legacy_update=True)
+            # We will use either the service credentials defined in
+            # config file or the user context credentials
+            cinder_client = self.get_cinderclient(context=context)
             cinder_volume_type = self.store_conf.cinder_volume_type
-            volume = cinder_client.volumes.get(volume_id)
+            # Here we are assuming that the volume is stored in the
+            # service project or context user's project else this
+            # will return NotFound exception.
+            # Ideally we should be using service user's credentials
+            # defined in the config and the volume should be stored
+            # in the service (internal) project else we are opening the
+            # image-volume to modification by users which might lead
+            # to corruption of image.
+            try:
+                volume = cinder_client.volumes.get(volume_id)
+            except cinder_exception.NotFound:
+                reason = (_LW("Image-Volume %s not found. If you have "
+                              "upgraded your environment from single store "
+                              "to multi store, transfer all your "
+                              "Image-Volumes from user projects to service "
+                              "project."
+                          % volume_id))
+                LOG.warning(reason)
+                return False
             if cinder_volume_type and volume.volume_type == cinder_volume_type:
                 return True
             elif not cinder_volume_type:
                 default_type = cinder_client.volume_types.default()
                 if volume.volume_type == default_type.name:
                     return True
         except Exception:
@@ -580,25 +599,16 @@
         return 'sudo glance-rootwrap %s' % rootwrap
 
     def is_user_overriden(self):
         return all([self.store_conf.get('cinder_store_' + key)
                     for key in ['user_name', 'password',
                                 'project_name', 'auth_address']])
 
-    def get_cinderclient(self, context=None, legacy_update=False,
-                         version='3.0'):
-        # NOTE: For legacy image update from single store to multiple
-        # stores we need to use admin context rather than user provided
-        # credentials
-        if legacy_update:
-            user_overriden = False
-            context = context.elevated()
-        else:
-            user_overriden = self.is_user_overriden()
-
+    def get_cinderclient(self, context=None, version='3.0'):
+        user_overriden = self.is_user_overriden()
         session = get_cinder_session(self.store_conf)
 
         if user_overriden:
             username = self.store_conf.cinder_store_user_name
             url = self.store_conf.cinder_store_auth_address
             # use auth that is already in the session
             auth = None
```

### Comparing `glance_store-4.7.0/glance_store/_drivers/filesystem.py` & `glance_store-4.8.0/glance_store/_drivers/filesystem.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/_drivers/http.py` & `glance_store-4.8.0/glance_store/_drivers/http.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/_drivers/rbd.py` & `glance_store-4.8.0/glance_store/_drivers/rbd.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/_drivers/s3.py` & `glance_store-4.8.0/glance_store/_drivers/s3.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/_drivers/swift/__init__.py` & `glance_store-4.8.0/glance_store/_drivers/swift/__init__.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/_drivers/swift/buffered.py` & `glance_store-4.8.0/glance_store/_drivers/swift/buffered.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/_drivers/swift/connection_manager.py` & `glance_store-4.8.0/glance_store/_drivers/swift/connection_manager.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/_drivers/swift/store.py` & `glance_store-4.8.0/glance_store/_drivers/swift/store.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/_drivers/swift/utils.py` & `glance_store-4.8.0/glance_store/_drivers/swift/utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/_drivers/vmware_datastore.py` & `glance_store-4.8.0/glance_store/_drivers/vmware_datastore.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/backend.py` & `glance_store-4.8.0/glance_store/backend.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/capabilities.py` & `glance_store-4.8.0/glance_store/capabilities.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/common/attachment_state_manager.py` & `glance_store-4.8.0/glance_store/common/attachment_state_manager.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/common/cinder_utils.py` & `glance_store-4.8.0/glance_store/common/cinder_utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/common/fs_mount.py` & `glance_store-4.8.0/glance_store/common/fs_mount.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/common/utils.py` & `glance_store-4.8.0/glance_store/common/utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/driver.py` & `glance_store-4.8.0/glance_store/driver.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/exceptions.py` & `glance_store-4.8.0/glance_store/exceptions.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/i18n.py` & `glance_store-4.8.0/glance_store/i18n.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/locale/en_GB/LC_MESSAGES/glance_store.po` & `glance_store-4.8.0/glance_store/locale/en_GB/LC_MESSAGES/glance_store.po`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/locale/ko_KR/LC_MESSAGES/glance_store.po` & `glance_store-4.8.0/glance_store/locale/ko_KR/LC_MESSAGES/glance_store.po`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/location.py` & `glance_store-4.8.0/glance_store/location.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/multi_backend.py` & `glance_store-4.8.0/glance_store/multi_backend.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/base.py` & `glance_store-4.8.0/glance_store/tests/base.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/etc/glance-swift.conf` & `glance_store-4.8.0/glance_store/tests/etc/glance-swift.conf`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/fakes.py` & `glance_store-4.8.0/glance_store/tests/fakes.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/functional/README.rst` & `glance_store-4.8.0/glance_store/tests/functional/README.rst`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/functional/base.py` & `glance_store-4.8.0/glance_store/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/functional/filesystem/test_functional_filesystem.py` & `glance_store-4.8.0/glance_store/tests/functional/filesystem/test_functional_filesystem.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/functional/swift/test_functional_swift.py` & `glance_store-4.8.0/glance_store/tests/functional/swift/test_functional_swift.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/cinder/test_base.py` & `glance_store-4.8.0/glance_store/tests/unit/cinder/test_base.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/cinder/test_cinder_base.py` & `glance_store-4.8.0/glance_store/tests/unit/cinder/test_cinder_base.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/cinder/test_cinder_store.py` & `glance_store-4.8.0/glance_store/tests/unit/cinder/test_cinder_store.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/cinder/test_multistore_cinder.py` & `glance_store-4.8.0/glance_store/tests/unit/cinder/test_multistore_cinder.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,18 +108,20 @@
     def test_get_cinderclient_with_api_insecure(self):
         self._test_get_cinderclient_with_api_insecure(group='cinder1')
 
     def test_get_cinderclient_with_ca_certificates(self):
         self._test_get_cinderclient_with_ca_certificates(group='cinder1')
 
     def test_get_cinderclient_legacy_update(self):
-        cc = self.store.get_cinderclient(self.fake_admin_context,
-                                         legacy_update=True)
-        self.assertEqual('admin_token', cc.client.auth.token)
-        self.assertEqual('http://foo/public_url', cc.client.auth.endpoint)
+        fake_endpoint = 'http://cinder.openstack.example.com/v2/fake_project'
+        self.config(cinder_endpoint_template=fake_endpoint, group='cinder1')
+        cc = self.store.get_cinderclient(self.context)
+        self.assertEqual(self.context.auth_token,
+                         cc.client.auth.token)
+        self.assertEqual(fake_endpoint, cc.client.auth.endpoint)
 
     def test_open_cinder_volume_multipath_enabled(self):
         self.config(cinder_use_multipath=True, group='cinder1')
         self._test_open_cinder_volume('wb', 'rw', None,
                                       multipath_supported=True)
 
     def test_open_cinder_volume_multipath_disabled(self):
@@ -217,14 +219,27 @@
             # When cinder_volume_type is not set and volume's type does not
             # match with default volume type
             mocked_cc.return_value.volume_types = mock.MagicMock(
                 default=lambda: {'name': 'random_type'})
             type_match = self.store.is_image_associated_with_store(
                 self.context, fake_vol_id)
             self.assertFalse(type_match)
+            # When the Image-Volume is not found
+            mocked_cc.return_value.volumes.get = mock.MagicMock(
+                side_effect=cinder.cinder_exception.NotFound(code=404))
+            with mock.patch.object(cinder, 'LOG') as mock_log:
+                type_match = self.store.is_image_associated_with_store(
+                    self.context, fake_vol_id)
+                mock_log.warning.assert_called_with(
+                    "Image-Volume %s not found. If you have "
+                    "upgraded your environment from single store "
+                    "to multi store, transfer all your "
+                    "Image-Volumes from user projects to service "
+                    "project." % fake_vol_id)
+            self.assertFalse(type_match)
 
     def test_cinder_get(self):
         self._test_cinder_get(is_multi_store=True)
 
     def test_cinder_get_size(self):
         self._test_cinder_get_size(is_multi_store=True)
```

### Comparing `glance_store-4.7.0/glance_store/tests/unit/cinder/test_nfs.py` & `glance_store-4.8.0/glance_store/tests/unit/cinder/test_nfs.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/cinder/test_scaleio.py` & `glance_store-4.8.0/glance_store/tests/unit/cinder/test_scaleio.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/common/test_attachment_state_manager.py` & `glance_store-4.8.0/glance_store/tests/unit/common/test_attachment_state_manager.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/common/test_cinder_utils.py` & `glance_store-4.8.0/glance_store/tests/unit/common/test_cinder_utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/common/test_fs_mount.py` & `glance_store-4.8.0/glance_store/tests/unit/common/test_fs_mount.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/common/test_utils.py` & `glance_store-4.8.0/glance_store/tests/unit/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/test_backend.py` & `glance_store-4.8.0/glance_store/tests/unit/test_backend.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/test_connection_manager.py` & `glance_store-4.8.0/glance_store/tests/unit/test_connection_manager.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/test_driver.py` & `glance_store-4.8.0/glance_store/tests/unit/test_driver.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/test_exceptions.py` & `glance_store-4.8.0/glance_store/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/test_filesystem_store.py` & `glance_store-4.8.0/glance_store/tests/unit/test_filesystem_store.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/test_http_store.py` & `glance_store-4.8.0/glance_store/tests/unit/test_http_store.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/test_location.py` & `glance_store-4.8.0/glance_store/tests/unit/test_location.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/test_multistore_filesystem.py` & `glance_store-4.8.0/glance_store/tests/unit/test_multistore_filesystem.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/test_multistore_rbd.py` & `glance_store-4.8.0/glance_store/tests/unit/test_multistore_rbd.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/test_multistore_s3.py` & `glance_store-4.8.0/glance_store/tests/unit/test_multistore_s3.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/test_multistore_vmware.py` & `glance_store-4.8.0/glance_store/tests/unit/test_multistore_vmware.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/test_opts.py` & `glance_store-4.8.0/glance_store/tests/unit/test_opts.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/test_rbd_store.py` & `glance_store-4.8.0/glance_store/tests/unit/test_rbd_store.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/test_s3_store.py` & `glance_store-4.8.0/glance_store/tests/unit/test_s3_store.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/test_store_base.py` & `glance_store-4.8.0/glance_store/tests/unit/test_store_base.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/test_store_capabilities.py` & `glance_store-4.8.0/glance_store/tests/unit/test_store_capabilities.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/test_swift_store.py` & `glance_store-4.8.0/glance_store/tests/unit/test_swift_store.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/test_swift_store_multibackend.py` & `glance_store-4.8.0/glance_store/tests/unit/test_swift_store_multibackend.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/test_swift_store_utils.py` & `glance_store-4.8.0/glance_store/tests/unit/test_swift_store_utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/test_test_utils.py` & `glance_store-4.8.0/glance_store/tests/unit/test_test_utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/unit/test_vmware_store.py` & `glance_store-4.8.0/glance_store/tests/unit/test_vmware_store.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store/tests/utils.py` & `glance_store-4.8.0/glance_store/tests/utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store.egg-info/PKG-INFO` & `glance_store-4.8.0/glance_store.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glance-store
-Version: 4.7.0
+Version: 4.8.0
 Summary: OpenStack Image Service Store Library
 Home-page: https://docs.openstack.org/glance_store/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `glance_store-4.7.0/glance_store.egg-info/SOURCES.txt` & `glance_store-4.8.0/glance_store.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,15 @@
 releasenotes/notes/deprecate-store_capabilities_update_min_interval-039389fa296e2494.yaml
 releasenotes/notes/deprecate-vmware-store-2f720c6074b843b0.yaml
 releasenotes/notes/drop-py-2-7-345cafc9c1d3f892.yaml
 releasenotes/notes/drop-python-3-6-and-3-7-41af87576c4fd7b1.yaml
 releasenotes/notes/fix-exception-logging-during-attach-9546e24189db83c4.yaml
 releasenotes/notes/fix-interval-in-retries-471155ff34d9f0e9.yaml
 releasenotes/notes/fix-ip-in-connector-info-36b95d9959f10f63.yaml
+releasenotes/notes/fix-legacy-image-update-49a149ec267dccb6.yaml
 releasenotes/notes/fix-rados_connect_timeout-39e5074bc1a3b65b.yaml
 releasenotes/notes/fix-rbd-lockup-3aa2bb86f7d29e19.yaml
 releasenotes/notes/fix-wait-device-resize-c282940b71a3748e.yaml
 releasenotes/notes/fs-drv-chunk-sz-a1b2f6a72fad92d5.yaml
 releasenotes/notes/handle-sparse-image-a3ecfc4ae1c00d48.yaml
 releasenotes/notes/improved-configuration-options-3635b56aba3072c9.yaml
 releasenotes/notes/lock_path-cef9d6f5f52c3211.yaml
@@ -162,14 +163,15 @@
 releasenotes/notes/victoria-milestone-1-c1f9de5b90e8c326.yaml
 releasenotes/notes/vmware-store-requests-369485d2cfdb6175.yaml
 releasenotes/notes/volume-type-validation-check-011a400d7fb3b307.yaml
 releasenotes/notes/wallaby-final-release-00f0f851ff7d93ab.yaml
 releasenotes/notes/xena-final-release-3c6e19dfba43b40d.yaml
 releasenotes/source/2023.1.rst
 releasenotes/source/2023.2.rst
+releasenotes/source/2024.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/liberty.rst
 releasenotes/source/mitaka.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
```

### Comparing `glance_store-4.7.0/glance_store.egg-info/entry_points.txt` & `glance_store-4.8.0/glance_store.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/glance_store.egg-info/requires.txt` & `glance_store-4.8.0/glance_store.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/notes/0.29.1-notes-ded2a1d473a306c7.yaml` & `glance_store-4.8.0/releasenotes/notes/0.29.1-notes-ded2a1d473a306c7.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/notes/Stein_final_release-c7df5838028b8c7e.yaml` & `glance_store-4.8.0/releasenotes/notes/Stein_final_release-c7df5838028b8c7e.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/notes/deprecate-sheepdog-driver-1f9689c327f313d4.yaml` & `glance_store-4.8.0/releasenotes/notes/deprecate-sheepdog-driver-1f9689c327f313d4.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/notes/deprecate-store_add_to_backend-f419e5c4210613d2.yaml` & `glance_store-4.8.0/releasenotes/notes/deprecate-store_add_to_backend-f419e5c4210613d2.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/notes/deprecate-store_capabilities_update_min_interval-039389fa296e2494.yaml` & `glance_store-4.8.0/releasenotes/notes/deprecate-store_capabilities_update_min_interval-039389fa296e2494.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/notes/fix-rados_connect_timeout-39e5074bc1a3b65b.yaml` & `glance_store-4.8.0/releasenotes/notes/fix-rados_connect_timeout-39e5074bc1a3b65b.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/notes/handle-sparse-image-a3ecfc4ae1c00d48.yaml` & `glance_store-4.8.0/releasenotes/notes/handle-sparse-image-a3ecfc4ae1c00d48.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/notes/improved-configuration-options-3635b56aba3072c9.yaml` & `glance_store-4.8.0/releasenotes/notes/improved-configuration-options-3635b56aba3072c9.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/notes/multi-store-0c004fc8aba2a25d.yaml` & `glance_store-4.8.0/releasenotes/notes/multi-store-0c004fc8aba2a25d.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/notes/multihash-support-629e9cbc283a8b47.yaml` & `glance_store-4.8.0/releasenotes/notes/multihash-support-629e9cbc283a8b47.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/notes/pike-relnote-9f547df14184d18c.yaml` & `glance_store-4.8.0/releasenotes/notes/pike-relnote-9f547df14184d18c.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/notes/prevent-unauthorized-errors-ebb9cf2236595cd0.yaml` & `glance_store-4.8.0/releasenotes/notes/prevent-unauthorized-errors-ebb9cf2236595cd0.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/notes/queens-relnote-5fa2d009d9a9e458.yaml` & `glance_store-4.8.0/releasenotes/notes/queens-relnote-5fa2d009d9a9e458.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/notes/release-1.0.0-7ab43e91523eb3c8.yaml` & `glance_store-4.8.0/releasenotes/notes/release-1.0.0-7ab43e91523eb3c8.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/notes/release-1.0.1-098b1487ac8cc9a1.yaml` & `glance_store-4.8.0/releasenotes/notes/release-1.0.1-098b1487ac8cc9a1.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/notes/release-1.2.0-8d239f01cd8ff0bf.yaml` & `glance_store-4.8.0/releasenotes/notes/release-1.2.0-8d239f01cd8ff0bf.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/notes/releasenote-0.17.0-efee3f557ea2096a.yaml` & `glance_store-4.8.0/releasenotes/notes/releasenote-0.17.0-efee3f557ea2096a.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/notes/remove-s3-driver-f432afa1f53ecdf8.yaml` & `glance_store-4.8.0/releasenotes/notes/remove-s3-driver-f432afa1f53ecdf8.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/notes/sorted-drivers-for-configs-a905f07d3bf9c973.yaml` & `glance_store-4.8.0/releasenotes/notes/sorted-drivers-for-configs-a905f07d3bf9c973.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/notes/volume-type-validation-check-011a400d7fb3b307.yaml` & `glance_store-4.8.0/releasenotes/notes/volume-type-validation-check-011a400d7fb3b307.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/notes/xena-final-release-3c6e19dfba43b40d.yaml` & `glance_store-4.8.0/releasenotes/notes/xena-final-release-3c6e19dfba43b40d.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/source/conf.py` & `glance_store-4.8.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po` & `glance_store-4.8.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `glance_store-4.8.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po` & `glance_store-4.8.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/setup.cfg` & `glance_store-4.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/setup.py` & `glance_store-4.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/test-requirements.txt` & `glance_store-4.8.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `glance_store-4.7.0/tox.ini` & `glance_store-4.8.0/tox.ini`

 * *Files identical despite different names*

