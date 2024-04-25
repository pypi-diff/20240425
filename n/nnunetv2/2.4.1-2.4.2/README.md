# Comparing `tmp/nnunetv2-2.4.1.tar.gz` & `tmp/nnunetv2-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnunetv2-2.4.1.tar", last modified: Thu Apr 18 12:39:05 2024, max compression
+gzip compressed data, was "nnunetv2-2.4.2.tar", last modified: Thu Apr 25 09:15:30 2024, max compression
```

## Comparing `nnunetv2-2.4.1.tar` & `nnunetv2-2.4.2.tar`

### file list

```diff
@@ -1,226 +1,226 @@
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.970145 nnunetv2-2.4.1/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    11427 2023-03-17 08:55:29.000000 nnunetv2-2.4.1/LICENSE
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    24713 2024-04-18 12:39:05.970145 nnunetv2-2.4.1/PKG-INFO
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.954144 nnunetv2-2.4.1/nnunetv2/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/__init__.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.954144 nnunetv2-2.4.1/nnunetv2/batch_running/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/batch_running/__init__.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.954144 nnunetv2-2.4.1/nnunetv2/batch_running/benchmarking/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/batch_running/benchmarking/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2041 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/batch_running/benchmarking/generate_benchmarking_commands.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3272 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/batch_running/benchmarking/summarize_benchmark_results.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     5798 2024-04-18 10:12:32.000000 nnunetv2-2.4.1/nnunetv2/batch_running/collect_results_custom_Decathlon.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      708 2024-04-18 10:12:32.000000 nnunetv2-2.4.1/nnunetv2/batch_running/collect_results_custom_Decathlon_2d.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3300 2024-04-18 10:12:32.000000 nnunetv2-2.4.1/nnunetv2/batch_running/generate_lsf_runs_customDecathlon.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.954144 nnunetv2-2.4.1/nnunetv2/batch_running/release_trainings/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/batch_running/release_trainings/__init__.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.954144 nnunetv2-2.4.1/nnunetv2/batch_running/release_trainings/nnunetv2_v1/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/batch_running/release_trainings/nnunetv2_v1/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     5662 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/batch_running/release_trainings/nnunetv2_v1/collect_results.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3833 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/batch_running/release_trainings/nnunetv2_v1/generate_lsf_commands.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      416 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/configuration.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.958145 nnunetv2-2.4.1/nnunetv2/dataset_conversion/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     4545 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset027_ACDC.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     4162 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset073_Fluo_C3DH_A549_SIM.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     9018 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset114_MNMs.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2406 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset115_EMIDEC.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3430 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset120_RoadSegmentation.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3994 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset137_BraTS21.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3742 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset218_Amos2022_task1.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3555 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset219_Amos2022_task2.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2080 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset220_KiTS2023.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3167 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset221_AutoPETII_2023.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2653 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset223_AMOS2022postChallenge.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1369 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset988_dummyDataset4.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/dataset_conversion/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     6074 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/dataset_conversion/convert_MSD_dataset.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2930 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/dataset_conversion/convert_raw_dataset_from_old_nnunet_format.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.958145 nnunetv2-2.4.1/nnunetv2/dataset_conversion/datasets_for_integration_tests/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3250 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset996_IntegrationTest_Hippocampus_regions_ignore.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1468 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset997_IntegrationTest_Hippocampus_regions.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1364 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset998_IntegrationTest_Hippocampus_ignore.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1085 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset999_IntegrationTest_Hippocampus.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/dataset_conversion/datasets_for_integration_tests/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     4045 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/dataset_conversion/generate_dataset_json.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.958145 nnunetv2-2.4.1/nnunetv2/ensembling/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/ensembling/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    10027 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/ensembling/ensemble.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.958145 nnunetv2-2.4.1/nnunetv2/evaluation/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/evaluation/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3273 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/evaluation/accumulate_cv_results.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    12556 2024-04-18 10:12:32.000000 nnunetv2-2.4.1/nnunetv2/evaluation/evaluate_predictions.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    18653 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/evaluation/find_best_configuration.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.958145 nnunetv2-2.4.1/nnunetv2/experiment_planning/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/experiment_planning/__init__.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.958145 nnunetv2-2.4.1/nnunetv2/experiment_planning/dataset_fingerprint/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/experiment_planning/dataset_fingerprint/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    11935 2024-04-18 09:53:09.000000 nnunetv2-2.4.1/nnunetv2/experiment_planning/dataset_fingerprint/fingerprint_extractor.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.958145 nnunetv2-2.4.1/nnunetv2/experiment_planning/experiment_planners/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/experiment_planning/experiment_planners/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    33576 2024-04-18 10:12:32.000000 nnunetv2-2.4.1/nnunetv2/experiment_planning/experiment_planners/default_experiment_planner.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3928 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/experiment_planning/experiment_planners/network_topology.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    14292 2024-04-18 09:53:09.000000 nnunetv2-2.4.1/nnunetv2/experiment_planning/experiment_planners/resencUNet_planner.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.958145 nnunetv2-2.4.1/nnunetv2/experiment_planning/experiment_planners/residual_unets/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-18 09:53:09.000000 nnunetv2-2.4.1/nnunetv2/experiment_planning/experiment_planners/residual_unets/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    18309 2024-04-18 09:53:09.000000 nnunetv2-2.4.1/nnunetv2/experiment_planning/experiment_planners/residual_unets/residual_encoder_unet_planners.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     8566 2024-04-18 09:53:09.000000 nnunetv2-2.4.1/nnunetv2/experiment_planning/plan_and_preprocess_api.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    16650 2024-04-18 09:53:09.000000 nnunetv2-2.4.1/nnunetv2/experiment_planning/plan_and_preprocess_entrypoints.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.958145 nnunetv2-2.4.1/nnunetv2/experiment_planning/plans_for_pretraining/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/experiment_planning/plans_for_pretraining/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     4469 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/experiment_planning/plans_for_pretraining/move_plans_between_datasets.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    12234 2024-04-18 09:53:09.000000 nnunetv2-2.4.1/nnunetv2/experiment_planning/verify_dataset_integrity.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.958145 nnunetv2-2.4.1/nnunetv2/imageio/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/imageio/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     5626 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/imageio/base_reader_writer.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3344 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/imageio/natural_image_reader_writer.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     8639 2024-04-18 09:53:09.000000 nnunetv2-2.4.1/nnunetv2/imageio/nibabel_reader_writer.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3865 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/imageio/reader_writer_registry.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     5665 2024-04-18 09:53:09.000000 nnunetv2-2.4.1/nnunetv2/imageio/simpleitk_reader_writer.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     4731 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/imageio/tif_reader_writer.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.962144 nnunetv2-2.4.1/nnunetv2/inference/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/inference/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    16219 2024-04-18 09:53:09.000000 nnunetv2-2.4.1/nnunetv2/inference/data_iterators.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     6488 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/inference/examples.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     8259 2024-04-18 12:33:09.000000 nnunetv2-2.4.1/nnunetv2/inference/export_prediction.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    56414 2024-04-18 10:12:32.000000 nnunetv2-2.4.1/nnunetv2/inference/predict_from_raw_data.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2895 2024-04-18 09:53:09.000000 nnunetv2-2.4.1/nnunetv2/inference/sliding_window_prediction.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.962144 nnunetv2-2.4.1/nnunetv2/model_sharing/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/model_sharing/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3528 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/model_sharing/entry_points.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1856 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/model_sharing/model_download.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     6830 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/model_sharing/model_export.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      202 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/model_sharing/model_import.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1865 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/paths.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.962144 nnunetv2-2.4.1/nnunetv2/postprocessing/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/postprocessing/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    20662 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/postprocessing/remove_connected_components.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.962144 nnunetv2-2.4.1/nnunetv2/preprocessing/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/preprocessing/__init__.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.962144 nnunetv2-2.4.1/nnunetv2/preprocessing/cropping/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/preprocessing/cropping/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1274 2024-04-18 09:53:09.000000 nnunetv2-2.4.1/nnunetv2/preprocessing/cropping/cropping.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.962144 nnunetv2-2.4.1/nnunetv2/preprocessing/normalization/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/preprocessing/normalization/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     4145 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/preprocessing/normalization/default_normalization_schemes.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      976 2024-04-18 09:53:09.000000 nnunetv2-2.4.1/nnunetv2/preprocessing/normalization/map_channel_name_to_normalization.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.962144 nnunetv2-2.4.1/nnunetv2/preprocessing/preprocessors/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/preprocessing/preprocessors/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    16266 2024-04-18 12:33:09.000000 nnunetv2-2.4.1/nnunetv2/preprocessing/preprocessors/default_preprocessor.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.962144 nnunetv2-2.4.1/nnunetv2/preprocessing/resampling/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/preprocessing/resampling/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     9599 2024-04-18 10:12:32.000000 nnunetv2-2.4.1/nnunetv2/preprocessing/resampling/default_resampling.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      713 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/preprocessing/resampling/utils.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.962144 nnunetv2-2.4.1/nnunetv2/run/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/run/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3345 2024-04-18 08:44:04.000000 nnunetv2-2.4.1/nnunetv2/run/load_pretrained_weights.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    14405 2024-04-18 12:33:09.000000 nnunetv2-2.4.1/nnunetv2/run/run_training.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.962144 nnunetv2-2.4.1/nnunetv2/tests/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/tests/__init__.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.962144 nnunetv2-2.4.1/nnunetv2/tests/integration_tests/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/tests/integration_tests/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1550 2024-04-18 12:33:09.000000 nnunetv2-2.4.1/nnunetv2/tests/integration_tests/add_lowres_and_cascade.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      659 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/tests/integration_tests/cleanup_integration_test.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     4244 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/tests/integration_tests/run_integration_test_bestconfig_inference.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.962144 nnunetv2-2.4.1/nnunetv2/training/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/__init__.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.962144 nnunetv2-2.4.1/nnunetv2/training/data_augmentation/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/data_augmentation/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1157 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/data_augmentation/compute_initial_patch_size.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.962144 nnunetv2-2.4.1/nnunetv2/training/data_augmentation/custom_transforms/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/data_augmentation/custom_transforms/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     7310 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/data_augmentation/custom_transforms/cascade_transforms.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2601 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/data_augmentation/custom_transforms/deep_supervision_donwsampling.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      349 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/data_augmentation/custom_transforms/limited_length_multithreaded_augmenter.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      326 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/data_augmentation/custom_transforms/manipulating_data_dict.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      893 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/data_augmentation/custom_transforms/masking.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1665 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/data_augmentation/custom_transforms/region_based_training.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2455 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/data_augmentation/custom_transforms/transforms_for_dummy_2d.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.966144 nnunetv2-2.4.1/nnunetv2/training/dataloading/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/dataloading/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     8214 2024-04-18 12:33:09.000000 nnunetv2-2.4.1/nnunetv2/training/dataloading/base_data_loader.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     5638 2024-04-18 12:33:09.000000 nnunetv2-2.4.1/nnunetv2/training/dataloading/data_loader_2d.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3142 2024-04-18 12:33:09.000000 nnunetv2-2.4.1/nnunetv2/training/dataloading/data_loader_3d.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     6510 2024-04-18 12:33:09.000000 nnunetv2-2.4.1/nnunetv2/training/dataloading/nnunet_dataset.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3393 2024-04-18 12:33:09.000000 nnunetv2-2.4.1/nnunetv2/training/dataloading/utils.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.966144 nnunetv2-2.4.1/nnunetv2/training/logging/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/logging/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     4718 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/logging/nnunet_logger.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.966144 nnunetv2-2.4.1/nnunetv2/training/loss/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/loss/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     5924 2024-04-18 10:12:32.000000 nnunetv2-2.4.1/nnunetv2/training/loss/compound_losses.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1398 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/loss/deep_supervision.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     6681 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/loss/dice.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1153 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/loss/robust_ce_loss.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.966144 nnunetv2-2.4.1/nnunetv2/training/lr_scheduler/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/lr_scheduler/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      803 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/lr_scheduler/polylr.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.966144 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    70639 2024-04-18 12:38:00.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/nnUNetTrainer.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.966144 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/__init__.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.966144 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/benchmarking/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/benchmarking/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2858 2024-04-18 12:33:09.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/benchmarking/nnUNetTrainerBenchmark_5epochs.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2566 2024-04-18 12:33:09.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/benchmarking/nnUNetTrainerBenchmark_5epochs_noDataLoading.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.966144 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    20171 2024-04-18 12:33:09.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerDA5.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     8889 2024-04-18 10:12:32.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerDAOrd0.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2105 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerNoDA.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1230 2024-04-18 10:12:32.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerNoMirroring.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.966144 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/loss/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/loss/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1690 2024-04-18 12:33:09.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerCELoss.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3051 2024-04-18 10:12:32.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerDiceLoss.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3473 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerTopkLoss.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.966144 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/lr_schedule/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/lr_schedule/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      517 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/lr_schedule/nnUNetTrainerCosAnneal.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.966144 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/network_architecture/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/network_architecture/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1710 2024-04-18 08:44:04.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/network_architecture/nnUNetTrainerBN.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      501 2024-04-18 12:33:09.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/network_architecture/nnUNetTrainerNoDeepSupervision.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.966144 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/optimizer/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/optimizer/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2882 2024-04-18 12:33:09.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/optimizer/nnUNetTrainerAdam.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3259 2024-04-18 12:33:09.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/optimizer/nnUNetTrainerAdan.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.966144 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/sampling/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/sampling/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     5088 2024-04-18 12:33:09.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/sampling/nnUNetTrainer_probabilisticOversampling.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.966144 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/training_length/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/training_length/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3690 2024-04-18 12:33:09.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/training_length/nnUNetTrainer_Xepochs.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3157 2024-04-18 12:33:09.000000 nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/training_length/nnUNetTrainer_Xepochs_NoMirroring.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.970145 nnunetv2-2.4.1/nnunetv2/utilities/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/utilities/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      906 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/utilities/collate_outputs.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      619 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/utilities/crossval_split.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3925 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/utilities/dataset_name_id_conversion.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1748 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/utilities/ddp_allgather.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1854 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/utilities/default_n_proc_DA.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     5545 2024-04-18 10:12:32.000000 nnunetv2-2.4.1/nnunetv2/utilities/file_path_utilities.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      868 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/utilities/find_class_by_name.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     1910 2024-04-18 08:44:04.000000 nnunetv2-2.4.1/nnunetv2/utilities/get_network_from_plans.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      543 2024-04-18 10:12:32.000000 nnunetv2-2.4.1/nnunetv2/utilities/helpers.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2420 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/utilities/json_export.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.970145 nnunetv2-2.4.1/nnunetv2/utilities/label_handling/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/utilities/label_handling/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    14925 2024-04-18 10:12:32.000000 nnunetv2-2.4.1/nnunetv2/utilities/label_handling/label_handling.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      509 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/utilities/network_initialization.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    11953 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/utilities/overlay_plots.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.970145 nnunetv2-2.4.1/nnunetv2/utilities/plans_handling/
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/utilities/plans_handling/__init__.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    15055 2024-04-18 10:12:32.000000 nnunetv2-2.4.1/nnunetv2/utilities/plans_handling/plans_handler.py
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     3139 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/nnunetv2/utilities/utils.py
-drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-18 12:39:05.954144 nnunetv2-2.4.1/nnunetv2.egg-info/
--rw-r--r--   0 isensee   (1000) isensee   (1000)    24713 2024-04-18 12:39:05.000000 nnunetv2-2.4.1/nnunetv2.egg-info/PKG-INFO
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     9469 2024-04-18 12:39:05.000000 nnunetv2-2.4.1/nnunetv2.egg-info/SOURCES.txt
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        1 2024-04-18 12:39:05.000000 nnunetv2-2.4.1/nnunetv2.egg-info/dependency_links.txt
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     2244 2024-04-18 12:39:05.000000 nnunetv2-2.4.1/nnunetv2.egg-info/entry_points.txt
--rw-rw-r--   0 isensee   (1000) isensee   (1000)      285 2024-04-18 12:39:05.000000 nnunetv2-2.4.1/nnunetv2.egg-info/requires.txt
--rw-rw-r--   0 isensee   (1000) isensee   (1000)        9 2024-04-18 12:39:05.000000 nnunetv2-2.4.1/nnunetv2.egg-info/top_level.txt
--rw-rw-r--   0 isensee   (1000) isensee   (1000)     4218 2024-04-18 12:38:25.000000 nnunetv2-2.4.1/pyproject.toml
--rw-rw-r--   0 isensee   (1000) isensee   (1000)    10566 2024-04-18 09:53:09.000000 nnunetv2-2.4.1/readme.md
--rw-rw-r--   0 isensee   (1000) isensee   (1000)       38 2024-04-18 12:39:05.970145 nnunetv2-2.4.1/setup.cfg
--rwxrwxr-x   0 isensee   (1000) isensee   (1000)       69 2024-04-09 18:40:42.000000 nnunetv2-2.4.1/setup.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.249843 nnunetv2-2.4.2/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    11427 2023-03-17 08:55:29.000000 nnunetv2-2.4.2/LICENSE
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    24713 2024-04-25 09:15:30.249843 nnunetv2-2.4.2/PKG-INFO
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.229843 nnunetv2-2.4.2/nnunetv2/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/__init__.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.229843 nnunetv2-2.4.2/nnunetv2/batch_running/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/batch_running/__init__.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.229843 nnunetv2-2.4.2/nnunetv2/batch_running/benchmarking/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/batch_running/benchmarking/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2041 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/batch_running/benchmarking/generate_benchmarking_commands.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3272 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/batch_running/benchmarking/summarize_benchmark_results.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     5798 2024-04-20 11:06:50.000000 nnunetv2-2.4.2/nnunetv2/batch_running/collect_results_custom_Decathlon.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      708 2024-04-20 11:06:50.000000 nnunetv2-2.4.2/nnunetv2/batch_running/collect_results_custom_Decathlon_2d.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3300 2024-04-25 09:10:04.000000 nnunetv2-2.4.2/nnunetv2/batch_running/generate_lsf_runs_customDecathlon.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.229843 nnunetv2-2.4.2/nnunetv2/batch_running/release_trainings/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/batch_running/release_trainings/__init__.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.229843 nnunetv2-2.4.2/nnunetv2/batch_running/release_trainings/nnunetv2_v1/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/batch_running/release_trainings/nnunetv2_v1/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     5662 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/batch_running/release_trainings/nnunetv2_v1/collect_results.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3833 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/batch_running/release_trainings/nnunetv2_v1/generate_lsf_commands.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      416 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/configuration.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.233843 nnunetv2-2.4.2/nnunetv2/dataset_conversion/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     4545 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset027_ACDC.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     4162 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset073_Fluo_C3DH_A549_SIM.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     9018 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset114_MNMs.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2406 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset115_EMIDEC.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3430 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset120_RoadSegmentation.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3994 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset137_BraTS21.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3742 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset218_Amos2022_task1.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3555 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset219_Amos2022_task2.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2080 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset220_KiTS2023.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3167 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset221_AutoPETII_2023.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2653 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset223_AMOS2022postChallenge.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1369 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset988_dummyDataset4.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/dataset_conversion/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     6074 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/dataset_conversion/convert_MSD_dataset.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2930 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/dataset_conversion/convert_raw_dataset_from_old_nnunet_format.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.233843 nnunetv2-2.4.2/nnunetv2/dataset_conversion/datasets_for_integration_tests/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3250 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset996_IntegrationTest_Hippocampus_regions_ignore.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1468 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset997_IntegrationTest_Hippocampus_regions.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1364 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset998_IntegrationTest_Hippocampus_ignore.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1085 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset999_IntegrationTest_Hippocampus.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/dataset_conversion/datasets_for_integration_tests/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     4045 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/dataset_conversion/generate_dataset_json.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.233843 nnunetv2-2.4.2/nnunetv2/ensembling/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/ensembling/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    10027 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/ensembling/ensemble.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.233843 nnunetv2-2.4.2/nnunetv2/evaluation/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/evaluation/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3273 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/evaluation/accumulate_cv_results.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    12556 2024-04-20 11:06:50.000000 nnunetv2-2.4.2/nnunetv2/evaluation/evaluate_predictions.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    18653 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/evaluation/find_best_configuration.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.233843 nnunetv2-2.4.2/nnunetv2/experiment_planning/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/experiment_planning/__init__.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.233843 nnunetv2-2.4.2/nnunetv2/experiment_planning/dataset_fingerprint/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/experiment_planning/dataset_fingerprint/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    11935 2024-04-18 09:53:09.000000 nnunetv2-2.4.2/nnunetv2/experiment_planning/dataset_fingerprint/fingerprint_extractor.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.233843 nnunetv2-2.4.2/nnunetv2/experiment_planning/experiment_planners/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/experiment_planning/experiment_planners/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    33576 2024-04-20 11:06:50.000000 nnunetv2-2.4.2/nnunetv2/experiment_planning/experiment_planners/default_experiment_planner.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3928 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/experiment_planning/experiment_planners/network_topology.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    14292 2024-04-18 09:53:09.000000 nnunetv2-2.4.2/nnunetv2/experiment_planning/experiment_planners/resencUNet_planner.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.237843 nnunetv2-2.4.2/nnunetv2/experiment_planning/experiment_planners/residual_unets/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-20 21:08:15.000000 nnunetv2-2.4.2/nnunetv2/experiment_planning/experiment_planners/residual_unets/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    18309 2024-04-20 21:08:15.000000 nnunetv2-2.4.2/nnunetv2/experiment_planning/experiment_planners/residual_unets/residual_encoder_unet_planners.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     8566 2024-04-20 21:08:15.000000 nnunetv2-2.4.2/nnunetv2/experiment_planning/plan_and_preprocess_api.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    16650 2024-04-20 21:08:15.000000 nnunetv2-2.4.2/nnunetv2/experiment_planning/plan_and_preprocess_entrypoints.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.237843 nnunetv2-2.4.2/nnunetv2/experiment_planning/plans_for_pretraining/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/experiment_planning/plans_for_pretraining/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     4469 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/experiment_planning/plans_for_pretraining/move_plans_between_datasets.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    12234 2024-04-20 21:08:15.000000 nnunetv2-2.4.2/nnunetv2/experiment_planning/verify_dataset_integrity.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.237843 nnunetv2-2.4.2/nnunetv2/imageio/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/imageio/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     5626 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/imageio/base_reader_writer.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3344 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/imageio/natural_image_reader_writer.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     8639 2024-04-20 21:08:15.000000 nnunetv2-2.4.2/nnunetv2/imageio/nibabel_reader_writer.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3865 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/imageio/reader_writer_registry.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     5665 2024-04-20 21:08:15.000000 nnunetv2-2.4.2/nnunetv2/imageio/simpleitk_reader_writer.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     4731 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/imageio/tif_reader_writer.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.237843 nnunetv2-2.4.2/nnunetv2/inference/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/inference/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    16213 2024-04-25 07:45:48.000000 nnunetv2-2.4.2/nnunetv2/inference/data_iterators.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     6488 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/inference/examples.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     8259 2024-04-25 09:10:04.000000 nnunetv2-2.4.2/nnunetv2/inference/export_prediction.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    56414 2024-04-20 21:08:15.000000 nnunetv2-2.4.2/nnunetv2/inference/predict_from_raw_data.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2895 2024-04-20 21:08:15.000000 nnunetv2-2.4.2/nnunetv2/inference/sliding_window_prediction.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.237843 nnunetv2-2.4.2/nnunetv2/model_sharing/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/model_sharing/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3528 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/model_sharing/entry_points.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1856 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/model_sharing/model_download.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     6830 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/model_sharing/model_export.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      202 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/model_sharing/model_import.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1865 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/paths.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.237843 nnunetv2-2.4.2/nnunetv2/postprocessing/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/postprocessing/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    20662 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/postprocessing/remove_connected_components.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.237843 nnunetv2-2.4.2/nnunetv2/preprocessing/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/preprocessing/__init__.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.237843 nnunetv2-2.4.2/nnunetv2/preprocessing/cropping/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/preprocessing/cropping/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1274 2024-04-18 09:53:09.000000 nnunetv2-2.4.2/nnunetv2/preprocessing/cropping/cropping.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.241843 nnunetv2-2.4.2/nnunetv2/preprocessing/normalization/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/preprocessing/normalization/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     4145 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/preprocessing/normalization/default_normalization_schemes.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      976 2024-04-18 09:53:09.000000 nnunetv2-2.4.2/nnunetv2/preprocessing/normalization/map_channel_name_to_normalization.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.241843 nnunetv2-2.4.2/nnunetv2/preprocessing/preprocessors/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/preprocessing/preprocessors/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    16205 2024-04-25 09:10:04.000000 nnunetv2-2.4.2/nnunetv2/preprocessing/preprocessors/default_preprocessor.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.241843 nnunetv2-2.4.2/nnunetv2/preprocessing/resampling/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/preprocessing/resampling/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     9226 2024-04-25 09:10:04.000000 nnunetv2-2.4.2/nnunetv2/preprocessing/resampling/default_resampling.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      713 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/preprocessing/resampling/utils.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.241843 nnunetv2-2.4.2/nnunetv2/run/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/run/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3345 2024-04-18 08:44:04.000000 nnunetv2-2.4.2/nnunetv2/run/load_pretrained_weights.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    14405 2024-04-25 09:10:04.000000 nnunetv2-2.4.2/nnunetv2/run/run_training.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.241843 nnunetv2-2.4.2/nnunetv2/tests/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/tests/__init__.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.241843 nnunetv2-2.4.2/nnunetv2/tests/integration_tests/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/tests/integration_tests/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1550 2024-04-25 09:10:04.000000 nnunetv2-2.4.2/nnunetv2/tests/integration_tests/add_lowres_and_cascade.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      659 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/tests/integration_tests/cleanup_integration_test.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     4244 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/tests/integration_tests/run_integration_test_bestconfig_inference.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.241843 nnunetv2-2.4.2/nnunetv2/training/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/__init__.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.241843 nnunetv2-2.4.2/nnunetv2/training/data_augmentation/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/data_augmentation/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1157 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/data_augmentation/compute_initial_patch_size.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.241843 nnunetv2-2.4.2/nnunetv2/training/data_augmentation/custom_transforms/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/data_augmentation/custom_transforms/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     7310 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/data_augmentation/custom_transforms/cascade_transforms.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2601 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/data_augmentation/custom_transforms/deep_supervision_donwsampling.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      349 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/data_augmentation/custom_transforms/limited_length_multithreaded_augmenter.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      326 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/data_augmentation/custom_transforms/manipulating_data_dict.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      893 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/data_augmentation/custom_transforms/masking.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1665 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/data_augmentation/custom_transforms/region_based_training.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2455 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/data_augmentation/custom_transforms/transforms_for_dummy_2d.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.245843 nnunetv2-2.4.2/nnunetv2/training/dataloading/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/dataloading/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     8214 2024-04-25 09:10:04.000000 nnunetv2-2.4.2/nnunetv2/training/dataloading/base_data_loader.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     5638 2024-04-25 09:10:04.000000 nnunetv2-2.4.2/nnunetv2/training/dataloading/data_loader_2d.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3142 2024-04-25 09:10:04.000000 nnunetv2-2.4.2/nnunetv2/training/dataloading/data_loader_3d.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     6510 2024-04-25 09:10:04.000000 nnunetv2-2.4.2/nnunetv2/training/dataloading/nnunet_dataset.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3393 2024-04-25 09:10:04.000000 nnunetv2-2.4.2/nnunetv2/training/dataloading/utils.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.245843 nnunetv2-2.4.2/nnunetv2/training/logging/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/logging/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     4718 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/logging/nnunet_logger.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.245843 nnunetv2-2.4.2/nnunetv2/training/loss/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/loss/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     5924 2024-04-20 18:36:41.000000 nnunetv2-2.4.2/nnunetv2/training/loss/compound_losses.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1398 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/loss/deep_supervision.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     6681 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/loss/dice.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1153 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/loss/robust_ce_loss.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.245843 nnunetv2-2.4.2/nnunetv2/training/lr_scheduler/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/lr_scheduler/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      803 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/lr_scheduler/polylr.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.245843 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    70639 2024-04-25 09:10:04.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/nnUNetTrainer.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.245843 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/__init__.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.245843 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/benchmarking/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/benchmarking/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2858 2024-04-25 09:10:04.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/benchmarking/nnUNetTrainerBenchmark_5epochs.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2566 2024-04-25 09:10:04.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/benchmarking/nnUNetTrainerBenchmark_5epochs_noDataLoading.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.245843 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    20171 2024-04-25 09:10:04.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerDA5.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     8889 2024-04-20 11:06:50.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerDAOrd0.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2105 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerNoDA.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1230 2024-04-20 11:06:50.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerNoMirroring.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.245843 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/loss/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/loss/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1690 2024-04-25 09:10:04.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerCELoss.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3051 2024-04-20 11:06:50.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerDiceLoss.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3473 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerTopkLoss.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.245843 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/lr_schedule/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/lr_schedule/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      517 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/lr_schedule/nnUNetTrainerCosAnneal.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.245843 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/network_architecture/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/network_architecture/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1710 2024-04-18 08:44:04.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/network_architecture/nnUNetTrainerBN.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      501 2024-04-25 09:10:04.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/network_architecture/nnUNetTrainerNoDeepSupervision.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.245843 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/optimizer/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/optimizer/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2882 2024-04-25 09:10:04.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/optimizer/nnUNetTrainerAdam.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3259 2024-04-25 09:10:04.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/optimizer/nnUNetTrainerAdan.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.249843 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/sampling/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/sampling/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     5088 2024-04-25 09:10:04.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/sampling/nnUNetTrainer_probabilisticOversampling.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.249843 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/training_length/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/training_length/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3690 2024-04-25 09:10:04.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/training_length/nnUNetTrainer_Xepochs.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3157 2024-04-25 09:10:04.000000 nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/training_length/nnUNetTrainer_Xepochs_NoMirroring.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.249843 nnunetv2-2.4.2/nnunetv2/utilities/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/utilities/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      906 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/utilities/collate_outputs.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      619 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/utilities/crossval_split.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3925 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/utilities/dataset_name_id_conversion.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1748 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/utilities/ddp_allgather.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1854 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/utilities/default_n_proc_DA.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     5545 2024-04-20 11:06:50.000000 nnunetv2-2.4.2/nnunetv2/utilities/file_path_utilities.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      868 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/utilities/find_class_by_name.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     1910 2024-04-18 08:44:04.000000 nnunetv2-2.4.2/nnunetv2/utilities/get_network_from_plans.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      543 2024-04-20 11:06:50.000000 nnunetv2-2.4.2/nnunetv2/utilities/helpers.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2420 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/utilities/json_export.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.249843 nnunetv2-2.4.2/nnunetv2/utilities/label_handling/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/utilities/label_handling/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    14925 2024-04-20 11:06:50.000000 nnunetv2-2.4.2/nnunetv2/utilities/label_handling/label_handling.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      509 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/utilities/network_initialization.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    11953 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/utilities/overlay_plots.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.249843 nnunetv2-2.4.2/nnunetv2/utilities/plans_handling/
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        0 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/utilities/plans_handling/__init__.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    15055 2024-04-20 11:06:50.000000 nnunetv2-2.4.2/nnunetv2/utilities/plans_handling/plans_handler.py
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     3139 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/nnunetv2/utilities/utils.py
+drwxrwxr-x   0 isensee   (1000) isensee   (1000)        0 2024-04-25 09:15:30.229843 nnunetv2-2.4.2/nnunetv2.egg-info/
+-rw-r--r--   0 isensee   (1000) isensee   (1000)    24713 2024-04-25 09:15:30.000000 nnunetv2-2.4.2/nnunetv2.egg-info/PKG-INFO
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     9469 2024-04-25 09:15:30.000000 nnunetv2-2.4.2/nnunetv2.egg-info/SOURCES.txt
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        1 2024-04-25 09:15:30.000000 nnunetv2-2.4.2/nnunetv2.egg-info/dependency_links.txt
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     2244 2024-04-25 09:15:30.000000 nnunetv2-2.4.2/nnunetv2.egg-info/entry_points.txt
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)      285 2024-04-25 09:15:30.000000 nnunetv2-2.4.2/nnunetv2.egg-info/requires.txt
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)        9 2024-04-25 09:15:30.000000 nnunetv2-2.4.2/nnunetv2.egg-info/top_level.txt
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)     4218 2024-04-25 09:13:59.000000 nnunetv2-2.4.2/pyproject.toml
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)    10566 2024-04-20 21:08:15.000000 nnunetv2-2.4.2/readme.md
+-rw-rw-r--   0 isensee   (1000) isensee   (1000)       38 2024-04-25 09:15:30.249843 nnunetv2-2.4.2/setup.cfg
+-rwxrwxr-x   0 isensee   (1000) isensee   (1000)       69 2024-04-09 18:40:42.000000 nnunetv2-2.4.2/setup.py
```

### Comparing `nnunetv2-2.4.1/LICENSE` & `nnunetv2-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/PKG-INFO` & `nnunetv2-2.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnunetv2
-Version: 2.4.1
+Version: 2.4.2
 Summary: nnU-Net is a framework for out-of-the box image segmentation.
 Author: Helmholtz Imaging Applied Computer Vision Lab
 Author-email: Fabian Isensee <f.isensee@dkfz-heidelberg.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `nnunetv2-2.4.1/nnunetv2/batch_running/benchmarking/generate_benchmarking_commands.py` & `nnunetv2-2.4.2/nnunetv2/batch_running/benchmarking/generate_benchmarking_commands.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/batch_running/benchmarking/summarize_benchmark_results.py` & `nnunetv2-2.4.2/nnunetv2/batch_running/benchmarking/summarize_benchmark_results.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/batch_running/collect_results_custom_Decathlon.py` & `nnunetv2-2.4.2/nnunetv2/batch_running/collect_results_custom_Decathlon.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/batch_running/collect_results_custom_Decathlon_2d.py` & `nnunetv2-2.4.2/nnunetv2/batch_running/collect_results_custom_Decathlon_2d.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/batch_running/generate_lsf_runs_customDecathlon.py` & `nnunetv2-2.4.2/nnunetv2/batch_running/generate_lsf_runs_customDecathlon.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/batch_running/release_trainings/nnunetv2_v1/collect_results.py` & `nnunetv2-2.4.2/nnunetv2/batch_running/release_trainings/nnunetv2_v1/collect_results.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/batch_running/release_trainings/nnunetv2_v1/generate_lsf_commands.py` & `nnunetv2-2.4.2/nnunetv2/batch_running/release_trainings/nnunetv2_v1/generate_lsf_commands.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset027_ACDC.py` & `nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset027_ACDC.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset073_Fluo_C3DH_A549_SIM.py` & `nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset073_Fluo_C3DH_A549_SIM.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset114_MNMs.py` & `nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset114_MNMs.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset115_EMIDEC.py` & `nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset115_EMIDEC.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset120_RoadSegmentation.py` & `nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset120_RoadSegmentation.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset137_BraTS21.py` & `nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset137_BraTS21.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset218_Amos2022_task1.py` & `nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset218_Amos2022_task1.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset219_Amos2022_task2.py` & `nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset219_Amos2022_task2.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset220_KiTS2023.py` & `nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset220_KiTS2023.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset221_AutoPETII_2023.py` & `nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset221_AutoPETII_2023.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset223_AMOS2022postChallenge.py` & `nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset223_AMOS2022postChallenge.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/dataset_conversion/Dataset988_dummyDataset4.py` & `nnunetv2-2.4.2/nnunetv2/dataset_conversion/Dataset988_dummyDataset4.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/dataset_conversion/convert_MSD_dataset.py` & `nnunetv2-2.4.2/nnunetv2/dataset_conversion/convert_MSD_dataset.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/dataset_conversion/convert_raw_dataset_from_old_nnunet_format.py` & `nnunetv2-2.4.2/nnunetv2/dataset_conversion/convert_raw_dataset_from_old_nnunet_format.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset996_IntegrationTest_Hippocampus_regions_ignore.py` & `nnunetv2-2.4.2/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset996_IntegrationTest_Hippocampus_regions_ignore.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset997_IntegrationTest_Hippocampus_regions.py` & `nnunetv2-2.4.2/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset997_IntegrationTest_Hippocampus_regions.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset998_IntegrationTest_Hippocampus_ignore.py` & `nnunetv2-2.4.2/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset998_IntegrationTest_Hippocampus_ignore.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset999_IntegrationTest_Hippocampus.py` & `nnunetv2-2.4.2/nnunetv2/dataset_conversion/datasets_for_integration_tests/Dataset999_IntegrationTest_Hippocampus.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/dataset_conversion/generate_dataset_json.py` & `nnunetv2-2.4.2/nnunetv2/dataset_conversion/generate_dataset_json.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/ensembling/ensemble.py` & `nnunetv2-2.4.2/nnunetv2/ensembling/ensemble.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/evaluation/accumulate_cv_results.py` & `nnunetv2-2.4.2/nnunetv2/evaluation/accumulate_cv_results.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/evaluation/evaluate_predictions.py` & `nnunetv2-2.4.2/nnunetv2/evaluation/evaluate_predictions.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/evaluation/find_best_configuration.py` & `nnunetv2-2.4.2/nnunetv2/evaluation/find_best_configuration.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/experiment_planning/dataset_fingerprint/fingerprint_extractor.py` & `nnunetv2-2.4.2/nnunetv2/experiment_planning/dataset_fingerprint/fingerprint_extractor.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/experiment_planning/experiment_planners/default_experiment_planner.py` & `nnunetv2-2.4.2/nnunetv2/experiment_planning/experiment_planners/default_experiment_planner.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/experiment_planning/experiment_planners/network_topology.py` & `nnunetv2-2.4.2/nnunetv2/experiment_planning/experiment_planners/network_topology.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/experiment_planning/experiment_planners/resencUNet_planner.py` & `nnunetv2-2.4.2/nnunetv2/experiment_planning/experiment_planners/resencUNet_planner.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/experiment_planning/experiment_planners/residual_unets/residual_encoder_unet_planners.py` & `nnunetv2-2.4.2/nnunetv2/experiment_planning/experiment_planners/residual_unets/residual_encoder_unet_planners.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/experiment_planning/plan_and_preprocess_api.py` & `nnunetv2-2.4.2/nnunetv2/experiment_planning/plan_and_preprocess_api.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/experiment_planning/plan_and_preprocess_entrypoints.py` & `nnunetv2-2.4.2/nnunetv2/experiment_planning/plan_and_preprocess_entrypoints.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/experiment_planning/plans_for_pretraining/move_plans_between_datasets.py` & `nnunetv2-2.4.2/nnunetv2/experiment_planning/plans_for_pretraining/move_plans_between_datasets.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/experiment_planning/verify_dataset_integrity.py` & `nnunetv2-2.4.2/nnunetv2/experiment_planning/verify_dataset_integrity.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/imageio/base_reader_writer.py` & `nnunetv2-2.4.2/nnunetv2/imageio/base_reader_writer.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/imageio/natural_image_reader_writer.py` & `nnunetv2-2.4.2/nnunetv2/imageio/natural_image_reader_writer.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/imageio/nibabel_reader_writer.py` & `nnunetv2-2.4.2/nnunetv2/imageio/nibabel_reader_writer.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/imageio/reader_writer_registry.py` & `nnunetv2-2.4.2/nnunetv2/imageio/reader_writer_registry.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/imageio/simpleitk_reader_writer.py` & `nnunetv2-2.4.2/nnunetv2/imageio/simpleitk_reader_writer.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/imageio/tif_reader_writer.py` & `nnunetv2-2.4.2/nnunetv2/imageio/tif_reader_writer.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/inference/data_iterators.py` & `nnunetv2-2.4.2/nnunetv2/inference/data_iterators.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
                          seed_for_shuffle=1, return_incomplete=True,
                          shuffle=False, infinite=False, sampling_probabilities=None)
 
         self.indices = list(range(len(list_of_lists)))
 
     def generate_train_batch(self):
         idx = self.get_indices()[0]
-        files, seg_prev_stage, ofile = self._data[idx][0]
+        files, seg_prev_stage, ofile = self._data[idx]
         # if we have a segmentation from the previous stage we have to process it together with the images so that we
         # can crop it appropriately (if needed). Otherwise it would just be resized to the shape of the data after
         # preprocessing and then there might be misalignments
         data, seg, data_properties = self.preprocessor.run_case(files, seg_prev_stage, self.plans_manager,
                                                                 self.configuration_manager,
                                                                 self.dataset_json)
         if seg_prev_stage is not None:
@@ -186,15 +186,15 @@
             seed_for_shuffle=1, return_incomplete=True,
             shuffle=False, infinite=False, sampling_probabilities=None)
 
         self.indices = list(range(len(list_of_images)))
 
     def generate_train_batch(self):
         idx = self.get_indices()[0]
-        image, seg_prev_stage, props, ofname = self._data[idx][0]
+        image, seg_prev_stage, props, ofname = self._data[idx]
         # if we have a segmentation from the previous stage we have to process it together with the images so that we
         # can crop it appropriately (if needed). Otherwise it would just be resized to the shape of the data after
         # preprocessing and then there might be misalignments
         data, seg = self.preprocessor.run_case_npy(image, seg_prev_stage, props,
                                                    self.plans_manager,
                                                    self.configuration_manager,
                                                    self.dataset_json)
```

### Comparing `nnunetv2-2.4.1/nnunetv2/inference/examples.py` & `nnunetv2-2.4.2/nnunetv2/inference/examples.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/inference/export_prediction.py` & `nnunetv2-2.4.2/nnunetv2/inference/export_prediction.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/inference/predict_from_raw_data.py` & `nnunetv2-2.4.2/nnunetv2/inference/predict_from_raw_data.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/inference/sliding_window_prediction.py` & `nnunetv2-2.4.2/nnunetv2/inference/sliding_window_prediction.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/model_sharing/entry_points.py` & `nnunetv2-2.4.2/nnunetv2/model_sharing/entry_points.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/model_sharing/model_download.py` & `nnunetv2-2.4.2/nnunetv2/model_sharing/model_download.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/model_sharing/model_export.py` & `nnunetv2-2.4.2/nnunetv2/model_sharing/model_export.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/paths.py` & `nnunetv2-2.4.2/nnunetv2/paths.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/postprocessing/remove_connected_components.py` & `nnunetv2-2.4.2/nnunetv2/postprocessing/remove_connected_components.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/preprocessing/cropping/cropping.py` & `nnunetv2-2.4.2/nnunetv2/preprocessing/cropping/cropping.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/preprocessing/normalization/default_normalization_schemes.py` & `nnunetv2-2.4.2/nnunetv2/preprocessing/normalization/default_normalization_schemes.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/preprocessing/normalization/map_channel_name_to_normalization.py` & `nnunetv2-2.4.2/nnunetv2/preprocessing/normalization/map_channel_name_to_normalization.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/preprocessing/preprocessors/default_preprocessor.py` & `nnunetv2-2.4.2/nnunetv2/preprocessing/preprocessors/default_preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,42 +10,42 @@
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 import multiprocessing
 import shutil
 from time import sleep
-from typing import Union, Tuple
+from typing import Tuple, Union
 
-import nnunetv2
 import numpy as np
 from batchgenerators.utilities.file_and_folder_operations import *
+from tqdm import tqdm
+
+import nnunetv2
 from nnunetv2.paths import nnUNet_preprocessed, nnUNet_raw
 from nnunetv2.preprocessing.cropping.cropping import crop_to_nonzero
 from nnunetv2.preprocessing.resampling.default_resampling import compute_new_shape
 from nnunetv2.utilities.dataset_name_id_conversion import maybe_convert_to_dataset_name
 from nnunetv2.utilities.find_class_by_name import recursive_find_python_class
 from nnunetv2.utilities.plans_handling.plans_handler import PlansManager, ConfigurationManager
-from nnunetv2.utilities.utils import get_identifiers_from_splitted_dataset_folder, \
-    create_lists_from_splitted_dataset_folder, get_filenames_of_train_images_and_targets
-from tqdm import tqdm
+from nnunetv2.utilities.utils import get_filenames_of_train_images_and_targets
 
 
 class DefaultPreprocessor(object):
     def __init__(self, verbose: bool = True):
         self.verbose = verbose
         """
         Everything we need is in the plans. Those are given when run() is called
         """
 
     def run_case_npy(self, data: np.ndarray, seg: Union[np.ndarray, None], properties: dict,
                      plans_manager: PlansManager, configuration_manager: ConfigurationManager,
                      dataset_json: Union[dict, str]):
         # let's not mess up the inputs!
-        data = np.copy(data)
+        data = data.astype(np.float32)  # this creates a copy
         if seg is not None:
             assert data.shape[1:] == seg.shape[1:], "Shape mismatch between image and segmentation. Please fix your dataset and make use of the --verify_dataset_integrity flag to ensure everything is correct"
             seg = np.copy(seg)
 
         has_seg = seg is not None
 
         # apply transpose_forward, this also needs to be applied to the spacing!
```

### Comparing `nnunetv2-2.4.1/nnunetv2/preprocessing/resampling/default_resampling.py` & `nnunetv2-2.4.2/nnunetv2/preprocessing/resampling/default_resampling.py`

 * *Files 12% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
     data_reshaped = resample_data_or_seg(data, new_shape, is_seg, axis, order, do_separate_z, order_z=order_z)
     return data_reshaped
 
 
 def resample_data_or_seg(data: np.ndarray, new_shape: Union[Tuple[float, ...], List[float], np.ndarray],
                          is_seg: bool = False, axis: Union[None, int] = None, order: int = 3,
-                         do_separate_z: bool = False, order_z: int = 0):
+                         do_separate_z: bool = False, order_z: int = 0, dtype_out = None):
     """
     separate_z=True will resample with order 0 along z
     :param data:
     :param new_shape:
     :param is_seg:
     :param axis:
     :param order:
@@ -141,76 +141,68 @@
 
     if is_seg:
         resize_fn = resize_segmentation
         kwargs = OrderedDict()
     else:
         resize_fn = resize
         kwargs = {'mode': 'edge', 'anti_aliasing': False}
-    dtype_data = data.dtype
     shape = np.array(data[0].shape)
     new_shape = np.array(new_shape)
+    if dtype_out is None:
+        dtype_out = data.dtype
+    reshaped_final = np.zeros((data.shape[0], *new_shape), dtype=dtype_out)
     if np.any(shape != new_shape):
-        data = data.astype(float)
+        data = data.astype(float, copy=False)
         if do_separate_z:
             # print("separate z, order in z is", order_z, "order inplane is", order)
             assert len(axis) == 1, "only one anisotropic axis supported"
             axis = axis[0]
             if axis == 0:
                 new_shape_2d = new_shape[1:]
             elif axis == 1:
                 new_shape_2d = new_shape[[0, 2]]
             else:
                 new_shape_2d = new_shape[:-1]
 
-            reshaped_final_data = []
             for c in range(data.shape[0]):
-                reshaped_data = []
+                reshaped_here = np.zeros((data.shape[1], *new_shape_2d))
                 for slice_id in range(shape[axis]):
                     if axis == 0:
-                        reshaped_data.append(resize_fn(data[c, slice_id], new_shape_2d, order, **kwargs))
+                        reshaped_here[slice_id] = resize_fn(data[c, slice_id], new_shape_2d, order, **kwargs)
                     elif axis == 1:
-                        reshaped_data.append(resize_fn(data[c, :, slice_id], new_shape_2d, order, **kwargs))
+                        reshaped_here[slice_id] = resize_fn(data[c, :, slice_id], new_shape_2d, order, **kwargs)
                     else:
-                        reshaped_data.append(resize_fn(data[c, :, :, slice_id], new_shape_2d, order, **kwargs))
-                reshaped_data = np.stack(reshaped_data, axis)
+                        reshaped_here[slice_id] = resize_fn(data[c, :, :, slice_id], new_shape_2d, order, **kwargs)
                 if shape[axis] != new_shape[axis]:
 
                     # The following few lines are blatantly copied and modified from sklearn's resize()
                     rows, cols, dim = new_shape[0], new_shape[1], new_shape[2]
-                    orig_rows, orig_cols, orig_dim = reshaped_data.shape
+                    orig_rows, orig_cols, orig_dim = reshaped_here.shape
 
                     row_scale = float(orig_rows) / rows
                     col_scale = float(orig_cols) / cols
                     dim_scale = float(orig_dim) / dim
 
                     map_rows, map_cols, map_dims = np.mgrid[:rows, :cols, :dim]
                     map_rows = row_scale * (map_rows + 0.5) - 0.5
                     map_cols = col_scale * (map_cols + 0.5) - 0.5
                     map_dims = dim_scale * (map_dims + 0.5) - 0.5
 
                     coord_map = np.array([map_rows, map_cols, map_dims])
                     if not is_seg or order_z == 0:
-                        reshaped_final_data.append(map_coordinates(reshaped_data, coord_map, order=order_z,
-                                                                   mode='nearest')[None])
+                        reshaped_final[c] = map_coordinates(reshaped_here, coord_map, order=order_z, mode='nearest')[None]
                     else:
-                        unique_labels = np.sort(pd.unique(reshaped_data.ravel()))  # np.unique(reshaped_data)
-                        reshaped = np.zeros(new_shape, dtype=dtype_data)
-
+                        unique_labels = np.sort(pd.unique(reshaped_here.ravel()))  # np.unique(reshaped_data)
                         for i, cl in enumerate(unique_labels):
-                            reshaped_multihot = np.round(
-                                map_coordinates((reshaped_data == cl).astype(float), coord_map, order=order_z,
-                                                mode='nearest'))
-                            reshaped[reshaped_multihot > 0.5] = cl
-                        reshaped_final_data.append(reshaped[None])
+                            reshaped_final[c][np.round(
+                                map_coordinates((reshaped_here == cl).astype(float), coord_map, order=order_z,
+                                                mode='nearest')) > 0.5] = cl
                 else:
-                    reshaped_final_data.append(reshaped_data[None])
-            reshaped_final_data = np.vstack(reshaped_final_data)
+                    reshaped_final[c] = reshaped_here
         else:
             # print("no separate z, order", order)
-            reshaped = []
             for c in range(data.shape[0]):
-                reshaped.append(resize_fn(data[c], new_shape, order, **kwargs)[None])
-            reshaped_final_data = np.vstack(reshaped)
-        return reshaped_final_data.astype(dtype_data)
+                reshaped_final[c] = resize_fn(data[c], new_shape, order, **kwargs)
+        return reshaped_final
     else:
         # print("no resampling necessary")
         return data
```

### Comparing `nnunetv2-2.4.1/nnunetv2/preprocessing/resampling/utils.py` & `nnunetv2-2.4.2/nnunetv2/preprocessing/resampling/utils.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/run/load_pretrained_weights.py` & `nnunetv2-2.4.2/nnunetv2/run/load_pretrained_weights.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/run/run_training.py` & `nnunetv2-2.4.2/nnunetv2/run/run_training.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/tests/integration_tests/add_lowres_and_cascade.py` & `nnunetv2-2.4.2/nnunetv2/tests/integration_tests/add_lowres_and_cascade.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/tests/integration_tests/cleanup_integration_test.py` & `nnunetv2-2.4.2/nnunetv2/tests/integration_tests/cleanup_integration_test.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/tests/integration_tests/run_integration_test_bestconfig_inference.py` & `nnunetv2-2.4.2/nnunetv2/tests/integration_tests/run_integration_test_bestconfig_inference.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/data_augmentation/compute_initial_patch_size.py` & `nnunetv2-2.4.2/nnunetv2/training/data_augmentation/compute_initial_patch_size.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/data_augmentation/custom_transforms/cascade_transforms.py` & `nnunetv2-2.4.2/nnunetv2/training/data_augmentation/custom_transforms/cascade_transforms.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/data_augmentation/custom_transforms/deep_supervision_donwsampling.py` & `nnunetv2-2.4.2/nnunetv2/training/data_augmentation/custom_transforms/deep_supervision_donwsampling.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/data_augmentation/custom_transforms/masking.py` & `nnunetv2-2.4.2/nnunetv2/training/data_augmentation/custom_transforms/masking.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/data_augmentation/custom_transforms/region_based_training.py` & `nnunetv2-2.4.2/nnunetv2/training/data_augmentation/custom_transforms/region_based_training.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/data_augmentation/custom_transforms/transforms_for_dummy_2d.py` & `nnunetv2-2.4.2/nnunetv2/training/data_augmentation/custom_transforms/transforms_for_dummy_2d.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/dataloading/base_data_loader.py` & `nnunetv2-2.4.2/nnunetv2/training/dataloading/base_data_loader.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/dataloading/data_loader_2d.py` & `nnunetv2-2.4.2/nnunetv2/training/dataloading/data_loader_2d.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/dataloading/data_loader_3d.py` & `nnunetv2-2.4.2/nnunetv2/training/dataloading/data_loader_3d.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/dataloading/nnunet_dataset.py` & `nnunetv2-2.4.2/nnunetv2/training/dataloading/nnunet_dataset.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/dataloading/utils.py` & `nnunetv2-2.4.2/nnunetv2/training/dataloading/utils.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/logging/nnunet_logger.py` & `nnunetv2-2.4.2/nnunetv2/training/logging/nnunet_logger.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/loss/compound_losses.py` & `nnunetv2-2.4.2/nnunetv2/training/loss/compound_losses.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/loss/deep_supervision.py` & `nnunetv2-2.4.2/nnunetv2/training/loss/deep_supervision.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/loss/dice.py` & `nnunetv2-2.4.2/nnunetv2/training/loss/dice.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/loss/robust_ce_loss.py` & `nnunetv2-2.4.2/nnunetv2/training/loss/robust_ce_loss.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/lr_scheduler/polylr.py` & `nnunetv2-2.4.2/nnunetv2/training/lr_scheduler/polylr.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/nnUNetTrainer.py` & `nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/nnUNetTrainer.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/benchmarking/nnUNetTrainerBenchmark_5epochs.py` & `nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/benchmarking/nnUNetTrainerBenchmark_5epochs.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/benchmarking/nnUNetTrainerBenchmark_5epochs_noDataLoading.py` & `nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/benchmarking/nnUNetTrainerBenchmark_5epochs_noDataLoading.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerDA5.py` & `nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerDA5.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerDAOrd0.py` & `nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerDAOrd0.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerNoDA.py` & `nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerNoDA.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerNoMirroring.py` & `nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/data_augmentation/nnUNetTrainerNoMirroring.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerCELoss.py` & `nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerCELoss.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerDiceLoss.py` & `nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerDiceLoss.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerTopkLoss.py` & `nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/loss/nnUNetTrainerTopkLoss.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/lr_schedule/nnUNetTrainerCosAnneal.py` & `nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/lr_schedule/nnUNetTrainerCosAnneal.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/network_architecture/nnUNetTrainerBN.py` & `nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/network_architecture/nnUNetTrainerBN.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/optimizer/nnUNetTrainerAdam.py` & `nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/optimizer/nnUNetTrainerAdam.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/optimizer/nnUNetTrainerAdan.py` & `nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/optimizer/nnUNetTrainerAdan.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/sampling/nnUNetTrainer_probabilisticOversampling.py` & `nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/sampling/nnUNetTrainer_probabilisticOversampling.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/training_length/nnUNetTrainer_Xepochs.py` & `nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/training_length/nnUNetTrainer_Xepochs.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/training/nnUNetTrainer/variants/training_length/nnUNetTrainer_Xepochs_NoMirroring.py` & `nnunetv2-2.4.2/nnunetv2/training/nnUNetTrainer/variants/training_length/nnUNetTrainer_Xepochs_NoMirroring.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/utilities/collate_outputs.py` & `nnunetv2-2.4.2/nnunetv2/utilities/collate_outputs.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/utilities/crossval_split.py` & `nnunetv2-2.4.2/nnunetv2/utilities/crossval_split.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/utilities/dataset_name_id_conversion.py` & `nnunetv2-2.4.2/nnunetv2/utilities/dataset_name_id_conversion.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/utilities/ddp_allgather.py` & `nnunetv2-2.4.2/nnunetv2/utilities/ddp_allgather.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/utilities/default_n_proc_DA.py` & `nnunetv2-2.4.2/nnunetv2/utilities/default_n_proc_DA.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/utilities/file_path_utilities.py` & `nnunetv2-2.4.2/nnunetv2/utilities/file_path_utilities.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/utilities/find_class_by_name.py` & `nnunetv2-2.4.2/nnunetv2/utilities/find_class_by_name.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/utilities/get_network_from_plans.py` & `nnunetv2-2.4.2/nnunetv2/utilities/get_network_from_plans.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/utilities/helpers.py` & `nnunetv2-2.4.2/nnunetv2/utilities/helpers.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/utilities/json_export.py` & `nnunetv2-2.4.2/nnunetv2/utilities/json_export.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/utilities/label_handling/label_handling.py` & `nnunetv2-2.4.2/nnunetv2/utilities/label_handling/label_handling.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/utilities/overlay_plots.py` & `nnunetv2-2.4.2/nnunetv2/utilities/overlay_plots.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/utilities/plans_handling/plans_handler.py` & `nnunetv2-2.4.2/nnunetv2/utilities/plans_handling/plans_handler.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2/utilities/utils.py` & `nnunetv2-2.4.2/nnunetv2/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2.egg-info/PKG-INFO` & `nnunetv2-2.4.2/nnunetv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnunetv2
-Version: 2.4.1
+Version: 2.4.2
 Summary: nnU-Net is a framework for out-of-the box image segmentation.
 Author: Helmholtz Imaging Applied Computer Vision Lab
 Author-email: Fabian Isensee <f.isensee@dkfz-heidelberg.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `nnunetv2-2.4.1/nnunetv2.egg-info/SOURCES.txt` & `nnunetv2-2.4.2/nnunetv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/nnunetv2.egg-info/entry_points.txt` & `nnunetv2-2.4.2/nnunetv2.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `nnunetv2-2.4.1/pyproject.toml` & `nnunetv2-2.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nnunetv2"
-version = "2.4.1"
+version = "2.4.2"
 requires-python = ">=3.9"
 description = "nnU-Net is a framework for out-of-the box image segmentation."
 readme = "readme.md"
 license = { file = "LICENSE" }
 authors = [
     { name = "Fabian Isensee", email = "f.isensee@dkfz-heidelberg.de"},
     { name = "Helmholtz Imaging Applied Computer Vision Lab" }
```

### Comparing `nnunetv2-2.4.1/readme.md` & `nnunetv2-2.4.2/readme.md`

 * *Files identical despite different names*

