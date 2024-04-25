# Comparing `tmp/gentab-0.1.1.tar.gz` & `tmp/gentab-0.1.2.tar.gz`

## Comparing `gentab-0.1.1.tar` & `gentab-0.1.2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 gentab-0.1.1/correlation.py
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 gentab-0.1.1/dcr.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 gentab-0.1.1/environment.yaml
--rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 gentab-0.1.1/fidelity.py
--rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 gentab-0.1.1/performance.py
--rw-r--r--   0        0        0     6987 2020-02-02 00:00:00.000000 gentab-0.1.1/results.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 gentab-0.1.1/test_adult_baseline.py
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 gentab-0.1.1/test_adult_baseline_correlation.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 gentab-0.1.1/test_adult_catboost.py
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 gentab-0.1.1/test_adult_lightgbm.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 gentab-0.1.1/test_adult_xgboost.py
--rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 gentab-0.1.1/test_baseline_correlation.py
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 gentab-0.1.1/test_car_eval_4_baseline.py
--rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 gentab-0.1.1/test_car_evaluation_baseline_correlation.py
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 gentab-0.1.1/test_playnet_baseline.py
--rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 gentab-0.1.1/test_playnet_mlp.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 gentab-0.1.1/tune.py
--rw-r--r--   0        0        0     5149 2020-02-02 00:00:00.000000 gentab-0.1.1/visual_heatmap_playnet.py
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 gentab-0.1.1/visual_playnet.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 gentab-0.1.1/configs/adult.json
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 gentab-0.1.1/configs/adult_cr.json
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 gentab-0.1.1/configs/car_eval_4.json
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 gentab-0.1.1/configs/car_evaluation_cr.json
--rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 gentab-0.1.1/configs/playnet.json
--rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 gentab-0.1.1/configs/playnet_cr.json
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/__init__.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/utils.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/data/__init__.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/data/config.py
--rw-r--r--   0        0        0    21840 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/data/dataset.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/evaluators/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/evaluators/catboost.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/evaluators/evaluator.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/evaluators/knn.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/evaluators/lightgbm.py
--rw-r--r--   0        0        0     9219 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/evaluators/mlp.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/evaluators/xgboost.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/__init__.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/adasyn.py
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/autodiffusion.py
--rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/copulagan.py
--rwxr-xr-x   0        0        0     4335 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/ctabgan.py
--rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/ctabganplus.py
--rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/ctgan.py
--rw-r--r--   0        0        0     6444 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/forestdiffusion.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/gaussiancopula.py
--rw-r--r--   0        0        0     5694 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/generator.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/great.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/randomoversampler.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/smote.py
--rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/tabula.py
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/tvae.py
--rw-r--r--   0        0        0    13286 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/autodiff/TabDDPMdiff.py
--rw-r--r--   0        0        0     7884 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/autodiff/autoencoder.py
--rw-r--r--   0        0        0    10825 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/autodiff/diffusion.py
--rw-r--r--   0        0        0    14603 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/autodiff/process_GQ.py
--rw-r--r--   0        0        0    14354 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/autodiff/process_edited.py
--rwxr-xr-x   0        0        0     7098 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/ctabg/pipeline/data_preparation.py
--rwxr-xr-x   0        0        0    37499 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/ctabg/synthesizer/ctabgan_synthesizer.py
--rwxr-xr-x   0        0        0    23261 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/ctabg/synthesizer/transformer.py
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/ctabgplus/pipeline/data_preparation.py
--rw-r--r--   0        0        0     8040 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/ctabgplus/privacy_utils/rdp_accountant.py
--rw-r--r--   0        0        0    21971 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/ctabgplus/synthesizer/ctabgan_synthesizer.py
--rw-r--r--   0        0        0    18238 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/ctabgplus/synthesizer/transformer.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/dae/__init__.py
--rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/dae/data.py
--rw-r--r--   0        0        0     7307 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/dae/engine.py
--rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/dae/model.py
--rw-r--r--   0        0        0    11333 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/dae/network.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/dae/util.py
--rw-r--r--   0        0        0    20077 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/tabu/tabula.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/tabu/tabula_dataset.py
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/tabu/tabula_start.py
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/tabu/tabula_trainer.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/tabu/tabula_utils.py
--rw-r--r--   0        0        0    18255 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/tabump/tabula.py
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/tabump/tabula_dataset.py
--rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/tabump/tabula_start.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/tabump/tabula_trainer.py
--rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/generators/tabump/tabula_utils.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/tuners/__init__.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/tuners/adasyn.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/tuners/autodiffusion.py
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/tuners/copulagan.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/tuners/ctabgan.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/tuners/ctabganplus.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/tuners/ctgan.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/tuners/forestdiffusion.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/tuners/gaussiancopula.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/tuners/great.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/tuners/smote.py
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/tuners/tabula.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/tuners/tuner.py
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 gentab-0.1.1/gentab/tuners/tvae.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 gentab-0.1.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 gentab-0.1.1/LICENSE
--rw-r--r--   0        0        0     8793 2020-02-02 00:00:00.000000 gentab-0.1.1/README.md
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 gentab-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    10145 2020-02-02 00:00:00.000000 gentab-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 gentab-0.1.2/correlation.py
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 gentab-0.1.2/dcr.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 gentab-0.1.2/environment.yaml
+-rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 gentab-0.1.2/fidelity.py
+-rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 gentab-0.1.2/performance.py
+-rw-r--r--   0        0        0     6953 2020-02-02 00:00:00.000000 gentab-0.1.2/results.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 gentab-0.1.2/test_adult_baseline.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 gentab-0.1.2/test_adult_baseline_correlation.py
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 gentab-0.1.2/test_adult_catboost.py
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 gentab-0.1.2/test_adult_lightgbm.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 gentab-0.1.2/test_adult_xgboost.py
+-rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 gentab-0.1.2/test_baseline_correlation.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 gentab-0.1.2/test_car_eval_4_baseline.py
+-rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 gentab-0.1.2/test_car_evaluation_baseline_correlation.py
+-rw-r--r--   0        0        0     4087 2020-02-02 00:00:00.000000 gentab-0.1.2/test_playnet_baseline.py
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 gentab-0.1.2/test_playnet_mlp.py
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 gentab-0.1.2/tune.py
+-rw-r--r--   0        0        0     5149 2020-02-02 00:00:00.000000 gentab-0.1.2/visual_heatmap_playnet.py
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 gentab-0.1.2/visual_playnet.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 gentab-0.1.2/configs/adult.json
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 gentab-0.1.2/configs/adult_cr.json
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 gentab-0.1.2/configs/car_eval_4.json
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 gentab-0.1.2/configs/car_evaluation_cr.json
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 gentab-0.1.2/configs/playnet.json
+-rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 gentab-0.1.2/configs/playnet_cr.json
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/__init__.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/utils.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/data/__init__.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/data/config.py
+-rw-r--r--   0        0        0    22687 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/data/dataset.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/evaluators/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/evaluators/catboost.py
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/evaluators/evaluator.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/evaluators/knn.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/evaluators/lightgbm.py
+-rw-r--r--   0        0        0     9229 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/evaluators/mlp.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/evaluators/xgboost.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/__init__.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/adasyn.py
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/autodiffusion.py
+-rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/copulagan.py
+-rwxr-xr-x   0        0        0     4335 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/ctabgan.py
+-rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/ctabganplus.py
+-rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/ctgan.py
+-rw-r--r--   0        0        0     6444 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/forestdiffusion.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/gaussiancopula.py
+-rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/generator.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/great.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/randomoversampler.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/smote.py
+-rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/tabula.py
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/tvae.py
+-rw-r--r--   0        0        0    13286 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/autodiff/TabDDPMdiff.py
+-rw-r--r--   0        0        0     7884 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/autodiff/autoencoder.py
+-rw-r--r--   0        0        0    10825 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/autodiff/diffusion.py
+-rw-r--r--   0        0        0    14603 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/autodiff/process_GQ.py
+-rw-r--r--   0        0        0    14354 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/autodiff/process_edited.py
+-rwxr-xr-x   0        0        0     7098 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/ctabg/pipeline/data_preparation.py
+-rwxr-xr-x   0        0        0    37499 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/ctabg/synthesizer/ctabgan_synthesizer.py
+-rwxr-xr-x   0        0        0    23261 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/ctabg/synthesizer/transformer.py
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/ctabgplus/pipeline/data_preparation.py
+-rw-r--r--   0        0        0     8040 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/ctabgplus/privacy_utils/rdp_accountant.py
+-rw-r--r--   0        0        0    21971 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/ctabgplus/synthesizer/ctabgan_synthesizer.py
+-rw-r--r--   0        0        0    18238 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/ctabgplus/synthesizer/transformer.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/dae/__init__.py
+-rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/dae/data.py
+-rw-r--r--   0        0        0     7307 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/dae/engine.py
+-rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/dae/model.py
+-rw-r--r--   0        0        0    11333 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/dae/network.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/dae/util.py
+-rw-r--r--   0        0        0    20077 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/tabu/tabula.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/tabu/tabula_dataset.py
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/tabu/tabula_start.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/tabu/tabula_trainer.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/tabu/tabula_utils.py
+-rw-r--r--   0        0        0    18255 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/tabump/tabula.py
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/tabump/tabula_dataset.py
+-rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/tabump/tabula_start.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/tabump/tabula_trainer.py
+-rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/generators/tabump/tabula_utils.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/tuners/__init__.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/tuners/adasyn.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/tuners/autodiffusion.py
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/tuners/copulagan.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/tuners/ctabgan.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/tuners/ctabganplus.py
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/tuners/ctgan.py
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/tuners/forestdiffusion.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/tuners/gaussiancopula.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/tuners/great.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/tuners/smote.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/tuners/tabula.py
+-rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/tuners/tuner.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 gentab-0.1.2/gentab/tuners/tvae.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 gentab-0.1.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 gentab-0.1.2/LICENSE
+-rw-r--r--   0        0        0     9621 2020-02-02 00:00:00.000000 gentab-0.1.2/README.md
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 gentab-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    10973 2020-02-02 00:00:00.000000 gentab-0.1.2/PKG-INFO
```

### Comparing `gentab-0.1.1/correlation.py` & `gentab-0.1.2/correlation.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/dcr.py` & `gentab-0.1.2/dcr.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/environment.yaml` & `gentab-0.1.2/environment.yaml`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/fidelity.py` & `gentab-0.1.2/fidelity.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/performance.py` & `gentab-0.1.2/performance.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,19 +63,19 @@
 
 
 configs = [
     ("configs/adult.json", preproc_adult, "Adult"),
 ]
 
 gens = [
-    # (SMOTE, "SMOTE \cite{chawla2002smote}", SMOTETuner),
-    # (ADASYN, "ADASYN \cite{he2008adasyn}", ADASYNTuner),
+    (SMOTE, "SMOTE \cite{chawla2002smote}", SMOTETuner),
+    (ADASYN, "ADASYN \cite{he2008adasyn}", ADASYNTuner),
     (TVAE, "TVAE \cite{xu2019modeling}", TVAETuner),
     (CTGAN, "CTGAN \cite{xu2019modeling}", CTGANTuner),
-    # (GaussianCopula, "GaussianCopula \cite{patki2016synthetic}", GaussianCopulaTuner),
+    (GaussianCopula, "GaussianCopula \cite{patki2016synthetic}", GaussianCopulaTuner),
     (CopulaGAN, "CopulaGAN \cite{xu2019modeling}", CopulaGANTuner),
     (CTABGAN, "CTAB-GAN \cite{zhao2021ctab}", CTABGANTuner),
     (CTABGANPlus, "CTAB-GAN+ \cite{zhao2022ctab}", CTABGANPlusTuner),
     (AutoDiffusion, "AutoDiffusion \cite{suh2023autodiff}", AutoDiffusionTuner),
     (
         ForestDiffusion,
         "ForestDiffusion \cite{jolicoeur2023generating}",
```

### Comparing `gentab-0.1.1/results.py` & `gentab-0.1.2/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,36 +181,36 @@
             )
         lines.append(line)
 
     return lines
 
 
 configs = [
-    # ("configs/playnet.json", preproc_playnet, "PlayNet"),
+    ("configs/playnet.json", preproc_playnet, "PlayNet"),
     ("configs/adult.json", preproc_adult, "Adult"),
-    # ("configs/car_eval_4.json", preproc_car_eval_4, "Car Evaluation"),
+    ("configs/car_eval_4.json", preproc_car_eval_4, "Car Evaluation"),
 ]
 
 gens = [
-    # (SMOTE, "SMOTE \cite{chawla2002smote}", "SMOTE"),
-    # (ADASYN, "ADASYN \cite{he2008adasyn}", "ADASYN"),
-    # (TVAE, "TVAE \cite{xu2019modeling}", "TVAE"),
-    # (CTGAN, "CTGAN \cite{xu2019modeling}", "CTGAN"),
+    (SMOTE, "SMOTE \cite{chawla2002smote}", "SMOTE"),
+    (ADASYN, "ADASYN \cite{he2008adasyn}", "ADASYN"),
+    (TVAE, "TVAE \cite{xu2019modeling}", "TVAE"),
+    (CTGAN, "CTGAN \cite{xu2019modeling}", "CTGAN"),
     (GaussianCopula, "GaussianCopula \cite{patki2016synthetic}", "GaussianCopula"),
-    # (CopulaGAN, "CopulaGAN \cite{xu2019modeling}", "CopulaGAN"),
-    # (CTABGAN, "CTAB-GAN \cite{zhao2021ctab}", "CTAB-GAN"),
-    # (CTABGANPlus, "CTAB-GAN+ \cite{zhao2022ctab}", "CTAB-GAN+"),
-    # (AutoDiffusion, "AutoDiffusion \cite{suh2023autodiff}", "AutoDiffusion"),
-    # (
-    #     ForestDiffusion,
-    #     "ForestDiffusion \cite{jolicoeur2023generating}",
-    #     "ForestDiffusion",
-    # ),
-    # (GReaT, "GReaT \cite{borisov2022language}", "GReaT"),
-    # (Tabula, "Tabula \cite{zhao2023tabula}", "Tabula"),
+    (CopulaGAN, "CopulaGAN \cite{xu2019modeling}", "CopulaGAN"),
+    (CTABGAN, "CTAB-GAN \cite{zhao2021ctab}", "CTAB-GAN"),
+    (CTABGANPlus, "CTAB-GAN+ \cite{zhao2022ctab}", "CTAB-GAN+"),
+    (AutoDiffusion, "AutoDiffusion \cite{suh2023autodiff}", "AutoDiffusion"),
+    (
+        ForestDiffusion,
+        "ForestDiffusion \cite{jolicoeur2023generating}",
+        "ForestDiffusion",
+    ),
+    (GReaT, "GReaT \cite{borisov2022language}", "GReaT"),
+    (Tabula, "Tabula \cite{zhao2023tabula}", "Tabula"),
 ]
 
 evals = [
     (
         LightGBM,
         "\multirow{" + str(len(gens)) + "}{*}{LightGBM \cite{ke2017lightgbm}}",
         "LightGBM",
```

### Comparing `gentab-0.1.1/test_adult_baseline.py` & `gentab-0.1.2/test_adult_baseline.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/test_adult_baseline_correlation.py` & `gentab-0.1.2/test_adult_baseline_correlation.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/test_adult_catboost.py` & `gentab-0.1.2/test_adult_catboost.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/test_adult_lightgbm.py` & `gentab-0.1.2/test_adult_lightgbm.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/test_adult_xgboost.py` & `gentab-0.1.2/test_adult_xgboost.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/test_baseline_correlation.py` & `gentab-0.1.2/test_baseline_correlation.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/test_car_eval_4_baseline.py` & `gentab-0.1.2/test_car_eval_4_baseline.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     ForestDiffusion,
     Tabula,
     GReaT,
 )
 from gentab.data import Config, Dataset
 from gentab.utils import console
 
-config = Config("datasets/car_eval_4/info.json")
+config = Config("configs/car_eval_4.json")
 
 dataset = Dataset(config)
 
 console.print(dataset.class_counts(), dataset.row_count())
 generator = SMOTE(dataset)
 generator.generate()
 dataset.save_to_disk(generator)
```

### Comparing `gentab-0.1.1/test_car_evaluation_baseline_correlation.py` & `gentab-0.1.2/test_car_evaluation_baseline_correlation.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/test_playnet_baseline.py` & `gentab-0.1.2/test_playnet_baseline.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     CTABGAN,
     CTABGANPlus,
     AutoDiffusion,
     ForestDiffusion,
     Tabula,
     GReaT,
 )
+from gentab.evaluators import MLP
 from gentab.data import Config, Dataset
 from gentab.utils import console
 
 config = Config("configs/playnet.json")
 
 dataset = Dataset(config)
 console.print(dataset.class_counts(), dataset.row_count())
```

### Comparing `gentab-0.1.1/test_playnet_mlp.py` & `gentab-0.1.2/test_playnet_mlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,21 +116,21 @@
 generator = AutoDiffusion(dataset)
 evaluator = MLP(generator)
 tuner = AutoDiffusionTuner(evaluator, trials)
 tuner.tune()
 tuner.save_to_disk()
 console.print(dataset.generated_class_counts(), dataset.generated_row_count())
 
-# console.print(dataset.class_counts(), dataset.row_count())
-# generator = ForestDiffusion(dataset, n_jobs=1, duplicate_K=4, n_estimators=100)
-# evaluator = MLP(generator)
-# tuner = ForestDiffusionTuner(evaluator, trials)
-# tuner.tune()
-# tuner.save_to_disk()
-# console.print(dataset.generated_class_counts(), dataset.generated_row_count())
+console.print(dataset.class_counts(), dataset.row_count())
+generator = ForestDiffusion(dataset, n_jobs=1, duplicate_K=4, n_estimators=100)
+evaluator = MLP(generator)
+tuner = ForestDiffusionTuner(evaluator, trials)
+tuner.tune()
+tuner.save_to_disk()
+console.print(dataset.generated_class_counts(), dataset.generated_row_count())
 
 console.print(dataset.class_counts(), dataset.row_count())
 generator = GReaT(
     dataset,
     epochs=15,
     max_length=1024,
     temperature=0.6,
```

### Comparing `gentab-0.1.1/tune.py` & `gentab-0.1.2/tune.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     CTABGAN,
     CTABGANPlus,
     AutoDiffusion,
     ForestDiffusion,
     Tabula,
     GReaT,
 )
-from gentab.evaluators import KNN, LightGBM, XGBoost, MLP
+from gentab.evaluators import LightGBM, XGBoost, CatBoost, MLP
 from gentab.tuners import (
     SMOTETuner,
     ADASYNTuner,
     TVAETuner,
     CTGANTuner,
     GaussianCopulaTuner,
     CopulaGANTuner,
@@ -75,39 +75,39 @@
     tuner.save_to_disk()
     console.print(dataset.generated_class_counts(), dataset.generated_row_count())
 
 
 trials = 10
 
 configs = [
-    # ("configs/playnet.json", preproc_playnet, "PlayNet"),
+    ("configs/playnet.json", preproc_playnet, "PlayNet"),
     ("configs/adult.json", preproc_adult, "Adult"),
-    # ("configs/car_eval_4.json", preproc_car_eval_4, "Car Evaluation"),
+    ("configs/car_eval_4.json", preproc_car_eval_4, "Car Evaluation"),
 ]
 
 gens = [
     (SMOTE, "SMOTE", SMOTETuner),
     (ADASYN, "ADASYN", ADASYNTuner),
     (TVAE, "TVAE", TVAETuner),
     (CTGAN, "CTGAN", CTGANTuner),
     (GaussianCopula, "GaussianCopula", GaussianCopulaTuner),
     (CopulaGAN, "CopulaGAN", CopulaGANTuner),
     (CTABGAN, "CTAB-GAN", CTABGANTuner),
     (CTABGANPlus, "CTAB-GAN+", CTABGANPlusTuner),
     (AutoDiffusion, "AutoDiffusion", AutoDiffusionTuner),
     (ForestDiffusion, "ForestDiffusion", ForestDiffusionTuner),
-    (Tabula, "Tabula", TabulaTuner),
     (GReaT, "GReaT", GReaTTuner),
+    (Tabula, "Tabula", TabulaTuner),
 ]
 
 evals = [
-    (KNN, "KNN"),
     (LightGBM, "LightGBM"),
     (XGBoost, "XGBoost"),
-    # (MLP, "MLP"),
+    (CatBoost, "CatBoost"),
+    (MLP, "MLP"),
 ]
 
 for c in configs:
     console.print(c[2])
     dataset = c[1](Dataset(Config(c[0])))
 
     for g in gens:
```

### Comparing `gentab-0.1.1/visual_heatmap_playnet.py` & `gentab-0.1.2/visual_heatmap_playnet.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/visual_playnet.py` & `gentab-0.1.2/visual_playnet.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/configs/adult.json` & `gentab-0.1.2/configs/adult.json`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/configs/adult_cr.json` & `gentab-0.1.2/configs/adult_cr.json`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/configs/car_evaluation_cr.json` & `gentab-0.1.2/configs/car_evaluation_cr.json`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/configs/playnet.json` & `gentab-0.1.2/configs/playnet.json`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/configs/playnet_cr.json` & `gentab-0.1.2/configs/playnet_cr.json`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/utils.py` & `gentab-0.1.2/gentab/utils.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/data/dataset.py` & `gentab-0.1.2/gentab/data/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 from scipy.spatial.distance import jensenshannon
 from dython.nominal import theils_u
 from imblearn.datasets import fetch_datasets
 from ucimlrepo import fetch_ucirepo
 
 
 class Dataset:
-    def __init__(self, config) -> None:
+    def __init__(self, config, cache_path="datasets") -> None:
         self.config = config
+        self.cache_path = cache_path
         self.X_gen = None
         self.y_gen = None
 
         with ProgressBar(indeterminate=True).progress as p:
             gen_task = p.add_task(
                 "Loading dataset {}...".format(self.config["name"]), total=None
             )
@@ -65,17 +66,19 @@
             self.y,
             test_size=self.config["val_size"],
             random_state=SEED,
             stratify=self.y,
         )
 
     def download_imb(self) -> None:
+        Path(self.cache_path).mkdir(parents=True, exist_ok=True)
+
         data = fetch_datasets(
             filter_data=(self.config["name"],),
-            data_home=self.config["save_path"],
+            data_home=self.cache_path,
             random_state=SEED,
         )[self.config["name"]]
 
         features = pd.DataFrame(
             data=data.data,
             columns=["f" + str(i + 1) for i in range(data.data.shape[1])],
         )
@@ -100,27 +103,46 @@
         self.reset_indexes()
 
         self.config["binary_columns"] = self.X.columns.values.tolist()
         self.config["categorical_columns"] = []
         self.config["integer_columns"] = []
 
     def download_uci(self) -> None:
-        uci = fetch_ucirepo(name=self.config["name"])
+        Path(os.path.join(self.cache_path, "uci")).mkdir(parents=True, exist_ok=True)
+
+        path_features = os.path.join(
+            self.cache_path, "uci", self.config["name"] + "_features.csv"
+        )
+        path_targets = os.path.join(
+            self.cache_path, "uci", self.config["name"] + "_targets.csv"
+        )
 
-        # metadata
-        console.print(uci.variables)
+        if Path(path_features).is_file() and Path(path_targets).is_file():
+            features = pd.read_csv(path_features)
+            targets = pd.read_csv(path_targets)
+        else:
+            uci = fetch_ucirepo(name=self.config["name"])
 
-        uci.data.features.fillna("Missing", inplace=True)
+            # metadata
+            console.print(uci.variables)
+
+            uci.data.features.fillna("Missing", inplace=True)
+
+            uci.data.features.to_csv(path_features, index=False)
+            uci.data.targets.to_csv(path_targets, index=False)
+
+            features = uci.data.features
+            targets = uci.data.targets
 
         self.X, self.X_test, self.y, self.y_test = train_test_split(
-            uci.data.features,
-            uci.data.targets,
+            features,
+            targets,
             test_size=1 - self.config["train_size"],
             random_state=SEED,
-            stratify=uci.data.targets,
+            stratify=targets,
         )
         self.X_val, self.X_test, self.y_val, self.y_test = train_test_split(
             self.X_test,
             self.y_test,
             test_size=self.config["test_size"]
             / (self.config["test_size"] + self.config["val_size"]),
             random_state=SEED,
@@ -165,15 +187,15 @@
             self.X_gen = pd.read_csv(
                 os.path.join(path, "X_gen_" + str(generator) + ".csv")
             )
             self.y_gen = pd.read_csv(
                 os.path.join(path, "y_gen_" + str(generator) + ".csv")
             )
 
-        console.print("✅ {} dataset loaded...".format(generator))
+        console.print("✅ {} dataset loaded from {}...".format(generator, path))
 
     def compute_categories(self) -> None:
         self.cats = self.config["categorical_columns"] + self.config["binary_columns"]
         self.X_cats = self.X[self.cats].copy()
         self.X_cats[self.cats] = self.X_cats[self.cats].apply(
             lambda col: pd.Categorical(col)
         )
```

### Comparing `gentab-0.1.1/gentab/evaluators/catboost.py` & `gentab-0.1.2/gentab/evaluators/catboost.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class CatBoost(Evaluator):
     def __init__(
         self,
         generator,
         *args,
         **kwargs,
     ) -> None:
-        super().__init__(generator)
+        super().__init__(generator, **kwargs)
 
         self.model = CatBoostClassifier(
             *args,
             random_state=self.seed,
             silent=True,
             **kwargs,
         )
```

### Comparing `gentab-0.1.1/gentab/evaluators/evaluator.py` & `gentab-0.1.2/gentab/evaluators/evaluator.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,19 @@
     precision_recall_fscore_support,
     accuracy_score,
     matthews_corrcoef,
 )
 
 
 class Evaluator:
-    def __init__(self, generator) -> None:
+    def __init__(self, generator, round=2) -> None:
         self.seed = SEED
         self.generator = generator
         self.dataset = generator.dataset
+        self.round = round
         self.accuracy = None
         self.macro = None
         self.weighted = None
         self.callbacks = None
 
     def __str__(self) -> str:
         return self.__class__.__name__
@@ -80,17 +81,21 @@
                     self.dataset.y_test, predictions, "macro"
                 )
                 self.weighted = self.compute_f1_p_r(
                     self.dataset.y_test, predictions, "weighted"
                 )
 
             console.print(
-                "🎯 {} Accuracy: {}".format(generator, round(self.accuracy * 100, 1))
+                "🎯 {} Accuracy: {}".format(
+                    generator, round(self.accuracy * 100, self.round - 1)
+                )
+            )
+            console.print(
+                "🎯 {} MCC: {}".format(generator, round(self.mcc, self.round))
             )
-            console.print("🎯 {} MCC: {}".format(generator, round(self.mcc, 2)))
 
         console.print(
             "✅ Evaluation complete with {} for {} in {}...".format(
                 self, generator, self.dataset
             )
         )
```

### Comparing `gentab-0.1.1/gentab/evaluators/knn.py` & `gentab-0.1.2/gentab/evaluators/knn.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class KNN(Evaluator):
     def __init__(
         self,
         generator,
         *args,
         **kwargs,
     ) -> None:
-        super().__init__(generator)
+        super().__init__(generator, **kwargs)
         self.model = KNeighborsClassifier(
             *args,
             **kwargs,
         )
 
     def preprocess(self, X, y, X_test, y_test):
         X = self.dataset.encode_categories(X)
```

### Comparing `gentab-0.1.1/gentab/evaluators/lightgbm.py` & `gentab-0.1.2/gentab/evaluators/lightgbm.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class LightGBM(Evaluator):
     def __init__(
         self,
         generator,
         *args,
         **kwargs,
     ) -> None:
-        super().__init__(generator)
+        super().__init__(generator, **kwargs)
         self.model = lgb.LGBMClassifier(
             *args,
             random_state=self.seed,
             verbosity=0,
             **kwargs,
         )
         self.callbacks = [lgb.log_evaluation(period=0)]
```

### Comparing `gentab-0.1.1/gentab/evaluators/mlp.py` & `gentab-0.1.2/gentab/evaluators/mlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,15 +279,15 @@
         *args,
         layers: List[int] = [128, 128],
         dropout: float = 0.1,
         epochs: int = 1000,
         batch_size: int = 1024,
         **kwargs,
     ) -> None:
-        super().__init__(generator)
+        super().__init__(generator, **kwargs)
         self.model = MLPClassifier(
             self.dataset.num_features(),
             self.dataset.num_classes(),
             *args,
             layers,
             dropout,
             epochs=epochs,
```

### Comparing `gentab-0.1.1/gentab/evaluators/xgboost.py` & `gentab-0.1.2/gentab/evaluators/xgboost.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class XGBoost(Evaluator):
     def __init__(
         self,
         generator,
         *args,
         **kwargs,
     ) -> None:
-        super().__init__(generator)
+        super().__init__(generator, **kwargs)
         self.model = XGBClassifier(
             *args,
             verbosity=0,
             random_state=self.seed,
             # enable_categorical=True,
             # tree_method="hist",
             **kwargs,
```

### Comparing `gentab-0.1.1/gentab/generators/adasyn.py` & `gentab-0.1.2/gentab/generators/adasyn.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/autodiffusion.py` & `gentab-0.1.2/gentab/generators/autodiffusion.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/copulagan.py` & `gentab-0.1.2/gentab/generators/copulagan.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/ctabgan.py` & `gentab-0.1.2/gentab/generators/ctabgan.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/ctabganplus.py` & `gentab-0.1.2/gentab/generators/ctabganplus.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/ctgan.py` & `gentab-0.1.2/gentab/generators/ctgan.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/forestdiffusion.py` & `gentab-0.1.2/gentab/generators/forestdiffusion.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/gaussiancopula.py` & `gentab-0.1.2/gentab/generators/gaussiancopula.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/generator.py` & `gentab-0.1.2/gentab/generators/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def sample(self) -> pd.DataFrame:
         pass
 
     # def save_to_disk(self, tuner: str = "") -> None:
     #     self.dataset.save_to_disk(self, tuner)
 
     def load_from_disk(self, tuner: str = "") -> None:
-        self.dataset.load_from_disk(self, tuner)
+        self.dataset.load_from_disk(self)
 
     def resample(self, n_samples, append) -> None:
         n_samples = n_samples.copy()
 
         if append:
             data_gen = self.dataset.get_single_df()
         else:
```

### Comparing `gentab-0.1.1/gentab/generators/great.py` & `gentab-0.1.2/gentab/generators/great.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/randomoversampler.py` & `gentab-0.1.2/gentab/generators/randomoversampler.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/smote.py` & `gentab-0.1.2/gentab/generators/smote.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/tabula.py` & `gentab-0.1.2/gentab/generators/tabula.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/tvae.py` & `gentab-0.1.2/gentab/generators/tvae.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/autodiff/TabDDPMdiff.py` & `gentab-0.1.2/gentab/generators/autodiff/TabDDPMdiff.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/autodiff/autoencoder.py` & `gentab-0.1.2/gentab/generators/autodiff/autoencoder.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/autodiff/diffusion.py` & `gentab-0.1.2/gentab/generators/autodiff/diffusion.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/autodiff/process_GQ.py` & `gentab-0.1.2/gentab/generators/autodiff/process_GQ.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/autodiff/process_edited.py` & `gentab-0.1.2/gentab/generators/autodiff/process_edited.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/ctabg/pipeline/data_preparation.py` & `gentab-0.1.2/gentab/generators/ctabg/pipeline/data_preparation.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/ctabg/synthesizer/ctabgan_synthesizer.py` & `gentab-0.1.2/gentab/generators/ctabg/synthesizer/ctabgan_synthesizer.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/ctabg/synthesizer/transformer.py` & `gentab-0.1.2/gentab/generators/ctabg/synthesizer/transformer.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/ctabgplus/pipeline/data_preparation.py` & `gentab-0.1.2/gentab/generators/ctabgplus/pipeline/data_preparation.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/ctabgplus/privacy_utils/rdp_accountant.py` & `gentab-0.1.2/gentab/generators/ctabgplus/privacy_utils/rdp_accountant.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/ctabgplus/synthesizer/ctabgan_synthesizer.py` & `gentab-0.1.2/gentab/generators/ctabgplus/synthesizer/ctabgan_synthesizer.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/ctabgplus/synthesizer/transformer.py` & `gentab-0.1.2/gentab/generators/ctabgplus/synthesizer/transformer.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/dae/data.py` & `gentab-0.1.2/gentab/generators/dae/data.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/dae/engine.py` & `gentab-0.1.2/gentab/generators/dae/engine.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/dae/model.py` & `gentab-0.1.2/gentab/generators/dae/model.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/dae/network.py` & `gentab-0.1.2/gentab/generators/dae/network.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/dae/util.py` & `gentab-0.1.2/gentab/generators/dae/util.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/tabu/tabula.py` & `gentab-0.1.2/gentab/generators/tabu/tabula.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/tabu/tabula_dataset.py` & `gentab-0.1.2/gentab/generators/tabu/tabula_dataset.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/tabu/tabula_start.py` & `gentab-0.1.2/gentab/generators/tabu/tabula_start.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/tabu/tabula_trainer.py` & `gentab-0.1.2/gentab/generators/tabu/tabula_trainer.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/tabu/tabula_utils.py` & `gentab-0.1.2/gentab/generators/tabu/tabula_utils.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/tabump/tabula.py` & `gentab-0.1.2/gentab/generators/tabump/tabula.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/tabump/tabula_dataset.py` & `gentab-0.1.2/gentab/generators/tabump/tabula_dataset.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/tabump/tabula_start.py` & `gentab-0.1.2/gentab/generators/tabump/tabula_start.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/tabump/tabula_trainer.py` & `gentab-0.1.2/gentab/generators/tabump/tabula_trainer.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/generators/tabump/tabula_utils.py` & `gentab-0.1.2/gentab/generators/tabump/tabula_utils.py`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/gentab/tuners/adasyn.py` & `gentab-0.1.2/gentab/tuners/adasyn.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from . import Tuner
 from gentab.generators import ADASYN
 from gentab.evaluators import Evaluator
 from gentab.utils import console, SPINNER, REFRESH
 
 import optuna
-import copy
 
 
 class ADASYNTuner(Tuner):
     def __init__(
         self,
         evaluator: Evaluator,
         trials: int,
@@ -22,13 +21,12 @@
         n_neighbors = trial.suggest_int(
             "n_neighbors", 2, self.dataset.min_class_count(), log=True
         )
 
         self.generator = ADASYN(self.dataset, n_neighbors=n_neighbors)
         self.generator.generate()
 
-        trial.set_user_attr("timing", self.generator.timer.history)
-        trial.set_user_attr("dataset", copy.copy(self.dataset))
+        self.store_data(trial)
 
         acc, mcc = self.evaluator.evaluate(validation=True)
 
         return mcc
```

### Comparing `gentab-0.1.1/gentab/tuners/autodiffusion.py` & `gentab-0.1.2/gentab/tuners/autodiffusion.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,13 +66,12 @@
             sigma=sigma,
             T=T,
             batch_size=batch_size,
             max_tries_per_batch=self.max_tries_per_batch,
         )
         self.generator.generate()
 
-        trial.set_user_attr("timing", self.generator.timer.history)
-        trial.set_user_attr("dataset", self.dataset)
+        self.store_data(trial)
 
         acc, mcc = self.evaluator.evaluate(validation=True)
 
         return mcc
```

### Comparing `gentab-0.1.1/gentab/tuners/copulagan.py` & `gentab-0.1.2/gentab/tuners/copulagan.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,13 +75,12 @@
             generator_lr=generator_lr,
             log_frequency=log_frequency,
             pac=pac,
             max_tries_per_batch=self.max_tries_per_batch,
         )
         self.generator.generate()
 
-        trial.set_user_attr("timing", self.generator.timer.history)
-        trial.set_user_attr("dataset", self.dataset)
+        self.store_data(trial)
 
         acc, mcc = self.evaluator.evaluate(validation=True)
 
         return mcc
```

### Comparing `gentab-0.1.1/gentab/tuners/ctabgan.py` & `gentab-0.1.2/gentab/tuners/ctabgan.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,13 +56,12 @@
             random_dim=random_dim,
             l2scale=l2scale,
             batch_size=batch_size,
             max_tries_per_batch=self.max_tries_per_batch,
         )
         self.generator.generate()
 
-        trial.set_user_attr("timing", self.generator.timer.history)
-        trial.set_user_attr("dataset", self.dataset)
+        self.store_data(trial)
 
         acc, mcc = self.evaluator.evaluate(validation=True)
 
         return mcc
```

### Comparing `gentab-0.1.1/gentab/tuners/ctabganplus.py` & `gentab-0.1.2/gentab/tuners/ctabganplus.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,13 +56,12 @@
             random_dim=random_dim,
             l2scale=l2scale,
             batch_size=batch_size,
             max_tries_per_batch=self.max_tries_per_batch,
         )
         self.generator.generate()
 
-        trial.set_user_attr("timing", self.generator.timer.history)
-        trial.set_user_attr("dataset", self.dataset)
+        self.store_data(trial)
 
         acc, mcc = self.evaluator.evaluate(validation=True)
 
         return mcc
```

### Comparing `gentab-0.1.1/gentab/tuners/ctgan.py` & `gentab-0.1.2/gentab/tuners/ctgan.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,13 +70,12 @@
             generator_lr=generator_lr,
             log_frequency=log_frequency,
             pac=pac,
             max_tries_per_batch=self.max_tries_per_batch,
         )
         self.generator.generate()
 
-        trial.set_user_attr("timing", self.generator.timer.history)
-        trial.set_user_attr("dataset", self.dataset)
+        self.store_data(trial)
 
         acc, mcc = self.evaluator.evaluate(validation=True)
 
         return mcc
```

### Comparing `gentab-0.1.1/gentab/tuners/forestdiffusion.py` & `gentab-0.1.2/gentab/tuners/forestdiffusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,13 +68,12 @@
             beta_min=beta_min,
             beta_max=beta_max,
             # n_batch=batch_size,
             max_tries_per_batch=self.max_tries_per_batch,
         )
         self.generator.generate()
 
-        trial.set_user_attr("timing", self.generator.timer.history)
-        trial.set_user_attr("dataset", self.dataset)
+        self.store_data(trial)
 
         acc, mcc = self.evaluator.evaluate(validation=True)
 
         return mcc
```

### Comparing `gentab-0.1.1/gentab/tuners/gaussiancopula.py` & `gentab-0.1.2/gentab/tuners/gaussiancopula.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,13 +29,12 @@
         self.generator = GaussianCopula(
             self.dataset,
             default_distribution=default_distribution,
             max_tries_per_batch=self.max_tries_per_batch,
         )
         self.generator.generate()
 
-        trial.set_user_attr("timing", self.generator.timer.history)
-        trial.set_user_attr("dataset", self.dataset)
+        self.store_data(trial)
 
         acc, mcc = self.evaluator.evaluate(validation=True)
 
         return mcc
```

### Comparing `gentab-0.1.1/gentab/tuners/great.py` & `gentab-0.1.2/gentab/tuners/great.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,13 +43,12 @@
             batch_size=batch_size,
             temperature=temperature,
             k=k,
             max_tries_per_batch=self.max_tries_per_batch,
         )
         self.generator.generate()
 
-        trial.set_user_attr("timing", self.generator.timer.history)
-        trial.set_user_attr("dataset", self.dataset)
+        self.store_data(trial)
 
         acc, mcc = self.evaluator.evaluate(validation=True)
 
         return mcc
```

### Comparing `gentab-0.1.1/gentab/tuners/smote.py` & `gentab-0.1.2/gentab/tuners/smote.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,13 +21,12 @@
         k_neighbors = trial.suggest_int(
             "k_neighbors", 2, self.dataset.min_class_count(), log=True
         )
 
         self.generator = SMOTE(self.dataset, k_neighbors=k_neighbors)
         self.generator.generate()
 
-        trial.set_user_attr("timing", self.generator.timer.history)
-        trial.set_user_attr("dataset", self.dataset)
+        self.store_data(trial)
 
         acc, mcc = self.evaluator.evaluate(validation=True)
 
         return mcc
```

### Comparing `gentab-0.1.1/gentab/tuners/tabula.py` & `gentab-0.1.2/gentab/tuners/tabula.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,13 +53,12 @@
             batch_size=batch_size,
             temperature=temperature,
             k=k,
             max_tries_per_batch=self.max_tries_per_batch,
         )
         self.generator.generate()
 
-        trial.set_user_attr("timing", self.generator.timer.history)
-        trial.set_user_attr("dataset", self.dataset)
+        self.store_data(trial)
 
         acc, mcc = self.evaluator.evaluate(validation=True)
 
         return mcc
```

### Comparing `gentab-0.1.1/gentab/tuners/tuner.py` & `gentab-0.1.2/gentab/tuners/tuner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from gentab.evaluators import Evaluator
 from gentab.utils import console, SPINNER, REFRESH
 from gentab import SEED
 
 from pathlib import Path
 import json
 import os
+import copy
+
 import optuna
 
 
 class Tuner:
     def __init__(
         self,
         evaluator: Evaluator,
@@ -37,20 +39,27 @@
         self.max_tries_per_batch = max_tries_per_batch
         self.folder = "tuning"
         self.timeout = timeout
 
     def __str__(self) -> str:
         return self.__class__.__name__
 
+    def store_data(self, trial: optuna.trial.Trial) -> None:
+        trial.set_user_attr("timing", self.generator.timer.history)
+        trial.set_user_attr("dataset", copy.deepcopy(self.dataset))
+
     def objective(self, trial: optuna.trial.Trial) -> float:
         pass
 
     def save_to_disk(self):
         self.dataset.save_to_disk(self.generator, self.evaluator)
 
+    def load_from_disk(self):
+        self.dataset.load_from_disk(self.generator, self.evaluator)
+
     def tune(self) -> None:
         # pruner: optuna.pruners.BasePruner(optuna.pruners.NopPruner())
 
         self.study = optuna.create_study(
             study_name=self,
             direction="maximize",
             sampler=optuna.samplers.TPESampler(seed=self.seed),
```

### Comparing `gentab-0.1.1/gentab/tuners/tvae.py` & `gentab-0.1.2/gentab/tuners/tvae.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,13 +57,12 @@
             l2scale=l2scale,
             loss_factor=loss_factor,
             pac=pac,
             max_tries_per_batch=self.max_tries_per_batch,
         )
         self.generator.generate()
 
-        trial.set_user_attr("timing", self.generator.timer.history)
-        trial.set_user_attr("dataset", self.dataset)
+        self.store_data(trial)
 
         acc, mcc = self.evaluator.evaluate(validation=True)
 
         return mcc
```

### Comparing `gentab-0.1.1/.gitignore` & `gentab-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/LICENSE` & `gentab-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gentab-0.1.1/README.md` & `gentab-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -155,7 +155,41 @@
 
 trials = 10
 time = 60 * 60 * 8
 tuner = AutoDiffusionTuner(evaluator, trials, timeout=time)
 tuner.tune()
 tuner.save_to_disk()
 ```
+
+### Loading Stored Synthetic Datasets
+
+``` python
+from gentab.generators import AutoDiffusion
+from gentab.evaluators import LightGBM
+from gentab.tuners import AutoDiffusionTuner
+from gentab.data import Config, Dataset
+
+config = Config("configs/adult.json")
+
+dataset = Dataset(config)
+dataset.merge_classes({
+    "<=50K": ["<=50K."], ">50K": [">50K."]
+})
+dataset.reduce_mem()
+
+# Load previously saved dataset...
+generator = AutoDiffusion(dataset)
+generator.load_from_disk()
+
+# Do work with previously generated but not tuned dataset...
+evaluator = LightGBM(generator)
+evaluator.evaluate()
+evaluator.evaluate_baseline()
+
+# Load previously tuned and saved dataset...
+tuner = AutoDiffusionTuner(evaluator, 0)
+tuner.load_from_disk()
+
+# Do work with previously tuned dataset...
+evaluator.evaluate()
+evaluator.evaluate_baseline()
+```
```

#### html2text {}

```diff
@@ -81,8 +81,20 @@
 dataset.save_to_disk(generator) ``` ### Tuning ``` python from
 gentab.generators import AutoDiffusion from gentab.evaluators import LightGBM
 from gentab.tuners import AutoDiffusionTuner from gentab.data import Config,
 Dataset config = Config("configs/adult.json") dataset = Dataset(config)
 dataset.merge_classes({ "<=50K": ["<=50K."], ">50K": [">50K."] })
 dataset.reduce_mem() generator = AutoDiffusion(dataset) evaluator = LightGBM
 (generator) trials = 10 time = 60 * 60 * 8 tuner = AutoDiffusionTuner
-(evaluator, trials, timeout=time) tuner.tune() tuner.save_to_disk() ```
+(evaluator, trials, timeout=time) tuner.tune() tuner.save_to_disk() ``` ###
+Loading Stored Synthetic Datasets ``` python from gentab.generators import
+AutoDiffusion from gentab.evaluators import LightGBM from gentab.tuners import
+AutoDiffusionTuner from gentab.data import Config, Dataset config = Config
+("configs/adult.json") dataset = Dataset(config) dataset.merge_classes(
+{ "<=50K": ["<=50K."], ">50K": [">50K."] }) dataset.reduce_mem() # Load
+previously saved dataset... generator = AutoDiffusion(dataset)
+generator.load_from_disk() # Do work with previously generated but not tuned
+dataset... evaluator = LightGBM(generator) evaluator.evaluate()
+evaluator.evaluate_baseline() # Load previously tuned and saved dataset...
+tuner = AutoDiffusionTuner(evaluator, 0) tuner.load_from_disk() # Do work with
+previously tuned dataset... evaluator.evaluate() evaluator.evaluate_baseline()
+```
```

### Comparing `gentab-0.1.1/pyproject.toml` & `gentab-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gentab"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Omar A. Mures", email="omar.alvarez@udc.es" },
 ]
 description = "A synthetic tabular data generation library."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `gentab-0.1.1/PKG-INFO` & `gentab-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gentab
-Version: 0.1.1
+Version: 0.1.2
 Summary: A synthetic tabular data generation library.
 Project-URL: Homepage, https://github.com/omaralvarez/gentab
 Project-URL: Issues, https://github.com/omaralvarez/gentab/issues
 Author-email: "Omar A. Mures" <omar.alvarez@udc.es>
 License-File: LICENSE
 Keywords: data,deep learning,generation,machine learning,synthetic,tabular
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -193,7 +193,41 @@
 
 trials = 10
 time = 60 * 60 * 8
 tuner = AutoDiffusionTuner(evaluator, trials, timeout=time)
 tuner.tune()
 tuner.save_to_disk()
 ```
+
+### Loading Stored Synthetic Datasets
+
+``` python
+from gentab.generators import AutoDiffusion
+from gentab.evaluators import LightGBM
+from gentab.tuners import AutoDiffusionTuner
+from gentab.data import Config, Dataset
+
+config = Config("configs/adult.json")
+
+dataset = Dataset(config)
+dataset.merge_classes({
+    "<=50K": ["<=50K."], ">50K": [">50K."]
+})
+dataset.reduce_mem()
+
+# Load previously saved dataset...
+generator = AutoDiffusion(dataset)
+generator.load_from_disk()
+
+# Do work with previously generated but not tuned dataset...
+evaluator = LightGBM(generator)
+evaluator.evaluate()
+evaluator.evaluate_baseline()
+
+# Load previously tuned and saved dataset...
+tuner = AutoDiffusionTuner(evaluator, 0)
+tuner.load_from_disk()
+
+# Do work with previously tuned dataset...
+evaluator.evaluate()
+evaluator.evaluate_baseline()
+```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: gentab Version: 0.1.1 Summary: A synthetic tabular
+Metadata-Version: 2.3 Name: gentab Version: 0.1.2 Summary: A synthetic tabular
 data generation library. Project-URL: Homepage, https://github.com/omaralvarez/
 gentab Project-URL: Issues, https://github.com/omaralvarez/gentab/issues
 Author-email: "Omar A. Mures"
 udc.es> License-File: LICENSE Keywords: data,deep learning,generation,machine
 learning,synthetic,tabular Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.9
@@ -100,8 +100,20 @@
 dataset.save_to_disk(generator) ``` ### Tuning ``` python from
 gentab.generators import AutoDiffusion from gentab.evaluators import LightGBM
 from gentab.tuners import AutoDiffusionTuner from gentab.data import Config,
 Dataset config = Config("configs/adult.json") dataset = Dataset(config)
 dataset.merge_classes({ "<=50K": ["<=50K."], ">50K": [">50K."] })
 dataset.reduce_mem() generator = AutoDiffusion(dataset) evaluator = LightGBM
 (generator) trials = 10 time = 60 * 60 * 8 tuner = AutoDiffusionTuner
-(evaluator, trials, timeout=time) tuner.tune() tuner.save_to_disk() ```
+(evaluator, trials, timeout=time) tuner.tune() tuner.save_to_disk() ``` ###
+Loading Stored Synthetic Datasets ``` python from gentab.generators import
+AutoDiffusion from gentab.evaluators import LightGBM from gentab.tuners import
+AutoDiffusionTuner from gentab.data import Config, Dataset config = Config
+("configs/adult.json") dataset = Dataset(config) dataset.merge_classes(
+{ "<=50K": ["<=50K."], ">50K": [">50K."] }) dataset.reduce_mem() # Load
+previously saved dataset... generator = AutoDiffusion(dataset)
+generator.load_from_disk() # Do work with previously generated but not tuned
+dataset... evaluator = LightGBM(generator) evaluator.evaluate()
+evaluator.evaluate_baseline() # Load previously tuned and saved dataset...
+tuner = AutoDiffusionTuner(evaluator, 0) tuner.load_from_disk() # Do work with
+previously tuned dataset... evaluator.evaluate() evaluator.evaluate_baseline()
+```
```

