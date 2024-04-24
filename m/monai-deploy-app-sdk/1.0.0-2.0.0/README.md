# Comparing `tmp/monai_deploy_app_sdk-1.0.0-py3-none-any.whl.zip` & `tmp/monai_deploy_app_sdk-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,66 +1,66 @@
-Zip file size: 132371 bytes, number of entries: 64
--rw-rw-r--  2.0 unx      832 b- defN 24-Mar-28 01:46 monai/deploy/__init__.py
--rw-rw-r--  2.0 unx      497 b- defN 24-Apr-11 21:37 monai/deploy/_version.py
--rw-rw-r--  2.0 unx      496 b- defN 24-Mar-28 00:46 monai/deploy/_version_1.0.py
--rw-rw-r--  2.0 unx     1359 b- defN 23-Sep-01 03:58 monai/deploy/exceptions.py
--rw-r--r--  2.0 unx      665 b- defN 23-Sep-01 03:58 monai/deploy/logging.json
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-30 23:50 monai/deploy/py.typed
--rw-rw-r--  2.0 unx      324 b- defN 24-Apr-10 00:08 monai/deploy/conditions/__init__.py
--rw-rw-r--  2.0 unx     1592 b- defN 23-Sep-01 03:58 monai/deploy/core/__init__.py
--rw-rw-r--  2.0 unx     3380 b- defN 23-Sep-01 03:58 monai/deploy/core/app_context.py
--rw-rw-r--  2.0 unx     3684 b- defN 23-Sep-01 03:58 monai/deploy/core/arg_parser.py
--rw-rw-r--  2.0 unx      741 b- defN 23-Sep-01 03:58 monai/deploy/core/io_type.py
--rw-rw-r--  2.0 unx     1472 b- defN 23-Sep-01 03:58 monai/deploy/core/runtime_env.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Sep-01 03:58 monai/deploy/core/datastores/__init__.py
--rw-rw-r--  2.0 unx     2062 b- defN 23-Sep-01 03:58 monai/deploy/core/datastores/datastore.py
--rw-rw-r--  2.0 unx     1522 b- defN 23-Sep-01 03:58 monai/deploy/core/datastores/factory.py
--rw-rw-r--  2.0 unx     1258 b- defN 23-Sep-01 03:58 monai/deploy/core/datastores/memory.py
--rw-rw-r--  2.0 unx     1068 b- defN 23-Sep-01 03:58 monai/deploy/core/domain/__init__.py
--rw-rw-r--  2.0 unx     2901 b- defN 23-Sep-01 03:58 monai/deploy/core/domain/datapath.py
--rw-rw-r--  2.0 unx     8530 b- defN 23-Sep-01 03:58 monai/deploy/core/domain/dicom_series.py
--rw-rw-r--  2.0 unx     5605 b- defN 23-Sep-01 03:58 monai/deploy/core/domain/dicom_series_selection.py
--rw-rw-r--  2.0 unx     1963 b- defN 23-Sep-01 03:58 monai/deploy/core/domain/dicom_sop_instance.py
--rw-rw-r--  2.0 unx     3611 b- defN 23-Sep-01 03:58 monai/deploy/core/domain/dicom_study.py
--rw-rw-r--  2.0 unx     1057 b- defN 23-Sep-01 03:58 monai/deploy/core/domain/domain.py
--rw-rw-r--  2.0 unx     1863 b- defN 23-Sep-01 03:58 monai/deploy/core/domain/image.py
--rw-rw-r--  2.0 unx      950 b- defN 23-Sep-01 03:58 monai/deploy/core/models/__init__.py
--rw-rw-r--  2.0 unx     2248 b- defN 23-Sep-01 03:58 monai/deploy/core/models/factory.py
--rw-rw-r--  2.0 unx     7865 b- defN 23-Sep-01 03:58 monai/deploy/core/models/model.py
--rw-rw-r--  2.0 unx     3398 b- defN 23-Sep-01 03:58 monai/deploy/core/models/named_model.py
--rw-rw-r--  2.0 unx     4472 b- defN 23-Sep-01 03:58 monai/deploy/core/models/torch_model.py
--rw-rw-r--  2.0 unx     4650 b- defN 23-Sep-01 03:58 monai/deploy/core/models/triton_model.py
--rw-rw-r--  2.0 unx       33 b- defN 23-Sep-01 03:58 monai/deploy/executors/__init__.py
--rw-rw-r--  2.0 unx       30 b- defN 23-Sep-01 03:58 monai/deploy/graphs/__init__.py
--rw-rw-r--  2.0 unx      110 b- defN 23-Sep-01 03:58 monai/deploy/logger/__init__.py
--rw-rw-r--  2.0 unx     2378 b- defN 23-Sep-01 03:58 monai/deploy/operators/__init__.py
--rw-rw-r--  2.0 unx     6178 b- defN 23-Sep-01 03:58 monai/deploy/operators/clara_viz_operator.py
--rw-rw-r--  2.0 unx    16371 b- defN 23-Sep-01 03:58 monai/deploy/operators/dicom_data_loader_operator.py
--rw-rw-r--  2.0 unx    13996 b- defN 23-Sep-01 03:58 monai/deploy/operators/dicom_encapsulated_pdf_writer_operator.py
--rw-rw-r--  2.0 unx    22005 b- defN 23-Nov-20 02:56 monai/deploy/operators/dicom_seg_writer_operator.py
--rw-rw-r--  2.0 unx    21940 b- defN 23-Nov-16 22:03 monai/deploy/operators/dicom_seg_writer_operator_all_frames.py
--rw-rw-r--  2.0 unx    16536 b- defN 23-Sep-01 03:58 monai/deploy/operators/dicom_series_selector_operator.py
--rw-rw-r--  2.0 unx    17354 b- defN 23-Sep-01 03:58 monai/deploy/operators/dicom_series_to_volume_operator.py
--rw-rw-r--  2.0 unx    14428 b- defN 23-Sep-01 03:58 monai/deploy/operators/dicom_text_sr_writer_operator.py
--rw-rw-r--  2.0 unx    12722 b- defN 23-Sep-01 03:58 monai/deploy/operators/dicom_utils.py
--rw-rw-r--  2.0 unx     2918 b- defN 23-Sep-01 03:58 monai/deploy/operators/inference_operator.py
--rw-rw-r--  2.0 unx    40183 b- defN 23-Sep-01 03:58 monai/deploy/operators/monai_bundle_inference_operator.py
--rw-rw-r--  2.0 unx    24697 b- defN 23-Sep-01 03:58 monai/deploy/operators/monai_seg_inference_operator.py
--rw-rw-r--  2.0 unx     3898 b- defN 23-Sep-01 03:58 monai/deploy/operators/nii_data_loader_operator.py
--rw-rw-r--  2.0 unx     4664 b- defN 23-Sep-01 03:58 monai/deploy/operators/png_converter_operator.py
--rw-rw-r--  2.0 unx    23242 b- defN 24-Mar-19 23:14 monai/deploy/operators/publisher_operator.py
--rw-rw-r--  2.0 unx    18115 b- defN 23-Dec-06 04:38 monai/deploy/operators/stl_conversion_operator.py
--rw-rw-r--  2.0 unx       33 b- defN 23-Sep-01 03:58 monai/deploy/resources/__init__.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Sep-01 03:58 monai/deploy/utils/__init__.py
--rw-rw-r--  2.0 unx     2897 b- defN 23-Sep-01 03:58 monai/deploy/utils/argparse_types.py
--rw-rw-r--  2.0 unx     1140 b- defN 23-Sep-01 03:58 monai/deploy/utils/deviceutil.py
--rw-rw-r--  2.0 unx     1838 b- defN 23-Sep-01 03:58 monai/deploy/utils/fileutil.py
--rw-rw-r--  2.0 unx    17078 b- defN 23-Sep-01 03:58 monai/deploy/utils/importutil.py
--rw-rw-r--  2.0 unx     4142 b- defN 23-Sep-01 03:58 monai/deploy/utils/sizeutil.py
--rw-rw-r--  2.0 unx     2597 b- defN 23-Sep-01 03:58 monai/deploy/utils/spinner.py
--rw-rw-r--  2.0 unx     4514 b- defN 23-Sep-01 03:58 monai/deploy/utils/version.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Apr-11 21:37 monai_deploy_app_sdk-1.0.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     7611 b- defN 24-Apr-11 21:37 monai_deploy_app_sdk-1.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-11 21:37 monai_deploy_app_sdk-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 24-Apr-11 21:37 monai_deploy_app_sdk-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6071 b- defN 24-Apr-11 21:37 monai_deploy_app_sdk-1.0.0.dist-info/RECORD
-64 files, 392029 bytes uncompressed, 122507 bytes compressed:  68.8%
+Zip file size: 132595 bytes, number of entries: 64
+-rw-rw-r--  2.0 unx      832 b- defN 24-Apr-16 23:22 monai/deploy/__init__.py
+-rw-rw-r--  2.0 unx      497 b- defN 24-Apr-24 23:21 monai/deploy/_version.py
+-rw-rw-r--  2.0 unx      496 b- defN 24-Apr-22 23:34 monai/deploy/_version_1.0.py
+-rw-rw-r--  2.0 unx     1359 b- defN 24-Apr-12 00:06 monai/deploy/exceptions.py
+-rw-rw-r--  2.0 unx      665 b- defN 24-Apr-12 00:06 monai/deploy/logging.json
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-12 00:06 monai/deploy/py.typed
+-rw-rw-r--  2.0 unx      324 b- defN 24-Apr-16 23:22 monai/deploy/conditions/__init__.py
+-rw-rw-r--  2.0 unx     1592 b- defN 24-Apr-16 23:22 monai/deploy/core/__init__.py
+-rw-rw-r--  2.0 unx     3380 b- defN 24-Apr-16 23:22 monai/deploy/core/app_context.py
+-rw-rw-r--  2.0 unx     3684 b- defN 24-Apr-16 23:22 monai/deploy/core/arg_parser.py
+-rw-rw-r--  2.0 unx      741 b- defN 24-Apr-16 23:22 monai/deploy/core/io_type.py
+-rw-rw-r--  2.0 unx     1472 b- defN 24-Apr-16 23:22 monai/deploy/core/runtime_env.py
+-rw-rw-r--  2.0 unx      790 b- defN 24-Apr-12 00:06 monai/deploy/core/datastores/__init__.py
+-rw-rw-r--  2.0 unx     2062 b- defN 24-Apr-12 00:06 monai/deploy/core/datastores/datastore.py
+-rw-rw-r--  2.0 unx     1522 b- defN 24-Apr-12 00:06 monai/deploy/core/datastores/factory.py
+-rw-rw-r--  2.0 unx     1258 b- defN 24-Apr-12 00:06 monai/deploy/core/datastores/memory.py
+-rw-rw-r--  2.0 unx     1068 b- defN 24-Apr-12 00:06 monai/deploy/core/domain/__init__.py
+-rw-rw-r--  2.0 unx     2901 b- defN 24-Apr-16 23:22 monai/deploy/core/domain/datapath.py
+-rw-rw-r--  2.0 unx     8530 b- defN 24-Apr-12 00:06 monai/deploy/core/domain/dicom_series.py
+-rw-rw-r--  2.0 unx     5605 b- defN 24-Apr-12 00:06 monai/deploy/core/domain/dicom_series_selection.py
+-rw-rw-r--  2.0 unx     1963 b- defN 24-Apr-12 00:06 monai/deploy/core/domain/dicom_sop_instance.py
+-rw-rw-r--  2.0 unx     3611 b- defN 24-Apr-12 00:06 monai/deploy/core/domain/dicom_study.py
+-rw-rw-r--  2.0 unx     1057 b- defN 24-Apr-12 00:06 monai/deploy/core/domain/domain.py
+-rw-rw-r--  2.0 unx     1863 b- defN 24-Apr-12 00:06 monai/deploy/core/domain/image.py
+-rw-rw-r--  2.0 unx      950 b- defN 24-Apr-12 00:06 monai/deploy/core/models/__init__.py
+-rw-rw-r--  2.0 unx     2248 b- defN 24-Apr-12 00:06 monai/deploy/core/models/factory.py
+-rw-rw-r--  2.0 unx     7865 b- defN 24-Apr-16 23:22 monai/deploy/core/models/model.py
+-rw-rw-r--  2.0 unx     3398 b- defN 24-Apr-16 23:22 monai/deploy/core/models/named_model.py
+-rw-rw-r--  2.0 unx     4472 b- defN 24-Apr-12 00:06 monai/deploy/core/models/torch_model.py
+-rw-rw-r--  2.0 unx     4650 b- defN 24-Apr-12 00:06 monai/deploy/core/models/triton_model.py
+-rw-rw-r--  2.0 unx       33 b- defN 24-Apr-16 23:22 monai/deploy/executors/__init__.py
+-rw-rw-r--  2.0 unx       30 b- defN 24-Apr-16 23:22 monai/deploy/graphs/__init__.py
+-rw-rw-r--  2.0 unx      110 b- defN 24-Apr-16 23:22 monai/deploy/logger/__init__.py
+-rw-rw-r--  2.0 unx     2378 b- defN 24-Apr-16 23:22 monai/deploy/operators/__init__.py
+-rw-rw-r--  2.0 unx     6178 b- defN 24-Apr-16 23:22 monai/deploy/operators/clara_viz_operator.py
+-rw-rw-r--  2.0 unx    17228 b- defN 24-Apr-24 18:24 monai/deploy/operators/dicom_data_loader_operator.py
+-rw-rw-r--  2.0 unx    13996 b- defN 24-Apr-16 23:22 monai/deploy/operators/dicom_encapsulated_pdf_writer_operator.py
+-rw-rw-r--  2.0 unx    22005 b- defN 24-Apr-16 23:22 monai/deploy/operators/dicom_seg_writer_operator.py
+-rw-rw-r--  2.0 unx    21940 b- defN 24-Apr-12 00:06 monai/deploy/operators/dicom_seg_writer_operator_all_frames.py
+-rw-rw-r--  2.0 unx    16536 b- defN 24-Apr-16 23:22 monai/deploy/operators/dicom_series_selector_operator.py
+-rw-rw-r--  2.0 unx    17354 b- defN 24-Apr-16 23:22 monai/deploy/operators/dicom_series_to_volume_operator.py
+-rw-rw-r--  2.0 unx    14428 b- defN 24-Apr-16 23:22 monai/deploy/operators/dicom_text_sr_writer_operator.py
+-rw-rw-r--  2.0 unx    12722 b- defN 24-Apr-16 23:22 monai/deploy/operators/dicom_utils.py
+-rw-rw-r--  2.0 unx     2918 b- defN 24-Apr-16 23:22 monai/deploy/operators/inference_operator.py
+-rw-rw-r--  2.0 unx    40183 b- defN 24-Apr-16 23:22 monai/deploy/operators/monai_bundle_inference_operator.py
+-rw-rw-r--  2.0 unx    24697 b- defN 24-Apr-16 23:22 monai/deploy/operators/monai_seg_inference_operator.py
+-rw-rw-r--  2.0 unx     3898 b- defN 24-Apr-16 23:22 monai/deploy/operators/nii_data_loader_operator.py
+-rw-rw-r--  2.0 unx     4664 b- defN 24-Apr-16 23:22 monai/deploy/operators/png_converter_operator.py
+-rw-rw-r--  2.0 unx    23242 b- defN 24-Apr-16 23:22 monai/deploy/operators/publisher_operator.py
+-rw-rw-r--  2.0 unx    18115 b- defN 24-Apr-16 23:22 monai/deploy/operators/stl_conversion_operator.py
+-rw-rw-r--  2.0 unx       33 b- defN 24-Apr-16 23:22 monai/deploy/resources/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-12 00:06 monai/deploy/utils/__init__.py
+-rw-rw-r--  2.0 unx     2897 b- defN 24-Apr-16 23:22 monai/deploy/utils/argparse_types.py
+-rw-rw-r--  2.0 unx     1140 b- defN 24-Apr-16 23:22 monai/deploy/utils/deviceutil.py
+-rw-rw-r--  2.0 unx     1838 b- defN 24-Apr-12 00:06 monai/deploy/utils/fileutil.py
+-rw-rw-r--  2.0 unx    17078 b- defN 24-Apr-16 23:22 monai/deploy/utils/importutil.py
+-rw-rw-r--  2.0 unx     4142 b- defN 24-Apr-16 23:22 monai/deploy/utils/sizeutil.py
+-rw-rw-r--  2.0 unx     2597 b- defN 24-Apr-12 00:06 monai/deploy/utils/spinner.py
+-rw-rw-r--  2.0 unx     4514 b- defN 24-Apr-16 23:22 monai/deploy/utils/version.py
+-rw-rw-r--  2.0 unx    11357 b- defN 24-Apr-24 23:21 monai_deploy_app_sdk-2.0.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     7611 b- defN 24-Apr-24 23:21 monai_deploy_app_sdk-2.0.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-24 23:21 monai_deploy_app_sdk-2.0.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 24-Apr-24 23:21 monai_deploy_app_sdk-2.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6071 b- defN 24-Apr-24 23:21 monai_deploy_app_sdk-2.0.0.dist-info/RECORD
+64 files, 392886 bytes uncompressed, 122731 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -171,23 +171,23 @@
 
 Filename: monai/deploy/utils/spinner.py
 Comment: 
 
 Filename: monai/deploy/utils/version.py
 Comment: 
 
-Filename: monai_deploy_app_sdk-1.0.0.dist-info/LICENSE
+Filename: monai_deploy_app_sdk-2.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: monai_deploy_app_sdk-1.0.0.dist-info/METADATA
+Filename: monai_deploy_app_sdk-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: monai_deploy_app_sdk-1.0.0.dist-info/WHEEL
+Filename: monai_deploy_app_sdk-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: monai_deploy_app_sdk-1.0.0.dist-info/top_level.txt
+Filename: monai_deploy_app_sdk-2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: monai_deploy_app_sdk-1.0.0.dist-info/RECORD
+Filename: monai_deploy_app_sdk-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## monai/deploy/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2024-04-11T14:37:33-0700",
+ "date": "2024-04-24T16:20:37-0700",
  "dirty": false,
  "error": null,
- "full-revisionid": "24762f85bbf4874cfd0a46a3ad4471a2bbb9cbd9",
- "version": "1.0.0"
+ "full-revisionid": "d0760904a1248ce316ae0237c8a1127ac5673d7f",
+ "version": "2.0.0"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## monai/deploy/_version_1.0.py

```diff
@@ -3,18 +3,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = """
 {
- "date": "2024-03-27T21:54:08-0700",
+ "date": "2024-04-11T14:37:33-0700",
  "dirty": false,
  "error": null,
- "full-revisionid": "95f5ec64d53fabfa9da3066644c681854befe44f",
+ "full-revisionid": "24762f85bbf4874cfd0a46a3ad4471a2bbb9cbd9",
  "version": "1.0.0"
 }
 """  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## monai/deploy/operators/dicom_data_loader_operator.py

```diff
@@ -38,14 +38,17 @@
 
     Name Output:
         dicom_study_list: A list of DICOMStudy objects in memory. The name can be changed via attribute, `output_name`.
     """
 
     DEFAULT_INPUT_FOLDER = Path.cwd() / "input"
     DEFAULT_OUTPUT_NAME = "dicom_study_list"
+    SOP_CLASSES_TO_IGNORE = [
+        "1.2.840.10008.1.3.10",  # Media Storage Directory Storage, aka DICOMDIR
+    ]
 
     # For now, need to have the input folder as an instance attribute, set on init, because even there is the optional
     # named input to receive data containing the path, there might not be upstream operator to emit the data.
     def __init__(
         self,
         fragment: Fragment,
         *args,
@@ -166,14 +169,26 @@
                 sop_instances.append(dcmread(file))
             except InvalidDicomError as ex:
                 self._logger.warn(f"Ignored {file}, reason being: {ex}")
 
         for sop_instance in sop_instances:
             study_instance_uid = sop_instance[0x0020, 0x000D].value.name  # name is the UID as str
 
+            # First need to eliminate the SOP instances whose SOP Class is to be ignored.
+            if "SOPInstanceUID" not in sop_instance:
+                self._logger.warn("Instance ignored due to missing SOP instance UID tag")
+                continue
+            sop_instance_uid = sop_instance["SOPInstanceUID"].value
+            if "SOPClassUID" not in sop_instance:
+                self._logger.warn(f"Instance ignored due to missing SOP Class UID tag, {sop_instance_uid}")
+                continue
+            if sop_instance["SOPClassUID"].value in DICOMDataLoaderOperator.SOP_CLASSES_TO_IGNORE:
+                self._logger.warn(f"Instance ignored for being in the ignored class, {sop_instance_uid}")
+                continue
+
             if study_instance_uid not in study_dict:
                 study = DICOMStudy(study_instance_uid)
                 self.populate_study_attributes(study, sop_instance)
                 study_dict[study_instance_uid] = study
 
             series_instance_uid = sop_instance[0x0020, 0x000E].value.name  # name is the UID as str
```

## Comparing `monai_deploy_app_sdk-1.0.0.dist-info/LICENSE` & `monai_deploy_app_sdk-2.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `monai_deploy_app_sdk-1.0.0.dist-info/METADATA` & `monai_deploy_app_sdk-2.0.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: monai-deploy-app-sdk
-Version: 1.0.0
+Version: 2.0.0
 Summary: A framework and associated tools to design, verify and analyze performance of MONAI apps
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/projects/monai-deploy-app-sdk/en/stable/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/monai-deploy-app-sdk/issues
 Project-URL: Source Code, https://github.com/Project-MONAI/monai-deploy-app-sdk
 Platform: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 Requires-Dist: numpy >=1.21.6
-Requires-Dist: holoscan ~=1.0
+Requires-Dist: holoscan ~=2.0
 Requires-Dist: colorama >=0.4.1
 Requires-Dist: typeguard >=3.0.0
 Provides-Extra: all
 Requires-Dist: cucim ~=21.06 ; extra == 'all'
 Provides-Extra: cucim
 Requires-Dist: cucim ~=21.06 ; extra == 'cucim'
```

## Comparing `monai_deploy_app_sdk-1.0.0.dist-info/RECORD` & `monai_deploy_app_sdk-2.0.0.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 monai/deploy/__init__.py,sha256=DXLIYcUMLcOsT6XIjDWqmGdpzaUPe-qj8PxVYSMMl1E,832
-monai/deploy/_version.py,sha256=N_auHepqoE2sx9B5nEcyFC-9iO4wSuFxfnpr5PIHyjQ,497
-monai/deploy/_version_1.0.py,sha256=yHsRFOvx_TjaPIv2EGhrg2XtE6WExFTqUlWqbqD0Npg,496
+monai/deploy/_version.py,sha256=9qPD8dGC3Ks14qJc_Ft_w6umpDpM4VrMS1x6rbe0RcM,497
+monai/deploy/_version_1.0.py,sha256=Aed4hSgNtfHgAOfybAAw_psLVH_gkCV_cpVNFOrn-Rw,496
 monai/deploy/exceptions.py,sha256=8o4Xym6WQktL2FRiei7D06Jr9zlrNu91aIHc4bWNCdw,1359
 monai/deploy/logging.json,sha256=50nU8-uOWnPkw9JHXySMscMOFdB-W0rELBRPmDfw04g,665
 monai/deploy/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 monai/deploy/conditions/__init__.py,sha256=50y80pXBcTJqS3nplAKIuF3qr12G1AniQluDJZE3Bi0,324
 monai/deploy/core/__init__.py,sha256=aa2nAaqRA7goOdoPIJISgP1dmfNnWChFookU4TZYF30,1592
 monai/deploy/core/app_context.py,sha256=I-FmQO4SSWmWm3MPou9qZUVGUrYYiOf0oqsurhk4DzI,3380
 monai/deploy/core/arg_parser.py,sha256=BPO3NqI9CdpdWJxEb5X8J4aR30YkavjlMe4XP3knmAI,3684
@@ -29,15 +29,15 @@
 monai/deploy/core/models/torch_model.py,sha256=tkqSnkMOdprTcTUbfXZaNRCuOd3d_uak2xLd7Psw4gI,4472
 monai/deploy/core/models/triton_model.py,sha256=PpK9_bwJ1YidjAKsxwuJXLopEyfUWzn_iitaeKvwFCA,4650
 monai/deploy/executors/__init__.py,sha256=jF9ZoW2aUeLjnnS5-VS8GtiHKJE7fl8SM-SKf7dxxtM,33
 monai/deploy/graphs/__init__.py,sha256=rgFo8AvtKZCsA2_NWNDQ5cHWtg7sQ1PS2j4DmYIAw8w,30
 monai/deploy/logger/__init__.py,sha256=lShzexwc5OqkxSaR7r7iL6CubSwsfkmEUW7E350N_Ww,110
 monai/deploy/operators/__init__.py,sha256=fIEeFBRPwVLkuV7vfnK-1xpx4RWno6G23OZhvnYMams,2378
 monai/deploy/operators/clara_viz_operator.py,sha256=8yrl78CfAN8qLlqhQCG4NQguuYHTpX8C2upPVcVDPJQ,6178
-monai/deploy/operators/dicom_data_loader_operator.py,sha256=Fz0Wdh1zc3FYjmgUZiftfCkXT7juMsUxz2chg4G4xFQ,16371
+monai/deploy/operators/dicom_data_loader_operator.py,sha256=DjagEiS1IyEgVXxC6hh_KIfrYXMj1gWWbb6F0Jr5ZG0,17228
 monai/deploy/operators/dicom_encapsulated_pdf_writer_operator.py,sha256=gAB4b_ONCwqMDJKdBCUIOSrhALtucMcWwDH1GIOjGn4,13996
 monai/deploy/operators/dicom_seg_writer_operator.py,sha256=TL4Zd9JkVFi21OxD1yrk7FHcRPl2RrqxEQnEvtchZVY,22005
 monai/deploy/operators/dicom_seg_writer_operator_all_frames.py,sha256=lrbI861Hf3DjYj5EDFTft-Bm7dWnBA8AdjeGpBj9hO4,21940
 monai/deploy/operators/dicom_series_selector_operator.py,sha256=vwWwhThak1XITXgFYWeWV_CZmMQLudkP13CeTPEWGf8,16536
 monai/deploy/operators/dicom_series_to_volume_operator.py,sha256=Rv0UVNLD234FtBFIxTTq2pgffTvK8uNpllwwZ8vcoLw,17354
 monai/deploy/operators/dicom_text_sr_writer_operator.py,sha256=99pMWBuO2xbWGFiEUcsN-dM96jrZEJZsOiVQvymeVtY,14428
 monai/deploy/operators/dicom_utils.py,sha256=gX2kQ7Ug-gYG0mMYJ_qth9m1_snvEomxaocYDC0-cvQ,12722
@@ -53,12 +53,12 @@
 monai/deploy/utils/argparse_types.py,sha256=zCg8E61qQA8IRBmX708TMFNyAiMnZBw3aoRvXeFafls,2897
 monai/deploy/utils/deviceutil.py,sha256=hXmkMaKuHxrmpoKuc4tExr7BB7zOQIqnPLncznZzkuk,1140
 monai/deploy/utils/fileutil.py,sha256=9ep1glfCrCm-h85x5j_TKVs9KwxYTWrOtr_JV4Kb3Z0,1838
 monai/deploy/utils/importutil.py,sha256=5LKIac9aLAZZPPlSwokFu8YbB5jxhOow1fKjVOdZTSY,17078
 monai/deploy/utils/sizeutil.py,sha256=yej-GxO3NlguVhyy8WjcZB-Ard49eubtxAi90z0v5UE,4142
 monai/deploy/utils/spinner.py,sha256=PpqAE2CfBXEw1qEWUP9woW-vw28L4Tyn5AUeWsbnXwc,2597
 monai/deploy/utils/version.py,sha256=mSZ95TI2YV8Grxc7fUO-LISGK_GB6pe_tWF9Q-Ezdoc,4514
-monai_deploy_app_sdk-1.0.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-monai_deploy_app_sdk-1.0.0.dist-info/METADATA,sha256=NI1kZ_V2l4qT3Mc1XXruB0wfsL23F8BTvpMiFROyl2s,7611
-monai_deploy_app_sdk-1.0.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-monai_deploy_app_sdk-1.0.0.dist-info/top_level.txt,sha256=UaNwRzLGORdus41Ip446s3bBfViLkdkDsXDo34J2P44,6
-monai_deploy_app_sdk-1.0.0.dist-info/RECORD,,
+monai_deploy_app_sdk-2.0.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+monai_deploy_app_sdk-2.0.0.dist-info/METADATA,sha256=Bmb529eQyG9QADEd-j7mCFWU5oeI-P1lxUPhNHLAdUI,7611
+monai_deploy_app_sdk-2.0.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+monai_deploy_app_sdk-2.0.0.dist-info/top_level.txt,sha256=UaNwRzLGORdus41Ip446s3bBfViLkdkDsXDo34J2P44,6
+monai_deploy_app_sdk-2.0.0.dist-info/RECORD,,
```

