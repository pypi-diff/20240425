# Comparing `tmp/mindspore_gs-0.3.0-py3-none-any.whl.zip` & `tmp/mindspore_gs-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,86 +1,122 @@
-Zip file size: 157253 bytes, number of entries: 84
--rw-r--r--  2.0 unx       82 b- defN 23-Jan-31 01:22 mindspore_gs/.commit_id
--rw-------  2.0 unx     1156 b- defN 23-Jan-31 01:21 mindspore_gs/__init__.py
--rw-------  2.0 unx     9205 b- defN 23-Jan-31 01:21 mindspore_gs/comp_algo.py
--rw-------  2.0 unx     4088 b- defN 23-Jan-31 01:21 mindspore_gs/net_transform.py
--rw-------  2.0 unx     2584 b- defN 23-Jan-31 01:21 mindspore_gs/version.py
--rw-------  2.0 unx      703 b- defN 23-Jan-31 01:21 mindspore_gs/ops/__init__.py
--rw-------  2.0 unx      710 b- defN 23-Jan-31 01:21 mindspore_gs/ops/common/__init__.py
--rw-------  2.0 unx     1005 b- defN 23-Jan-31 01:21 mindspore_gs/ops/common/quant_op_utils.py
--rw-------  2.0 unx     5210 b- defN 23-Jan-31 01:21 mindspore_gs/ops/kernel/gpu/fake_quant_impl.cuh
--rw-------  2.0 unx     5032 b- defN 23-Jan-31 01:21 mindspore_gs/ops/kernel/gpu/fake_quant_per_channel_grad_impl.cu
--rw-------  2.0 unx     6210 b- defN 23-Jan-31 01:21 mindspore_gs/ops/kernel/gpu/fake_quant_per_channel_impl.cu
--rw-------  2.0 unx     4650 b- defN 23-Jan-31 01:21 mindspore_gs/ops/kernel/gpu/fake_quant_per_layer_grad_impl.cu
--rw-------  2.0 unx     5350 b- defN 23-Jan-31 01:21 mindspore_gs/ops/kernel/gpu/fake_quant_per_layer_impl.cu
--rw-------  2.0 unx     4199 b- defN 23-Jan-31 01:21 mindspore_gs/ops/kernel/gpu/min_max_update_per_channel_impl.cu
--rw-------  2.0 unx     4204 b- defN 23-Jan-31 01:21 mindspore_gs/ops/kernel/gpu/min_max_update_per_layer_impl.cu
--rw-------  2.0 unx     2961 b- defN 23-Jan-31 01:21 mindspore_gs/ops/kernel/gpu/aot/custom_aot_extra.h
--rw-------  2.0 unx     1433 b- defN 23-Jan-31 01:21 mindspore_gs/ops/nn/__init__.py
--rw-------  2.0 unx     5519 b- defN 23-Jan-31 01:21 mindspore_gs/ops/nn/act_quant.py
--rw-------  2.0 unx     3698 b- defN 23-Jan-31 01:21 mindspore_gs/ops/nn/batchnorm_fold_cell.py
--rw-------  2.0 unx    15276 b- defN 23-Jan-31 01:21 mindspore_gs/ops/nn/conv2d_bn_fold_quant.py
--rw-------  2.0 unx    14582 b- defN 23-Jan-31 01:21 mindspore_gs/ops/nn/conv2d_bn_fold_quant_one_conv.py
--rw-------  2.0 unx    10469 b- defN 23-Jan-31 01:21 mindspore_gs/ops/nn/conv2d_bn_without_fold_quant.py
--rw-------  2.0 unx    10454 b- defN 23-Jan-31 01:21 mindspore_gs/ops/nn/conv2d_quant.py
--rw-------  2.0 unx     8550 b- defN 23-Jan-31 01:21 mindspore_gs/ops/nn/dense_quant.py
--rw-------  2.0 unx    21743 b- defN 23-Jan-31 01:21 mindspore_gs/ops/nn/fake_quant_with_min_max_observer.py
--rw-------  2.0 unx     3646 b- defN 23-Jan-31 01:21 mindspore_gs/ops/nn/mul_quant.py
--rw-------  2.0 unx     3693 b- defN 23-Jan-31 01:21 mindspore_gs/ops/nn/tensor_add_quant.py
--rw-------  2.0 unx     1165 b- defN 23-Jan-31 01:21 mindspore_gs/ops/operations/__init__.py
--rw-------  2.0 unx     5702 b- defN 23-Jan-31 01:21 mindspore_gs/ops/operations/fake_quant_perchannel.py
--rw-------  2.0 unx     5350 b- defN 23-Jan-31 01:21 mindspore_gs/ops/operations/fake_quant_perlayer.py
--rw-------  2.0 unx    14042 b- defN 23-Jan-31 01:21 mindspore_gs/ops/operations/gs_custom.py
--rw-------  2.0 unx     3821 b- defN 23-Jan-31 01:21 mindspore_gs/ops/operations/min_max_update_perchannel.py
--rw-------  2.0 unx     3535 b- defN 23-Jan-31 01:21 mindspore_gs/ops/operations/min_max_update_perlayer.py
--rw-------  2.0 unx      914 b- defN 23-Jan-31 01:21 mindspore_gs/ops/operations/grad_operations/__init__.py
--rw-------  2.0 unx     2615 b- defN 23-Jan-31 01:21 mindspore_gs/ops/operations/grad_operations/fake_quant_perchannel_grad.py
--rw-------  2.0 unx     2575 b- defN 23-Jan-31 01:21 mindspore_gs/ops/operations/grad_operations/fake_quant_perlayer_grad.py
--rw-------  2.0 unx      982 b- defN 23-Jan-31 01:21 mindspore_gs/pruner/__init__.py
--rw-------  2.0 unx      833 b- defN 23-Jan-31 01:21 mindspore_gs/pruner/scop/__init__.py
--rw-------  2.0 unx    22191 b- defN 23-Jan-31 01:21 mindspore_gs/pruner/scop/scop_pruner.py
--rw-------  2.0 unx      768 b- defN 23-Jan-31 01:21 mindspore_gs/pruner/uni_pruning/__init__.py
--rw-------  2.0 unx    14990 b- defN 23-Jan-31 01:21 mindspore_gs/pruner/uni_pruning/graph_analyzer_mindir.py
--rw-------  2.0 unx    12909 b- defN 23-Jan-31 01:21 mindspore_gs/pruner/uni_pruning/uni_pruner.py
--rw-------  2.0 unx     1092 b- defN 23-Jan-31 01:21 mindspore_gs/pruner/uni_pruning/utils/__init__.py
--rw-------  2.0 unx     3497 b- defN 23-Jan-31 01:21 mindspore_gs/pruner/uni_pruning/utils/importance_criteria.py
--rw-------  2.0 unx     5658 b- defN 23-Jan-31 01:21 mindspore_gs/pruner/uni_pruning/utils/mask.py
--rw-------  2.0 unx     4484 b- defN 23-Jan-31 01:21 mindspore_gs/pruner/uni_pruning/utils/model_utils.py
--rw-------  2.0 unx     3900 b- defN 23-Jan-31 01:21 mindspore_gs/pruner/uni_pruning/utils/prune.py
--rw-------  2.0 unx     1019 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/__init__.py
--rw-------  2.0 unx      808 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/fake_quantizer.py
--rw-------  2.0 unx     4061 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/layer_policy.py
--rw-------  2.0 unx     1690 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/net_policy.py
--rw-------  2.0 unx     8947 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/quant_utils.py
--rw-------  2.0 unx     8793 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/quantization_aware_training.py
--rw-------  2.0 unx     2869 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/quantize_wrapper_cell.py
--rw-------  2.0 unx     4671 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/transformer.py
--rw-------  2.0 unx      887 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/learned_step_size_quantization/__init__.py
--rw-------  2.0 unx     6775 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_fake_quantizers.py
--rw-------  2.0 unx    21841 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_quantization_aware_training.py
--rw-------  2.0 unx     1367 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_quantization_config.py
--rw-------  2.0 unx     5482 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_quantization_layer_policy.py
--rw-------  2.0 unx     1859 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_quantization_net_policy.py
--rw-------  2.0 unx      859 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/simulated_quantization/__init__.py
--rw-------  2.0 unx     5959 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/simulated_quantization/combined.py
--rw-------  2.0 unx     9067 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/simulated_quantization/simulated_fake_quantizers.py
--rw-------  2.0 unx    25779 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/simulated_quantization/simulated_quantization_aware_training.py
--rw-------  2.0 unx     1600 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/simulated_quantization/simulated_quantization_config.py
--rw-------  2.0 unx     7586 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/simulated_quantization/simulated_quantization_convert.py
--rw-------  2.0 unx     6668 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/simulated_quantization/simulated_quantization_layer_policy.py
--rw-------  2.0 unx     3052 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/simulated_quantization/simulated_quantization_net_policy.py
--rw-------  2.0 unx     9319 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/simulated_quantization/simulated_quantization_transforms.py
--rw-------  2.0 unx      847 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/slb/__init__.py
--rw-------  2.0 unx     8428 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/slb/slb_fake_quantizer.py
--rw-------  2.0 unx     4499 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/slb/slb_layer_policy.py
--rw-------  2.0 unx     1551 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/slb/slb_net_policy.py
--rw-------  2.0 unx    10802 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/slb/slb_quant.py
--rw-------  2.0 unx    28645 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/slb/slb_quant_aware_training.py
--rw-------  2.0 unx     1409 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/slb/slb_quant_config.py
--rw-------  2.0 unx     8421 b- defN 23-Jan-31 01:21 mindspore_gs/quantization/slb/slb_quant_convert.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jan-31 01:22 mindspore_gs-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1123 b- defN 23-Jan-31 01:22 mindspore_gs-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       67 b- defN 23-Jan-31 01:22 mindspore_gs-0.3.0.dist-info/NOTICE
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-31 01:22 mindspore_gs-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Jan-31 01:22 mindspore_gs-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     9077 b- defN 23-Jan-31 01:22 mindspore_gs-0.3.0.dist-info/RECORD
-84 files, 494724 bytes uncompressed, 142153 bytes compressed:  71.3%
+Zip file size: 204330 bytes, number of entries: 120
+-rw-r--r--  2.0 unx       70 b- defN 24-Mar-31 08:02 mindspore_gs/.commit_id
+-rw-------  2.0 unx     1412 b- defN 24-Mar-31 08:01 mindspore_gs/__init__.py
+-rw-------  2.0 unx     9365 b- defN 24-Mar-31 08:01 mindspore_gs/comp_algo.py
+-rw-------  2.0 unx     6007 b- defN 24-Mar-31 08:01 mindspore_gs/net_transform.py
+-rw-------  2.0 unx      916 b- defN 24-Mar-31 08:01 mindspore_gs/validator.py
+-rw-------  2.0 unx     2627 b- defN 24-Mar-31 08:01 mindspore_gs/version.py
+-rw-------  2.0 unx      774 b- defN 24-Mar-31 08:01 mindspore_gs/common/__init__.py
+-rw-------  2.0 unx     2010 b- defN 24-Mar-31 08:01 mindspore_gs/common/config.py
+-rw-------  2.0 unx     1486 b- defN 24-Mar-31 08:01 mindspore_gs/common/gs_enum.py
+-rw-------  2.0 unx     2079 b- defN 24-Mar-31 08:01 mindspore_gs/common/register.py
+-rw-------  2.0 unx     1942 b- defN 24-Mar-31 08:01 mindspore_gs/common/utils.py
+-rw-------  2.0 unx      796 b- defN 24-Mar-31 08:01 mindspore_gs/datasets/__init__.py
+-rw-------  2.0 unx     6237 b- defN 24-Mar-31 08:01 mindspore_gs/datasets/squad.py
+-rw-------  2.0 unx     4230 b- defN 24-Mar-31 08:01 mindspore_gs/datasets/wikitext2.py
+-rw-------  2.0 unx      874 b- defN 24-Mar-31 08:01 mindspore_gs/ghost/__init__.py
+-rw-------  2.0 unx     9654 b- defN 24-Mar-31 08:01 mindspore_gs/ghost/ghost.py
+-rw-------  2.0 unx      822 b- defN 24-Mar-31 08:01 mindspore_gs/ops/__init__.py
+-rw-------  2.0 unx    13247 b- defN 24-Mar-31 08:01 mindspore_gs/ops/gs_custom.py
+-rw-------  2.0 unx      995 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/__init__.py
+-rw-------  2.0 unx      843 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/heads/__init__.py
+-rw-------  2.0 unx     4351 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/heads/abstract.py
+-rw-------  2.0 unx     1860 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/heads/factory.py
+-rw-------  2.0 unx      837 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/heads/supported.py
+-rw-------  2.0 unx      806 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/heads/type.py
+-rw-------  2.0 unx      763 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/heads/lrp/__init__.py
+-rw-------  2.0 unx     3095 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/heads/lrp/abstract_lrp.py
+-rw-------  2.0 unx    10973 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/heads/lrp/utils.py
+-rw-------  2.0 unx      892 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/ops/__init__.py
+-rw-------  2.0 unx     3732 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/ops/masked_cell.py
+-rw-------  2.0 unx     2019 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/ops/masked_conv2d.py
+-rw-------  2.0 unx     2011 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/ops/masked_dense.py
+-rw-------  2.0 unx      833 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/scop/__init__.py
+-rw-------  2.0 unx    22203 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/scop/scop_pruner.py
+-rw-------  2.0 unx      768 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/uni_pruning/__init__.py
+-rw-------  2.0 unx    15494 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/uni_pruning/uni_pruner.py
+-rw-------  2.0 unx     6558 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/uni_pruning/unipruning_masked_layer.py
+-rw-------  2.0 unx      766 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/uni_pruning/graph_analyzer/__init__.py
+-rw-------  2.0 unx     4197 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/uni_pruning/graph_analyzer/equichannel_group.py
+-rw-------  2.0 unx     5044 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/uni_pruning/graph_analyzer/graph.py
+-rw-------  2.0 unx     6559 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/uni_pruning/graph_analyzer/graph_analyzer.py
+-rw-------  2.0 unx     1092 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/uni_pruning/utils/__init__.py
+-rw-------  2.0 unx     3495 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/uni_pruning/utils/importance_criteria.py
+-rw-------  2.0 unx     5658 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/uni_pruning/utils/mask.py
+-rw-------  2.0 unx     4482 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/uni_pruning/utils/model_utils.py
+-rw-------  2.0 unx     3900 b- defN 24-Mar-31 08:01 mindspore_gs/pruner/uni_pruning/utils/prune.py
+-rw-------  2.0 unx      803 b- defN 24-Mar-31 08:01 mindspore_gs/ptq/__init__.py
+-rw-------  2.0 unx     9769 b- defN 24-Mar-31 08:01 mindspore_gs/ptq/convert_utils.py
+-rw-------  2.0 unx     9712 b- defN 24-Mar-31 08:01 mindspore_gs/ptq/fake_quantizer.py
+-rw-------  2.0 unx     1521 b- defN 24-Mar-31 08:01 mindspore_gs/ptq/processor.py
+-rw-------  2.0 unx     8405 b- defN 24-Mar-31 08:01 mindspore_gs/ptq/ptq_config.py
+-rw-------  2.0 unx    10320 b- defN 24-Mar-31 08:01 mindspore_gs/ptq/quant_cells.py
+-rw-------  2.0 unx      765 b- defN 24-Mar-31 08:01 mindspore_gs/ptq/round_to_nearest/__init__.py
+-rw-------  2.0 unx     8436 b- defN 24-Mar-31 08:01 mindspore_gs/ptq/round_to_nearest/round_to_nearest.py
+-rw-------  2.0 unx     5308 b- defN 24-Mar-31 08:01 mindspore_gs/ptq/round_to_nearest/rtn_layer_policy.py
+-rw-------  2.0 unx     1728 b- defN 24-Mar-31 08:01 mindspore_gs/ptq/round_to_nearest/rtn_net_policy.py
+-rw-------  2.0 unx     1019 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/__init__.py
+-rw-------  2.0 unx     4741 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/fake_quantizer.py
+-rw-------  2.0 unx     5614 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/layer_policy.py
+-rw-------  2.0 unx     1684 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/net_policy.py
+-rw-------  2.0 unx     4039 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/quant_cell.py
+-rw-------  2.0 unx    13203 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/quant_utils.py
+-rw-------  2.0 unx     7994 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/quantization_aware_training.py
+-rw-------  2.0 unx     4671 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/transformer.py
+-rw-------  2.0 unx      887 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/learned_step_size_quantization/__init__.py
+-rw-------  2.0 unx     8168 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_fake_quantizers.py
+-rw-------  2.0 unx    21769 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_quantization_aware_training.py
+-rw-------  2.0 unx     1367 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_quantization_config.py
+-rw-------  2.0 unx     6733 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_quantization_layer_policy.py
+-rw-------  2.0 unx     1687 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_quantization_net_policy.py
+-rw-------  2.0 unx      723 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/__init__.py
+-rw-------  2.0 unx     5210 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/kernel/gpu/fake_quant_impl.cuh
+-rw-------  2.0 unx     5032 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/kernel/gpu/fake_quant_per_channel_grad_impl.cu
+-rw-------  2.0 unx     6210 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/kernel/gpu/fake_quant_per_channel_impl.cu
+-rw-------  2.0 unx     4650 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/kernel/gpu/fake_quant_per_layer_grad_impl.cu
+-rw-------  2.0 unx     5350 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/kernel/gpu/fake_quant_per_layer_impl.cu
+-rw-------  2.0 unx     4199 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/kernel/gpu/min_max_update_per_channel_impl.cu
+-rw-------  2.0 unx     4204 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/kernel/gpu/min_max_update_per_layer_impl.cu
+-rw-------  2.0 unx     2961 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/kernel/gpu/aot/custom_aot_extra.h
+-rw-------  2.0 unx     1432 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/nn/__init__.py
+-rw-------  2.0 unx     2639 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/nn/act_quant.py
+-rw-------  2.0 unx     3698 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/nn/batchnorm_fold_cell.py
+-rw-------  2.0 unx    10281 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/nn/conv2d_bn_fold_quant.py
+-rw-------  2.0 unx    11957 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/nn/conv2d_bn_fold_quant_one_conv.py
+-rw-------  2.0 unx     8377 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/nn/conv2d_bn_without_fold_quant.py
+-rw-------  2.0 unx     5654 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/nn/conv2d_quant.py
+-rw-------  2.0 unx     6220 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/nn/dense_quant.py
+-rw-------  2.0 unx    21830 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/nn/fake_quant_with_min_max_observer.py
+-rw-------  2.0 unx     3055 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/nn/mul_quant.py
+-rw-------  2.0 unx     3101 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/nn/tensor_add_quant.py
+-rw-------  2.0 unx     1062 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/operations/__init__.py
+-rw-------  2.0 unx     6519 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/operations/fake_quant_perchannel.py
+-rw-------  2.0 unx     6165 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/operations/fake_quant_perlayer.py
+-rw-------  2.0 unx     4669 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/operations/min_max_update_perchannel.py
+-rw-------  2.0 unx     4381 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/operations/min_max_update_perlayer.py
+-rw-------  2.0 unx      914 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/operations/grad_operations/__init__.py
+-rw-------  2.0 unx     3466 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/operations/grad_operations/fake_quant_perchannel_grad.py
+-rw-------  2.0 unx     3424 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/ops/operations/grad_operations/fake_quant_perlayer_grad.py
+-rw-------  2.0 unx      859 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/simulated_quantization/__init__.py
+-rw-------  2.0 unx     5537 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/simulated_quantization/combined.py
+-rw-------  2.0 unx     9049 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/simulated_quantization/simulated_fake_quantizers.py
+-rw-------  2.0 unx    26050 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/simulated_quantization/simulated_quantization_aware_training.py
+-rw-------  2.0 unx     1610 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/simulated_quantization/simulated_quantization_config.py
+-rw-------  2.0 unx     1760 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/simulated_quantization/simulated_quantization_convert.py
+-rw-------  2.0 unx     7372 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/simulated_quantization/simulated_quantization_layer_policy.py
+-rw-------  2.0 unx     2761 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/simulated_quantization/simulated_quantization_net_policy.py
+-rw-------  2.0 unx     9319 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/simulated_quantization/simulated_quantization_transforms.py
+-rw-------  2.0 unx      847 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/slb/__init__.py
+-rw-------  2.0 unx     9745 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/slb/slb_fake_quantizer.py
+-rw-------  2.0 unx     3871 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/slb/slb_layer_policy.py
+-rw-------  2.0 unx     1575 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/slb/slb_net_policy.py
+-rw-------  2.0 unx     8986 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/slb/slb_quant.py
+-rw-------  2.0 unx    28708 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/slb/slb_quant_aware_training.py
+-rw-------  2.0 unx     1419 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/slb/slb_quant_config.py
+-rw-------  2.0 unx     2065 b- defN 24-Mar-31 08:01 mindspore_gs/quantization/slb/slb_quant_convert.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-Mar-31 08:02 mindspore_gs-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1138 b- defN 24-Mar-31 08:02 mindspore_gs-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       67 b- defN 24-Mar-31 08:02 mindspore_gs-0.4.0.dist-info/NOTICE
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-31 08:02 mindspore_gs-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-Mar-31 08:02 mindspore_gs-0.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    12829 b- defN 24-Mar-31 08:02 mindspore_gs-0.4.0.dist-info/RECORD
+120 files, 613529 bytes uncompressed, 183070 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -6,126 +6,120 @@
 
 Filename: mindspore_gs/comp_algo.py
 Comment: 
 
 Filename: mindspore_gs/net_transform.py
 Comment: 
 
-Filename: mindspore_gs/version.py
-Comment: 
-
-Filename: mindspore_gs/ops/__init__.py
+Filename: mindspore_gs/validator.py
 Comment: 
 
-Filename: mindspore_gs/ops/common/__init__.py
-Comment: 
-
-Filename: mindspore_gs/ops/common/quant_op_utils.py
+Filename: mindspore_gs/version.py
 Comment: 
 
-Filename: mindspore_gs/ops/kernel/gpu/fake_quant_impl.cuh
+Filename: mindspore_gs/common/__init__.py
 Comment: 
 
-Filename: mindspore_gs/ops/kernel/gpu/fake_quant_per_channel_grad_impl.cu
+Filename: mindspore_gs/common/config.py
 Comment: 
 
-Filename: mindspore_gs/ops/kernel/gpu/fake_quant_per_channel_impl.cu
+Filename: mindspore_gs/common/gs_enum.py
 Comment: 
 
-Filename: mindspore_gs/ops/kernel/gpu/fake_quant_per_layer_grad_impl.cu
+Filename: mindspore_gs/common/register.py
 Comment: 
 
-Filename: mindspore_gs/ops/kernel/gpu/fake_quant_per_layer_impl.cu
+Filename: mindspore_gs/common/utils.py
 Comment: 
 
-Filename: mindspore_gs/ops/kernel/gpu/min_max_update_per_channel_impl.cu
+Filename: mindspore_gs/datasets/__init__.py
 Comment: 
 
-Filename: mindspore_gs/ops/kernel/gpu/min_max_update_per_layer_impl.cu
+Filename: mindspore_gs/datasets/squad.py
 Comment: 
 
-Filename: mindspore_gs/ops/kernel/gpu/aot/custom_aot_extra.h
+Filename: mindspore_gs/datasets/wikitext2.py
 Comment: 
 
-Filename: mindspore_gs/ops/nn/__init__.py
+Filename: mindspore_gs/ghost/__init__.py
 Comment: 
 
-Filename: mindspore_gs/ops/nn/act_quant.py
+Filename: mindspore_gs/ghost/ghost.py
 Comment: 
 
-Filename: mindspore_gs/ops/nn/batchnorm_fold_cell.py
+Filename: mindspore_gs/ops/__init__.py
 Comment: 
 
-Filename: mindspore_gs/ops/nn/conv2d_bn_fold_quant.py
+Filename: mindspore_gs/ops/gs_custom.py
 Comment: 
 
-Filename: mindspore_gs/ops/nn/conv2d_bn_fold_quant_one_conv.py
+Filename: mindspore_gs/pruner/__init__.py
 Comment: 
 
-Filename: mindspore_gs/ops/nn/conv2d_bn_without_fold_quant.py
+Filename: mindspore_gs/pruner/heads/__init__.py
 Comment: 
 
-Filename: mindspore_gs/ops/nn/conv2d_quant.py
+Filename: mindspore_gs/pruner/heads/abstract.py
 Comment: 
 
-Filename: mindspore_gs/ops/nn/dense_quant.py
+Filename: mindspore_gs/pruner/heads/factory.py
 Comment: 
 
-Filename: mindspore_gs/ops/nn/fake_quant_with_min_max_observer.py
+Filename: mindspore_gs/pruner/heads/supported.py
 Comment: 
 
-Filename: mindspore_gs/ops/nn/mul_quant.py
+Filename: mindspore_gs/pruner/heads/type.py
 Comment: 
 
-Filename: mindspore_gs/ops/nn/tensor_add_quant.py
+Filename: mindspore_gs/pruner/heads/lrp/__init__.py
 Comment: 
 
-Filename: mindspore_gs/ops/operations/__init__.py
+Filename: mindspore_gs/pruner/heads/lrp/abstract_lrp.py
 Comment: 
 
-Filename: mindspore_gs/ops/operations/fake_quant_perchannel.py
+Filename: mindspore_gs/pruner/heads/lrp/utils.py
 Comment: 
 
-Filename: mindspore_gs/ops/operations/fake_quant_perlayer.py
+Filename: mindspore_gs/pruner/ops/__init__.py
 Comment: 
 
-Filename: mindspore_gs/ops/operations/gs_custom.py
+Filename: mindspore_gs/pruner/ops/masked_cell.py
 Comment: 
 
-Filename: mindspore_gs/ops/operations/min_max_update_perchannel.py
+Filename: mindspore_gs/pruner/ops/masked_conv2d.py
 Comment: 
 
-Filename: mindspore_gs/ops/operations/min_max_update_perlayer.py
+Filename: mindspore_gs/pruner/ops/masked_dense.py
 Comment: 
 
-Filename: mindspore_gs/ops/operations/grad_operations/__init__.py
+Filename: mindspore_gs/pruner/scop/__init__.py
 Comment: 
 
-Filename: mindspore_gs/ops/operations/grad_operations/fake_quant_perchannel_grad.py
+Filename: mindspore_gs/pruner/scop/scop_pruner.py
 Comment: 
 
-Filename: mindspore_gs/ops/operations/grad_operations/fake_quant_perlayer_grad.py
+Filename: mindspore_gs/pruner/uni_pruning/__init__.py
 Comment: 
 
-Filename: mindspore_gs/pruner/__init__.py
+Filename: mindspore_gs/pruner/uni_pruning/uni_pruner.py
 Comment: 
 
-Filename: mindspore_gs/pruner/scop/__init__.py
+Filename: mindspore_gs/pruner/uni_pruning/unipruning_masked_layer.py
 Comment: 
 
-Filename: mindspore_gs/pruner/scop/scop_pruner.py
+Filename: mindspore_gs/pruner/uni_pruning/graph_analyzer/__init__.py
 Comment: 
 
-Filename: mindspore_gs/pruner/uni_pruning/__init__.py
+Filename: mindspore_gs/pruner/uni_pruning/graph_analyzer/equichannel_group.py
 Comment: 
 
-Filename: mindspore_gs/pruner/uni_pruning/graph_analyzer_mindir.py
+Filename: mindspore_gs/pruner/uni_pruning/graph_analyzer/graph.py
 Comment: 
 
-Filename: mindspore_gs/pruner/uni_pruning/uni_pruner.py
+Filename: mindspore_gs/pruner/uni_pruning/graph_analyzer/graph_analyzer.py
 Comment: 
 
 Filename: mindspore_gs/pruner/uni_pruning/utils/__init__.py
 Comment: 
 
 Filename: mindspore_gs/pruner/uni_pruning/utils/importance_criteria.py
 Comment: 
@@ -135,33 +129,63 @@
 
 Filename: mindspore_gs/pruner/uni_pruning/utils/model_utils.py
 Comment: 
 
 Filename: mindspore_gs/pruner/uni_pruning/utils/prune.py
 Comment: 
 
+Filename: mindspore_gs/ptq/__init__.py
+Comment: 
+
+Filename: mindspore_gs/ptq/convert_utils.py
+Comment: 
+
+Filename: mindspore_gs/ptq/fake_quantizer.py
+Comment: 
+
+Filename: mindspore_gs/ptq/processor.py
+Comment: 
+
+Filename: mindspore_gs/ptq/ptq_config.py
+Comment: 
+
+Filename: mindspore_gs/ptq/quant_cells.py
+Comment: 
+
+Filename: mindspore_gs/ptq/round_to_nearest/__init__.py
+Comment: 
+
+Filename: mindspore_gs/ptq/round_to_nearest/round_to_nearest.py
+Comment: 
+
+Filename: mindspore_gs/ptq/round_to_nearest/rtn_layer_policy.py
+Comment: 
+
+Filename: mindspore_gs/ptq/round_to_nearest/rtn_net_policy.py
+Comment: 
+
 Filename: mindspore_gs/quantization/__init__.py
 Comment: 
 
 Filename: mindspore_gs/quantization/fake_quantizer.py
 Comment: 
 
 Filename: mindspore_gs/quantization/layer_policy.py
 Comment: 
 
 Filename: mindspore_gs/quantization/net_policy.py
 Comment: 
 
-Filename: mindspore_gs/quantization/quant_utils.py
+Filename: mindspore_gs/quantization/quant_cell.py
 Comment: 
 
-Filename: mindspore_gs/quantization/quantization_aware_training.py
+Filename: mindspore_gs/quantization/quant_utils.py
 Comment: 
 
-Filename: mindspore_gs/quantization/quantize_wrapper_cell.py
+Filename: mindspore_gs/quantization/quantization_aware_training.py
 Comment: 
 
 Filename: mindspore_gs/quantization/transformer.py
 Comment: 
 
 Filename: mindspore_gs/quantization/learned_step_size_quantization/__init__.py
 Comment: 
@@ -177,14 +201,98 @@
 
 Filename: mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_quantization_layer_policy.py
 Comment: 
 
 Filename: mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_quantization_net_policy.py
 Comment: 
 
+Filename: mindspore_gs/quantization/ops/__init__.py
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/kernel/gpu/fake_quant_impl.cuh
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/kernel/gpu/fake_quant_per_channel_grad_impl.cu
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/kernel/gpu/fake_quant_per_channel_impl.cu
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/kernel/gpu/fake_quant_per_layer_grad_impl.cu
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/kernel/gpu/fake_quant_per_layer_impl.cu
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/kernel/gpu/min_max_update_per_channel_impl.cu
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/kernel/gpu/min_max_update_per_layer_impl.cu
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/kernel/gpu/aot/custom_aot_extra.h
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/nn/__init__.py
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/nn/act_quant.py
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/nn/batchnorm_fold_cell.py
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/nn/conv2d_bn_fold_quant.py
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/nn/conv2d_bn_fold_quant_one_conv.py
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/nn/conv2d_bn_without_fold_quant.py
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/nn/conv2d_quant.py
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/nn/dense_quant.py
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/nn/fake_quant_with_min_max_observer.py
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/nn/mul_quant.py
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/nn/tensor_add_quant.py
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/operations/__init__.py
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/operations/fake_quant_perchannel.py
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/operations/fake_quant_perlayer.py
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/operations/min_max_update_perchannel.py
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/operations/min_max_update_perlayer.py
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/operations/grad_operations/__init__.py
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/operations/grad_operations/fake_quant_perchannel_grad.py
+Comment: 
+
+Filename: mindspore_gs/quantization/ops/operations/grad_operations/fake_quant_perlayer_grad.py
+Comment: 
+
 Filename: mindspore_gs/quantization/simulated_quantization/__init__.py
 Comment: 
 
 Filename: mindspore_gs/quantization/simulated_quantization/combined.py
 Comment: 
 
 Filename: mindspore_gs/quantization/simulated_quantization/simulated_fake_quantizers.py
@@ -228,26 +336,26 @@
 
 Filename: mindspore_gs/quantization/slb/slb_quant_config.py
 Comment: 
 
 Filename: mindspore_gs/quantization/slb/slb_quant_convert.py
 Comment: 
 
-Filename: mindspore_gs-0.3.0.dist-info/LICENSE
+Filename: mindspore_gs-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: mindspore_gs-0.3.0.dist-info/METADATA
+Filename: mindspore_gs-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: mindspore_gs-0.3.0.dist-info/NOTICE
+Filename: mindspore_gs-0.4.0.dist-info/NOTICE
 Comment: 
 
-Filename: mindspore_gs-0.3.0.dist-info/WHEEL
+Filename: mindspore_gs-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: mindspore_gs-0.3.0.dist-info/top_level.txt
+Filename: mindspore_gs-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mindspore_gs-0.3.0.dist-info/RECORD
+Filename: mindspore_gs-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mindspore_gs/.commit_id

```diff
@@ -1 +1 @@
-__commit_id__ = '[sha1]:10a2c1ec,[branch]: (HEAD, origin/r0.3-alpha, r0.3-alpha)'
+__commit_id__ = '[sha1]:83ac6045,[branch]: (HEAD, origin/r0.4, r0.4)'
```

## mindspore_gs/__init__.py

```diff
@@ -12,17 +12,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """
 MindSpore golden stick module.
 """
 
+
 from .comp_algo import CompAlgo
+from .common import BackendTarget
 from .quantization import SimulatedQuantizationAwareTraining, SlbQuantAwareTraining
 from .pruner import PrunerKfCompressAlgo, PrunerFtCompressAlgo, UniPruner
-from .version import __version__, mindspore_version_check
+from .ghost import GhostAlgo
+from .ptq.ptq_config import PTQConfig, PTQMode
+from .ptq.round_to_nearest import RoundToNearest
 
 __all__ = ["SimulatedQuantizationAwareTraining", "SlbQuantAwareTraining", "PrunerKfCompressAlgo",
-           "PrunerFtCompressAlgo", "CompAlgo"]
-__all__.extend(__version__)
+           "PrunerFtCompressAlgo", "UniPruner", "CompAlgo", "GhostAlgo", 'PTQConfig', 'PTQMode', 'BackendTarget',
+           "RoundToNearest"]
 
+from .version import __version__, mindspore_version_check
 mindspore_version_check()
+__all__.extend(__version__)
```

## mindspore_gs/comp_algo.py

```diff
@@ -11,35 +11,42 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """GoldenStick."""
 
 import abc
+import enum
 import os.path
 
 from mindspore.nn.cell import Cell
 from mindspore.train.callback import Callback
 from mindspore import export, context
-from mindspore._checkparam import Validator
 from mindspore import log as logger
+from mindspore_gs.validator import Validator
+
+
+class Backend(enum.Enum):
+    MS = 0
+    FAKE_QUANT = 1
+    GE_ASCEND = 2
 
 
 class CompAlgo(abc.ABC):
     """
     Base class of algorithms in GoldenStick.
 
     Args:
-        config (dict): User config for network compression, default is None. Algorithm config specification is default
-            by derived class, base attributes are listed below:
+        config (dict): User config for network compression, default is ``None``. Algorithm config specification
+            is default by derived class, base attributes are listed below:
 
-            - save_mindir (bool): If true, export MindIR automatically after training, else not. Default: False.
+            - save_mindir (bool): If ``True``, export MindIR automatically after training, else not. Default: ``False``.
             - save_mindir_path (str): The path to export MindIR, the path includes the directory and file name, which
               can be a relative path or an absolute path, the user needs to ensure write permission.
-              Default: './network'.
+              Default: ``'./network'``.
     """
 
     def __init__(self, config=None):
         if config is None:
             config = {}
         Validator.check_value_type("config", config, [dict], self.__class__.__name__)
         self._is_cpu = context.get_context('device_target') == "CPU"
@@ -93,15 +100,15 @@
         return cb
 
     def set_save_mindir(self, save_mindir: bool):
         """
         Set whether to automatically export MindIR after training.
 
         Args:
-            save_mindir (bool): If true, export MindIR automatically after training, else not.
+            save_mindir (bool): If ``True``, export MindIR automatically after training, else not.
 
         Raises:
             TypeError: If `need_save` is not bool.
 
         Examples:
             >>> import mindspore as ms
             >>> from mindspore_gs.quantization import SimulatedQuantizationAwareTraining as SimQAT
@@ -125,15 +132,15 @@
             >>> model.train(1, train_dataset, callbacks=algo.callbacks())
         """
         Validator.check_bool(save_mindir, "save_mindir", self.__class__.__name__)
         self._config.save_mindir = save_mindir
 
     def set_save_mindir_path(self, save_mindir_path: str):
         """
-        Set the path to export MindIR, only takes effect if `save_mindir` is True.
+        Set the path to export MindIR, only takes effect if `save_mindir` is ``True``.
 
         Args:
             save_mindir_path (str): The path to export MindIR, the path includes the directory and file name, which can
                 be a relative path or an absolute path, the user needs to ensure write permission.
 
         Raises:
             ValueError: if `save_mindir_path` is not Non-empty str.
@@ -148,16 +155,16 @@
 
     def convert(self, net_opt: Cell, ckpt_path="") -> Cell:
         """
         Define how to convert a compressed network to a standard network before exporting to MindIR.
 
         Args:
             net_opt (Cell): Network to be converted which is transformed by `CompAlgo.apply`.
-            ckpt_path (str): Path to checkpoint file for `net_opt`. Default is a empty string which means not loading
-                checkpoint file to `net_opt`.
+            ckpt_path (str): Path to checkpoint file for `net_opt`. Default is ``""``, which means not loading
+                checkpoint file to `net_opt`. this parameter would be deprecated in future version.
 
         Returns:
             An instance of Cell represents converted network.
 
         Examples:
             >>> from mindspore_gs.quantization import SimulatedQuantizationAwareTraining as SimQAT
             >>> ## 1) Define network to be trained
```

## mindspore_gs/net_transform.py

```diff
@@ -11,16 +11,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """NetTransform."""
 from typing import Union, Optional
 
+import mindspore
 from mindspore.nn.cell import Cell
-from mindspore.rewrite import PatternEngine, SymbolTree, Node, ScopedValue, TreeNodeHelper
+from mindspore.rewrite import PatternEngine, SymbolTree, Node, ScopedValue, NodeType
+from mindspore_gs.quantization.quant_cell import QuantCell
+
+
+mindspore.rewrite.common.namespace._subtree_black_list.append(QuantCell)
 
 
 class NetTransformer:
     """
     NetTransformer is define for transform network in MindSpore.
 
     Args:
@@ -28,52 +33,62 @@
     """
 
     def __init__(self, net: Cell, symbol_tree: SymbolTree = None):
         if symbol_tree is None:
             self._net = net
             try:
                 self._symbol_tree = SymbolTree.create(net)
+                self._symbol_tree.flatten_static_if_control_flow()
             except (RuntimeError, ValueError, TypeError, NotImplementedError):
                 raise RuntimeError(f"For MindSpore Golden Stick, input network type '{type(net).__name__}' "
                                    f"is not supported right now.")
             except Exception:
                 raise Exception("For MindSpore Golden Stick, analysis input network fail.")
             return
         self._symbol_tree = symbol_tree
 
     @staticmethod
     def create_from_tree_node(node):
-        modify_tree = TreeNodeHelper.get_sub_tree(node)
+        modify_tree = node.get_sub_tree()
         return NetTransformer(None, modify_tree)
 
+    @staticmethod
+    def create_node(cell: Cell, targets: [Union[ScopedValue, str]], args: [ScopedValue] = None,
+                    kwargs: {str: ScopedValue}=None, name: str = "") -> Node:
+        return Node.create_call_cell(cell, targets, args, kwargs, name)
+
     def get_network(self) -> Cell:
         return self._symbol_tree.get_network()
 
     def get_code(self):
         return self._symbol_tree.get_code()
 
+    def unfolded_nodes(self) -> {}:
+        """
+        Get a generator to generate unfolded nodes of corresponding network.
+        """
+
+        for node in self._symbol_tree.nodes():
+            for single_node in NodeUnfolder.unfold_nodes(node):
+                yield single_node
+
     def nodes(self) -> {}:
         """
         Returns:
             a list of BaseNode corresponding to all layers in original network.
         """
 
         return self._symbol_tree.nodes()
 
     def before(self, node_or_name: Union[Node, str]):
         return self._symbol_tree.before(node_or_name)
 
     def after(self, node_or_name: Union[Node, str]):
         return self._symbol_tree.after(node_or_name)
 
-    @staticmethod
-    def create_node(cell: Cell, targets: [Union[ScopedValue, str]], args: [ScopedValue] = None,
-                    kwargs: {str: ScopedValue}=None, name: str = "") -> Node:
-        return Node.create_call_cell(cell, targets, args, kwargs, name)
-
     def insert(self, position, node: Node) -> Optional[Node]:
         return self._symbol_tree.insert(position, node)
 
     def erase_node(self, node_or_name: Union[Node, str]) -> Optional[Node]:
         """
         Args:
             node_or_name (Node/str): node to be removed from original network.
@@ -86,29 +101,69 @@
     def replace(self, old_node: Node, new_nodes: [Node]) -> Node:
         """
         Replace an old_node with new_node from rewrite. Can only erase a node not being depended on.
 
         Args:
             old_node (Node): Node to be replaced.
             new_nodes (list[Node]): Node to replace
+
         Returns:
             new node.
 
         Raises:
             RuntimeError: old node is isolated.
         """
-        return self._symbol_tree.replace(old_node, new_nodes)
+        stree = SymbolTree(old_node.get_handler().get_belong_symbol_tree())
+        return stree.replace(old_node, new_nodes)
 
     def dump(self):
         self._symbol_tree.dump()
 
     # replace src_pattern with target_nodes.
     # target_nodes should has same inputs and outputs with src_pattern.
     def pattern_transform(self, pattern_engine: PatternEngine) -> bool:
         """
         Args:
-            pattern_engine (PatternEngine): Instance of PatternEngine. Apply `pattern_engine` on current network
+            pattern_engine (PatternEngine): Instance of PatternEngine. Apply `pattern_engine` on current network.
 
         Returns:
             a bool value indicating if transform occurred
         """
         return pattern_engine.apply(self._symbol_tree)
+
+
+class NodeUnfolder:
+    """
+    Unfold nodes from symbol tree.
+    node_type_to_unfold_list: [NodeType.Tree, NodeType.CellContainer]
+    """
+
+    @staticmethod
+    def _get_nodes_from_cell_container(node: Node):
+        cell_container = node.get_handler()
+        for i, sub_node in enumerate(cell_container.nodes()):
+            if i == 0 and not sub_node.get_inputs():
+                sub_node.set_arg_providers(0, (cell_container.get_inputs()[0], 0))
+            for single_node in NodeUnfolder.unfold_nodes(Node(sub_node)):
+                yield single_node
+
+    @staticmethod
+    def _get_nodes_from_sub_tree(node: Node):
+        sub_tree: SymbolTree = node.get_handler().symbol_tree
+        for sub_node in sub_tree.nodes():
+            for single_node in NodeUnfolder.unfold_nodes(Node(sub_node)):
+                yield single_node
+
+    @staticmethod
+    def unfold_nodes(node: Node):
+        """
+        Unfold cell container or subtree.
+        """
+        node_type: NodeType = node.get_node_type()
+        if node_type == NodeType.CellContainer:
+            for unfolded_node in NodeUnfolder._get_nodes_from_cell_container(node):
+                yield unfolded_node
+        elif node_type == NodeType.Tree:
+            for unfolded_node in NodeUnfolder._get_nodes_from_sub_tree(node):
+                yield unfolded_node
+        else:
+            yield node
```

## mindspore_gs/version.py

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 # ============================================================================
 """Define version of MindSpore Golden Stick and check version matching between MindSpore and MindSpore Golden Stick."""
 
 import time
 
 #pylint: disable=C0111
-__version__ = '0.3.0'
+__version__ = '0.4.0'
 
 
 def mindspore_version_check():
     """
     Do the MindSpore version check for MindSpore Golden Stick. If the MindSpore can not be imported, it will raise
     an ImportError. If its version is not compatible with current MindSpore Golden Stick version, it will print a
     warning.
@@ -36,15 +36,16 @@
     except (ImportError, ModuleNotFoundError):
         print("Can not find MindSpore in current environment. Please install MindSpore before using MindSpore Golden "
               "Stick, by following the instruction at https://www.mindspore.cn/install")
         raise
 
     ms_msgs_version_match = {'0.1': '1.8',
                              '0.2': '1.9',
-                             '0.3': '2.0'}
+                             '0.3': '2.0',
+                             '0.4': '2.3'}
 
     required_mindspore_verision = ms_msgs_version_match[__version__[:3]]
     ms_version = ms.__version__[:3]
 
     if required_mindspore_verision != ms_version:
         logger.warning("Current version of MindSpore is not compatible with MindSpore Golden Stick. Some functions "
                        "might not work or even raise error. Please install MindSpore version == {}. For more details "
```

## mindspore_gs/ops/__init__.py

```diff
@@ -11,7 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """
 MindSpore golden stick ops.
 """
+
+from .gs_custom import GSCustom, custom_op_attr_register
+
+__all__ = [
+    "GSCustom",
+    "custom_op_attr_register"
+]
```

## mindspore_gs/pruner/__init__.py

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """MindSpore golden stick pruner module."""
 
+from ..version import __version__, mindspore_version_check
+mindspore_version_check()
+
 from .scop import PrunerFtCompressAlgo, PrunerKfCompressAlgo
 from .uni_pruning import UniPruner
-from ..version import __version__, mindspore_version_check
 
-__all__ = ["PrunerKfCompressAlgo", "PrunerFtCompressAlgo"]
+__all__ = ["PrunerKfCompressAlgo", "PrunerFtCompressAlgo", "UniPruner"]
 __all__.extend(__version__)
-
-mindspore_version_check()
```

## mindspore_gs/pruner/scop/scop_pruner.py

```diff
@@ -13,21 +13,21 @@
 # limitations under the License.
 # ============================================================================
 """ScopPruner."""
 
 import mindspore
 import mindspore.nn as nn
 import mindspore.ops as ops
-from mindspore._checkparam import Validator, Rel
 import mindspore.context as context
 import mindspore.common.dtype as mstype
 from mindspore.train.callback import Callback
 from mindspore import Tensor
 from mindspore.ops import constexpr
 from mindspore import Parameter
+from mindspore_gs.validator import Validator, Rel
 from ...comp_algo import CompAlgo, CompAlgoConfig
 
 
 @constexpr
 def generate_int(shape):
     """Generate int."""
     return int(shape // 2)
@@ -39,15 +39,15 @@
     def __init__(self, conv_ori, bn_ori, prex):
         super(KfConv2d, self).__init__()
         self.conv = conv_ori
         self.bn = bn_ori
         self.out_channels = self.conv.out_channels
         self.kfscale = Parameter(ops.Ones()((1, self.out_channels, 1, 1), mindspore.float32), requires_grad=True,
                                  name=prex + '.kfscale')
-        self.kfscale.data.fill(0.5)
+        self.kfscale.data.asnumpy().fill(0.5)
         self.concat_op = ops.Concat(axis=0)
 
     def construct(self, x):
         """Calculate."""
         x = self.conv(x)
         if self.training:
             num_ori = generate_int(x.shape[0])
@@ -367,15 +367,15 @@
     `PrunerFtCompressAlgo` is a subclass of CompAlgo that implements the ability to remove redundant convolution kernels
     and fully train the network.
 
     Args:
         config (dict): Configuration of `PrunerFtCompressAlgo`, keys are attribute names,
             values are attribute values. Supported attribute are listed below:
 
-            - prune_rate (float): number in [0.0, 1.0)
+            - prune_rate (float): number in [0.0, 1.0).
 
     Raises:
         TypeError: If `prune_rate` is not float.
         ValueError: If `epoch_size` is less than 0 or greater than or equal to 1.
 
 
     Supported Platforms:
```

## mindspore_gs/pruner/uni_pruning/uni_pruner.py

```diff
@@ -13,26 +13,28 @@
 # limitations under the License.
 # ============================================================================
 """
 Implementation of UniPruning algorithm that zeroize model every n epochs according to UniPruning criterion.
 Pruning mask from the last step and zeroed weights are used to get physically pruned model for inference.
 """
 import os
-import json
+from collections import OrderedDict
 import numpy as np
 from mindspore import Tensor, load_checkpoint, load_param_into_net
 from mindspore import log as logger
-from mindspore._checkparam import Validator
-from mindspore.nn import Cell
+from mindspore.nn import Cell, Conv2d, Dense
 from mindspore.train.callback import Callback
 
+from mindspore_gs.validator import Validator
 from ...comp_algo import CompAlgo
-from .graph_analyzer_mindir import GraphAnalyzer
+from .graph_analyzer import GraphAnalyzer
 from .utils import do_mask, get_channel_importances, get_mask, prune_net, save_model_and_mask
-#pylint: disable=arguments-differ
+from .unipruning_masked_layer import UniPruningMaskedConv2d, UniPruningMaskedDense
+from ..ops import MaskedCell
+
 
 class UniPrunerCallback(Callback):
     """
     UniPruning Callback that applies UniZeroing during training.
     Argument description is given in UniPruner class.
 
     Raises:
@@ -43,18 +45,19 @@
         TypeError: If `frequency` is not int.
         TypeError: If `target_sparsity` is not float.
         TypeError: If `pruning_step` is not int.
         TypeError: If `filter_lower_threshold` is not int.
         TypeError: If `device_target` is not string.
         TypeError: If `rank` is not int.
     """
+
     def __init__(self, exp_name, output_path, input_size,
                  prune_flag, frequency, target_sparsity,
                  pruning_step, filter_lower_threshold,
-                 device_target, rank):
+                 device_target: GraphAnalyzer, rank):
         super().__init__()
         Validator.check_value_type("exp_name", exp_name, [str], self.__class__.__name__)
         Validator.check_value_type("output_path", output_path, [str], self.__class__.__name__)
         Validator.check_value_type("input_size", input_size, [tuple, list], self.__class__.__name__)
         Validator.check_value_type("prune_flag", prune_flag, [int], self.__class__.__name__)
         Validator.check_value_type("frequency", frequency, [int], self.__class__.__name__)
         Validator.check_value_type("target_sparsity", target_sparsity, [float], self.__class__.__name__)
@@ -66,15 +69,15 @@
         self.output_path = os.path.join(output_path, exp_name)
         self.input_size = input_size
         self._frequency = frequency
         self._target_sparsity = target_sparsity
         self.pruning_step = pruning_step
         self.filter_lower_threshold = filter_lower_threshold
         self.mask = {}
-        self.graph = {}
+        self.graph_anaylzer = None
         self.prune_flag = prune_flag
         self.rank = rank
         self.device_target = device_target
         if device_target == 'Ascend':
             self.save_model = True
         else:
             self.save_model = False
@@ -109,27 +112,28 @@
             3. At each layer compute channel group criterion as highest median in layer / median(group).
             4. Choose groups with highest criterion until reached target sparsity.
              Make mask as dict {layer: chosen channels}.
             5. Zeroize chosen channels.
             6. Save zeroed weights and pruning mask.
         """
         # compute channel importances and get pruning mask
-        norms = get_channel_importances(self.graph.groups, self.filter_lower_threshold)
-        self.mask = get_mask(self.graph.groups, norms, self.pruning_step,
+        norms = get_channel_importances(self.graph_anaylzer.groups, self.filter_lower_threshold)
+        self.mask = get_mask(self.graph_anaylzer.groups, norms, self.pruning_step,
                              self.filter_lower_threshold, self._target_sparsity)
         # apply pruning mask -> zero model
-        do_mask(self.graph.groups, self.mask)
+        do_mask(self.graph_anaylzer.groups, self.mask)
         origin_args = run_context.original_args()
         net: Cell = origin_args.network
         cur_epoch_num = origin_args.cur_epoch_num
         save_model_and_mask(net, self.output_path, f'{self.exp_name}_zeroed_rank{self.rank}',
                             cur_epoch_num, self.input_size, self.device_target, self.save_model,
                             self.mask)
         logger.info(f'UniZeroing ended rank{self.rank}')
 
+
 class UniPruner(CompAlgo):
     """
     Derived class of `CompAlgo`. Base class of UniPruning algorithm.
 
     Args:
         config (dict): store attributes for quantization aware training, keys are attribute names,
             values are attribute values. supported attribute are listed below:
@@ -188,30 +192,30 @@
         >>>     tag = 'pruned'
         >>> else:
         >>>     mask = None
         >>>     tag = 'original'
         >>> ms.load_checkpoint(config.checkpoint_file_path, net)
         >>> ## 7) Make pruning, save pruned network
         >>> algo.convert(net, mask, config, tag)
-
     """
+
     def __init__(self, config=None):
         super().__init__(config)
         Validator.check_value_type("config", config, [dict], self.__class__.__name__)
         self._callback = UniPrunerCallback(exp_name=config["exp_name"],
                                            output_path=config["output_path"],
                                            input_size=config["input_size"],
                                            frequency=config["frequency"],
                                            target_sparsity=config["target_sparsity"],
                                            pruning_step=config["pruning_step"],
                                            filter_lower_threshold=config["filter_lower_threshold"],
                                            prune_flag=config["prune_flag"],
                                            rank=config["rank"],
                                            device_target=config["device_target"])
-        self.graph = {}
+        self.graph_anaylzer = None
 
     def apply(self, network: Cell) -> Cell:
         """
         Analyze network computational graph.
         Currently supported networks:
             - Resnet-like models
             - VGG-like models
@@ -220,18 +224,47 @@
         Args:
             network (Cell): network for pruning.
 
         Raises:
             ValueError: If network type is not supported by graph analyzer.
         """
         fake_input = Tensor(np.ones(self._callback.input_size).astype(np.float32))
-        self.graph = GraphAnalyzer(network, fake_input)
-        if not self.graph.analyze():
-            raise ValueError('Analyzer for the chosen network does not work')
-        self._callback.graph = self.graph
+        self.graph_anaylzer = GraphAnalyzer(network, fake_input)
+        self._callback.graph_anaylzer = self.graph_anaylzer
+
+        name_cells: OrderedDict = network.name_cells()
+        cell_names = name_cells.keys()
+        for name in cell_names:
+            layer = name_cells.get(name)
+            if isinstance(layer, Conv2d):
+                origin_weight_name = layer.weight.name
+                origin_bias_name = "bias"
+                if layer.has_bias:
+                    origin_bias_name = layer.bias.name
+                new_cell = UniPruningMaskedConv2d(layer)
+                new_name = name.split('.')[-1]
+                network.insert_child_to_cell(new_name, new_cell)
+                new_cell.handler.weight.name = "masked_{}".format(origin_weight_name)
+                new_cell.in_mask.name = "{}.in_mask".format(new_name)
+                new_cell.out_mask.name = "{}.out_mask".format(new_name)
+                if layer.has_bias:
+                    new_cell.handler.bias.name = "masked_{}".format(origin_bias_name)
+            if isinstance(layer, Dense):
+                origin_weight_name = layer.weight.name
+                origin_bias_name = "bias"
+                if layer.has_bias:
+                    origin_bias_name = layer.bias.name
+                new_cell = UniPruningMaskedDense(layer)
+                new_name = name.split('.')[-1]
+                network.insert_child_to_cell(new_name, new_cell)
+                new_cell.handler.weight.name = "masked_{}".format(origin_weight_name)
+                new_cell.in_mask.name = "{}.in_mask".format(new_name)
+                new_cell.out_mask.name = "{}.out_mask".format(new_name)
+                if layer.has_bias:
+                    new_cell.handler.bias.name = "masked_{}".format(origin_bias_name)
         return network
 
     def prune_by_mask(self, net: Cell, mask, args, tag):
         """
         Prune network (optional) according to mask, save weights as .ckpt, model as .MINDIR and .AIR
 
         Args:
@@ -246,31 +279,41 @@
             TypeError: If `args` is not dict.
             TypeError: If `tag` is not string.
         """
         if mask is not None:
             Validator.check_value_type("mask", mask, [dict], self.__class__.__name__)
         Validator.check_value_type("tag", tag, [str], self.__class__.__name__)
         if mask is not None:
-            prune_net(self.graph.groups, mask)
+            prune_net(self.graph_anaylzer.groups, mask)
         save_model_and_mask(net, self._callback.output_path, f'{args.exp_name}_{tag}_{self._callback.rank}',
                             args.epoch_size, self._callback.input_size, args.device_target,
                             export_air=True)
 
-    def convert(self, **kwargs) -> Cell:
+    def convert(self, net_opt: Cell, ckpt_path="") -> Cell:
         """prune network using checkpoint with zeroed weights and pruning mask saved"""
-        net_opt = kwargs["net_opt"]
-
-        ckpt_path = kwargs["ckpt_path"]
-        ckpt = load_checkpoint(ckpt_path)
-        load_param_into_net(net_opt, ckpt)
-
-        mask_path = kwargs["mask_path"]
-        with open(mask_path, "r") as fp:
-            mask = json.load(fp)
-
-        self.apply(net_opt)
-        prune_net(self.graph.groups, mask)
+        if not isinstance(net_opt, Cell):
+            raise TypeError(
+                f'The parameter `net_opt` must be isinstance of Cell, but got {type(net_opt)}.')
+        if not isinstance(ckpt_path, str):
+            raise TypeError(
+                f'The parameter `ckpt_path` must be isinstance of str, but got {type(ckpt_path)}.')
+        real_path = os.path.realpath(ckpt_path)
+        if ckpt_path != "":
+            if os.path.isfile(real_path):
+                param_dict = load_checkpoint(ckpt_path)
+                not_load_param = load_param_into_net(net_opt, param_dict)
+                if not_load_param[0]:
+                    raise RuntimeError("Load param into net fail.")
+            else:
+                raise ValueError(
+                    f'The parameter `ckpt_path` can only be empty or a valid file, but got {real_path}.')
+        for name, layer in net_opt.cells_and_names():
+            if not isinstance(layer, MaskedCell):
+                continue
+            net_opt.insert_child_to_cell(name, layer.prune())
         return net_opt
 
     def callbacks(self, *args, **kwargs) -> [Callback]:
         """get UniPruner callback"""
+        if self.graph_anaylzer is None:
+            raise RuntimeError("Please call the apply interface first.")
         return [self._callback]
```

## mindspore_gs/pruner/uni_pruning/utils/importance_criteria.py

```diff
@@ -66,20 +66,20 @@
             length = len(median_group[key])
             cnt = 0
             for i in range(length - 1):
                 current_median = median_group[key][i]
                 if current_median == 0:
                     chosen_key, block_idx, chosen_idx = key, idx, i
                     zero_idx = np.array(norms[block_idx][chosen_key][1]\
-                        [chosen_idx * step : (chosen_idx + 1) * step])
+                        [chosen_idx * step: (chosen_idx + 1) * step])
                     return zero_idx, block_idx
                 ratio = highest_median / (current_median + 1e-5)
                 if ratio > max_ratio:
                     max_ratio = ratio
                     chosen_key, block_idx, chosen_idx = key, idx, i
 
                 cnt += step
                 if length * step - cnt <= filter_num_threshold:
                     break
     zero_idx = np.array(norms[block_idx][chosen_key][1]\
-                        [chosen_idx * step : (chosen_idx + 1) * step])
+                        [chosen_idx * step: (chosen_idx + 1) * step])
     return zero_idx, block_idx
```

## mindspore_gs/pruner/uni_pruning/utils/model_utils.py

```diff
@@ -27,21 +27,21 @@
     size = 0
     for group in groups:
         for layer in group.ms_starts:
             mod = group.ms_starts[layer]
             if isinstance(mod, nn.Conv2d):
                 shape = mod.weight.shape
                 size += (shape[0] - layer_mask[layer]['cout']) * \
-                    (shape[1]  - layer_mask[layer]['cin']) * shape[2] * shape[3]
+                    (shape[1] - layer_mask[layer]['cin']) * shape[2] * shape[3]
                 if mod.bias is not None:
                     size += (shape[0] - layer_mask[layer]['cout'])
             if isinstance(mod, nn.Dense):
                 shape = mod.weight.shape
                 size += (shape[0] - layer_mask[layer]['cout']) * \
-                    (shape[1]  - layer_mask[layer]['cin'])
+                    (shape[1] - layer_mask[layer]['cin'])
                 if mod.bias is not None:
                     size += (shape[0] - layer_mask[layer]['cout'])
         for layer in group.ms_middles:
             mod = group.ms_middles[layer]
             if isinstance(mod, nn.BatchNorm2d):
                 shape = mod.gamma.shape
                 size += (shape[0] - layer_mask[layer]['cout']) * 4
```

## mindspore_gs/quantization/__init__.py

 * *Ordering differences only*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """
 MindSpore golden stick quantization module.
 """
 
+from ..version import __version__, mindspore_version_check
+mindspore_version_check()
+
 from .simulated_quantization import SimulatedQuantizationAwareTraining
 from .slb import SlbQuantAwareTraining
-from ..version import __version__, mindspore_version_check
 
 __all__ = ["SimulatedQuantizationAwareTraining", "SlbQuantAwareTraining"]
 __all__.extend(__version__)
-
-mindspore_version_check()
```

## mindspore_gs/quantization/fake_quantizer.py

```diff
@@ -9,13 +9,131 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """
-FakeQuantizer.
-FakeQuantizer should be a Cell for automatic-differentiation
+FakeQuantizer, statistic distribute of input x and return quant param.
 """
+import abc
+from typing import Union
+
+import numpy as np
 from mindspore.nn.cell import Cell
+from mindspore import QuantDtype
+from mindspore.ops.operations._quant_ops import FakeQuantParam
+from mindspore_gs.quantization.quant_utils import get_quant_min_max, cal_quantization_params
+
+
+class FakeQuantParamCell(Cell):
+    """FakeQuantParamCell."""
+    def __init__(self, op: FakeQuantParam):
+        super().__init__()
+        if not isinstance(op, FakeQuantParam):
+            raise TypeError("Input ops should be a FakeQuantParam, but got: ", type(op))
+        self.fq = op
+
+    def construct(self, x):
+        return self.fq(x)
+
+    # pylint: disable=W0613
+    def shard(self, in_strategy, out_strategy=None, parameter_plan=None, device="Ascend", level=0):
+        self.fq = self.fq.shard(in_strategy=in_strategy, out_strategy=out_strategy)
+
+
+class FakeQuantizer(Cell):
+    """
+    Abstract class for cell which statistic distribute of input x and return quant param.
+    """
+    def __init__(self):
+        super().__init__()
+        self._attrs = {}
+
+    @abc.abstractmethod
+    def name(self) -> str:
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def quant_dtype(self) -> QuantDtype:
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def is_per_channel(self) -> bool:
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def quant_params(self) -> dict:
+        raise NotImplementedError
+
+    def set_attr(self, key, value):
+        self._attrs[key] = value
+
+    def get_attr(self, key, default=None):
+        return self._attrs.get(key, default)
+
+    def convert_to_fakequantparam(self) -> FakeQuantParamCell:
+        fq_param = FakeQuantParam(self.quant_dtype(), self.name(), self.is_per_channel(), **self.quant_params())
+        return FakeQuantParamCell(fq_param)
+
+
+class LinearFakeQuantizer(FakeQuantizer):
+    """
+    Abstract class derived from FakeQuantizer, suit for linear quantization.
+    """
+
+    attr_key_min = "min"
+    attr_key_max = "max"
+    attr_key_num_bits = "num_bits"
+    attr_key_narrow_range = "narrow_range"
+    attr_key_symmetric = "symmetric"
+    attr_key_channel_axis = "channel_axis"
+
+    def name(self) -> str:
+        return FakeQuantParam.attr_value_linear_quant_algo_name
+
+    def foo_init(self):
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def mins(self) -> Union[list, tuple]:
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def maxs(self) -> Union[list, tuple]:
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def num_bits(self) -> int:
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def narrow_range(self) -> bool:
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def symmetric(self) -> bool:
+        raise NotImplementedError
+
+    def channel_axis(self) -> int:
+        return -1
+
+    def get_scale_zp(self):
+        quant_min, quant_max = get_quant_min_max(self.num_bits(), self.symmetric(), self.narrow_range())
+        input_mins = np.array(self.mins(), dtype=np.float32)
+        input_maxs = np.array(self.maxs(), dtype=np.float32)
+        scale, zp = cal_quantization_params(input_mins, input_maxs, quant_min, quant_max, symmetric=self.symmetric())
+        scale = scale.tolist()
+        zp = zp.tolist()
+        return scale, zp
 
-FakeQuantizer = Cell
+    def quant_params(self) -> dict:
+        scale, zp = self.get_scale_zp()
+        params = {LinearFakeQuantizer.attr_key_min: self.mins(), LinearFakeQuantizer.attr_key_max: self.maxs(),
+                  LinearFakeQuantizer.attr_key_num_bits: self.num_bits(),
+                  LinearFakeQuantizer.attr_key_narrow_range: self.narrow_range(),
+                  LinearFakeQuantizer.attr_key_symmetric: self.symmetric(),
+                  FakeQuantParam.attr_key_linear_quant_scale: scale,
+                  FakeQuantParam.attr_key_linear_quant_zero_point: zp}
+        if self.is_per_channel():
+            params[LinearFakeQuantizer.attr_key_channel_axis] = self.channel_axis()
+        return params
```

## mindspore_gs/quantization/layer_policy.py

```diff
@@ -13,17 +13,25 @@
 # limitations under the License.
 # ============================================================================
 """LayerQConfig."""
 import abc
 from typing import Optional
 from mindspore.nn import Cell
 from .fake_quantizer import FakeQuantizer
+
 layer_policy_key = "layer_quant_policy"
 
 
+class PerChannelArgs:
+    def __init__(self, num_channels=-1, channel_axis=-1, rank=-1):
+        self.num_channels = num_channels
+        self.channel_axis = channel_axis
+        self.rank = rank
+
+
 class LayerPolicy(abc.ABC):
     """
     Base class for layer quantize configure.
     Configuration including:
         Which weights of layer to be fake-quantize and how they should be fake-quantized
         If input and output of activation of layer need to be fake-quantized and how they should be fake-quantized
         If output and layer need to be fake-quantized and how it should be fake-quantized
@@ -34,50 +42,79 @@
     Supported Config:
         ``quant_delay`` ``quant_dtype`` ``per_channel`` ``symmetric`` ``narrow_range`` ``one_conv_fold``.
 
     Note:
         Derived class must override `get_weight_name_and_quantizers`, `get_act_name_and_quantizers`,
             `get_output_quantizers` and `wrapper_cell`.
     """
+
     def __init__(self):
         self._input_num = 0
         self._inputs_insert_fq = []
+        self._output_insert_fq: bool = True
 
-    def get_weight_name_and_quantizers(self) -> [(str, FakeQuantizer)]:
+    @abc.abstractmethod
+    def get_weight_quantizer(self, weight_name="", perchannel_args: PerChannelArgs = PerChannelArgs(),
+                             **kwargs) -> FakeQuantizer:
         """
         Define how to fake-quantize weight data. This method must be overridden by all subclasses.
 
         Returns:
             Return a list of 2-tuple of weight_name and weight_quantizer.
             Return empty list if no need to fake-quant weight.
         """
+        raise NotImplementedError
 
-        return []
+    @abc.abstractmethod
+    def _get_input_quantizer(self, input_index=-1, perchannel_args: PerChannelArgs = PerChannelArgs(),
+                             **kwargs) -> FakeQuantizer:
+        """
+        Define how to fake-quantize input data. This method must be overridden by all subclasses.
 
-    def get_act_name_and_quantizers(self) -> [(str, (Optional[FakeQuantizer], Optional[FakeQuantizer]))]:
-        return []
+        Returns:
+            Return an instance of quantizer as quantizer for inputs.
+        """
+        raise NotImplementedError
 
-    def get_input_quantizer(self) -> Optional[FakeQuantizer]:
+    def get_input_quantizer(self, input_index=-1, perchannel_args: PerChannelArgs = PerChannelArgs(), **kwargs) -> \
+    Optional[FakeQuantizer]:
         """
-        Define how to fake-quantize input data. This method must be overridden by all subclasses.
+        Define how to fake-quantize input data.
 
         Returns:
-            Return a instance of quantizer as quantizer for inputs.
+            Return an instance of quantizer as quantizer for inputs.
             Return None if all inputs don't need to fake-quant.
         """
-        return None
+        if input_index >= self._input_num:
+            return None
+        if input_index >= 0 and not self._inputs_insert_fq[input_index]:
+            return None
+        return self._get_input_quantizer(input_index, perchannel_args, **kwargs)
 
-    def get_output_quantizer(self) -> Optional[FakeQuantizer]:
+    @abc.abstractmethod
+    def _get_output_quantizer(self, perchannel_args: PerChannelArgs = PerChannelArgs(), **kwargs) -> FakeQuantizer:
         """
         Define how to fake-quantize output data. This method must be overridden by all subclasses.
 
         Returns:
-            Return a instance of quantizer as quantizer for outputs.
+            Return an instance of quantizer as quantizer for outputs.
+        """
+        raise NotImplementedError
+
+    def get_output_quantizer(self, perchannel_args: PerChannelArgs = PerChannelArgs(),
+                             **kwargs) -> Optional[FakeQuantizer]:
+        """
+        Define how to fake-quantize output data.
+
+        Returns:
+            Return an instance of quantizer as quantizer for outputs.
             Return None if all outputs don't need to fake-quant.
         """
+        if self._output_insert_fq:
+            return self._get_output_quantizer(perchannel_args, **kwargs)
         return None
 
     @abc.abstractmethod
     def wrap_cell(self, handler: Cell) -> Cell:
         """
         Define how to wrapper `handler`. This method must be overridden by all subclasses.
 
@@ -85,26 +122,32 @@
             handler (Cell): cell to be wrapped.
 
         Returns:
             Wrapped cell.
         """
         raise NotImplementedError
 
+    @abc.abstractmethod
+    def get_config(self):
+        raise NotImplementedError
+
     def set_input_number(self, input_num: int):
         self._inputs_insert_fq.clear()
         self._input_num = input_num
         for _ in range(0, self._input_num):
             self._inputs_insert_fq.append(True)
 
     def set_input_not_insert_fq(self, index: Optional[int] = None):
-        if index is not None:
+        if index is None:
+            for i in range(0, self._input_num):
+                self._inputs_insert_fq[i] = False
+        else:
             if 0 <= index < self._input_num:
                 self._inputs_insert_fq[index] = False
             else:
                 raise RuntimeError("Index out of range of input number")
 
     def get_input_need_insert_fq(self) -> list:
         return self._inputs_insert_fq
 
-    # only support one-output-quantizer pre layer because we can not get how many outputs a cell would has
-    def set_output_not_insert_fq(self, index: Optional[int] = None):
-        pass
+    def set_output_not_insert_fq(self):
+        self._output_insert_fq = False
```

## mindspore_gs/quantization/net_policy.py

```diff
@@ -38,11 +38,11 @@
     def get_transformers(self) -> [Transformer]:
         return self._pattern_engines
 
     def get_layer_policy_map(self) -> {str, LayerPolicy}:
         return self._layer_policy_map
 
     def get_layer_policy(self, layer_type) -> Optional[LayerPolicy]:
-        return self._layer_policy_map.get(type(layer_type))
+        return self._layer_policy_map.get(layer_type)
 
     def get_net_layer_policy(self) -> Optional[LayerPolicy]:
         return self._net_layer_policy
```

## mindspore_gs/quantization/quant_utils.py

```diff
@@ -11,44 +11,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """Quantization utils."""
 
 import numpy as np
+import mindspore as ms
+from mindspore.common.dtype import QuantDtype
+from mindspore import Tensor
+
+__all__ = ["compute_kl_threshold", "fold_batchnorm", "cal_quantization_params", "get_quant_min_max",
+           "get_quant_dtype_num_bits"]
 
-from mindspore.ops.operations import _quant_ops as Q
-from mindspore.nn import Cell
 
-__all__ = ["compute_kl_threshold", "fold_batchnorm", "cal_quantization_params", "get_quant_min_max"]
-
-
-class LinearFakeQuantCell(Cell):
-    """
-    Fake quant layer with mindspore standard operator.
-    """
-
-    def __init__(self, quant_dtype, scale, zero_point, is_per_channel):
-        super(LinearFakeQuantCell, self).__init__()
-        self._quant_dtype = quant_dtype
-        self._scale = scale
-        self._zero_point = zero_point
-        self._is_per_channel = is_per_channel
-        self.fake_quant = Q.FakeQuantParam.linear_quant_param(quant_dtype=quant_dtype, scale=scale, zp=zero_point,
-                                                              is_per_channel=is_per_channel)
-
-    def extend_repr(self):
-        """Display instance object as string."""
-        s = 'quant_dtype={}, scale={}, zero_point={}, is_per_channel={}'.format(self._quant_dtype, self._scale,
-                                                                                self._zero_point, self._is_per_channel)
-        return s
-
-    def construct(self, x):
-        x = self.fake_quant(x)
-        return x
+def get_quant_dtype_num_bits(quant_dtype: QuantDtype):
+    if 0 <= quant_dtype.value() <= 15:
+        return quant_dtype.value() + 1
+    if 100 <= quant_dtype.value() <= 115:
+        return quant_dtype.value() - 99
+    raise ValueError("Unsupported QuantDtype.")
 
 
 def cal_quantization_params(input_min,
                             input_max,
                             quant_min,
                             quant_max,
                             symmetric=False):
@@ -65,30 +49,28 @@
     Returns:
         scale (numpy.ndarray): quantization param.
         zero point (numpy.ndarray): quantization param.
     """
 
     if input_min.shape != input_max.shape:
         raise ValueError("input min shape should be equal to input max.")
-    if len(input_min.shape) > 1:
-        raise ValueError("input min and max shape should be one dim.")
-    if (input_min > input_max).all():
-        raise ValueError("input_min min should be less than input max.")
+    #if (input_min > input_max).any():
+    #    raise ValueError("input_min should be smaller than input_max.")
     if (input_max == input_min).all():
         return np.ones(input_min.shape), np.zeros(input_min.shape)
 
     # calculate scale
     if symmetric:
-        input_max = np.maximum(-input_min, input_max)
+        input_max = np.maximum(np.abs(input_min), np.abs(input_max))
         input_min = -input_max
     scale = (input_max - input_min) / (quant_max - quant_min)
 
     # calculate zero point
     zp_double = quant_min - input_min / scale
-    zp = (np.floor(zp_double + 0.5)).astype(np.int)
+    zp = np.round(zp_double).astype(np.int)
 
     return scale, zp
 
 
 def get_quant_min_max(num_bits=8, signed=True, narrow_range=False):
     """Calculate quantization params for minimum/maximum quantization integer"""
     if signed:
@@ -98,14 +80,114 @@
         quant_min = 0
         quant_max = 2 ** num_bits - 1
     if narrow_range:
         quant_min = quant_min + 1
     return quant_min, quant_max
 
 
+def quant_tensor_data(tensor: Tensor, scale, zero_point, quant_min, quant_max, data_axis=-1, dtype=ms.dtype.int8):
+    r"""
+    Calculate int8/uint8 weight from fp32. the formula is defined as:
+
+    .. math::
+        int8/uint8 = round(float/scale) + offset
+
+    Args:
+        tensor (Tensor): The dimension of channel or 1. Should be NCHW.
+        scale (numpy.ndarray): The dimension of channel or 1.
+        zero_point (numpy.ndarray): The dimension of channel or 1.
+        quant_min (int): The minimum quantization integer.
+        quant_max (int): The maximum quantization integer.
+        data_axis (int): Quantize axis.
+
+    Returns:
+        weight (numpy.ndarray): The dimension of channel or 1.
+    """
+    if scale.shape != zero_point.shape:
+        raise ValueError("`scale` and `zero_point` should have the same shape.")
+    if scale.shape[0] < 0:
+        raise ValueError("`scale` and `zero_point` shape should be greater than zero.")
+    if tensor.shape[data_axis] != scale.shape[0]:
+        raise ValueError("Dim of `data`'s `data_axis` should be equal to `scale`'s shape.")
+    if data_axis >= len(tensor.shape):
+        raise ValueError("`data_axis` out of range of `data`'s shape.")
+
+    if data_axis >= 0:
+        # for perchannel
+        if data_axis == 0:
+            # `Conv2d` or `Dense` op weight
+            shape_list = [-1] + [1] * len(tensor.shape[1:])
+            scale = scale.reshape(shape_list)
+            zero_point = zero_point.reshape(shape_list)
+        elif data_axis == 1:
+            # `DepthwiseConv2d` op weight
+            shape_list = [1, -1] + [1] * len(tensor.shape[2:])
+            scale = scale.reshape(shape_list)
+            zero_point = zero_point.reshape(shape_list)
+        else:
+            raise ValueError("Unsupported data_axis({})".format(data_axis))
+
+    t_scale = Tensor(scale)
+    t_zp = Tensor(zero_point)
+    t_scale = ms.ops.cast(t_scale, tensor.dtype)
+    t_zp = ms.ops.cast(t_zp, tensor.dtype)
+    quanted_data = ms.ops.round((tensor / t_scale) + t_zp)
+    quanted_data = ms.ops.clamp(quanted_data, quant_min, quant_max)
+    quanted_data = ms.ops.cast(quanted_data, dtype)
+    return quanted_data
+
+
+def quant_data(data, scale, zero_point, quant_min, quant_max, data_axis=-1):
+    r"""
+    Calculate int8/uint8 weight from fp32. the formula is defined as:
+
+    .. math::
+        int8/uint8 = round(float/scale) + offset
+
+    Args:
+        data (numpy.ndarray): The dimension of channel or 1. Should be NCHW.
+        scale (numpy.ndarray): The dimension of channel or 1.
+        zero_point (numpy.ndarray): The dimension of channel or 1.
+        quant_min (int): The minimum quantization integer.
+        quant_max (int): The maximum quantization integer.
+        data_axis (int): Quantize axis.
+
+    Returns:
+        weight (numpy.ndarray): The dimension of channel or 1.
+    """
+    if scale.shape != zero_point.shape:
+        raise ValueError("`scale` and `zero_point` should have the same shape.")
+    if scale.shape[0] < 0:
+        raise ValueError("`scale` and `zero_point` shape should be greater than zero.")
+    if data.shape[data_axis] != scale.shape[0]:
+        raise ValueError("Dim of `data`'s `data_axis` should be equal to `scale`'s shape.")
+    if data_axis >= len(data.shape):
+        raise ValueError("`data_axis` out of range of `data`'s shape.")
+
+    if data_axis >= 0:
+        # for perchannel
+        if data_axis == 0:
+            # `Conv2d` or `Dense` op weight
+            shape_list = [-1] + [1] * len(data.shape[1:])
+            scale = scale.reshape(shape_list)
+            zero_point = zero_point.reshape(shape_list)
+        elif data_axis == 1:
+            # `DepthwiseConv2d` op weight
+            shape_list = [1, -1] + [1] * len(data.shape[2:])
+            scale = scale.reshape(shape_list)
+            zero_point = zero_point.reshape(shape_list)
+        else:
+            raise ValueError("Unsupported data_axis({})".format(data_axis))
+
+    quanted_data = np.round((data / scale) + zero_point)
+    quanted_data[quanted_data > quant_max] = quant_max
+    quanted_data[quanted_data < quant_min] = quant_min
+    return quanted_data
+
+
 def fold_batchnorm(weight, cell_quant):
     r"""
     Fold the batchnorm in `Conv2dBnFoldQuant` to weight.
 
     Calculate from `FakeQuantWithMinMax`'s Parameter or Fake quant primitive.
 
     Args:
@@ -229,7 +311,34 @@
         kl_tmp = np.sum((cumsum - cumsum_tmp) * np.log2(cumsum / cumsum_tmp))  # Kullback-Leibler-J
         kl = np.concatenate((kl, [kl_tmp]))
     th_layer_out = threshold[np.argmin(kl)]
     threshold = float(th_layer_out)
     if threshold < 1e-5:
         threshold = 1e-5
     return threshold
+
+
+def quant_bias_data(tensor: Tensor, scale, dtype=ms.dtype.int32):
+    r"""
+    Calculate int32 bias from fp32. the formula is defined as:
+
+    .. math::
+        int32 = round(bias / (scale_weight * scale_act))
+
+    Args:
+        tensor (Tensor): The bias tensor to be quanted
+        scale (numpy.ndarray): The dimension of channel or 1.
+        dtype(ms.dtype): default is dtype.int32
+
+    Returns:
+        quanted_bias (Tensor): quanted bias tensor
+    """
+
+    quant_scale = Tensor(np.squeeze(scale))
+    quanted_data = ms.ops.round(tensor / quant_scale)
+    print(f'quanted_data is {quanted_data.asnumpy()}')
+    quant_min = -2 ** 31
+    quant_max = 2 ** 31 - 1
+    quanted_data = ms.ops.clamp(quanted_data, quant_min, quant_max)
+    quanted_data = ms.ops.cast(quanted_data, dtype)
+    print(f'quanted data shape is {quanted_data.shape}, quant data is {quanted_data}')
+    return quanted_data
```

## mindspore_gs/quantization/quantization_aware_training.py

```diff
@@ -11,22 +11,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """Quantize."""
 import copy
 from typing import Optional
-from mindspore.rewrite import Node, NodeType
+from mindspore.rewrite import Node
 from mindspore.nn import Cell
 from .net_policy import NetPolicy
 from .layer_policy import LayerPolicy, layer_policy_key
 from .transformer import Transformer
-from .quantize_wrapper_cell import QuantizeWrapperCell
 from ..comp_algo import CompAlgo
 from ..net_transform import NetTransformer
+from .quant_cell import QuantCell
 
 
 class QuantizationAwareTraining(CompAlgo):
     """
     Derived class of `CompAlgo`. Base class of QAT-algorithm.
     """
 
@@ -46,50 +46,41 @@
         Args:
             nodes (List[Node]): nodes to be checked between which may find redundant fake-quantizer
         """
 
         # step1 apply net layer-policy first
         net_layer_policy: Optional[LayerPolicy] = self._qat_policy.get_net_layer_policy()
         if net_layer_policy:
-            for node in net_transformer.nodes():
+            for node in net_transformer.unfolded_nodes():
                 node.set_attribute(layer_policy_key, copy.copy(net_layer_policy))
         # step2 then apply layer-policy map, override policy if need
         layer_policy_map = self._qat_policy.get_layer_policy_map()
-        for node in net_transformer.nodes():
+        for node in net_transformer.unfolded_nodes():
             if not isinstance(node, Node):
                 continue
             layer_policy: LayerPolicy = self._custom_layer_policy_map.get(node.get_instance_type())
             if layer_policy is None:
                 layer_policy = layer_policy_map.get(node.get_instance_type())
             if isinstance(layer_policy, LayerPolicy):
                 new_layer_policy = copy.deepcopy(layer_policy)
-                new_layer_policy.set_input_number(len(node.get_inputs()))
                 node.set_attribute(layer_policy_key, new_layer_policy)
 
-        for node in net_transformer.nodes():
-            if node.get_node_type() == NodeType.Tree:
-                sub_net_trans = NetTransformer.create_from_tree_node(node)
-                self._propagate_layer_policy(sub_net_trans)
-
     @staticmethod
     def _reduce_redundant_fake_quant(net_transformer: NetTransformer):
         """
         Reduce redundant fake-quantizer node between nodes. It usually occurs when pre-node inserted output
         fake-quantizer and post-node inserted input fake-quantizer at the same time.
 
         Args:
             nodes (List[Node]): nodes to be checked between which may find redundant fake-quantizer
         """
 
-        for node in net_transformer.nodes():
+        for node in net_transformer.unfolded_nodes():
             if not isinstance(node, Node):
                 continue
-            if node.get_node_type() == NodeType.Tree:
-                sub_net_trans = NetTransformer.create_from_tree_node(node)
-                QuantizationAwareTraining._reduce_redundant_fake_quant(sub_net_trans)
             cur_policy: LayerPolicy = node.get_attribute(layer_policy_key)
             # cur-node has no quant policy, so no fq will insert into its inputs
             if cur_policy is None:
                 continue
             cur_in_quantizer = cur_policy.get_input_quantizer()
             # cur-node's input quantizer is None, so no fq will insert into its inputs
             if cur_in_quantizer is None:
@@ -126,16 +117,16 @@
                     transformers.append(transform)
         for transformer in transformers:
             # Transformer always return False
             net_transformer.pattern_transform(transformer)
 
     @staticmethod
     def _replace_node(net_transformer: NetTransformer, target_node: Node, result_cell: Cell):
-        if isinstance(result_cell, QuantizeWrapperCell):
-            node_name = type(getattr(result_cell, '_handler')).__name__
+        if isinstance(result_cell, QuantCell):
+            node_name = type(result_cell.handler()).__name__
         else:
             node_name = target_node.get_name()
         node = NetTransformer.create_node(result_cell, target_node.get_targets(), target_node.get_args(),
                                           target_node.get_kwargs(), node_name)
         net_transformer.replace(target_node, [node])
 
     @staticmethod
@@ -143,35 +134,31 @@
         """
         Apply layer-policy to corresponding layer.
         Replace layer with return value of wrap_cell of layer-policy by default.
 
         Args:
             net_transformer (NetTransformer): net_transformer is used to transform node according to layer policy.
         """
-        nodes = list(net_transformer.nodes())
+        nodes = list(net_transformer.unfolded_nodes())
         for node in nodes:
-            if node.get_node_type() == NodeType.Tree:
-                sub_net_transformer = NetTransformer.create_from_tree_node(node)
-                QuantizationAwareTraining._apply_layer_policy(sub_net_transformer)
-                continue
             layer_policy = node.get_attribute(layer_policy_key)
             if isinstance(layer_policy, LayerPolicy):
-                wrapped_cell = layer_policy.wrap_cell(node.get_instance())
-                wrapped_cell.update_parameters_name(node.get_name() + '.')
-                QuantizationAwareTraining._replace_node(net_transformer, node, wrapped_cell)
+                quant_cell = layer_policy.wrap_cell(node.get_instance())
+                quant_cell.update_parameters_name(node.get_name() + '.')
+                QuantizationAwareTraining._replace_node(net_transformer, node, quant_cell)
 
     def apply(self, network: Cell) -> Cell:
         """
         Apply QAT-Algorithm on `network`, use the following steps to make `network` available for quantization aware
         training:
 
         1. Fuse certain cells in `network` using pattern engine which is defined by net policy.
         2. Propagate layer policies defined through cells.
         3. Reduce redundant fake quantizers when they are redundant.
-        4. Apply layer policies to convert normal cell to `QuantizeWrapperCell`.
+        4. Apply layer policies to convert normal cell to `QuantCell`.
 
         Args:
             network (Cell): Network to be quantized.
 
         Returns:
             Quantized network.
         """
```

## mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_fake_quantizers.py

```diff
@@ -11,21 +11,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """learned step size fake quantizers."""
 
 from functools import partial
+from typing import Union
+
 import numpy as np
 import mindspore
+from mindspore import QuantDtype
 from mindspore.ops.operations import _quant_ops as Q
 from mindspore.common.parameter import Parameter
 from mindspore.common.tensor import Tensor
-from ..fake_quantizer import FakeQuantizer
-from ..quant_utils import compute_kl_threshold
+from mindspore_gs.quantization.fake_quantizer import LinearFakeQuantizer
+from mindspore_gs.quantization.quant_utils import compute_kl_threshold, get_quant_dtype_num_bits
 
 
 def _calculate_quant_max(num_bits, neg_trunc=False):
     """
     Define how to calculate the max value of quant data by bit num.
 
     Args:
@@ -38,35 +41,57 @@
     if neg_trunc:
         quant_max = (1 << num_bits) - 1
     else:
         quant_max = (1 << (num_bits - 1)) - 1
     return quant_max
 
 
-class LearnedStepSizeFakeQuantizerPerLayer(FakeQuantizer):
+class LearnedStepSizeFakeQuantizerPerLayer(LinearFakeQuantizer):
     """
     Derived class of FakeQuantizer. Use learning-rate from each epoch to compute scale and zero-point.
     """
 
-    def __init__(self, num_bits=8, quant_delay=0, min_init=-6, max_init=6, neg_trunc=False, symmetric=True,
-                 narrow_range=True):
+    def __init__(self, quant_delay=0, min_init=-6, max_init=6, neg_trunc=False, symmetric=True, narrow_range=True,
+                 quant_dtype=QuantDtype.INT8):
         super(LearnedStepSizeFakeQuantizerPerLayer, self).__init__()
-        self._num_bits = num_bits
         self._neg_trunc = neg_trunc
         self._symmetric = symmetric
         self._narrow_range = narrow_range
         self._quant_delay = quant_delay
+        self._quant_dtype = quant_dtype
+        self._num_bits = get_quant_dtype_num_bits(self._quant_dtype)
         self._quant_max = _calculate_quant_max(self._num_bits, self._neg_trunc)
         self.quant_max = Parameter(Tensor(np.array([self._quant_max]).astype(np.float32)))
         quant_func = partial(Q.FakeLearnedScaleQuantPerLayer, quant_delay=self._quant_delay, neg_trunc=self._neg_trunc)
         self.fake_quant_train = quant_func(training=True)
         self.fake_quant_infer = quant_func(training=False)
         self._float_min = Parameter(Tensor([min_init], mindspore.float32), name="float_min")
         self._float_max = Parameter(Tensor([max_init], mindspore.float32), name="float_max")
 
+    def mins(self) -> Union[list, tuple]:
+        return self._float_min.data.asnumpy().tolist()
+
+    def maxs(self) -> Union[list, tuple]:
+        return self._float_max.data.asnumpy().tolist()
+
+    def num_bits(self) -> int:
+        return self._num_bits
+
+    def narrow_range(self) -> bool:
+        return self._narrow_range
+
+    def symmetric(self) -> bool:
+        return self._symmetric
+
+    def quant_dtype(self) -> QuantDtype:
+        return self._quant_dtype
+
+    def is_per_channel(self) -> bool:
+        return False
+
     def compute_quant_param(self, weight_param):
         max_init = [compute_kl_threshold(weight_param, self._num_bits)]
         min_init = [-x for x in max_init]
         self._float_min.set_data(Tensor(self._get_init_array(max_init)))
         self._float_max.set_data(Tensor(self._get_init_array(min_init)))
 
     def construct(self, x):
@@ -80,28 +105,29 @@
         """Display instance object as string."""
         s = 'bit_num={}, neg_trunc={}, symmetric={}, narrow_range={}, ' \
             'per_channel={}, quant_delay={}'.format(self._num_bits, self._neg_trunc, self._symmetric,
                                                     self._narrow_range, False, self._quant_delay)
         return s
 
 
-class LearnedStepSizeFakeQuantizePerChannel(FakeQuantizer):
+class LearnedStepSizeFakeQuantizePerChannel(LinearFakeQuantizer):
     """
     Derived class of FakeQuantizer. perchannel version of LearnedFakeQuantizerPerLayer.
     """
 
-    def __init__(self, num_bits=8, num_channels=1, channel_axis=1, quant_delay=0,
-                 float_min=-6, float_max=6, neg_trunc=False, symmetric=True, narrow_range=True):
+    def __init__(self, num_channels=1, channel_axis=1, quant_delay=0, float_min=-6, float_max=6, neg_trunc=False,
+                 symmetric=True, narrow_range=True, quant_dtype=QuantDtype.INT8):
         super(LearnedStepSizeFakeQuantizePerChannel, self).__init__()
-        self._num_bits = num_bits
         self._symmetric = symmetric
         self._neg_trunc = neg_trunc
         self._narrow_range = narrow_range
         self._channel_axis = channel_axis
         self._quant_delay = quant_delay
+        self._quant_dtype = quant_dtype
+        self._num_bits = get_quant_dtype_num_bits(self._quant_dtype)
         self._quant_max = _calculate_quant_max(self._num_bits, self._neg_trunc)
         self.quant_max = Parameter(Tensor(np.array([self._quant_max]).astype(np.float32)))
         quant_func = partial(Q.FakeLearnedScaleQuantPerChannel, quant_delay=self._quant_delay,
                              neg_trunc=self._neg_trunc, channel_axis=self._channel_axis)
         self.fake_quant_train = quant_func(training=True)
         self.fake_quant_infer = quant_func(training=False)
         self._num_channels = num_channels
@@ -133,14 +159,35 @@
     def construct(self, x):
         if self.training:
             out = self.fake_quant_train(x, self._float_max, self.quant_max)
         else:
             out = self.fake_quant_infer(x, self._float_max, self.quant_max)
         return out
 
+    def mins(self) -> Union[list, tuple]:
+        return self._float_min.data.asnumpy().tolist()
+
+    def maxs(self) -> Union[list, tuple]:
+        return self._float_max.data.asnumpy().tolist()
+
+    def num_bits(self) -> int:
+        return self._num_bits
+
+    def narrow_range(self) -> bool:
+        return self._narrow_range
+
+    def symmetric(self) -> bool:
+        return self._symmetric
+
+    def quant_dtype(self) -> QuantDtype:
+        return self._quant_dtype
+
+    def is_per_channel(self) -> bool:
+        return False
+
     def extend_repr(self):
         """Display instance object as string."""
         s = 'num_bits={}, symmetric={}, narrow_range={}, neg_trunc={}, per_channel={}({}, {}), ' \
             'quant_delay={}'.format(self._num_bits, self._symmetric, self._narrow_range,
                                     self._neg_trunc, True,
                                     self._channel_axis, self._num_channels, self._quant_delay)
         return s
```

## mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_quantization_aware_training.py

```diff
@@ -10,24 +10,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """lsq algorithm"""
 from mindspore.nn import Cell
-from mindspore._checkparam import Validator
 from mindspore.common.dtype import QuantDtype
-from mindspore_gs.ops.nn import Conv2dQuant, DenseQuant, Conv2dBnFoldQuantOneConv, Conv2dBnWithoutFoldQuant, \
-    Conv2dBnFoldQuant
-from ..simulated_quantization.simulated_quantization_aware_training import SimulatedQuantizationAwareTraining as SimQAT
+from mindspore_gs.quantization.ops.nn import Conv2dQuant, DenseQuant, Conv2dBnFoldQuantOneConv, \
+    Conv2dBnWithoutFoldQuant, Conv2dBnFoldQuant
+from mindspore_gs.validator import Validator
+from mindspore_gs.quantization.simulated_quantization import SimulatedQuantizationAwareTraining as SimQAT
+from mindspore_gs.quantization.quant_cell import QuantCell
 from .learned_step_size_quantization_net_policy import LearnedStepSizeQuantizationNetPolicy as LsqNetPolicy
 from .learned_step_size_quantization_config import LearnedStepSizeQuantizationConfig as LsqConfig
 from .learned_step_size_fake_quantizers import LearnedStepSizeFakeQuantizerPerLayer as LsqFqPerLayer, \
     LearnedStepSizeFakeQuantizePerChannel as LsqFqPerChannel
-from ..quantize_wrapper_cell import QuantizeWrapperCell
 
 
 class LearnedStepSizeQuantizationAwareTraining(SimQAT):
     """
     Derived class of SimQAT. LSQ quantization algorithm.
 
     Args:
@@ -129,15 +129,15 @@
         >>> ## Since we set weight_quant_delay to be 0, the quant_delay value of fake_quant_weight are set to be 0.
         >>> print(net_qat)
         NetToQuantOpt<
           (_handler): NetToQuant<
             (conv): Conv2d<input_channels=1, output_channels=6, kernel_size=(5, 5), stride=(1, 1), pad_mode=valid, padding=0, dilation=(1, 1), group=1, has_bias=False, weight_init=normal, bias_init=zeros, format=NCHW>
             (bn): BatchNorm2d<num_features=6, eps=1e-05, momentum=0.09999999999999998, gamma=Parameter (name=_handler.bn.gamma, shape=(6,), dtype=Float32, requires_grad=True), beta=Parameter (name=_handler.bn.beta, shape=(6,), dtype=Float32, requires_grad=True), moving_mean=Parameter (name=_handler.bn.moving_mean, shape=(6,), dtype=Float32, requires_grad=False), moving_variance=Parameter (name=_handler.bn.moving_variance, shape=(6,), dtype=Float32, requires_grad=False)>
             >
-          (Conv2dBnWithoutFoldQuant): QuantizeWrapperCell<
+          (Conv2dBnWithoutFoldQuant): QuantCell<
             handler: in_channels=1, out_channels=6, kernel_size=(5, 5), stride=(1, 1), pad_mode=valid, padding=0, dilation=(1, 1), group=1, has_bias=False, input quantizer: bit_num=8, neg_trunc=False, symmetric=True, narrow_range=True, per_channel=False, quant_delay=0, output quantizer: bit_num=8, neg_trunc=False, symmetric=True, narrow_range=True, per_channel=False, quant_delay=0
             (_handler): Conv2dBnWithoutFoldQuant<
               in_channels=1, out_channels=6, kernel_size=(5, 5), stride=(1, 1), pad_mode=valid, padding=0, dilation=(1, 1), group=1, has_bias=False
               (fake_quant_weight): LearnedStepSizeFakeQuantizePerChannel<num_bits=8, symmetric=True, narrow_range=True, neg_trunc=False, per_channel=True(0, 6), quant_delay=0>
               (batchnorm): BatchNorm2d<num_features=6, eps=1e-05, momentum=0.0030000000000000027, gamma=Parameter (name=Conv2dBnWithoutFoldQuant._handler.batchnorm.gamma, shape=(6,), dtype=Float32, requires_grad=True), beta=Parameter (name=Conv2dBnWithoutFoldQuant._handler.batchnorm.beta, shape=(6,), dtype=Float32, requires_grad=True), moving_mean=Parameter (name=Conv2dBnWithoutFoldQuant._handler.batchnorm.moving_mean, shape=(6,), dtype=Float32, requires_grad=False), moving_variance=Parameter (name=Conv2dBnWithoutFoldQuant._handler.batchnorm.moving_variance, shape=(6,), dtype=Float32, requires_grad=False)>
               >
             (_input_quantizer): LearnedStepSizeFakeQuantizerPerLayer<bit_num=8, neg_trunc=False, symmetric=True, narrow_range=True, per_channel=False, quant_delay=0>
@@ -355,34 +355,34 @@
         """
         Apply LSQ Algorithm on `network`, use the following steps to make `network` available for quantization aware
         training:
 
         1. Fuse certain cells in `network` using pattern engine which is defined by net policy.
         2. Propagate layer policies defined through cells.
         3. Reduce redundant fake quantizers when they are redundant.
-        4. Apply layer policies to convert normal cell to `QuantizeWrapperCell`.
+        4. Apply layer policies to convert normal cell to `QuantCell`.
 
         Args:
             network (Cell): Network to be quantized.
 
         Returns:
             Quantized network.
         """
         quanted_net = super(LearnedStepSizeQuantizationAwareTraining, self).apply(network)
         self._reset_weights_quantization_params(quanted_net)
         return quanted_net
 
     def _reset_weights_quantization_params(self, network: Cell):
         for _, cell in network.name_cells().items():
-            if isinstance(cell, QuantizeWrapperCell):
-                if isinstance(cell.get_handler(), (Conv2dQuant, DenseQuant, Conv2dBnFoldQuantOneConv,
-                                                   Conv2dBnWithoutFoldQuant, Conv2dBnFoldQuant)):
-                    weight_fq = cell.get_handler().fake_quant_weight
+            if isinstance(cell, QuantCell):
+                if isinstance(cell, (Conv2dQuant, DenseQuant, Conv2dBnFoldQuantOneConv, Conv2dBnWithoutFoldQuant,
+                                     Conv2dBnFoldQuant)):
+                    weight_fq = cell.weight_quantizer()
                     if isinstance(weight_fq, (LsqFqPerLayer, LsqFqPerChannel)):
-                        weight_fq.compute_quant_param(cell.get_handler().weight)
+                        weight_fq.compute_quant_param(cell.handler().weight)
 
     def _init_net_policy(self, config):
         return LsqNetPolicy(config)
 
     def _create_config(self):
         """Create LsqConfig."""
         self._config = LsqConfig()
```

## mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_quantization_layer_policy.py

```diff
@@ -10,94 +10,123 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """learned step size quantization layer policy"""
 
-from typing import Optional
-from functools import partial
+import abc
+
 from mindspore.nn import Cell
-from mindspore_gs.ops.nn import Conv2dQuant, DenseQuant, Conv2dBnFoldQuantOneConv, Conv2dBnWithoutFoldQuant, \
-    Conv2dBnFoldQuant
+from mindspore_gs.quantization.ops.nn import Conv2dQuant, DenseQuant, Conv2dBnFoldQuantOneConv, \
+    Conv2dBnWithoutFoldQuant, Conv2dBnFoldQuant
+from mindspore_gs.quantization.fake_quantizer import FakeQuantizer
+from mindspore_gs.quantization.simulated_quantization.simulated_quantization_layer_policy import SimulatedLayerPolicy
+from mindspore_gs.quantization.layer_policy import PerChannelArgs
 from .learned_step_size_fake_quantizers import LearnedStepSizeFakeQuantizerPerLayer, \
     LearnedStepSizeFakeQuantizePerChannel
 from .learned_step_size_quantization_config import LearnedStepSizeQuantizationConfig
-from ..simulated_quantization.simulated_quantization_layer_policy import SimulatedLayerPolicy
-from ..fake_quantizer import FakeQuantizer
-from ..quantize_wrapper_cell import QuantizeWrapperCell
 
 
-class LearnedStepSizeQuantizationLayerPolicy(SimulatedLayerPolicy):
+class LearnedStepSizeQuantizationLayerPolicy(SimulatedLayerPolicy, abc.ABC):
     """
     Derived class of SimulatedLayerPolicy. LSQ layer policy.
     """
 
     def __init__(self, weight_names: [], act_names: [],
                  config: LearnedStepSizeQuantizationConfig = LearnedStepSizeQuantizationConfig()):
         super(LearnedStepSizeQuantizationLayerPolicy, self).__init__(weight_names, act_names, config)
-        if config.weight_per_channel:
-            self._weight_quantizer_partial = partial(LearnedStepSizeFakeQuantizePerChannel,
-                                                     quant_delay=config.weight_quant_delay,
-                                                     num_bits=self._num_bits,
-                                                     neg_trunc=config.weight_neg_trunc,
-                                                     symmetric=config.weight_symmetric,
-                                                     narrow_range=config.weight_narrow_range)
+        self._config: LearnedStepSizeQuantizationConfig = config
+        if config.act_per_channel:
+            raise ValueError("act quant only support perlayer now!")
+
+    def get_weight_quantizer(self, weight_name="", perchannel_args: PerChannelArgs = PerChannelArgs(),
+                             **kwargs) -> FakeQuantizer:
+        if self._config.weight_per_channel:
+            channel_axis = perchannel_args.channel_axis
+            num_channels = perchannel_args.num_channels
+            if channel_axis == -1:
+                raise RuntimeError("Please provide channel axis of weight for per-channel weight quantize.")
+            if num_channels == -1:
+                raise RuntimeError("Please provide channel number of weight for per-channel weight quantize.")
+            weight_quantizer = \
+                LearnedStepSizeFakeQuantizePerChannel(symmetric=self._config.weight_symmetric,
+                                                      quant_dtype=self._config.weight_quant_dtype,
+                                                      neg_trunc=self._config.weight_neg_trunc,
+                                                      quant_delay=self._config.weight_quant_delay,
+                                                      narrow_range=self._config.weight_narrow_range,
+                                                      channel_axis=channel_axis, num_channels=num_channels)
         else:
-            self._weight_quantizer_partial = partial(LearnedStepSizeFakeQuantizerPerLayer,
-                                                     quant_delay=config.weight_quant_delay,
-                                                     num_bits=self._num_bits,
-                                                     neg_trunc=config.weight_neg_trunc,
-                                                     symmetric=config.weight_symmetric,
-                                                     narrow_range=config.weight_narrow_range)
+            weight_quantizer = LearnedStepSizeFakeQuantizerPerLayer(symmetric=self._config.weight_symmetric,
+                                                                    quant_dtype=self._config.weight_quant_dtype,
+                                                                    quant_delay=self._config.weight_quant_delay,
+                                                                    narrow_range=self._config.weight_narrow_range)
+        return weight_quantizer
+
+    def _get_input_quantizer(self, input_index=-1, perchannel_args: PerChannelArgs = PerChannelArgs(),
+                             **kwargs) -> FakeQuantizer:
+        return LearnedStepSizeFakeQuantizerPerLayer(
+            quant_delay=self._config.act_quant_delay, quant_dtype=self._config.act_quant_dtype,
+            symmetric=self._config.act_symmetric,
+            narrow_range=self._config.act_narrow_range)
+
+    def _get_output_quantizer(self, perchannel_args: PerChannelArgs = PerChannelArgs(), **kwargs) -> FakeQuantizer:
+        return LearnedStepSizeFakeQuantizerPerLayer(
+            quant_delay=self._config.act_quant_delay, quant_dtype=self._config.act_quant_dtype,
+            symmetric=self._config.act_symmetric,
+            narrow_range=self._config.act_narrow_range)
 
-        if config.act_per_channel:
-            raise NotImplementedError("act quant only support perlayer now!")
-        self._act_quantizer: Optional[FakeQuantizer] = LearnedStepSizeFakeQuantizerPerLayer(
-            quant_delay=config.act_quant_delay, num_bits=self._num_bits, neg_trunc=config.act_neg_trunc,
-            symmetric=config.act_symmetric, narrow_range=config.act_narrow_range)
-        self._input_quantizer: Optional[FakeQuantizer] = LearnedStepSizeFakeQuantizerPerLayer(
-            quant_delay=config.act_quant_delay, num_bits=self._num_bits, symmetric=config.act_symmetric,
-            narrow_range=config.act_narrow_range)
-        self._output_quantizer: Optional[FakeQuantizer] = LearnedStepSizeFakeQuantizerPerLayer(
-            quant_delay=config.act_quant_delay, num_bits=self._num_bits, symmetric=config.act_symmetric,
-            narrow_range=config.act_narrow_range)
+    def get_config(self) -> LearnedStepSizeQuantizationConfig:
+        return self._config
+
+    @abc.abstractmethod
+    def wrap_cell(self, handler: Cell) -> Cell:
+        raise NotImplementedError
 
 
 class LearnedStepSizeQuantizationConvLayerPolicy(LearnedStepSizeQuantizationLayerPolicy):
     """
     Derived class of LearnedStepSizeQuantizationLayerPolicy. LayerPolicy used for nn.Conv2d.
     """
+    def __init__(self, weight_names: [], act_names: [],
+                 config: LearnedStepSizeQuantizationConfig = LearnedStepSizeQuantizationConfig()):
+        super().__init__(weight_names, act_names, config)
+        self.set_input_number(1)
 
     def wrap_cell(self, handler: Cell) -> Cell:
-        conv_quant = Conv2dQuant.from_conv2d(handler, self.get_quant_config())
-        return QuantizeWrapperCell(conv_quant, self)
+        return Conv2dQuant(handler, self)
 
 
 class LearnedStepSizeQuantizationDenseLayerPolicy(LearnedStepSizeQuantizationLayerPolicy):
     """
     Derived class of LearnedStepSizeQuantizationLayerPolicy. LayerPolicy used for nn.Conv2d.
     """
+    def __init__(self, weight_names: [], act_names: [],
+                 config: LearnedStepSizeQuantizationConfig = LearnedStepSizeQuantizationConfig()):
+        super().__init__(weight_names, act_names, config)
+        self.set_input_number(1)
 
     def wrap_cell(self, handler: Cell) -> Cell:
-        dense_quant = DenseQuant.from_dense(handler, self.get_quant_config())
-        return QuantizeWrapperCell(dense_quant, self)
+        return DenseQuant(handler, self)
 
 
 class LearnedStepSizeQuantizationConvBnLayerPolicy(LearnedStepSizeQuantizationLayerPolicy):
     """
     Derived class of LearnedStepSizeQuantizationLayerPolicy. LayerPolicy used for nn.Conv2d.
     """
+    def __init__(self, weight_names: [], act_names: [],
+                 config: LearnedStepSizeQuantizationConfig = LearnedStepSizeQuantizationConfig()):
+        super().__init__(weight_names, act_names, config)
+        self.set_input_number(1)
 
     def wrap_cell(self, handler: Cell) -> Cell:
         if handler.has_bn:
             if self._config.bn_fold:
                 if self._config.one_conv_fold:
-                    conv_quant = Conv2dBnFoldQuantOneConv.from_convbn(handler, self.get_quant_config())
+                    conv_quant = Conv2dBnFoldQuantOneConv(handler, self)
                 else:
-                    conv_quant = Conv2dBnFoldQuant.from_convbn(handler, self.get_quant_config(),
-                                                               {"freeze_bn": self._config.freeze_bn})
+                    conv_quant = Conv2dBnFoldQuant(handler, self, freeze_bn=self._config.freeze_bn)
             else:
-                conv_quant = Conv2dBnWithoutFoldQuant.from_convbn(handler, self.get_quant_config())
+                conv_quant = Conv2dBnWithoutFoldQuant(handler, self)
         else:
-            conv_quant = Conv2dQuant.from_convbn(handler, self.get_quant_config())
-        return QuantizeWrapperCell(conv_quant, self)
+            conv_quant = Conv2dQuant(handler, self)
+        return conv_quant
```

## mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_quantization_net_policy.py

```diff
@@ -10,18 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """learned step size quantization net_policy."""
 
-from mindspore.nn.layer import Conv2d, Dense, Conv2dBnAct
+from mindspore.nn.layer import Conv2d, Dense
 from ..simulated_quantization.simulated_quantization_net_policy import SimulatedNetPolicy
 from .learned_step_size_quantization_layer_policy import LearnedStepSizeQuantizationConvLayerPolicy, \
-    LearnedStepSizeQuantizationDenseLayerPolicy, LearnedStepSizeQuantizationConvBnLayerPolicy
+    LearnedStepSizeQuantizationDenseLayerPolicy
 from .learned_step_size_quantization_config import LearnedStepSizeQuantizationConfig
 
 
 class LearnedStepSizeQuantizationNetPolicy(SimulatedNetPolicy):
     """
     Derived class of SimulatedNetPolicy. LSQ quantization config.
     """
@@ -29,9 +29,8 @@
         super().__init__(config)
         self._config: LearnedStepSizeQuantizationConfig = config
 
     def build(self):
         super().build()
         self._layer_policy_map[Conv2d] = LearnedStepSizeQuantizationConvLayerPolicy([], [], self._config)
         self._layer_policy_map[Dense] = LearnedStepSizeQuantizationDenseLayerPolicy([], [], self._config)
-        self._layer_policy_map[Conv2dBnAct] = LearnedStepSizeQuantizationConvBnLayerPolicy([], [], self._config)
         self._build = True
```

## mindspore_gs/quantization/simulated_quantization/combined.py

```diff
@@ -10,21 +10,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """Combined layer."""
 
-from mindspore import nn
-from mindspore._checkparam import Validator
-from mindspore.nn.layer.normalization import BatchNorm2d
-from mindspore.nn.cell import Cell
+from mindspore.nn import Conv2d, BatchNorm2d
+from mindspore_gs.validator import Validator
 
 
-class Conv2dBn(Cell):
+class Conv2dBn(Conv2d):
     r"""
     A combination of convolution and Batchnorm layer.
 
     This part is a more detailed overview of Conv2d operation.
 
     Args:
         in_channels (int): The number of input channel :math:`C_{in}`.
@@ -93,29 +91,19 @@
                  has_bias=False,
                  weight_init='normal',
                  bias_init='zeros',
                  has_bn=False,
                  momentum=0.997,
                  eps=1e-5):
         """Initialize Conv2dBn."""
-        super(Conv2dBn, self).__init__()
+        super(Conv2dBn, self).__init__(in_channels, out_channels, kernel_size, stride, pad_mode, padding, dilation,
+                                       group, has_bias, weight_init, bias_init)
 
-        self.conv = nn.Conv2d(in_channels,
-                              out_channels,
-                              kernel_size=kernel_size,
-                              stride=stride,
-                              pad_mode=pad_mode,
-                              padding=padding,
-                              dilation=dilation,
-                              group=group,
-                              has_bias=has_bias,
-                              weight_init=weight_init,
-                              bias_init=bias_init)
         self.has_bn = Validator.check_bool(has_bn, "has_bn", self.cls_name)
         if has_bn:
             self.batchnorm = BatchNorm2d(out_channels, eps, momentum)
 
     def construct(self, x):
-        x = self.conv(x)
+        x = super(Conv2dBn, self).construct(x)
         if self.has_bn:
             x = self.batchnorm(x)
         return x
```

## mindspore_gs/quantization/simulated_quantization/simulated_fake_quantizers.py

```diff
@@ -11,27 +11,29 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """Simulated fake quantizers."""
 
 from functools import partial
+from typing import Union
+
 import numpy as np
 import mindspore
 from mindspore.ops.operations import _quant_ops as Q
 from mindspore.common.parameter import Parameter
 from mindspore.common.tensor import Tensor
 from mindspore.common.dtype import QuantDtype
 import mindspore.context as context
-from mindspore_gs.ops.common.quant_op_utils import get_quant_dtype_num_bits
-from ..fake_quantizer import FakeQuantizer
-from ..quant_utils import get_quant_min_max, cal_quantization_params, LinearFakeQuantCell
+from mindspore_gs.quantization.quant_utils import get_quant_dtype_num_bits
+from mindspore_gs.quantization.fake_quantizer import LinearFakeQuantizer
+from mindspore_gs.quantization.quant_utils import get_quant_min_max, cal_quantization_params
 
 
-class SimulatedFakeQuantizerPerLayer(FakeQuantizer):
+class SimulatedFakeQuantizerPerLayer(LinearFakeQuantizer):
     """
     Implement of SimFakeQuantizer.
     1. statistic the min max value passing through this op
     2. run fake quant execution to simulate the quantize loss
     """
 
     def __init__(self, ema=False, ema_decay=0.999, symmetric=False, narrow_range=False, quant_dtype=QuantDtype.INT8,
@@ -81,14 +83,38 @@
     def extend_repr(self):
         """Display instance object as string."""
         s = 'bit_num={}, symmetric={}, narrow_range={}, ema={}({}), per_channel={}, ' \
             'quant_delay={}'.format(self._num_bits, self._symmetric, self._narrow_range,
                                     self._ema, self._ema_decay, False, self._quant_delay)
         return s
 
+    def mins(self) -> Union[list, tuple]:
+        return self._float_min.data.asnumpy().tolist()
+
+    def maxs(self) -> Union[list, tuple]:
+        return self._float_max.data.asnumpy().tolist()
+
+    def num_bits(self) -> int:
+        return self._num_bits
+
+    def narrow_range(self) -> bool:
+        return self._narrow_range
+
+    def symmetric(self) -> bool:
+        return self._symmetric
+
+    def quant_dtype(self) -> QuantDtype:
+        if self._quant_dtype != QuantDtype.INT8:
+            raise TypeError("Only support int8 simulate quantization now!"
+                            "Please set quant_dtype=QuantDtype.INT8 for SimulatedQuantizationAwareTraining.")
+        return self._quant_dtype
+
+    def is_per_channel(self) -> bool:
+        return False
+
     def extract_quant_param(self):
         quant_min, quant_max = get_quant_min_max(num_bits=self._num_bits, signed=self._signed,
                                                  narrow_range=self._narrow_range)
         input_min = self._float_min.data.asnumpy()
         input_max = self._float_max.data.asnumpy()
         scale, zp = cal_quantization_params(input_min, input_max, quant_min, quant_max, symmetric=self._symmetric)
         return input_min, input_max, scale, zp
@@ -98,22 +124,14 @@
             self._float_min, self._float_max = \
                 self._min_max_update_func(x, self._float_min, self._float_max)
             out = self._fake_quant_train(x, self._float_min, self._float_max)
         else:
             out = self._fake_quant_infer(x, self._float_min, self._float_max)
         return out
 
-    def convert_to_fakequantparam(self):
-        if self._quant_dtype != QuantDtype.INT8:
-            raise TypeError("Only support int8 simulate quantization now!"
-                            "Please set quant_dtype=QuantDtype.INT8 for SimulatedQuantizationAwareTraining.")
-        _, _, scale, zero_point = self.extract_quant_param()
-        new_subcell = LinearFakeQuantCell(quant_dtype=self._quant_dtype, scale=tuple(scale),
-                                          zero_point=tuple(zero_point), is_per_channel=False)
-        return new_subcell
 
 class SimulatedFakeQuantizerPerChannel(SimulatedFakeQuantizerPerLayer):
     """
     Derived from SimFakeQuantizerPerLayer, perchannel version of sim fake quantizer
     """
 
     def __init__(self, num_channels=1, channel_axis=1, ema=False, ema_decay=0.999, symmetric=False, narrow_range=False,
@@ -142,23 +160,23 @@
         quant_min, quant_max = get_quant_min_max(num_bits=self._num_bits, signed=self._signed,
                                                  narrow_range=self._narrow_range)
         input_min = self._float_min.data.asnumpy()
         input_max = self._float_max.data.asnumpy()
         scale, zp = cal_quantization_params(input_min, input_max, quant_min, quant_max, symmetric=self._symmetric)
         return input_min, input_max, scale, zp
 
+    def mins(self) -> Union[list, tuple]:
+        return self._float_min.data.asnumpy().tolist()
+
+    def maxs(self) -> Union[list, tuple]:
+        return self._float_max.data.asnumpy().tolist()
+
+    def is_per_channel(self) -> bool:
+        return True
+
     def extend_repr(self):
         """Display instance object as string."""
         s = 'bit_num={}, symmetric={}, narrow_range={}, ema={}({}), per_channel={}({}, {}), ' \
             'quant_delay={}'.format(self._num_bits, self._symmetric, self._narrow_range,
                                     self._ema, self._ema_decay, True,
                                     self._channel_axis, self._num_channels, self._quant_delay)
         return s
-
-    def convert_to_fakequantparam(self):
-        if self._quant_dtype != QuantDtype.INT8:
-            raise TypeError("Only support int8 simulate quantization now!"
-                            "Please set quant_dtype=QuantDtype.INT8 for SimulatedQuantizationAwareTraining.")
-        _, _, scale, zero_point = self.extract_quant_param()
-        new_subcell = LinearFakeQuantCell(quant_dtype=self._quant_dtype, scale=tuple(scale),
-                                          zero_point=tuple(zero_point), is_per_channel=True)
-        return new_subcell
```

## mindspore_gs/quantization/simulated_quantization/simulated_quantization_aware_training.py

```diff
@@ -12,19 +12,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """SimulatedQuantizationAwareTraining."""
 
 import os
 from mindspore.nn import Cell
-from mindspore._checkparam import Validator, Rel
 from mindspore import log as logger
 from mindspore.train.serialization import load_checkpoint, load_param_into_net
 from mindspore.common.dtype import QuantDtype
-from ..quantization_aware_training import QuantizationAwareTraining
+from mindspore_gs.validator import Validator, Rel
+from mindspore_gs.quantization.quantization_aware_training import QuantizationAwareTraining
 from .simulated_quantization_net_policy import SimulatedNetPolicy
 from .simulated_quantization_config import SimulatedQuantizationConfig
 from .simulated_quantization_convert import ConvertToQuantInferNetwork
 
 
 class SimulatedQuantizationAwareTraining(QuantizationAwareTraining):
     """
@@ -35,38 +35,38 @@
 
     Args:
         config (dict): store attributes for quantization aware training, keys are attribute names,
             values are attribute values. The Default value is None, supported attribute are listed below:
 
             - quant_delay (Union[int, list, tuple]): Number of steps after which weights and activations are quantized
               during train and eval. The first element represents activations and the second element represents weights.
-              Default: (0, 0).
+              Default: ``(0, 0)``.
             - quant_dtype (Union[QuantDtype, list, tuple]): The target data type for quantization. It is necessary to
               consider the precision support of hardware devices when setting `quant_dtype`. The first element
               represents activations and the second element represents weights.
-              Default: (QuantDtype.INT8, QuantDtype.INT8).
-            - per_channel (Union[bool, list, tuple]):  Quantization granularity based on layer or on channel. If True
+              Default: ``(QuantDtype.INT8, QuantDtype.INT8)``.
+            - per_channel (Union[bool, list, tuple]):  Quantization granularity based on layer or on channel. If ``True``
               then base on per channel, otherwise base on per layer. The first element represents activations and the
-              second element represents weights, and the first element must be False now.
-              Default: (False, False).
-            - symmetric (Union[bool, list, tuple]): Whether the quantization algorithm is symmetric or not. If True
+              second element represents weights, and the first element must be ``False`` now.
+              Default: ``(False, False)``.
+            - symmetric (Union[bool, list, tuple]): Whether the quantization algorithm is symmetric or not. If ``True``
               then base on symmetric, otherwise base on asymmetric. The first element represents activations and the
               second element represents weights.
-              Default: (False, False).
+              Default: ``(False, False)``.
             - narrow_range (Union[bool, list, tuple]): Whether the quantization algorithm uses narrow range or not.
               The first element represents activations and the second element represents weights.
-              Default: (False, False).
+              Default: ``(False, False)``.
             - enable_fusion (bool): Whether apply fusion before applying quantization.
-              Default: False.
+              Default: ``False``.
             - freeze_bn (int): Number of steps after which BatchNorm OP parameters fixed to global mean and variance.
-              Default: 10000000.
+              Default: ``10000000``.
             - bn_fold (bool): Whether to use bn fold ops for simulation inference operation.
-              Default: False.
+              Default: ``False``.
             - one_conv_fold (bool): Whether to use one conv bn fold ops for simulation inference operation.
-              Default: True.
+              Default: ``True``.
 
     Raises:
         TypeError: If `bn_fold`, `one_conv_fold` or `enable_fusion` is not bool.
         TypeError: If `freeze_bn` is not int.
         TypeError: If `quant_delay` is not int, or every element of `quant_delay` is not int.
         TypeError: If `quant_dtype` is not `QuantDtype`, or every element of `quant_dtype` is not `QuantDtype`.
         TypeError: If `per_channel` is not bool, or every element of `per_channel` is not bool.
@@ -74,15 +74,15 @@
         TypeError: If `narrow_range` is not bool, or every element of `narrow_range` is not bool.
         ValueError: If `freeze_bn` is less than 0.
         ValueError: If the length of `quant_delay`, `quant_dtype`, `per_channel`, `symmetric` or `narrow_range` is more
             than 2.
         ValueError: If `quant_delay` is less than 0, or any element of `quant_delay` is less than 0.
         ValueError: If `quant_dtype` is not `QuantDtype.INT8`, or any element of `quant_dtype` is not
             `QuantDtype.INT8`.
-        ValueError: If `per_channel` is True, or the first element of `per_channel` is True.
+        ValueError: If `per_channel` is ``True``, or the first element of `per_channel` is ``True``.
 
     Supported Platforms:
         ``GPU``
 
     Examples:
         >>> from mindspore_gs.quantization import SimulatedQuantizationAwareTraining
         >>> from mindspore import nn
@@ -128,15 +128,15 @@
         >>> ## True.
         >>> print(net_qat)
         NetToQuantOpt<
           (_handler): NetToQuant<
             (conv): Conv2d<input_channels=1, output_channels=6, kernel_size=(5, 5), stride=(1, 1), pad_mode=valid, padding=0, dilation=(1, 1), group=1, has_bias=False, weight_init=normal, bias_init=zeros, format=NCHW>
             (bn): BatchNorm2d<num_features=6, eps=1e-05, momentum=0.09999999999999998, gamma=Parameter (name=_handler.bn.gamma, shape=(6,), dtype=Float32, requires_grad=True), beta=Parameter (name=_handler.bn.beta, shape=(6,), dtype=Float32, requires_grad=True), moving_mean=Parameter (name=_handler.bn.moving_mean, shape=(6,), dtype=Float32, requires_grad=False), moving_variance=Parameter (name=_handler.bn.moving_variance, shape=(6,), dtype=Float32, requires_grad=False)>
             >
-          (Conv2dBnWithoutFoldQuant): QuantizeWrapperCell<
+          (Conv2dBnWithoutFoldQuant): QuantCell<
             handler: in_channels=1, out_channels=6, kernel_size=(5, 5), stride=(1, 1), pad_mode=valid, padding=0, dilation=(1, 1), group=1, has_bias=False, input quantizer: bit_num=8, symmetric=False, narrow_range=False, ema=False(0.999), per_channel=False, quant_delay=900, output quantizer: bit_num=8, symmetric=False, narrow_range=False, ema=False(0.999), per_channel=False, quant_delay=900
             (_handler): Conv2dBnWithoutFoldQuant<
               in_channels=1, out_channels=6, kernel_size=(5, 5), stride=(1, 1), pad_mode=valid, padding=0, dilation=(1, 1), group=1, has_bias=False
               (fake_quant_weight): SimulatedFakeQuantizerPerChannel<bit_num=8, symmetric=True, narrow_range=False, ema=False(0.999), per_channel=True(0, 6), quant_delay=900>
               (batchnorm): BatchNorm2d<num_features=6, eps=1e-05, momentum=0.0030000000000000027, gamma=Parameter (name=Conv2dBnWithoutFoldQuant._handler.batchnorm.gamma, shape=(6,), dtype=Float32, requires_grad=True), beta=Parameter (name=Conv2dBnWithoutFoldQuant._handler.batchnorm.beta, shape=(6,), dtype=Float32, requires_grad=True), moving_mean=Parameter (name=Conv2dBnWithoutFoldQuant._handler.batchnorm.moving_mean, shape=(6,), dtype=Float32, requires_grad=False), moving_variance=Parameter (name=Conv2dBnWithoutFoldQuant._handler.batchnorm.moving_variance, shape=(6,), dtype=Float32, requires_grad=False)>
               >
             (_input_quantizer): SimulatedFakeQuantizerPerLayer<bit_num=8, symmetric=False, narrow_range=False, ema=False(0.999), per_channel=False, quant_delay=900>
@@ -196,58 +196,58 @@
         Set value of act_quant_delay of quantization aware training `config`
 
         Args:
             act_quant_delay (int): Number of steps after which activation is quantized during train and eval.
 
         Raises:
             TypeError: If `act_quant_delay` is not int.
-            ValueError: act_quant_delay is less than 0.
+            ValueError: `act_quant_delay` is less than 0.
         """
         Validator.check_is_int(act_quant_delay, "act_quant_delay", self.__class__.__name__)
         Validator.check_int(act_quant_delay, 0, Rel.GE, "act_quant_delay", self.__class__.__name__)
         self._config.act_quant_delay = act_quant_delay
 
     def set_weight_quant_delay(self, weight_quant_delay):
         """
         Set value of weight_quant_delay of quantization aware training `config`
 
         Args:
             weight_quant_delay (int): Number of steps after which weight is quantized during train and eval.
 
         Raises:
             TypeError: If `weight_quant_delay` is not int.
-            ValueError: weight_quant_delay is less than 0.
+            ValueError: `weight_quant_delay` is less than 0.
         """
         Validator.check_is_int(weight_quant_delay, "weight_quant_delay", self.__class__.__name__)
         Validator.check_int(weight_quant_delay, 0, Rel.GE, "weight_quant_delay", self.__class__.__name__)
         self._config.weight_quant_delay = weight_quant_delay
 
     def set_act_per_channel(self, act_per_channel):
         """
         Set value of act_per_channel of quantization aware training `config`
 
         Args:
-            act_per_channel (bool): Quantization granularity based on layer or on channel. If True then base on
-                per channel, otherwise base on per layer. Only support False now.
+            act_per_channel (bool): Quantization granularity based on layer or on channel. If ``True`` then base on
+                per channel, otherwise base on per layer. Only support ``False`` now.
 
         Raises:
             TypeError: If `act_per_channel` is not bool.
-            ValueError: Only supported if `act_per_channel` is False yet.
+            ValueError: Only supported if `act_per_channel` is ``False`` yet.
         """
         Validator.check_bool(act_per_channel, "act_per_channel", self.__class__.__name__)
         if act_per_channel:
             raise ValueError(f'Only supported if `act_per_channel` is False yet.')
         self._config.act_per_channel = act_per_channel
 
     def set_weight_per_channel(self, weight_per_channel):
         """
         Set value of weight_per_channel of quantization aware training `config`
 
         Args:
-            weight_per_channel (bool): Quantization granularity based on layer or on channel. If True then base on
+            weight_per_channel (bool): Quantization granularity based on layer or on channel. If ``True`` then base on
                 per channel, otherwise base on per layer.
 
         Raises:
             TypeError: If `weight_per_channel` is not bool.
         """
         Validator.check_bool(weight_per_channel, "weight_per_channel", self.__class__.__name__)
         self._config.weight_per_channel = weight_per_channel
@@ -268,15 +268,15 @@
                             f'but got {act_quant_dtype}.')
         if act_quant_dtype != QuantDtype.INT8:
             raise ValueError("Only supported if `act_quant_dtype` is `QuantDtype.INT8` yet.")
         self._config.act_quant_dtype = act_quant_dtype
 
     def set_weight_quant_dtype(self, weight_quant_dtype):
         """
-        Set value of weight_quant_dtype of quantization aware training `config`
+        Set value of weight_quant_dtype of quantization aware training `config`.
 
         Args:
             weight_quant_dtype (QuantDtype): Datatype used to quantize weight.
 
         Raises:
             TypeError: If `weight_quant_dtype` is not QuantDtype.
             ValueError: Only supported if `weight_quant_dtype` is `QuantDtype.INT8` yet.
@@ -286,61 +286,61 @@
                             f'but got {weight_quant_dtype}.')
         if weight_quant_dtype != QuantDtype.INT8:
             raise ValueError("Only supported if `weight_quant_dtype` is `QuantDtype.INT8` yet.")
         self._config.weight_quant_dtype = weight_quant_dtype
 
     def set_act_symmetric(self, act_symmetric):
         """
-        Set value of act_symmetric of quantization aware training `config`
+        Set value of act_symmetric of quantization aware training `config`.
 
         Args:
-            act_symmetric (bool): Whether the quantization algorithm use act symmetric or not. If True then base on
+            act_symmetric (bool): Whether the quantization algorithm use act symmetric or not. If ``True`` then base on
                 symmetric, otherwise base on asymmetric.
 
         Raises:
             TypeError: If `act_symmetric` is not bool.
         """
         Validator.check_bool(act_symmetric, "act_symmetric", self.__class__.__name__)
         self._config.act_symmetric = act_symmetric
 
     def set_weight_symmetric(self, weight_symmetric):
         """
         Set value of weight_symmetric of quantization aware training `config`
 
         Args:
-            weight_symmetric (bool): Whether the quantization algorithm use weight symmetric or not. If True then
+            weight_symmetric (bool): Whether the quantization algorithm use weight symmetric or not. If ``True`` then
                 base on symmetric, otherwise base on asymmetric.
 
         Raises:
             TypeError: If `weight_symmetric` is not bool.
         """
         Validator.check_bool(weight_symmetric, "weight_symmetric", self.__class__.__name__)
         self._config.weight_symmetric = weight_symmetric
 
     def set_act_narrow_range(self, act_narrow_range):
         """
         Set value of act_narrow_range of quantization aware training `config`
 
         Args:
-            act_narrow_range (bool): Whether the quantization algorithm use act narrow_range or not. If True then
+            act_narrow_range (bool): Whether the quantization algorithm use act narrow_range or not. If ``True`` then
                 base on narrow_range, otherwise base on not narrow_range.
 
         Raises:
             TypeError: If `act_narrow_range` is not bool.
         """
         Validator.check_bool(act_narrow_range, "act_narrow_range", self.__class__.__name__)
         self._config.act_narrow_range = act_narrow_range
 
     def set_weight_narrow_range(self, weight_narrow_range):
         """
         Set value of weight_narrow_range of quantization aware training `config`
 
         Args:
             weight_narrow_range (bool): Whether the quantization algorithm use weight narrow_range or not. If
-                True then base on narrow_range, otherwise base on not narrow_range.
+                ``True`` then base on narrow_range, otherwise base on not narrow_range.
 
         Raises:
             TypeError: If `weight_narrow_range` is not bool.
         """
         Validator.check_bool(weight_narrow_range, "weight_narrow_range", self.__class__.__name__)
         self._config.weight_narrow_range = weight_narrow_range
 
@@ -429,15 +429,15 @@
         Apply SimQAT Algorithm on `network`, use the following steps to make `network` available for quantization aware
         training:
 
         1. Fuse certain cells in `network` using pattern engine which is defined by net policy. Default fuse pattern:
            Conv2d + BatchNorm2d + ReLU, Conv2d + ReLU, Dense + BatchNorm2d + ReLU, Dense + BatchNorm2d, Dense + ReLU.
         2. Propagate LayerPolicies defined in NetPolicy through network.
         3. Reduce redundant fake quantizers which means two or more fake quantizers existing on one tensor.
-        4. Apply LayerPolicies to convert normal cell to `QuantizeWrapperCell`. We will insert real fake quantizer
+        4. Apply LayerPolicies to convert normal cell to `QuantCell`. We will insert real fake quantizer
            into network in this step.
 
         Args:
             network (Cell): Network to be quantized.
 
         Returns:
             Quantized network.
@@ -447,34 +447,37 @@
 
     def convert(self, net_opt: Cell, ckpt_path="") -> Cell:
         """
         Define how to convert a compressed network to a standard network before exporting to MindIR.
 
         Args:
             net_opt (Cell): Network to be converted which is transformed by `SimulatedQuantizationAwareTraining.apply`.
-            ckpt_path (str): Path to checkpoint file for `net_opt`. Default is a empty string which means not loading
+            ckpt_path (str): Path to checkpoint file for `net_opt`. Default is ``""``, which means not loading
                 checkpoint file to `net_opt`.
 
         Returns:
             An instance of Cell represents converted network.
 
         Raises:
             TypeError: If `net_opt` is not Cell.
             TypeError: If `ckpt_path` is not string.
             ValueError: If `ckpt_path` is not empty and invalid.
+            RuntimeError: If loading `ckpt_path` fails.
         """
         if not isinstance(net_opt, Cell):
             raise TypeError(
                 f'The parameter `net_opt` must be isinstance of Cell, but got {type(net_opt)}.')
         if not isinstance(ckpt_path, str):
             raise TypeError(
                 f'The parameter `ckpt_path` must be isinstance of str, but got {type(ckpt_path)}.')
         real_path = os.path.realpath(ckpt_path)
         if ckpt_path != "":
             if os.path.isfile(real_path):
                 param_dict = load_checkpoint(ckpt_path)
-                load_param_into_net(net_opt, param_dict)
+                not_load_param = load_param_into_net(net_opt, param_dict)
+                if not_load_param[0]:
+                    raise RuntimeError("Load param into net fail.")
             else:
                 raise ValueError(
                     f'The parameter `ckpt_path` can only be empty or a valid file, but got {real_path}.')
         exporter = ConvertToQuantInferNetwork(net_opt)
         return exporter.run()
```

## mindspore_gs/quantization/simulated_quantization/simulated_quantization_config.py

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """Config for aware-training-quantization."""
 
 from mindspore.common.dtype import QuantDtype
-from ...comp_algo import CompAlgoConfig
+from mindspore_gs.comp_algo import CompAlgoConfig
 
 
 class SimulatedQuantizationConfig(CompAlgoConfig):
     """
     Config for simulated quantization aware training.
     See more details in simulated_quantization_aware_training.py
     """
```

## mindspore_gs/quantization/simulated_quantization/simulated_quantization_convert.py

```diff
@@ -10,85 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """Simulated Quantization Convert Utils."""
 
-import numpy as np
-
-from mindspore.nn import Cell
-from mindspore.common import Tensor
-from mindspore.ops import operations as P
-from mindspore.ops.operations import _quant_ops as Q
-from mindspore.common import dtype as mstype
 from mindspore.common.dtype import QuantDtype
-from mindspore_gs.ops.nn import Conv2dQuant, DenseQuant, Conv2dBnFoldQuantOneConv, Conv2dBnWithoutFoldQuant, \
-    Conv2dBnFoldQuant
-from ..quantize_wrapper_cell import QuantizeWrapperCell
-from ..quant_utils import fold_batchnorm, without_fold_batchnorm
-from .simulated_fake_quantizers import SimulatedFakeQuantizerPerChannel
-
-
-class CellBlockWithFakeWeight(Cell):
-    """A block of Conv/Dense, activation layer with fake quantization weight for export MINDIR model.
-
-       Args:
-        core_op (Cell): The operation cell.
-        scale_w (tuple): The quantization parameter scale of the weight.
-        zp_w (tuple): The quantization parameter zero point of the weight.
-        weight (Tensor): The weight of the cell.
-        bias (Tensor): The bias of the cell. Default: None.
-        activation (str): The regularization function applied to the output of the layer, eg. 'relu'. Default: None.
-        param_dict (dict): The information of the cell.
-    """
-
-    def __init__(self,
-                 core_op,
-                 scale_w,
-                 zp_w,
-                 weight,
-                 bias=None,
-                 activation=None,
-                 param_dict=None):
-
-        super(CellBlockWithFakeWeight, self).__init__()
-        self.core_op = core_op
-        if activation is not None:
-            self.core_op.add_prim_attr(
-                "activation_name", activation.__class__.__name__)
-        if hasattr(core_op, 'pad_mode'):
-            self.core_op.add_prim_attr("pad_mode", core_op.pad_mode)
-
-        self.weight = weight
-        self.bias = bias
-        self.has_bias = bias is not None
-        self.activation = activation
-        self.has_act = activation is not None
-        self.bias_add = P.BiasAdd()
-        self.fake_weight = Q.FakeQuantParam.linear_quant_param(quant_dtype=param_dict["quant_dtype"],
-                                                               scale=scale_w, zp=zp_w,
-                                                               is_per_channel=param_dict["is_per_channel"])
-
-    def construct(self, x):
-        weight = self.fake_weight(self.weight)
-        x = self.core_op(x, weight)
-        if self.has_bias:
-            x = self.bias_add(x, self.bias)
-        if self.has_act:
-            x = self.activation(x)
-        return x
-
-    def extend_repr(self):
-        s = f'core_op={type(self.core_op)}, weight=shape[{self.weight.shape}]'
-        if self.has_bias:
-            s += f', bias=shape[{self.bias.shape}]'
-        if self.has_act:
-            s += f', activation={self.activation}'
-        return s
+from mindspore_gs.quantization.quant_cell import QuantCell
 
 
 class ConvertToQuantInferNetwork:
     """
     Convert quantization aware network to infer network.
 
     Args:
@@ -103,87 +34,19 @@
         self.network = network
 
     def run(self):
         """Start to convert."""
         self.network.update_cell_prefix()
         return self._convert_quant2deploy(self.network)
 
-    def _get_quant_block(self, cell_core):
-        """convert network's quant subcell to deploy subcell"""
-        scale_w, zp_w = self.__get_quant_param(cell_core)
-        activation = None
-
-        # get op
-        if isinstance(cell_core, DenseQuant):
-            op_core = P.MatMul()
-            activation = cell_core.activation
-        else:
-            op_core = cell_core.conv
-
-        # get the `weight` and `bias`
-        weight, bias = self.__get_weight_bias(cell_core)
-        is_per_channel = isinstance(
-            cell_core.fake_quant_weight, SimulatedFakeQuantizerPerChannel)
-        quant_params = {"quant_dtype": self.quant_dtype,
-                        "is_per_channel": is_per_channel}
-        block = CellBlockWithFakeWeight(op_core, tuple(scale_w), tuple(zp_w), weight, bias, activation, quant_params)
-        return block
-
-    def __get_quant_param(self, cell_core):
-        """Get scale and bias for fake quant weight"""
-        _, _, scale_w, zp_w = cell_core.fake_quant_weight.extract_quant_param()
-        return scale_w, zp_w
-
-    def __get_weight_bias(self, cell_core):
-        """Get weight and bias for quantizaiton"""
-        weight = cell_core.weight.data.asnumpy()
-        bias = None
-        if isinstance(cell_core, (Conv2dQuant, DenseQuant)):
-            if cell_core.has_bias:
-                bias = cell_core.bias.data.asnumpy()
-        elif isinstance(cell_core, (Conv2dBnFoldQuant, Conv2dBnFoldQuantOneConv)):
-            weight, bias = fold_batchnorm(weight, cell_core)
-        elif isinstance(cell_core, Conv2dBnWithoutFoldQuant):
-            weight, bias = without_fold_batchnorm(weight, cell_core)
-
-        if isinstance(cell_core, DenseQuant):
-            weight = np.transpose(weight)
-
-        weight_tensor = Tensor(weight)
-        if bias is not None:
-            bias_tensor = Tensor(bias, mstype.float32)
-            return weight_tensor, bias_tensor
-        return weight_tensor, None
-
-    def _convert_subcell(self, cell_core):
-        """Convert subcell to ant subcell."""
-        if cell_core is not None and hasattr(cell_core, "fake_quant_weight"):
-            new_subcell = self._get_quant_block(cell_core)
-            return new_subcell
-        return None
-
-    def _convert_core_subcell(self, cell_core):
-        """Convert subcell for conv and dense."""
-        if isinstance(cell_core, (Conv2dQuant, Conv2dBnFoldQuant, Conv2dBnFoldQuantOneConv, Conv2dBnWithoutFoldQuant,
-                                  DenseQuant)):
-            return self._convert_subcell(cell_core)
-        return cell_core
-
     def _convert_quant2deploy(self, network):
         """Convert network's all quant subcell to deploy subcell."""
         cells = network.name_cells()
         for name in cells:
             subcell = cells[name]
             if subcell == network:
                 continue
-            if isinstance(subcell, QuantizeWrapperCell):
-                handler_cell = subcell.get_handler()
-                new_subcell = self._convert_core_subcell(handler_cell)
-                subcell.insert_child_to_cell("_handler", new_subcell)
-
-                fake_quant_input = subcell.get_input_quantizer().convert_to_fakequantparam()
-                fake_quant_output = subcell.get_output_quantizer().convert_to_fakequantparam()
-                subcell.insert_child_to_cell("_input_quantizer", fake_quant_input)
-                subcell.insert_child_to_cell("_output_quantizer", fake_quant_output)
+            if isinstance(subcell, QuantCell):
+                subcell.convert()
             else:
                 self._convert_quant2deploy(subcell)
         return network
```

## mindspore_gs/quantization/simulated_quantization/simulated_quantization_layer_policy.py

```diff
@@ -10,135 +10,143 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """DefaultLayerPolicy."""
 
-from typing import Optional
-from functools import partial
+import abc
 
 from mindspore.nn import Cell
 from mindspore.common.dtype import QuantDtype
-from mindspore_gs.ops.nn.fake_quant_with_min_max_observer import QuantConfig as OpQuantConfig
-from mindspore_gs.ops.nn import Conv2dQuant, DenseQuant, Conv2dBnFoldQuantOneConv, Conv2dBnWithoutFoldQuant, \
-    Conv2dBnFoldQuant
-from ..layer_policy import LayerPolicy
-from ..quantize_wrapper_cell import QuantizeWrapperCell
-from ..fake_quantizer import FakeQuantizer
+from mindspore_gs.quantization.layer_policy import LayerPolicy, PerChannelArgs
+from mindspore_gs.quantization.fake_quantizer import FakeQuantizer
+from mindspore_gs.quantization.ops.nn import Conv2dQuant, DenseQuant, Conv2dBnFoldQuantOneConv, \
+    Conv2dBnWithoutFoldQuant, Conv2dBnFoldQuant, ActQuant
 from .simulated_fake_quantizers import SimulatedFakeQuantizerPerChannel, SimulatedFakeQuantizerPerLayer
 from .simulated_quantization_config import SimulatedQuantizationConfig
 
 
-class SimulatedLayerPolicy(LayerPolicy):
+class SimulatedLayerPolicy(LayerPolicy, abc.ABC):
     """
     Derived class of LayerPolicy. Sim-QAT layer policy.
     Use linear perchannel fake quantizer as weight fake quantizer, linear perlayer fake quantizer as act fake quantizer.
 
     Supported Config:
         ``quant_delay`` ``quant_dtype`` ``per_channel`` ``symmetric`` ``narrow_range`` ``one_conv_fold``.
     """
 
     def __init__(self, weight_names: [], act_names: [],
                  config: SimulatedQuantizationConfig = SimulatedQuantizationConfig()):
         super(SimulatedLayerPolicy, self).__init__()
-        self._config = config
+        self._config: SimulatedQuantizationConfig = config
         if config.weight_quant_dtype == QuantDtype.INT8:
             self._num_bits = 8
         else:
             raise TypeError("Only support int8 weight quant now!")
-        if config.weight_per_channel:
-            self._weight_quantizer_partial = partial(SimulatedFakeQuantizerPerChannel,
-                                                     ema=False,
-                                                     symmetric=config.weight_symmetric,
-                                                     quant_dtype=config.weight_quant_dtype,
-                                                     quant_delay=config.weight_quant_delay,
-                                                     narrow_range=config.weight_narrow_range)
-        else:
-            self._weight_quantizer_partial = partial(SimulatedFakeQuantizerPerLayer, ema=False,
-                                                     symmetric=config.weight_symmetric,
-                                                     quant_dtype=config.weight_quant_dtype,
-                                                     quant_delay=config.weight_quant_delay,
-                                                     narrow_range=config.weight_narrow_range)
         if config.act_per_channel:
             raise NotImplementedError("act quant only support perlayer now!")
-        self._act_quantizer: Optional[FakeQuantizer] = SimulatedFakeQuantizerPerLayer(
-            symmetric=config.act_symmetric, quant_dtype=config.act_quant_dtype, quant_delay=config.act_quant_delay,
-            narrow_range=config.act_narrow_range)
-        self._input_quantizer: Optional[FakeQuantizer] = SimulatedFakeQuantizerPerLayer(
-            symmetric=config.act_symmetric, quant_dtype=config.act_quant_dtype, quant_delay=config.act_quant_delay,
-            narrow_range=config.act_narrow_range)
-        self._output_quantizer: Optional[FakeQuantizer] = SimulatedFakeQuantizerPerLayer(
-            symmetric=config.act_symmetric, quant_dtype=config.act_quant_dtype, quant_delay=config.act_quant_delay,
-            narrow_range=config.act_narrow_range)
         self._weight_names = weight_names
         self._act_names = act_names
 
-    def get_weight_name_and_quantizers(self):
-        return [(name, self._weight_quantizer_partial) for name in self._weight_names]
-
-    def get_act_name_and_quantizers(self):
-        return [(name, self._act_quantizer) for name in self._act_names]
-
-    def get_input_quantizer(self) -> Optional[FakeQuantizer]:
-        return self._input_quantizer
-
-    def get_output_quantizer(self) -> Optional[FakeQuantizer]:
-        return self._output_quantizer
-
-    def set_output_not_insert_fq(self, index: Optional[int] = None):
-        self._output_quantizer = None
+    def get_weight_quantizer(self, weight_name="", perchannel_args: PerChannelArgs = PerChannelArgs(),
+                             **kwargs) -> FakeQuantizer:
+        if self._config.weight_per_channel:
+            channel_axis = perchannel_args.channel_axis
+            num_channels = perchannel_args.num_channels
+            if channel_axis == -1:
+                raise RuntimeError("Please provide channel axis of weight for per-channel weight quantize.")
+            if num_channels == -1:
+                raise RuntimeError("Please provide channel number of weight for per-channel weight quantize.")
+            weight_quantizer = SimulatedFakeQuantizerPerChannel(ema=False, symmetric=self._config.weight_symmetric,
+                                                                quant_dtype=self._config.weight_quant_dtype,
+                                                                quant_delay=self._config.weight_quant_delay,
+                                                                narrow_range=self._config.weight_narrow_range,
+                                                                channel_axis=channel_axis, num_channels=num_channels)
+        else:
+            weight_quantizer = SimulatedFakeQuantizerPerLayer(ema=False, symmetric=self._config.weight_symmetric,
+                                                              quant_dtype=self._config.weight_quant_dtype,
+                                                              quant_delay=self._config.weight_quant_delay,
+                                                              narrow_range=self._config.weight_narrow_range)
+        return weight_quantizer
+
+    def _get_input_quantizer(self, input_index=-1, perchannel_args: PerChannelArgs = PerChannelArgs(),
+                             **kwargs) -> FakeQuantizer:
+        return SimulatedFakeQuantizerPerLayer(symmetric=self._config.act_symmetric,
+                                              quant_dtype=self._config.act_quant_dtype,
+                                              quant_delay=self._config.act_quant_delay,
+                                              narrow_range=self._config.act_narrow_range)
+
+    def _get_output_quantizer(self, perchannel_args: PerChannelArgs = PerChannelArgs(), **kwargs) -> FakeQuantizer:
+        return SimulatedFakeQuantizerPerLayer(symmetric=self._config.act_symmetric,
+                                              quant_dtype=self._config.act_quant_dtype,
+                                              quant_delay=self._config.act_quant_delay,
+                                              narrow_range=self._config.act_narrow_range)
 
-    def get_quant_config(self):
-        return OpQuantConfig(self._weight_quantizer_partial, self._output_quantizer)
+    def get_config(self) -> SimulatedQuantizationConfig:
+        return self._config
 
+    @abc.abstractmethod
     def wrap_cell(self, handler: Cell) -> Cell:
-        return QuantizeWrapperCell(handler, self)
+        raise NotImplementedError
 
 
 class ConvLayerPolicy(SimulatedLayerPolicy):
     """
     Derived class of SimulatedLayerPolicy. LayerPolicy used for nn.Conv2d.
     """
+    def __init__(self, weight_names: [], act_names: [],
+                 config: SimulatedQuantizationConfig = SimulatedQuantizationConfig()):
+        super().__init__(weight_names, act_names, config)
+        self.set_input_number(1)
 
     def wrap_cell(self, handler: Cell) -> Cell:
-        conv_quant = Conv2dQuant.from_conv2d(handler, self.get_quant_config())
-        return QuantizeWrapperCell(conv_quant, self)
+        return Conv2dQuant(handler, self)
 
 
 class DenseLayerPolicy(SimulatedLayerPolicy):
     """
     Derived class of SimulatedLayerPolicy. LayerPolicy used for nn.Dense.
     """
+    def __init__(self, weight_names: [], act_names: [],
+                 config: SimulatedQuantizationConfig = SimulatedQuantizationConfig()):
+        super().__init__(weight_names, act_names, config)
+        self.set_input_number(1)
 
     def wrap_cell(self, handler: Cell) -> Cell:
-        dense_quant = DenseQuant.from_dense(handler, self.get_quant_config())
-        return QuantizeWrapperCell(dense_quant, self)
+        return DenseQuant(handler, self)
 
 
 class ConvBnLayerPolicy(SimulatedLayerPolicy):
     """
     Derived class of SimulatedLayerPolicy. LayerPolicy used for nn.ConvBn.
     """
+    def __init__(self, weight_names: [], act_names: [],
+                 config: SimulatedQuantizationConfig = SimulatedQuantizationConfig()):
+        super().__init__(weight_names, act_names, config)
+        self.set_input_number(1)
 
     def wrap_cell(self, handler: Cell) -> Cell:
         if handler.has_bn:
             if self._config.bn_fold:
                 if self._config.one_conv_fold:
-                    conv_quant = Conv2dBnFoldQuantOneConv.from_convbn(handler, self.get_quant_config())
+                    conv_quant = Conv2dBnFoldQuantOneConv(handler, self)
                 else:
-                    conv_quant = Conv2dBnFoldQuant.from_convbn(handler, self.get_quant_config(),
-                                                               {"freeze_bn": self._config.freeze_bn})
+                    conv_quant = Conv2dBnFoldQuant(handler, self, freeze_bn=self._config.freeze_bn)
             else:
-                conv_quant = Conv2dBnWithoutFoldQuant.from_convbn(handler, self.get_quant_config())
+                conv_quant = Conv2dBnWithoutFoldQuant(handler, self)
         else:
-            conv_quant = Conv2dQuant.from_convbn(handler, self.get_quant_config())
-        return QuantizeWrapperCell(conv_quant, self)
+            conv_quant = Conv2dQuant(handler, self)
+        return conv_quant
 
 
 class ActLayerPolicy(SimulatedLayerPolicy):
     """
     Derived class of SimulatedLayerPolicy. LayerPolicy used for activation layer.
     """
+    def __init__(self, weight_names: [], act_names: [],
+                 config: SimulatedQuantizationConfig = SimulatedQuantizationConfig()):
+        super().__init__(weight_names, act_names, config)
+        self.set_input_number(1)
 
     def wrap_cell(self, handler: Cell) -> Cell:
-        return QuantizeWrapperCell(handler, self)
+        return ActQuant(handler, self)
```

## mindspore_gs/quantization/simulated_quantization/simulated_quantization_net_policy.py

```diff
@@ -12,18 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """DefaultNetworkPolicy."""
 
 from mindspore.nn.layer import Conv2d, Dense, BatchNorm2d, ReLU, ReLU6, Sigmoid, LeakyReLU, HSigmoid, HSwish
 from mindspore.rewrite import PatternEngine
-from ..net_policy import NetPolicy
+from mindspore_gs.quantization.net_policy import NetPolicy
 from .combined import Conv2dBn
 from .simulated_quantization_layer_policy import ConvLayerPolicy, DenseLayerPolicy, ConvBnLayerPolicy, ActLayerPolicy
-from .simulated_quantization_transforms import Conv2dBnFuse, DenseBnActFuse, DenseActFuse
+from .simulated_quantization_transforms import Conv2dBnFuse
 from .simulated_quantization_config import SimulatedQuantizationConfig
 
 
 class SimulatedNetPolicy(NetPolicy):
     """
     Derived class of NetworkQConfig. Sim-QAT quant config.
 
@@ -41,17 +41,14 @@
 
     def build(self):
         """Initialize `SimulatedNetPolicy`. A `SimulatedNetPolicy` can only be built once."""
         if self._build:
             return
         if self._config.enable_fusion:
             self._pattern_engines.append(PatternEngine([Conv2d, BatchNorm2d], Conv2dBnFuse()))
-            self._pattern_engines.append(PatternEngine([Dense, BatchNorm2d, ReLU], DenseBnActFuse()))
-            self._pattern_engines.append(PatternEngine([Dense, BatchNorm2d], DenseBnActFuse()))
-            self._pattern_engines.append(PatternEngine([Dense, ReLU], DenseActFuse()))
         self._layer_policy_map[Conv2d] = ConvLayerPolicy([], [], self._config)
         self._layer_policy_map[Conv2dBn] = ConvBnLayerPolicy([], [], self._config)
         self._layer_policy_map[Dense] = DenseLayerPolicy([], [], self._config)
         self._layer_policy_map[ReLU] = ActLayerPolicy([], [], self._config)
         self._layer_policy_map[ReLU6] = ActLayerPolicy([], [], self._config)
         self._layer_policy_map[Sigmoid] = ActLayerPolicy([], [], self._config)
         self._layer_policy_map[LeakyReLU] = ActLayerPolicy([], [], self._config)
```

## mindspore_gs/quantization/slb/slb_fake_quantizer.py

```diff
@@ -11,25 +11,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """SlbFakeQuantizer."""
 
 from functools import partial
+from typing import Union
+
 import numpy as np
 import mindspore
 import mindspore.context as context
 from mindspore.ops.operations import _quant_ops as Q
 from mindspore.common.parameter import Parameter
 from mindspore.common.tensor import Tensor
 from mindspore.ops import operations as P
-from mindspore._checkparam import Validator
+from mindspore.ops.operations._quant_ops import FakeQuantParam
 from mindspore.common.dtype import QuantDtype
-from ..fake_quantizer import FakeQuantizer
-from ..quant_utils import get_quant_min_max, cal_quantization_params, LinearFakeQuantCell
+from mindspore_gs.validator import Validator
+from mindspore_gs.quantization.fake_quantizer import FakeQuantizer, LinearFakeQuantizer
+from mindspore_gs.quantization.quant_utils import get_quant_min_max, cal_quantization_params
 
 
 class SlbFakeQuantizerPerLayer(FakeQuantizer):
     """
     Implement of SlbFakeQuantizer.
     1. Define weight_list and auxiliary coefficient matrix.
     2. Optimize auxiliary coefficient matrix.
@@ -49,20 +52,19 @@
         self.softmax = P.Softmax()
         self.sum = P.ReduceSum()
         self.assign = P.Assign()
         self.true_tensor = Tensor(1, mindspore.float32)
         self.false_tensor = Tensor(0, mindspore.float32)
 
         if self.num_bits == 1:
-            self.w_list = Parameter(Tensor([-1, 1], mindspore.float32).view(1, 1, 1, 1, -1),
-                                    name='w_list', requires_grad=False)
+            self.w_list_init = np.array([-1, 1])
+            self.w_list = Parameter(Tensor(self.w_list_init, mindspore.float32), name='w_list', requires_grad=False)
         else:
             self.w_list_init = np.linspace(-1, 1, 2**self.num_bits)
-            self.w_list = Parameter(Tensor(self.w_list_init, mindspore.float32).view(1, 1, 1, 1, -1),
-                                    name='w_list', requires_grad=False)
+            self.w_list = Parameter(Tensor(self.w_list_init, mindspore.float32), name='w_list', requires_grad=False)
 
         self.temperature = Parameter(Tensor([1], mindspore.float32),
                                      name="temperature", requires_grad=False)
         self.flag_temperature_end_changing = Parameter(self.false_tensor,
                                                        name="flag_temperature_end_changing", requires_grad=False)
 
     def set_temperature(self, t):
@@ -85,15 +87,15 @@
         self.assign(self.flag_temperature_end_changing, self.true_tensor)
 
     def construct(self, x):
         """
         SlbFakeQuantizer apply method.
         """
         is_training = self.training
-        if is_training == False:
+        if not is_training:
             # Compute one-hot representation of matrix A's argmax
             weights = self.onehot(self.argmax(x), x.shape[-1], self.true_tensor, self.false_tensor)
         else:
             is_temperature_end_changing = self.flag_temperature_end_changing
             if is_temperature_end_changing == 0:
                 # Compute matrix P of probabilities (as softmax of A*T)
                 weights = self.softmax(x * self.temperature)
@@ -106,16 +108,40 @@
         return out
 
     def extend_repr(self):
         """Display instance object as string."""
         s = 'bit_num={}'.format(self.num_bits)
         return s
 
+    def name(self) -> str:
+        return "SLBQuant"
+
+    def quant_dtype(self) -> QuantDtype:
+        if self.num_bits == 1:
+            return QuantDtype.INT1
+        if self.num_bits == 2:
+            return QuantDtype.INT2
+        if self.num_bits == 4:
+            return QuantDtype.INT4
+        raise ValueError("Only support 1,2,4 bit weight quantize for slb quantization now!"
+                         "Please set weight_quant_dtype in [QuantDtype.INT1, QuantDtype.INT2, QuantDtype.INT4] for "
+                         "SlbQuantAwareTraining.")
+
+    def is_per_channel(self) -> bool:
+        return False
+
+    def quant_params(self) -> dict:
+        scale_w = np.ones(1) * 2. ** (self.num_bits - 1)
+        zp_w = np.zeros(1)
+        return {FakeQuantParam.attr_key_linear_quant_scale: scale_w.tolist(),
+                FakeQuantParam.attr_key_linear_quant_zero_point: zp_w.tolist(),
+                "num_bits": self.num_bits}
+
 
-class SlbActQuantizer(FakeQuantizer):
+class SlbActQuantizer(LinearFakeQuantizer):
     """
     Implement of SlbActQuantizer.
     1. statistic the min max value passing through this op
     2. run fake quant execution to simulate the quantize loss
     """
 
     def __init__(self, ema=False, ema_decay=0.999, symmetric=False, narrow_range=False, num_bits=8, quant_delay=900):
@@ -167,24 +193,39 @@
         quant_min, quant_max = get_quant_min_max(num_bits=self._num_bits, signed=self._symmetric,
                                                  narrow_range=self._narrow_range)
         input_min = self._float_min.data.asnumpy()
         input_max = self._float_max.data.asnumpy()
         scale, zp = cal_quantization_params(input_min, input_max, quant_min, quant_max, symmetric=self._symmetric)
         return input_min, input_max, scale, zp
 
+    def mins(self) -> Union[list, tuple]:
+        return self._float_min.data.asnumpy().tolist()
+
+    def maxs(self) -> Union[list, tuple]:
+        return self._float_max.data.asnumpy().tolist()
+
+    def num_bits(self) -> int:
+        return self._num_bits
+
+    def narrow_range(self) -> bool:
+        return self._narrow_range
+
+    def symmetric(self) -> bool:
+        return self._symmetric
+
+    def quant_dtype(self) -> QuantDtype:
+        if self._num_bits != 8:
+            raise TypeError("Only support int8 feature quantize for slb quantization now!"
+                            "Please set act_quant_dtype=QuantDtype.INT8 for SlbQuantAwareTraining.")
+        return QuantDtype.INT8
+
+    def is_per_channel(self) -> bool:
+        return False
+
     def construct(self, x):
         if self.training:
             self._float_min, self._float_max = \
                 self._min_max_update_func(x, self._float_min, self._float_max)
             out = self._fake_quant_train(x, self._float_min, self._float_max)
         else:
             out = self._fake_quant_infer(x, self._float_min, self._float_max)
         return out
-
-    def convert_to_fakequantparam(self):
-        if self._num_bits != 8:
-            raise ValueError("Only support int8 activation quant now!")
-        quant_dtype = QuantDtype.INT8
-        _, _, scale, zero_point = self.extract_quant_param()
-        new_subcell = LinearFakeQuantCell(quant_dtype=quant_dtype, scale=tuple(scale), zero_point=tuple(zero_point),
-                                          is_per_channel=False)
-        return new_subcell
```

## mindspore_gs/quantization/slb/slb_layer_policy.py

```diff
@@ -10,96 +10,83 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """SlbLayerPolicy."""
 
+import abc
 from typing import Optional
-from functools import partial
 from mindspore.nn import Cell
-from mindspore_gs.ops.nn.fake_quant_with_min_max_observer import QuantConfig as OpQuantConfig
-from mindspore_gs.ops.common.quant_op_utils import get_quant_dtype_num_bits
-from ..layer_policy import LayerPolicy
-from ..quantize_wrapper_cell import QuantizeWrapperCell
-from ..fake_quantizer import FakeQuantizer
+from mindspore_gs.quantization.quant_utils import get_quant_dtype_num_bits
+from mindspore_gs.quantization.layer_policy import LayerPolicy, PerChannelArgs
+from mindspore_gs.quantization.fake_quantizer import FakeQuantizer
 from .slb_fake_quantizer import SlbFakeQuantizerPerLayer, SlbActQuantizer
 from .slb_quant import Conv2dSlbQuant
 from .slb_quant_config import SlbQuantConfig
 
 
-class SlbLayerPolicy(LayerPolicy):
+class SlbLayerPolicy(LayerPolicy, abc.ABC):
     """
     Derived class of LayerPolicy. slb layer policy.
     Use slb perlayer fake quantizer as weight fake quantizer, linear perlayer fake quantizer as act fake quantizer.
 
     Supported Config:
         ``quant_dtype``.
     """
 
     def __init__(self, weight_names: [], act_names: [], config: SlbQuantConfig = SlbQuantConfig()):
         super().__init__()
         self._config = config
-        weight_num_bits = get_quant_dtype_num_bits(config.weight_quant_dtype)
-        act_num_bits = get_quant_dtype_num_bits(config.act_quant_dtype)
-        if weight_num_bits not in [1, 2, 4]:
+        self.weight_num_bits = get_quant_dtype_num_bits(config.weight_quant_dtype)
+        self.act_num_bits = get_quant_dtype_num_bits(config.act_quant_dtype)
+        if self.weight_num_bits not in [1, 2, 4]:
             raise ValueError("Only support int4|int2|int1 weight quant now!")
-        if act_num_bits not in [8]:
+        if self.act_num_bits not in [8]:
             raise ValueError("Only support int8 activation quant now!")
-
-        self._weight_quantizer_partial = partial(SlbFakeQuantizerPerLayer, num_bits=weight_num_bits)
-        if config.enable_act_quant:
-            self._act_quantizer: Optional[FakeQuantizer] = SlbActQuantizer(num_bits=act_num_bits)
-            self._input_quantizer: Optional[FakeQuantizer] = SlbActQuantizer(num_bits=act_num_bits)
-            self._output_quantizer: Optional[FakeQuantizer] = SlbActQuantizer(num_bits=act_num_bits)
-        else:
-            self._act_quantizer: Optional[FakeQuantizer] = None
-            self._input_quantizer: Optional[FakeQuantizer] = None
-            self._output_quantizer: Optional[FakeQuantizer] = None
         self._weight_names = weight_names
         self._act_names = act_names
         self._input_num = 0
         self._inputs_insert_fq = []
 
-    def get_weight_name_and_quantizers(self):
-        return [(name, self._weight_quantizer_partial) for name in self._weight_names]
-
-    def get_act_name_and_quantizers(self):
-        return [(name, self._act_quantizer) for name in self._act_names]
+    def get_config(self) -> SlbQuantConfig:
+        return self._config
 
-    def get_input_quantizer(self) -> Optional[FakeQuantizer]:
-        return self._input_quantizer
-
-    def get_output_quantizer(self) -> Optional[FakeQuantizer]:
-        return self._output_quantizer
-
-    def set_input_number(self, input_num: int):
-        self._input_num = input_num
-        for _ in range(0, self._input_num):
-            self._inputs_insert_fq.append(True)
+    def get_weight_quantizer(self, weight_name="", perchannel_args: PerChannelArgs = PerChannelArgs(),
+                             **kwargs) -> FakeQuantizer:
+        return SlbFakeQuantizerPerLayer(num_bits=self.weight_num_bits)
+
+    def _get_input_quantizer(self, input_index=-1, perchannel_args: PerChannelArgs = PerChannelArgs(),
+                             **kwargs) -> FakeQuantizer:
+        if self._config.enable_act_quant:
+            return SlbActQuantizer(num_bits=self.act_num_bits)
+        return None
+
+    def _get_output_quantizer(self, perchannel_args: PerChannelArgs = PerChannelArgs(), **kwargs) -> FakeQuantizer:
+        if self._config.enable_act_quant:
+            return SlbActQuantizer(num_bits=self.act_num_bits)
+        return None
 
     def set_input_not_insert_fq(self, index: Optional[int] = None):
         if index is None:
             for i in range(0, self._input_num):
                 self._inputs_insert_fq[i] = False
         else:
             if index >= self._input_num:
                 raise RuntimeError("Index out of range of input number")
             self._inputs_insert_fq[index] = False
 
-    def get_input_need_insert_fq(self):
-        return self._inputs_insert_fq
-
-    def set_output_not_insert_fq(self, index: Optional[int] = None):
-        self._output_quantizer = None
-
-    def get_quant_config(self):
-        return OpQuantConfig(self._weight_quantizer_partial, self._act_quantizer)
-
+    @abc.abstractmethod
     def wrap_cell(self, handler: Cell) -> Cell:
-        return QuantizeWrapperCell(handler, self)
+        raise NotImplementedError
 
 
 class ConvLayerPolicy(SlbLayerPolicy):
+    """
+    Derived class of SlbLayerPolicy. LayerPolicy used for nn.Conv2d.
+    """
+    def __init__(self, weight_names: [], act_names: [], config: SlbQuantConfig = SlbQuantConfig()):
+        super().__init__(weight_names, act_names, config)
+        self.set_input_number(1)
+
     def wrap_cell(self, handler: Cell) -> Cell:
-        conv_quant = Conv2dSlbQuant.from_float(handler, self.get_quant_config(), self._config.weight_quant_dtype)
-        return QuantizeWrapperCell(conv_quant, self)
+        return Conv2dSlbQuant(handler, self, self._config.weight_quant_dtype)
```

## mindspore_gs/quantization/slb/slb_net_policy.py

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """SlbNetPolicy."""
 
 from mindspore.nn.layer import Conv2d
 from mindspore.rewrite import PatternEngine
-from ..net_policy import NetPolicy
+from mindspore_gs.quantization.net_policy import NetPolicy
 from .slb_layer_policy import ConvLayerPolicy
 from .slb_quant_config import SlbQuantConfig
 
 
 class SlbNetPolicy(NetPolicy):
     """
     Derived class of NetworkQConfig. slb network-quant-config.
```

## mindspore_gs/quantization/slb/slb_quant.py

```diff
@@ -10,34 +10,31 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """SlbQuant."""
 
-from functools import partial
+import numpy as np
 import mindspore
-from mindspore import nn
 from mindspore.common.parameter import Parameter
 from mindspore.ops import operations as P
 from mindspore.nn.layer.conv import Conv2d
 from mindspore.common.initializer import initializer
 from mindspore.common import initializer as init
-from mindspore._checkparam import Validator, twice
 from mindspore.common.dtype import QuantDtype
-from mindspore_gs.ops.nn.fake_quant_with_min_max_observer import QuantConfig as OpQuantConfig
-from mindspore_gs.ops.common.quant_op_utils import get_quant_dtype_num_bits
-from .slb_fake_quantizer import SlbFakeQuantizerPerLayer
+from mindspore.common.tensor import Tensor
+from mindspore.common import dtype as mstype
+from mindspore_gs.common import BackendTarget
+from mindspore_gs.quantization.quant_utils import get_quant_dtype_num_bits
+from mindspore_gs.quantization.quant_cell import QuantCell
+from mindspore_gs.quantization.layer_policy import LayerPolicy
 
 
-quant_config_slb_default = OpQuantConfig(weight=partial(SlbFakeQuantizerPerLayer, num_bits=1),
-                                         activation=None)
-
-
-class Conv2dSlbQuant(nn.Cell):
+class Conv2dSlbQuant(QuantCell):
     r"""
     2D convolution with fake quantized operation layer.
 
     This part is a more detailed overview of Conv2d operation. For more details about Quantization,
     please refer to the implementation of class of `SlbFakeQuantizerPerLayer`,
     :class:`mindspore_gs.quantization.slb.slb_fake_quantizer.SlbFakeQuantizerPerLayer`.
 
@@ -80,140 +77,106 @@
 
     Supported Platforms:
         ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> import mindspore
-        >>> from mindspore_gs.quantization.slb.slb_quant import Conv2dSlbQuant, quant_config_slb_default
+        >>> from mindspore_gs.quantization.slb.slb_quant import Conv2dSlbQuant
         >>> from mindspore import Tensor
-        >>> conv2d_quant = Conv2dSlbQuant(1, 1, kernel_size=(2, 2), stride=(1, 1), pad_mode="valid",
-        ...                               weight_init='ones', quant_config=quant_config_slb_default)
+        >>> conv2d_quant = Conv2dSlbQuant(1, 1, kernel_size=(2, 2), stride=(1, 1), pad_mode="valid", weight_init='ones')
         >>> x = Tensor(np.array([[[[1, 0, 3], [1, 4, 7], [2, 5, 2]]]]), mindspore.float32)
         >>> result = conv2d_quant(x)
         >>> print(result)
         [[[[-4.  -8.]
            [-2.  4.]]]]
     """
 
-    def __init__(self,
-                 in_channels,
-                 out_channels,
-                 kernel_size,
-                 stride=1,
-                 pad_mode='same',
-                 padding=0,
-                 dilation=1,
-                 group=1,
-                 has_bias=False,
-                 weight_init='normal',
-                 bias_init='zeros',
-                 quant_config=quant_config_slb_default,
-                 quant_dtype=QuantDtype.INT1):
+    def __init__(self, handler: Conv2d, policy: LayerPolicy, weight_quant_dtype=QuantDtype.INT1):
         """Initialize Conv2dSlbQuant."""
-        super(Conv2dSlbQuant, self).__init__()
-        self.in_channels = Validator.check_positive_int(in_channels, "in_channels", self.cls_name)
-        self.out_channels = Validator.check_positive_int(out_channels, "out_channels", self.cls_name)
-        self.has_bias = has_bias
-        self.kernel_size = twice(kernel_size)
-        self.stride = twice(stride)
-        self.dilation = twice(dilation)
-        for kernel_size_elem in self.kernel_size:
-            Validator.check_positive_int(kernel_size_elem, 'kernel_size item', self.cls_name)
-        for stride_elem in self.stride:
-            Validator.check_positive_int(stride_elem, 'stride item', self.cls_name)
-        for dilation_elem in self.dilation:
-            Validator.check_positive_int(dilation_elem, 'dilation item', self.cls_name)
-        if pad_mode not in ('valid', 'same', 'pad'):
-            raise ValueError(f"For '{self.cls_name}', the 'pad_mode' must be one of values "
-                             f"in ('valid', 'same', 'pad'), but got {pad_mode}.")
-        self.pad_mode = pad_mode
-        if isinstance(padding, int):
-            Validator.check_non_negative_int(padding, 'padding', self.cls_name)
-            self.padding = padding
-        elif isinstance(padding, tuple):
-            for pad in padding:
-                Validator.check_non_negative_int(pad, 'padding item', self.cls_name)
-            self.padding = padding
-        else:
-            raise TypeError(f"For '{self.cls_name}', the type of 'padding' must be int/tuple(int), "
-                            f"but got {type(padding).__name__}!")
-        self.group = Validator.check_positive_int(group, "group", self.cls_name)
-
-        self._num_bits = get_quant_dtype_num_bits(quant_dtype)
-        self._weight_num = 2**self._num_bits
+        super(Conv2dSlbQuant, self).__init__(handler, policy)
+        self.in_channels = handler.in_channels
+        self.out_channels = handler.out_channels
+        self.has_bias = handler.has_bias
+        self.kernel_size = handler.kernel_size
+        self.stride = handler.stride
+        self.dilation = handler.dilation
+        self.pad_mode = handler.pad_mode
+        self.padding = handler.padding
+        self.group = handler.group
 
         weight_init = init.HeNormal(mode='fan_out', nonlinearity='relu')
-        weight_shape = [out_channels, in_channels // group, *self.kernel_size, self._weight_num]
+        self._weight_num_bits = get_quant_dtype_num_bits(weight_quant_dtype)
+        self._weight_num = 2 ** self._weight_num_bits
+        weight_shape = [self.out_channels, self.in_channels // self.group, *self.kernel_size, self._weight_num]
         self.weight = Parameter(initializer(weight_init, weight_shape, mindspore.float32),
                                 name='weight', requires_grad=True)
 
-
-        self.bias_add = P.BiasAdd()
-        if Validator.check_bool(has_bias, "has_bias", self.cls_name):
-            self.bias = Parameter(initializer(bias_init, [out_channels]), name='bias')
-        else:
-            self.bias = None
+        if self.has_bias:
+            self.bias_add = P.BiasAdd()
+            self.bias = handler.bias
 
         self.conv = P.Conv2D(out_channel=self.out_channels,
                              kernel_size=self.kernel_size,
                              mode=1,
                              pad_mode=self.pad_mode,
                              pad=self.padding,
                              stride=self.stride,
                              dilation=self.dilation,
                              group=self.group)
 
-        self.fake_quant_weight = quant_config.weight()
+        self._weight_quantizer = policy.get_weight_quantizer(self.weight.name)
 
-    @classmethod
-    def from_float(cls, conv: Conv2d, quant_config: OpQuantConfig, weight_quant_dtype: QuantDtype):
-        """
-        A class method to create `Conv2dSlbQuant` from a `Conv2d`
-
-        Examples:
-            >>> from functools import partial
-            >>> from mindspore import nn
-            >>> from mindspore.nn.layer.quant import QuantConfig as OpQuantConfig
-            >>> from mindspore_gs.quantization.slb.slb_quant import Conv2dSlbQuant
-            >>> from mindspore_gs.quantization.slb.slb_fake_quantizer import SlbFakeQuantizerPerLayer
-            >>> from mindspore.common.dtype import QuantDtype
-            >>> ic = 10
-            >>> oc = 100
-            >>> kernel_size = 3
-            >>> conv_op = nn.Conv2d(ic, oc, kernel_size)
-            >>> # when apply QAT on `conv_op`, QAT need to create a quant conv2d whose weight is fake-quanted
-            >>> quant_config: OpQuantConfig = OpQuantConfig(weight=partial(SlbFakeQuantizerPerLayer, num_bits=1),
-            >>>                                             activation=None)
-            >>> weight_quant_dtype: QuantDtype = QuantDtype.INT1
-            >>> conv_quant = Conv2dSlbQuant.from_float(conv_op, quant_config, weight_quant_dtype)
-        """
-        conv_quant = cls(
-            conv.in_channels,
-            conv.out_channels,
-            kernel_size=conv.kernel_size,
-            stride=conv.stride,
-            pad_mode=conv.pad_mode,
-            padding=conv.padding,
-            dilation=conv.dilation,
-            group=conv.group,
-            has_bias=conv.has_bias,
-            bias_init=conv.bias_init,
-            weight_init=conv.weight_init,
-            quant_config=quant_config,
-            quant_dtype=weight_quant_dtype)
-        return conv_quant
+    def weight_quantizer(self):
+        return self._weight_quantizer
 
-    def construct(self, x):
-        weight = self.fake_quant_weight(self.weight)
+    def __convert_weight5d_to_weight4d(self, conv2dquant_weights5d):
+        """Convert slb 5d weight to normal 4d weight"""
+        argmax = P.Argmax()
+        onehot = P.OneHot()
+        reduce_sum = P.ReduceSum()
+        true_tensor = Tensor(1, mstype.float32)
+        false_tensor = Tensor(0, mstype.float32)
+        num_bits = self._weight_num_bits
+
+        if num_bits == 1:
+            w_list = Parameter(Tensor([-1, 1], mstype.float32).view(1, 1, 1, 1, -1),
+                               name='w_list', requires_grad=False)
+        else:
+            w_list_init = np.linspace(-1, 1, 2**num_bits)
+            w_list = Parameter(Tensor(w_list_init, mstype.float32).view(1, 1, 1, 1, -1),
+                               name='w_list', requires_grad=False)
+
+        # Convert 5d weight to 4d weight
+        # Compute one-hot representation of matrix A's argmax
+        onehot_weights5d = onehot(argmax(conv2dquant_weights5d), conv2dquant_weights5d.shape[-1],
+                                  true_tensor, false_tensor)
+        # Compute continuous weights
+        weights_5d = onehot_weights5d * w_list
+        weights_4d = reduce_sum(weights_5d, -1)
+        return weights_4d
+
+    def convert(self, backend: BackendTarget = BackendTarget.NONE, is_deploy=False):
+        if self._converted:
+            return
+        if backend is not BackendTarget.NONE:
+            raise ValueError("Only support convert to MS Backend now, got: ", backend)
+        super(Conv2dSlbQuant, self).convert(backend, is_deploy)
+        self._weight_quantizer = self._weight_quantizer.convert_to_fakequantparam()
+        weight_tensor = self.__convert_weight5d_to_weight4d(self.weight)
+        self.weight = Parameter(weight_tensor, name=f"{self.weight.name}_4d")
+
+    # pylint: disable=arguments-differ
+    def core_construct(self, x):
+        weight = self._weight_quantizer(self.weight)
         out = self.conv(x, weight)
         if self.has_bias:
             return self.bias_add(out, self.bias)
         return out
 
     def extend_repr(self):
         """Display instance object as string."""
         s = 'in_channels={}, out_channels={}, kernel_size={}, weight_bit_num={}, stride={}, ' \
             'pad_mode={}, padding={}, dilation={}, group={}, ' \
-            'has_bias={}'.format(self.in_channels, self.out_channels, self.kernel_size, self._num_bits, self.stride,
-                                 self.pad_mode, self.padding, self.dilation, self.group, self.has_bias)
+            'has_bias={}'.format(self.in_channels, self.out_channels, self.kernel_size, self._weight_num_bits,
+                                 self.stride, self.pad_mode, self.padding, self.dilation, self.group, self.has_bias)
         return s
```

## mindspore_gs/quantization/slb/slb_quant_aware_training.py

```diff
@@ -16,18 +16,18 @@
 
 import os
 from mindspore.dataset import Dataset
 from mindspore import Model
 from mindspore.nn import Cell
 from mindspore.train.callback import Callback
 from mindspore.train.serialization import load_checkpoint, load_param_into_net
-from mindspore._checkparam import Validator, Rel
 from mindspore.common.dtype import QuantDtype
-from mindspore_gs.ops.common.quant_op_utils import get_quant_dtype_num_bits
-from ..quantization_aware_training import QuantizationAwareTraining
+from mindspore_gs.quantization.quant_utils import get_quant_dtype_num_bits
+from mindspore_gs.validator import Validator, Rel
+from mindspore_gs.quantization.quantization_aware_training import QuantizationAwareTraining
 from .slb_net_policy import SlbNetPolicy
 from .slb_quant_config import SlbQuantConfig
 from .slb_quant_convert import ConvertToQuantInferNetwork
 
 
 class SlbQuantAwareTraining(QuantizationAwareTraining):
     """
@@ -41,36 +41,36 @@
 
     Note:
         This method will call other set functions to set special values, please refer to the set function about the error.
         For example, `quant_dtype` need refer to `set_weight_quant_dtype` and `set_act_quant_dtype`.
 
     Args:
         config (dict): store attributes for quantization aware training, keys are attribute names,
-            values are attribute values. Default: None. Supported attribute are listed below:
+            values are attribute values. Default: ``None``. Supported attribute are listed below:
 
             - quant_dtype (Union[QuantDtype, list(QuantDtype), tuple(QuantDtype)]): Datatype used to quantize weights and
               activations. The type is a QuantDtype, a list of two QuantDtype or a tuple of two QuantDtype. If quant_dtype is a
               QuantDtype, it will be duplicated to a list of two QuantDtype. The first element represents the type of activations
               and the second element represents the type of weights. It is necessary to consider the precision support of
               hardware devices in the practical quantization infer scenaries. Weights quantization support int4|int2|int1,
               and activations quantization support int8 now.
-              Default: (QuantDtype.INT8, QuantDtype.INT1).
+              Default: ``(QuantDtype.INT8, QuantDtype.INT1)``.
             - enable_act_quant (bool): Whether apply activation quantization while training.
-              Default: False.
+              Default: ``False``.
             - enable_bn_calibration (bool): Whether apply batchnorm calibration while training.
-              Default: False.
+              Default: ``False``.
             - epoch_size (int): Total training epochs.
             - has_trained_epoch (int): The trained epochs.
-            - t_start_val (float): Initial value of temperature hyperparameters. Default: 1.
+            - t_start_val (float): Initial value of temperature hyperparameters. Default: ``1``.
             - t_start_time (float): Fraction of epochs after which temperature hyperparameters starting changing.
-              Default: 0.2.
+              Default: ``0.2``.
             - t_end_time (float): Fraction of epochs after which temperature hyperparameters stopping changing.
-              Default: 0.6.
+              Default: ``0.6``.
             - t_factor (float): Multiplicative factor of temperature hyperparameters changing.
-              Default: 1.2.
+              Default: ``1.2``.
 
     Raises:
         TypeError: If `quant_dtype` is not `QuantDtype`, or every element of `quant_dtype` is not `QuantDtype`.
         TypeError: If `enable_act_quant` or `enable_bn_calibration` is not bool.
         ValueError: If the length of `quant_dtype` is greater than 2.
         TypeError: If `epoch_size` or `has_trained_epoch` is not an int.
         TypeError: If `t_start_val`, `t_start_time`, `t_end_time` or `t_factor` is not float.
@@ -147,15 +147,15 @@
         >>> print(net_qat)
         NetToQuantOpt<
           (_handler): NetToQuant<
             (conv): Conv2d<input_channels=1, output_channels=6, kernel_size=(5, 5), stride=(1, 1), pad_mode=valid, padding=0, dilation=(1, 1), group=1, has_bias=False, weight_init=normal, bias_init=zeros, format=NCHW>
             (bn): BatchNorm2d<num_features=6, eps=1e-05, momentum=0.9, gamma=Parameter(name=bn.gamma, requires_grad=True, shape=[6], dtype=Float32, value= [1., 1., 1., 1., 1., 1.]), beta=Parameter(name=bn.beta, requires_grad=True, shape=[6], dtype=Float32, value= [0., 0., 0., 0., 0., 0.]), moving_mean=Parameter(name=bn.moving_mean, requires_grad=False, shape=[6], dtype=Float32, value= [0., 0., 0., 0., 0., 0.]), moving_variance=Parameter(name=bn.moving_variance, requires_grad=False, shape=[6], dtype=Float32, value= [1., 1., 1., 1., 1., 1.])>
             >
           (bn): BatchNorm2d<num_features=6, eps=1e-05, momentum=0.9, gamma=Parameter(name=bn.gamma, requires_grad=True, shape=[6], dtype=Float32, value= [1., 1., 1., 1., 1., 1.]), beta=Parameter(name=bn.beta, requires_grad=True, shape=[6], dtype=Float32, value= [0., 0., 0., 0., 0., 0.]), moving_mean=Parameter(name=bn.moving_mean, requires_grad=False, shape=[6], dtype=Float32, value= [0., 0., 0., 0., 0., 0.]), moving_variance=Parameter(name=bn.moving_variance, requires_grad=False, shape=[6], dtype=Float32, value= [1., 1., 1., 1., 1., 1.])>
-          (Conv2dSlbQuant): QuantizeWrapperCell<
+          (Conv2dSlbQuant): QuantCell<
             (_handler): Conv2dSlbQuant<
               in_channels=1, out_channels=6, kernel_size=(5, 5), weight_bit_num=1, stride=(1, 1), pad_mode=valid, padding=0, dilation=(1, 1), group=1, has_bias=False
               (fake_quant_weight): SlbFakeQuantizerPerLayer<bit_num=1>
               >
             (_input_quantizer): SlbActQuantizer<bit_num=8, symmetric=False, narrow_range=False, ema=False(0.999), per_channel=False, quant_delay=900>
             (_output_quantizer): SlbActQuantizer<bit_num=8, symmetric=False, narrow_range=False, ema=False(0.999), per_channel=False, quant_delay=900>
             >
@@ -182,66 +182,66 @@
             self._custom_layer_policy_map = config["custom_policies"]
 
     def set_weight_quant_dtype(self, weight_quant_dtype=QuantDtype.INT1):
         """
         Set value of weight_quant_dtype of quantization aware training `config`
 
         Args:
-            weight_quant_dtype (QuantDtype): Datatype used to quantize weights. Default: QuantDtype.INT1.
+            weight_quant_dtype (QuantDtype): Datatype used to quantize weights. Default: ``QuantDtype.INT1``.
 
         Raises:
             TypeError: If `weight_quant_dtype` is not QuantDtype.
-            ValueError: Only supported if `weight_quant_dtype` is `QuantDtype.INT1`, `QuantDtype.INT2`
-                or `QuantDtype.INT4` yet.
+            ValueError: Only supported if `weight_quant_dtype` is ``QuantDtype.INT1``, ``QuantDtype.INT2``
+                or ``QuantDtype.INT4`` yet.
         """
         if not isinstance(weight_quant_dtype, QuantDtype):
             raise TypeError("The parameter `weight quant dtype` must be isinstance of QuantDtype, "
                             "but got {}.".format(weight_quant_dtype))
         if weight_quant_dtype not in [QuantDtype.INT1, QuantDtype.INT2, QuantDtype.INT4]:
             raise ValueError("Only supported if `weight_quant_dtype` is `QuantDtype.INT1`, " \
                              "`QuantDtype.INT2` or `QuantDtype.INT4` yet.")
         self._config.weight_quant_dtype = weight_quant_dtype
 
     def set_act_quant_dtype(self, act_quant_dtype=QuantDtype.INT8):
         """
         Set value of act_quant_dtype of quantization aware training `config`
 
         Args:
-            act_quant_dtype (QuantDtype): Datatype used to quantize activations. Default: QuantDtype.INT8.
+            act_quant_dtype (QuantDtype): Datatype used to quantize activations. Default: ``QuantDtype.INT8``.
 
         Raises:
             TypeError: If `act_quant_dtype` is not QuantDtype.
-            ValueError: Only supported if `act_quant_dtype` is `QuantDtype.INT8` yet.
+            ValueError: Only supported if `act_quant_dtype` is ``QuantDtype.INT8`` yet.
         """
         if not isinstance(act_quant_dtype, QuantDtype):
             raise TypeError("The parameter `act quant dtype` must be isinstance of QuantDtype, "
                             "but got {}.".format(act_quant_dtype))
         if act_quant_dtype not in [QuantDtype.INT8]:
             raise ValueError("Only supported if `act_quant_dtype` is `QuantDtype.INT8` yet.")
         self._config.act_quant_dtype = act_quant_dtype
 
     def set_enable_act_quant(self, enable_act_quant=False):
         """
         Set value of enable_act_quant of quantization aware training `config`
 
         Args:
-            enable_act_quant (bool): Whether apply activation quantization while training, default is False.
+            enable_act_quant (bool): Whether apply activation quantization while training, default is ``False``.
 
         Raises:
             TypeError: If `enable_act_quant` is not bool.
         """
         enable_act_quant = Validator.check_bool(enable_act_quant, "enable_act_quant", self.__class__.__name__)
         self._config.enable_act_quant = enable_act_quant
 
     def set_enable_bn_calibration(self, enable_bn_calibration=False):
         """
         Set value of enable_bn_calibration of quantization aware training `config`
 
         Args:
-            enable_bn_calibration (bool): Whether apply batchnorm calibration while training, default is False.
+            enable_bn_calibration (bool): Whether apply batchnorm calibration while training, default is ``False``.
 
         Raises:
             TypeError: If `enable_bn_calibration` is not bool.
         """
         enable_bn_calibration = Validator.check_bool(enable_bn_calibration, "enable_bn_calibration",
                                                      self.__class__.__name__)
         self._config.enable_bn_calibration = enable_bn_calibration
@@ -273,62 +273,64 @@
         """
         has_trained_epoch = Validator.check_int(has_trained_epoch, 0, Rel.GE, "has_trained_epoch",
                                                 self.__class__.__name__)
         self._config.has_trained_epoch = has_trained_epoch
 
     def set_t_start_val(self, t_start_val=1.0):
         """
-        Set value of t_start_val of quantization aware training `config`
+        Set value of t_start_val of quantization aware training `config`.
 
         Args:
-            t_start_val (float): Initial value of temperature hyperparameters, default: 1.0.
+            t_start_val (float): Initial value of temperature hyperparameters, default: ``1.0``.
 
         Raises:
             TypeError: If `t_start_val` is not float.
             ValueError: If `t_start_val` is not greater than 0.
         """
         t_start_val = Validator.check_positive_float(t_start_val, "t_start_val", self.__class__.__name__)
         self._config.t_start_val = t_start_val
 
     def set_t_start_time(self, t_start_time=0.2):
         """
-        Set value of t_start_time of quantization aware training `config`
+        Set value of t_start_time of quantization aware training `config`.
 
         Args:
-            t_start_time (float): Fraction of epochs after which temperature hyperparameters starting changing, default: 0.2.
+            t_start_time (float): Fraction of epochs after which temperature hyperparameters starting changing,
+                default: ``0.2``.
 
         Raises:
             TypeError: If `t_start_time` is not float.
             ValueError: If `t_start_time` is less than 0. or greater than 1.
         """
         t_start_time = Validator.check_float_range(t_start_time, 0.0, 1.0, Rel.INC_BOTH, \
                                                    "t_start_time", self.__class__.__name__)
         self._config.t_start_time = t_start_time
 
     def set_t_end_time(self, t_end_time=0.6):
         """
         Set value of t_end_time of quantization aware training `config`
 
         Args:
-            t_end_time (float): Fraction of epochs after which temperature hyperparameters stopping changing, default: 0.6.
+            t_end_time (float): Fraction of epochs after which temperature hyperparameters stopping changing,
+                default: ``0.6``.
 
         Raises:
             TypeError: If `t_end_time` is not float.
             ValueError: If `t_end_time` is less than 0. or greater than 1.
         """
         t_end_time = Validator.check_float_range(t_end_time, 0.0, 1.0, Rel.INC_BOTH,
                                                  "t_end_time", self.__class__.__name__)
         self._config.t_end_time = t_end_time
 
     def set_t_factor(self, t_factor=1.2):
         """
         Set value of t_factor of quantization aware training `config`
 
         Args:
-            t_factor (float): Multiplicative factor of temperature hyperparameters changing, default: 1.2.
+            t_factor (float): Multiplicative factor of temperature hyperparameters changing, default: ``1.2``.
 
         Raises:
             TypeError: If `t_factor` is not float.
             ValueError: If `t_factor` is not greater than 0.
         """
         t_factor = Validator.check_positive_float(t_factor, "t_factor", self.__class__.__name__)
         self._config.t_factor = t_factor
@@ -377,19 +379,19 @@
             model (Model): Model to be used.
             dataset (Dataset): Dataset to be used.
 
         Returns:
             List of instance of Callbacks.
 
         Raises:
-            RuntimeError: If `epoch_size` is not initialized!
-            RuntimeError: If `has_trained_epoch` is not initialized!
+            RuntimeError: If `epoch_size` is not initialized.
+            RuntimeError: If `has_trained_epoch` is not initialized.
             ValueError: If `epoch_size` is not greater than `has_trained_epoch`.
             ValueError: If `t_end_time` is less than `t_start_time`.
-            TypeError: If `model` is not mindspore.Model.
+            TypeError: If `model` is not `mindspore.train.Model`.
             TypeError: If `dataset` is not mindspore.dataset.Dataset.
         """
 
         if self._config.epoch_size == -1:
             raise RuntimeError("The `epoch_size` need to be initialized!")
         if self._config.has_trained_epoch == -1:
             raise RuntimeError("The `has_trained_epoch` need to be initialized!")
@@ -422,15 +424,15 @@
         """
         Apply SLB quantization Algorithm on `network`, use the following steps to make `network` available for
         quantization aware training:
 
         1. Fuse certain cells in `network` using pattern engine which is defined by net policy.
         2. Propagate layer policies defined through cells.
         3. Reduce redundant fake quantizers when they are redundant.
-        4. Apply layer policies to convert normal cell to `QuantizeWrapperCell`.
+        4. Apply layer policies to convert normal cell to `QuantCell`.
 
         Args:
             network (Cell): Network to be quantized.
 
         Returns:
             Quantized network.
         """
@@ -440,43 +442,42 @@
 
     def convert(self, net_opt: Cell, ckpt_path="") -> Cell:
         """
         Define how to convert a compressed network to a standard network before exporting to MindIR.
 
         Args:
             net_opt (Cell): Network to be converted which is transformed by `SlbQuantAwareTraining.apply`.
-            ckpt_path (str): Path to checkpoint file for `net_opt`. Default is a empty string which means not loading
+            ckpt_path (str): Path to checkpoint file for `net_opt`. Default is ``""``, which means not loading
                 checkpoint file to `net_opt`.
 
         Returns:
             An instance of Cell represents converted network.
 
         Raises:
             TypeError: If `net_opt` is not Cell.
             TypeError: If `ckpt_path` is not string.
             ValueError: If `ckpt_path` is not empty and invalid.
-            RuntimeError: If `ckpt_path` is a valid file and load checkpoint file failed.
+            RuntimeError: If loading `ckpt_path` fails.
         """
-
         if not isinstance(net_opt, Cell):
             raise TypeError(f'The parameter `net_opt` must be isinstance of Cell, but got {type(net_opt)}.')
         if not isinstance(ckpt_path, str):
             raise TypeError(f'The parameter `ckpt_path` must be isinstance of str, but got {type(ckpt_path)}.')
         if ckpt_path != "" and not os.path.isfile(ckpt_path):
-            raise ValueError(
-                f'The parameter `ckpt_path` can only be empty or a valid file, but got {os.path.realpath(ckpt_path)}.')
+            raise ValueError(f'The parameter `ckpt_path` can only be empty or a valid file, but got {os.path.realpath(ckpt_path)}.')
         ckpt_path = os.path.realpath(ckpt_path)
         if os.path.isfile(ckpt_path):
             param_dict = load_checkpoint(ckpt_path)
             not_load_param = load_param_into_net(net_opt, param_dict)
-            if not_load_param:
+            if not_load_param[0]:
                 raise RuntimeError("Load param into net fail.")
         exporter = ConvertToQuantInferNetwork(net_opt, get_quant_dtype_num_bits(self._config.weight_quant_dtype))
         return exporter.run()
 
+
     def __repr__(self):
         """Display instance object as string."""
         s = 'SlbQuantAwareTraining<weight_quant_dtype={}, act_quant_dtype={}, enable_act_quant={}, ' \
             'enable_bn_calibration={}, epoch_size={}, has_trained_epoch={}, t_start_val={}, t_start_time={}, ' \
             't_end_time={}, t_factor={}>'.format(self._config.weight_quant_dtype, self._config.act_quant_dtype,
                                                  self._config.enable_act_quant, self._config.enable_bn_calibration,
                                                  self._config.epoch_size, self._config.has_trained_epoch,
```

## mindspore_gs/quantization/slb/slb_quant_config.py

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """Config for aware-training-quantization."""
 
 from mindspore.common.dtype import QuantDtype
-from ...comp_algo import CompAlgoConfig
+from mindspore_gs.comp_algo import CompAlgoConfig
 
 
 class SlbQuantConfig(CompAlgoConfig):
     """
     Config for SLB(Searching for Low-Bit Weights) QAT-algorithm.
     See more details in slb_quant_aware_training.py
     """
```

## mindspore_gs/quantization/slb/slb_quant_convert.py

```diff
@@ -10,84 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """SlbQuantConvert."""
 
-import numpy as np
-from mindspore.nn import Cell
-from mindspore.common.parameter import Parameter
-from mindspore.common.tensor import Tensor
-from mindspore.ops import operations as P
-from mindspore.ops.operations import _quant_ops as Q
-from mindspore.common import dtype as mstype
 from mindspore.common.dtype import QuantDtype
-from ..quantize_wrapper_cell import QuantizeWrapperCell
-from .slb_quant import Conv2dSlbQuant
-
-
-class CellBlockWithFakeWeight(Cell):
-    """A block of Conv, activation layer with fake quantization weight for export MINDIR model.
-
-       Args:
-        core_op (Cell): The operation cell.
-        scale_w (tuple): The quantization parameter scale of the weight.
-        zp_w (tuple): The quantization parameter zero point of the weight.
-        weight (Tensor): The weight of the cell.
-        bias (Tensor): The bias of the cell. Default: None.
-        activation (str): The regularization function applied to the output of the layer, eg. 'relu'. Default: None.
-        param_dict (dict): The information of the cell.
-    """
-
-    def __init__(self,
-                 core_op,
-                 scale_w,
-                 zp_w,
-                 weight,
-                 bias=None,
-                 activation=None,
-                 param_dict=None):
-
-        super(CellBlockWithFakeWeight, self).__init__()
-        self.core_op = core_op
-        if activation is not None:
-            self.core_op.add_prim_attr(
-                "activation_name", activation.__class__.__name__)
-        if hasattr(core_op, 'pad_mode'):
-            self.core_op.add_prim_attr("pad_mode", core_op.pad_mode)
-
-        self.weight = weight
-        self.bias = bias
-        self.has_bias = bias is not None
-        self.activation = activation
-        self.has_act = activation is not None
-        self.bias_add = P.BiasAdd()
-        self.fake_weight = Q.FakeQuantParam.linear_quant_param(quant_dtype=param_dict["quant_dtype"],
-                                                               scale=scale_w, zp=zp_w,
-                                                               is_per_channel=param_dict["is_per_channel"])
-
-    def construct(self, x):
-        weight = self.fake_weight(self.weight)
-        if self.has_bias:
-            x = self.core_op(x, weight)
-            x = self.bias_add(x, self.bias)
-        else:
-            x = self.core_op(x, weight)
-        if self.has_act:
-            x = self.activation(x)
-        return x
-
-    def extend_repr(self):
-        s = f'core_op={type(self.core_op)}, weight=shape[{self.weight.shape}]'
-        if self.has_bias:
-            s += f', bias=shape[{self.bias.shape}]'
-        if self.has_act:
-            s += f', activation={self.activation}'
-        return s
+from ..quant_cell import QuantCell
 
 
 class ConvertToQuantInferNetwork:
     """
     Convert quantization aware network to infer network.
 
     Args:
@@ -110,102 +42,19 @@
         self.network = network
 
     def run(self):
         """Start to convert."""
         self.network.update_cell_prefix()
         return self._convert_quant2deploy(self.network)
 
-    def _get_quant_block(self, cell_core):
-        """convert network's quant subcell to deploy subcell"""
-        scale_w, zp_w = self.__get_quant_param()
-        activation = None
-
-        # get op
-        op_core = cell_core.conv
-
-        # get the `weight` and `bias`
-        weight, bias = self.__get_weight_bias(cell_core)
-        quant_params = {"quant_dtype": self.quant_dtype,
-                        "is_per_channel": False}
-        block = CellBlockWithFakeWeight(op_core, tuple(scale_w), tuple(
-            zp_w), weight, bias, activation, quant_params)
-        return block
-
-    def __get_quant_param(self,):
-        """Get scale and bias for fake quant weight"""
-        scale_w = np.ones(1) * 2. ** (self.weight_quant_bit - 1)
-        zp_w = np.zeros(1)
-        return scale_w, zp_w
-
-    def __convert_weight5d_to_weight4d(self, cell_core):
-        """Convert slb 5d weight to normal 4d weight"""
-        argmax = P.Argmax()
-        onehot = P.OneHot()
-        reduce_sum = P.ReduceSum()
-        true_tensor = Tensor(1, mstype.float32)
-        false_tensor = Tensor(0, mstype.float32)
-        num_bits = self.weight_quant_bit
-
-        if num_bits == 1:
-            w_list = Parameter(Tensor([-1, 1], mstype.float32).view(1, 1, 1, 1, -1),
-                               name='w_list', requires_grad=False)
-        else:
-            w_list_init = np.linspace(-1, 1, 2**num_bits)
-            w_list = Parameter(Tensor(w_list_init, mstype.float32).view(1, 1, 1, 1, -1),
-                               name='w_list', requires_grad=False)
-
-        # Convert 5d weight to 4d weight
-        conv2dquant_weights5d = cell_core.weight
-        # Compute one-hot representation of matrix A's argmax
-        onehot_weights5d = onehot(argmax(conv2dquant_weights5d), conv2dquant_weights5d.shape[-1],
-                                  true_tensor, false_tensor)
-        # Compute continuous weights
-        weights_5d = onehot_weights5d * w_list
-        weights_4d = reduce_sum(weights_5d, -1)
-        return weights_4d
-
-    def __get_weight_bias(self, cell_core):
-        """Get weight and bias for quantizaiton"""
-        weight_tensor = self.__convert_weight5d_to_weight4d(cell_core)
-        bias = None
-        if isinstance(cell_core, Conv2dSlbQuant):
-            if cell_core.has_bias:
-                bias = cell_core.bias.data.asnumpy()
-
-        if bias is not None:
-            bias_tensor = Tensor(bias, mstype.float32)
-            return weight_tensor, bias_tensor
-        return weight_tensor, None
-
-    def _convert_subcell(self, cell_core):
-        """Convert subcell to ant subcell."""
-        if cell_core is not None and hasattr(cell_core, "fake_quant_weight"):
-            new_subcell = self._get_quant_block(cell_core)
-            return new_subcell
-        return None
-
-    def _convert_core_quant_subcell(self, cell_core):
-        """Convert subcell for conv and dense."""
-        if isinstance(cell_core, (Conv2dSlbQuant)):
-            return self._convert_subcell(cell_core)
-        raise ValueError("Unsupported quant cell.")
-
     def _convert_quant2deploy(self, network):
         """Convert network's all quant subcell to deploy subcell."""
         cells = network.name_cells()
         for name in cells:
             subcell = cells[name]
             if subcell == network:
                 continue
-            if isinstance(subcell, QuantizeWrapperCell):
-                quant_cell = subcell.get_handler()
-                new_subcell = self._convert_core_quant_subcell(quant_cell)
-                subcell.insert_child_to_cell("_handler", new_subcell)
-                if subcell.get_input_quantizer() is not None:
-                    fake_quant_input = subcell.get_input_quantizer().convert_to_fakequantparam()
-                    subcell.insert_child_to_cell("_input_quantizer", fake_quant_input)
-                if subcell.get_output_quantizer() is not None:
-                    fake_quant_output = subcell.get_output_quantizer().convert_to_fakequantparam()
-                    subcell.insert_child_to_cell("_output_quantizer", fake_quant_output)
+            if isinstance(subcell, QuantCell):
+                subcell.convert()
             else:
                 self._convert_quant2deploy(subcell)
         return network
```

## Comparing `mindspore_gs/ops/common/quant_op_utils.py` & `mindspore_gs/ptq/round_to_nearest/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,19 @@
-# Copyright 2022 Huawei Technologies Co., Ltd
+# Copyright 2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
-"""Quantization utils."""
+"""
+MindSpore golden stick MinMaxPTQ Algorithm.
+"""
 
-from mindspore.common.dtype import QuantDtype
-
-
-def get_quant_dtype_num_bits(quant_dtype: QuantDtype):
-    if 0 <= quant_dtype.value() <= 15:
-        return quant_dtype.value() + 1
-    if 100 <= quant_dtype.value() <= 115:
-        return quant_dtype.value() - 99
-    raise ValueError("Unsupported QuantDtype.")
+from .round_to_nearest import RoundToNearest
```

## Comparing `mindspore_gs/ops/kernel/gpu/fake_quant_impl.cuh` & `mindspore_gs/quantization/ops/kernel/gpu/fake_quant_impl.cuh`

 * *Files identical despite different names*

## Comparing `mindspore_gs/ops/kernel/gpu/fake_quant_per_channel_grad_impl.cu` & `mindspore_gs/quantization/ops/kernel/gpu/fake_quant_per_channel_grad_impl.cu`

 * *Files identical despite different names*

## Comparing `mindspore_gs/ops/kernel/gpu/fake_quant_per_channel_impl.cu` & `mindspore_gs/quantization/ops/kernel/gpu/fake_quant_per_channel_impl.cu`

 * *Files identical despite different names*

## Comparing `mindspore_gs/ops/kernel/gpu/fake_quant_per_layer_grad_impl.cu` & `mindspore_gs/quantization/ops/kernel/gpu/fake_quant_per_layer_grad_impl.cu`

 * *Files identical despite different names*

## Comparing `mindspore_gs/ops/kernel/gpu/fake_quant_per_layer_impl.cu` & `mindspore_gs/quantization/ops/kernel/gpu/fake_quant_per_layer_impl.cu`

 * *Files identical despite different names*

## Comparing `mindspore_gs/ops/kernel/gpu/min_max_update_per_channel_impl.cu` & `mindspore_gs/quantization/ops/kernel/gpu/min_max_update_per_channel_impl.cu`

 * *Files identical despite different names*

## Comparing `mindspore_gs/ops/kernel/gpu/min_max_update_per_layer_impl.cu` & `mindspore_gs/quantization/ops/kernel/gpu/min_max_update_per_layer_impl.cu`

 * *Files identical despite different names*

## Comparing `mindspore_gs/ops/kernel/gpu/aot/custom_aot_extra.h` & `mindspore_gs/quantization/ops/kernel/gpu/aot/custom_aot_extra.h`

 * *Files identical despite different names*

## Comparing `mindspore_gs/ops/nn/__init__.py` & `mindspore_gs/quantization/ops/nn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from .conv2d_bn_fold_quant_one_conv import Conv2dBnFoldQuantOneConv
 from .conv2d_quant import Conv2dQuant
 from .dense_quant import DenseQuant
 from .fake_quant_with_min_max_observer import FakeQuantWithMinMaxObserver
 from .mul_quant import MulQuant
 from .tensor_add_quant import TensorAddQuant
 
-
 __all__ = [
     'FakeQuantWithMinMaxObserver',
     'Conv2dBnFoldQuantOneConv',
     'Conv2dBnFoldQuant',
     'Conv2dBnWithoutFoldQuant',
     'Conv2dQuant',
     'DenseQuant',
```

## Comparing `mindspore_gs/ops/nn/batchnorm_fold_cell.py` & `mindspore_gs/quantization/ops/nn/batchnorm_fold_cell.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """BatchNormFoldCell."""
 from __future__ import absolute_import
 
-from mindspore.ops import operations as P
 import mindspore.context as context
+from mindspore.ops import operations as P
 from mindspore.nn.cell import Cell
 from mindspore.ops.operations import _quant_ops as Q
 
 
 class BatchNormFoldCell(Cell):
     """
     Batch Normalization folded.
```

## Comparing `mindspore_gs/ops/nn/conv2d_bn_fold_quant.py` & `mindspore_gs/quantization/ops/nn/conv2d_bn_fold_quant_one_conv.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,64 +8,64 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
-"""Conv2dBnFoldQuant."""
+"""Conv2dBnFoldQuantOneConv."""
 from __future__ import absolute_import
 
+import mindspore.context as context
 import mindspore.common.dtype as mstype
+from mindspore import Tensor
 from mindspore.ops import operations as P
 from mindspore.common.parameter import Parameter
-from mindspore.common.initializer import initializer
-from mindspore.common.tensor import Tensor
-from mindspore._checkparam import Validator, twice
 from mindspore.common.dtype import QuantDtype
-import mindspore.context as context
-from mindspore.nn.cell import Cell
-from mindspore.ops.operations import _quant_ops as Q
-from ...quantization.simulated_quantization.combined import Conv2dBn
-from .fake_quant_with_min_max_observer import quant_config_default, QuantConfig
-from .batchnorm_fold_cell import BatchNormFoldCell
+from mindspore_gs.common import BackendTarget
+from mindspore_gs.validator import Validator
+from mindspore_gs.quantization.simulated_quantization.combined import Conv2dBn
+from mindspore_gs.quantization.quant_cell import QuantCell
+from mindspore_gs.quantization.layer_policy import LayerPolicy, PerChannelArgs
+from mindspore_gs.quantization.quant_utils import fold_batchnorm
 
 
-class Conv2dBnFoldQuant(Cell):
+class Conv2dBnFoldQuantOneConv(QuantCell):
     r"""
-    2D convolution with Batch Normalization operation folded construct.
+    2D convolution which use the convolution layer statistics once to calculate Batch Normalization
+    operation folded construct.
 
     This part is a more detailed overview of Conv2d operation. For more details about Quantization,
     please refer to the implementation of class of `FakeQuantWithMinMaxObserver`,
     :class:`FakeQuantWithMinMaxObserver`.
 
     .. math::
-        y = x\times w+  b
+        w_{q}=quant(\frac{w}{\sqrt{var_{G}+\epsilon}}*\gamma )
 
-        w_{q}=quant(\frac{w}{\sqrt{Var[y]+\epsilon}}*\gamma )
+        b=\frac{-\mu _{G} }{\sqrt{var_{G}+\epsilon }}*\gamma +\beta
 
-        y_{out}= w_{q}\times x+\frac{b-E[y]}{\sqrt{Var[y]+\epsilon}}*\gamma +\beta
+        y=w_{q}\times x+b
 
-    where :math:`quant` is the continuous execution of quant and dequant. Two convolution
-    and Batch Normalization operation are used here, the purpose of the first convolution and Batch Normalization
-    is to count the mean `E[y]` and variance `Var[y]` of current batch output for quantization.
+    where :math:`quant` is the continuous execution of quant and dequant, you can refer to the implementation of
+    subclass of `FakeQuantWithMinMaxObserver`, :class:`mindspore.nn.FakeQuantWithMinMaxObserver`.
+    `mu _{G}` and `var_{G}` represent the global mean and variance respectively.
 
     Args:
         in_channels (int): The number of input channel :math:`C_{in}`.
         out_channels (int): The number of output channel :math:`C_{out}`.
         kernel_size (Union[int, tuple[int]]): Specifies the height and width of the 2D convolution window.
         stride (Union[int, tuple[int]]): Specifies stride for all spatial dimensions with the same value. Default: 1.
         pad_mode (str): Specifies padding mode. The optional values are "same", "valid", "pad". Default: "same".
         padding (Union[int, tuple[int]]): Implicit paddings on both sides of the `x`. Default: 0.
         dilation (Union[int, tuple[int]]): Specifies the dilation rate to use for dilated convolution. Default: 1.
         group (int): Splits filter into groups, `in_channels` and `out_channels` must be
             divisible by the number of groups. Default: 1.
         eps (float): Parameters for Batch Normalization. Default: 1e-5.
         momentum (float): Parameters for Batch Normalization op. Default: 0.997.
-        has_bias (bool): Specifies whether the layer uses a bias vector. Default: False.
+        has_bias (bool): Specifies whether the layer uses a bias vector, which is temporarily invalid. Default: False.
         weight_init (Union[Tensor, str, Initializer, numbers.Number]): Initializer for the
             convolution kernel. Default: 'normal'.
         bias_init (Union[Tensor, str, Initializer, numbers.Number]): Initializer for the
             bias vector. Default: 'zeros'.
         beta_init (Union[Tensor, str, Initializer, numbers.Number]): Initializer for the
             beta vector. Default: 'zeros'.
         gamma_init (Union[Tensor, str, Initializer, numbers.Number]): Initializer for the
@@ -76,214 +76,164 @@
             variance vector. Default: 'ones'.
         fake (bool): Whether Conv2dBnFoldQuant Cell adds FakeQuantWithMinMaxObserver. Default: True.
         quant_config (QuantConfig): Configures the types of quant observer and quant settings of weight and
             activation. Note that, QuantConfig is a special namedtuple, which is designed for quantization
             and can be generated by :func:`mindspore.compression.quant.create_quant_config` method.
             Default: QuantConfig with both items set to default :class:`FakeQuantWithMinMaxObserver`.
         quant_dtype (QuantDtype): Specifies the FakeQuant datatype. Default: QuantDtype.INT8.
-        freeze_bn (int): The quantization freeze Batch Normalization op is according to the global step.
-            Default: 100000.
 
     Inputs:
         - **x** (Tensor) - Tensor of shape :math:`(N, C_{in}, H_{in}, W_{in})`.
 
     Outputs:
         Tensor of shape :math:`(N, C_{out}, H_{out}, W_{out})`.
 
     Raises:
         TypeError: If `in_channels`, `out_channels` or `group` is not an int.
         TypeError: If `kernel_size`, `stride`, `padding` or `dilation` is neither an int nor a tuple.
         TypeError: If `has_bias` or `fake` is not a bool.
+        TypeError: If `data_format` is not a string.
         ValueError: If `in_channels`, `out_channels`, `kernel_size`, `stride` or `dilation` is less than 1.
         ValueError: If `padding` is less than 0.
         ValueError: If `pad_mode` is not one of 'same', 'valid', 'pad'.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> import mindspore
-        >>> from mindspore.compression import quant
         >>> from mindspore import Tensor, nn
-        >>> qconfig = quant.create_quant_config()
-        >>> conv2d_bnfold = nn.Conv2dBnFoldQuant(1, 1, kernel_size=(2, 2), stride=(1, 1), pad_mode="valid",
-        ...                                      weight_init="ones", quant_config=qconfig)
+        >>> conv2d_bnfold = nn.Conv2dBnFoldQuantOneConv(1, 1, kernel_size=(2, 2), stride=(1, 1), pad_mode="valid",
+        ...                                             weight_init="ones")
         >>> x = Tensor(np.array([[[[1, 0, 3], [1, 4, 7], [2, 5, 2]]]]), mindspore.float32)
         >>> result = conv2d_bnfold(x)
         >>> print(result)
         [[[[5.9296875 13.8359375]
            [11.859375 17.78125]]]]
     """
 
-    def __init__(self,
-                 in_channels,
-                 out_channels,
-                 kernel_size,
-                 stride=1,
-                 pad_mode='same',
-                 padding=0,
-                 dilation=1,
-                 group=1,
-                 eps=1e-5,
-                 momentum=0.997,
-                 has_bias=False,
-                 weight_init='normal',
-                 bias_init='zeros',
-                 beta_init='zeros',
-                 gamma_init='ones',
-                 mean_init='zeros',
-                 var_init='ones',
-                 fake=True,
-                 quant_config=quant_config_default,
-                 quant_dtype=QuantDtype.INT8,
-                 freeze_bn=100000):
+    def __init__(self, handler: Conv2dBn, policy: LayerPolicy, fake=True, quant_dtype=QuantDtype.INT8):
         """Initialize Conv2dBnFoldQuant layer"""
-        super(Conv2dBnFoldQuant, self).__init__()
-        if context.get_context('device_target') == "CPU":
-            raise ValueError(f"For '{self.cls_name}', only the 'Ascend' and 'GPU' platforms"
-                             f" are supported, but got {context.get_context('device_target')}.")
-        self.in_channels = Validator.check_positive_int(in_channels, "in_channels", self.cls_name)
-        self.out_channels = Validator.check_positive_int(out_channels, "out_channels", self.cls_name)
-        self.kernel_size = twice(kernel_size)
-        self.stride = twice(stride)
-        self.dilation = twice(dilation)
-        for kernel_size_elem in self.kernel_size:
-            Validator.check_positive_int(kernel_size_elem, 'kernel_size item', self.cls_name)
-        for stride_elem in self.stride:
-            Validator.check_positive_int(stride_elem, 'stride item', self.cls_name)
-        for dilation_elem in self.dilation:
-            Validator.check_positive_int(dilation_elem, 'dilation item', self.cls_name)
-        if pad_mode not in ('valid', 'same', 'pad'):
-            raise ValueError(f"For '{self.cls_name}', the 'pad_mode' must be one of values in "
-                             f"('valid', 'same', 'pad'), but got {pad_mode}.")
-        self.pad_mode = pad_mode
-        if isinstance(padding, int):
-            Validator.check_non_negative_int(padding, 'padding', self.cls_name)
-            self.padding = padding
-        elif isinstance(padding, tuple):
-            for pad in padding:
-                Validator.check_non_negative_int(pad, 'padding item', self.cls_name)
-            self.padding = padding
-        else:
-            raise TypeError(f"For '{self.cls_name}', the type of 'padding' must be int/tuple(int), "
-                            f"but got {type(padding).__name__}!")
-        self.group = Validator.check_positive_int(group, "group", self.cls_name)
-        self.eps = eps
-        self.momentum = momentum
-        self.has_bias = has_bias
-        self.freeze_bn = freeze_bn
+        if not handler.has_bn:
+            raise ValueError(f"For '{self.cls_name}', input Conv2dBn should has batchnorm.")
+        super(Conv2dBnFoldQuantOneConv, self).__init__(handler, policy)
+        self.in_channels = handler.in_channels
+        self.out_channels = handler.out_channels
+        self.kernel_size = handler.kernel_size
+        self.stride = handler.stride
+        self.dilation = handler.dilation
+        self.pad_mode = handler.pad_mode
+        self.padding = handler.padding
+        self.group = handler.group
+        self.has_bias = handler.has_bias
+        self.eps = handler.batchnorm.eps
+        self.momentum = 1 - handler.batchnorm.momentum
         self.fake = Validator.check_bool(fake, "fake", self.cls_name)
-        self.quant_config = quant_config
-        self.quant_dtype = quant_dtype
-        self.is_gpu = context.get_context('device_target') == "GPU"
+        self.format = 'NCHW'
+        self._target = context.get_context("device_target")
+        self.is_graph_mode = context.get_context("mode") == context.GRAPH_MODE
+        self.is_ge_backend = False
+        if context.get_context("enable_ge"):
+            self.is_ge_backend = True
+        self.enable_default_train = self.is_graph_mode and (self.is_ge_backend or self._target == "Ascend")
 
         # initialize convolution op and Parameter
-        self.conv = P.Conv2D(out_channel=out_channels,
+        self.conv = P.Conv2D(out_channel=self.out_channels,
                              kernel_size=self.kernel_size,
-                             pad_mode=pad_mode,
-                             pad=padding,
+                             pad_mode=self.pad_mode,
+                             pad=self.padding,
                              stride=self.stride,
                              dilation=self.dilation,
-                             group=group)
-        weight_shape = [out_channels, in_channels // group, *self.kernel_size]
+                             group=self.group)
         channel_axis = 0
-        self.weight = Parameter(initializer(weight_init, weight_shape), name='weight')
+        self.channel_axis = channel_axis
+        self.weight = handler.weight
         self.bias_add = P.BiasAdd()
-        self.bias = None
-        if Validator.check_bool(has_bias, "has_bias", self.cls_name):
-            self.bias = Parameter(initializer(bias_init, [out_channels]), name='bias')
+        if self.has_bias:
+            self.bias = handler.bias
 
         # initialize BatchNorm Parameter
-        self.gamma = Parameter(initializer(gamma_init, [out_channels]), name='gamma')
-        self.beta = Parameter(initializer(beta_init, [out_channels]), name='beta')
-        self.moving_mean = Parameter(initializer(mean_init, [out_channels]), name='moving_mean', requires_grad=False)
-        self.moving_variance = Parameter(initializer(var_init, [out_channels]), name='moving_variance',
-                                         requires_grad=False)
+        self.gamma = handler.batchnorm.gamma
+        self.beta = handler.batchnorm.beta
+        self.moving_mean = handler.batchnorm.moving_mean
+        self.moving_variance = handler.batchnorm.moving_variance
 
         # initialize fake ops
-        self.fake_quant_weight = quant_config.weight(channel_axis=channel_axis,
-                                                     num_channels=out_channels)
-        self.batchnorm_fold = BatchNormFoldCell(epsilon=eps, momentum=momentum, freeze_bn=freeze_bn)
-        self.correct_mul = Q.CorrectionMul(channel_axis)
-        if context.get_context('device_target') == "Ascend":
-            self.batchnorm_fold2_train = Q.BatchNormFold2D(freeze_bn=freeze_bn)
-            self.batchnorm_fold2_infer = Q.BatchNormFold2D(freeze_bn=0)
-        elif context.get_context('device_target') == "GPU":
-            self.batchnorm_fold2_train = Q.BatchNormFold2(freeze_bn=freeze_bn)
-            self.batchnorm_fold2_infer = Q.BatchNormFold2(freeze_bn=0)
-        self.step = Parameter(initializer('normal', [1], dtype=mstype.int32), name='step', requires_grad=False)
-        self.one = Tensor(1, mstype.int32)
-        self.assignadd = P.AssignAdd()
-
-    @classmethod
-    def from_convbn(cls, convbn: Conv2dBn, quant_config: QuantConfig, extra_args: dict):
-        """
-        A class method to create `Conv2dBnFoldQuant` from a `Conv2dBn`
-        """
-        conv_quant = cls(in_channels=convbn.conv.in_channels,
-                         out_channels=convbn.conv.out_channels,
-                         kernel_size=convbn.conv.kernel_size,
-                         stride=convbn.conv.stride,
-                         pad_mode=convbn.conv.pad_mode,
-                         padding=convbn.conv.padding,
-                         dilation=convbn.conv.dilation,
-                         group=convbn.conv.group,
-                         eps=convbn.batchnorm.eps,
-                         momentum=convbn.batchnorm.momentum,
-                         has_bias=convbn.conv.has_bias,
-                         bias_init=convbn.conv.bias_init,
-                         weight_init=convbn.conv.weight_init,
-                         quant_config=quant_config,
-                         fake=True,
-                         freeze_bn=extra_args["freeze_bn"])
-        conv_quant.gamma = convbn.batchnorm.gamma
-        conv_quant.beta = convbn.batchnorm.beta
-        conv_quant.moving_mean = convbn.batchnorm.moving_mean
-        conv_quant.moving_variance = convbn.batchnorm.moving_variance
-        conv_quant.weight = convbn.conv.weight
-        if convbn.conv.has_bias:
-            conv_quant.bias = convbn.conv.bias
-        return conv_quant
+        weight_perchannel_args = PerChannelArgs(self.out_channels, channel_axis)
+        self._weight_quantizer = policy.get_weight_quantizer(self.weight.name, weight_perchannel_args)
+        self.freeze_bn = False
+        self.bn_train = P.BatchNorm(is_training=True, epsilon=self.eps, momentum=self.momentum, data_format=self.format)
+
+        self.bn_infer = P.BatchNorm(is_training=False, epsilon=self.eps, data_format=self.format)
+        self.sub_mean = P.Sub()
+        self.sub_var = P.Sub()
+        self.mul_mean = P.Mul()
+        self.mul_var = P.Mul()
+        self.assign_sub_mean = P.AssignSub()
+        self.assign_sub_var = P.AssignSub()
+        self.reshape = P.Reshape()
+        _ = quant_dtype  # for fix pylint unused-argument
+
+    def weight_quantizer(self):
+        return self._weight_quantizer
 
     def extend_repr(self):
         """Display instance object as string."""
         s = 'in_channels={}, out_channels={}, kernel_size={}, stride={}, ' \
             'pad_mode={}, padding={}, dilation={}, group={}, ' \
-            'fake={}, freeze_bn={}, momentum={}'.format(self.in_channels, self.out_channels, self.kernel_size,
-                                                        self.stride, self.pad_mode, self.padding, self.dilation,
-                                                        self.group, self.fake, self.freeze_bn, self.momentum)
+            'fake={}, momentum={}'.format(self.in_channels, self.out_channels, self.kernel_size, self.stride,
+                                          self.pad_mode, self.padding, self.dilation, self.group, self.fake,
+                                          self.momentum)
         return s
 
-    def construct(self, x):
+    def convert(self, backend: BackendTarget = BackendTarget.NONE, is_deploy=False):
+        if self._converted:
+            return
+        if backend is not BackendTarget.NONE:
+            raise ValueError("Only support convert to MS Backend now, got: ", backend)
+        if self.has_bias and self.bias:
+            raise ValueError("Only support conv2d with out bias.")
+        super(Conv2dBnFoldQuantOneConv, self).convert(backend, is_deploy)
+        self._weight_quantizer = self._weight_quantizer.convert_to_fakequantparam()
+        weight, bias = fold_batchnorm(self.weight.data.asnumpy(), self)
+        weight_tensor = Tensor(weight)
+        bias_tensor = Tensor(bias, mstype.float32)
+        self.weight = Parameter(weight_tensor, name=f"{self.weight.name}_bnfold")
+        bias_name = f"{self.weight.name}_bias_bnfold"
+        self.bias = Parameter(bias_tensor, name=bias_name)
+        self.has_bias = True
+
+    # pylint: disable=arguments-differ
+    def core_construct(self, x):
         """construct."""
-        out_conv = self.conv(x, self.weight)
-        if self.has_bias:
-            out_conv = self.bias_add(out_conv, self.bias)
-        # BN fold1
-        batch_mean, batch_std, running_mean, running_std = self.batchnorm_fold(out_conv,
-                                                                               self.moving_mean,
-                                                                               self.moving_variance,
-                                                                               self.step)
-        # fake weight
-        weight = self.correct_mul(self.weight, self.gamma, running_std)
+        running_std = P.Sqrt()(P.Add()(self.moving_variance, self.eps))
+        scale_factor = self.gamma / running_std
+        if self.channel_axis:
+            scale_factor = self.reshape(scale_factor, (1, -1, 1, 1))
+        else:
+            scale_factor = self.reshape(scale_factor, (-1, 1, 1, 1))
+        weight = self.weight * scale_factor
         if self.fake:
-            weight = self.fake_quant_weight(weight)
-        out = self.conv(x, weight)
-        if self.has_bias:
-            out = self.bias_add(out, self.bias)
-        # BN fold2
-        if self.is_gpu:
-            if self.training:
-                out = self.batchnorm_fold2_train(out, self.beta, self.gamma,
-                                                 batch_std, batch_mean, running_std, running_mean, self.step)
-                self.assignadd(self.step, self.one)
-            else:
-                out = self.batchnorm_fold2_infer(out, self.beta, self.gamma,
-                                                 batch_std, batch_mean, running_std, running_mean, self.step)
+            weight = self._weight_quantizer(weight)
+        conv = self.conv(x, weight)
+
+        if self.freeze_bn:
+            return conv + self.reshape((self.beta - self.gamma * self.moving_mean / running_std), (1, -1, 1, 1))
+        scale_factor = self.reshape(scale_factor, (1, -1, 1, 1))
+        if self.enable_default_train:
+            scale_factor = P.Reciprocal()(scale_factor)
+            conv_orig = conv * scale_factor
         else:
-            if self.training:
-                out = self.batchnorm_fold2_train(out, self.beta, self.gamma, batch_std, batch_mean, running_std)
-                self.assignadd(self.step, self.one)
-            else:
-                out = self.batchnorm_fold2_infer(out, self.beta, self.gamma, running_std, running_mean, running_std)
-        return out
+            conv_orig = conv / scale_factor
+        if self.training:
+            return self.bn_train(conv_orig,
+                                 self.gamma,
+                                 self.beta,
+                                 self.moving_mean,
+                                 self.moving_variance)[0]
+
+        return self.bn_infer(conv_orig,
+                             self.gamma,
+                             self.beta,
+                             self.moving_mean,
+                             self.moving_variance)[0]
```

## Comparing `mindspore_gs/ops/nn/conv2d_bn_without_fold_quant.py` & `mindspore_gs/quantization/ops/nn/conv2d_bn_fold_quant.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,198 +8,204 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
-"""Conv2dBnWithoutFoldQuant."""
+"""Conv2dBnFoldQuant."""
 from __future__ import absolute_import
 
+import mindspore.common.dtype as mstype
+import mindspore.context as context
 from mindspore.ops import operations as P
 from mindspore.common.parameter import Parameter
 from mindspore.common.initializer import initializer
-from mindspore._checkparam import Validator, twice
-from mindspore.nn.layer.normalization import BatchNorm2d
-from mindspore.nn.cell import Cell
-from ...quantization.simulated_quantization.combined import Conv2dBn
-from .fake_quant_with_min_max_observer import quant_config_default, QuantConfig
+from mindspore.common.tensor import Tensor
+from mindspore.common.dtype import QuantDtype
+from mindspore.ops.operations import _quant_ops as Q
+from mindspore_gs.common import BackendTarget
+from mindspore_gs.validator import Validator
+from mindspore_gs.quantization.layer_policy import LayerPolicy, PerChannelArgs
+from mindspore_gs.quantization.simulated_quantization.combined import Conv2dBn
+from mindspore_gs.quantization.quant_cell import QuantCell
+from mindspore_gs.quantization.quant_utils import fold_batchnorm
+from .batchnorm_fold_cell import BatchNormFoldCell
 
 
-class Conv2dBnWithoutFoldQuant(Cell):
+class Conv2dBnFoldQuant(QuantCell):
     r"""
-    2D convolution and batchnorm without fold with fake quantized construct.
+    2D convolution with Batch Normalization operation folded construct.
 
     This part is a more detailed overview of Conv2d operation. For more details about Quantization,
     please refer to the implementation of class of `FakeQuantWithMinMaxObserver`,
-    :class:`mindspore.nn.FakeQuantWithMinMaxObserver`.
+    :class:`FakeQuantWithMinMaxObserver`.
 
     .. math::
-        y =x\times quant(w)+  b
+        y = x\times w+  b
 
-        y_{bn} =\frac{y-E[y] }{\sqrt{Var[y]+  \epsilon  } } *\gamma +  \beta
+        w_{q}=quant(\frac{w}{\sqrt{Var[y]+\epsilon}}*\gamma )
 
-    where :math:`quant` is the continuous execution of quant and dequant, you can refer to the implementation of
-    class of `FakeQuantWithMinMaxObserver`, :class:`mindspore.nn.FakeQuantWithMinMaxObserver`.
+        y_{out}= w_{q}\times x+\frac{b-E[y]}{\sqrt{Var[y]+\epsilon}}*\gamma +\beta
+
+    where :math:`quant` is the continuous execution of quant and dequant. Two convolution
+    and Batch Normalization operation are used here, the purpose of the first convolution and Batch Normalization
+    is to count the mean `E[y]` and variance `Var[y]` of current batch output for quantization.
 
     Args:
-        in_channels (int): The number of input channel :math:`C_{in}`.
-        out_channels (int): The number of output channel :math:`C_{out}`.
-        kernel_size (Union[int, tuple[int]]): Specifies the height and width of the 2D convolution window.
-        stride (Union[int, tuple[int]]): Specifies stride for all spatial dimensions with the same value. Default: 1.
-        pad_mode (str): Specifies padding mode. The optional values are "same", "valid", "pad". Default: "same".
-        padding (Union[int, tuple[int]]): Implicit paddings on both sides of the `x`. Default: 0.
-        dilation (Union[int, tuple[int]]): Specifies the dilation rate to use for dilated convolution. Default: 1.
-        group (int): Splits filter into groups, `in_ channels` and `out_channels` must be
-            divisible by the number of groups. Default: 1.
-        has_bias (bool): Specifies whether the layer uses a bias vector. Default: False.
-        eps (float): Parameters for Batch Normalization. Default: 1e-5.
-        momentum (float): Parameters for Batch Normalization op. Default: 0.997.
-        weight_init (Union[Tensor, str, Initializer, numbers.Number]): Initializer for the convolution kernel.
-            Default: 'normal'.
-        bias_init (Union[Tensor, str, Initializer, numbers.Number]): Initializer for the bias vector. Default: 'zeros'.
-        quant_config (QuantConfig): Configures the types of quant observer and quant settings of weight and
-            activation. Note that, QuantConfig is a special namedtuple, which is designed for quantization
-            and can be generated by :func:`mindspore.compression.quant.create_quant_config` method.
-            Default: QuantConfig with both items set to default :class:`FakeQuantWithMinMaxObserver`.
+        fake (bool): Whether Conv2dBnFoldQuant Cell adds FakeQuantWithMinMaxObserver. Default: True.
+        quant_dtype (QuantDtype): Specifies the FakeQuant datatype. Default: QuantDtype.INT8.
+        freeze_bn (int): The quantization freeze Batch Normalization op is according to the global step.
+            Default: 100000.
 
     Inputs:
         - **x** (Tensor) - Tensor of shape :math:`(N, C_{in}, H_{in}, W_{in})`.
 
     Outputs:
         Tensor of shape :math:`(N, C_{out}, H_{out}, W_{out})`.
 
-    Supported Platforms:
-        ``Ascend`` ``GPU``
-
     Raises:
         TypeError: If `in_channels`, `out_channels` or `group` is not an int.
         TypeError: If `kernel_size`, `stride`, `padding` or `dilation` is neither an int nor a tuple.
-        TypeError: If `has_bias` is not a bool.
+        TypeError: If `has_bias` or `fake` is not a bool.
         ValueError: If `in_channels`, `out_channels`, `kernel_size`, `stride` or `dilation` is less than 1.
         ValueError: If `padding` is less than 0.
         ValueError: If `pad_mode` is not one of 'same', 'valid', 'pad'.
 
+    Supported Platforms:
+        ``Ascend`` ``GPU``
+
     Examples:
         >>> import numpy as np
         >>> import mindspore
-        >>> from mindspore.compression import quant
         >>> from mindspore import Tensor, nn
-        >>> qconfig = quant.create_quant_config()
-        >>> conv2d_no_bnfold = nn.Conv2dBnWithoutFoldQuant(1, 1, kernel_size=(2, 2), stride=(1, 1), pad_mode="valid",
-        ...                                                weight_init='ones', quant_config=qconfig)
+        >>> conv2d_bnfold = nn.Conv2dBnFoldQuant(1, 1, kernel_size=(2, 2), stride=(1, 1), pad_mode="valid",
+        ...                                      weight_init="ones")
         >>> x = Tensor(np.array([[[[1, 0, 3], [1, 4, 7], [2, 5, 2]]]]), mindspore.float32)
-        >>> result = conv2d_no_bnfold(x)
+        >>> result = conv2d_bnfold(x)
         >>> print(result)
-        [[[[5.929658  13.835868]
-           [11.859316  17.78116]]]]
+        [[[[5.9296875 13.8359375]
+           [11.859375 17.78125]]]]
     """
 
-    def __init__(self,
-                 in_channels,
-                 out_channels,
-                 kernel_size,
-                 stride=1,
-                 pad_mode='same',
-                 padding=0,
-                 dilation=1,
-                 group=1,
-                 has_bias=False,
-                 eps=1e-5,
-                 momentum=0.997,
-                 weight_init='normal',
-                 bias_init='zeros',
-                 quant_config=quant_config_default):
-        """Initialize Conv2dBnWithoutFoldQuant."""
-        super(Conv2dBnWithoutFoldQuant, self).__init__()
-        self.in_channels = Validator.check_positive_int(in_channels, "in_channels", self.cls_name)
-        self.out_channels = Validator.check_positive_int(out_channels, "out_channels", self.cls_name)
-        self.has_bias = has_bias
-        self.kernel_size = twice(kernel_size)
-        self.stride = twice(stride)
-        self.dilation = twice(dilation)
-        for kernel_size_elem in self.kernel_size:
-            Validator.check_positive_int(kernel_size_elem, 'kernel_size item', self.cls_name)
-        for stride_elem in self.stride:
-            Validator.check_positive_int(stride_elem, 'stride item', self.cls_name)
-        for dilation_elem in self.dilation:
-            Validator.check_positive_int(dilation_elem, 'dilation item', self.cls_name)
-        if pad_mode not in ('valid', 'same', 'pad'):
-            raise ValueError(f"For '{self.cls_name}', the 'pad_mode' must be one of values in "
-                             f"('valid', 'same', 'pad'), but got {pad_mode}.")
-        self.pad_mode = pad_mode
-        if isinstance(padding, int):
-            Validator.check_non_negative_int(padding, 'padding', self.cls_name)
-            self.padding = padding
-        elif isinstance(padding, tuple):
-            for pad in padding:
-                Validator.check_non_negative_int(pad, 'padding item', self.cls_name)
-            self.padding = padding
-        else:
-            raise TypeError(f"For '{self.cls_name}', the type of 'padding' must be int/tuple(int), "
-                            f"but got {type(padding).__name__}!")
-        self.group = Validator.check_positive_int(group, "group", self.cls_name)
-        self.bias_add = P.BiasAdd()
-        if Validator.check_bool(has_bias, "has_bias", self.cls_name):
-            self.bias = Parameter(initializer(bias_init, [out_channels]), name='bias')
-        else:
-            self.bias = None
+    def __init__(self, handler: Conv2dBn, policy: LayerPolicy, fake=True, quant_dtype=QuantDtype.INT8,
+                 freeze_bn=100000):
+        """Initialize Conv2dBnFoldQuant layer"""
+        super(Conv2dBnFoldQuant, self).__init__(handler, policy)
+        if not handler.has_bn:
+            raise ValueError(f"For '{self.cls_name}', input Conv2dBn should has batchnorm.")
+        if context.get_context('device_target') == "CPU":
+            raise ValueError(f"For '{self.cls_name}', only the 'Ascend' and 'GPU' platforms"
+                             f" are supported, but got {context.get_context('device_target')}.")
+        self.in_channels = handler.in_channels
+        self.out_channels = handler.out_channels
+        self.kernel_size = handler.kernel_size
+        self.stride = handler.stride
+        self.dilation = handler.dilation
+        self.pad_mode = handler.pad_mode
+        self.padding = handler.padding
+        self.group = handler.group
+        self.has_bias = handler.has_bias
+        self.freeze_bn = freeze_bn
+        self.fake = Validator.check_bool(fake, "fake", self.cls_name)
+        self.quant_dtype = quant_dtype
+        self.is_gpu = context.get_context('device_target') == "GPU"
+
         # initialize convolution op and Parameter
         self.conv = P.Conv2D(out_channel=self.out_channels,
                              kernel_size=self.kernel_size,
-                             mode=1,
                              pad_mode=self.pad_mode,
                              pad=self.padding,
                              stride=self.stride,
                              dilation=self.dilation,
                              group=self.group)
-        weight_shape = [out_channels, in_channels // group, *self.kernel_size]
         channel_axis = 0
-        self.weight = Parameter(initializer(weight_init, weight_shape), name='weight')
-        self.fake_quant_weight = quant_config.weight(channel_axis=channel_axis,
-                                                     num_channels=out_channels)
-        self.batchnorm = BatchNorm2d(out_channels, eps=eps, momentum=momentum)
-
-    @classmethod
-    def from_float(cls, convbn: Conv2dBn, quant_config: QuantConfig):
-        """
-        A class method to create `Conv2dBnWithoutFoldQuant` from`Conv2dBn`
-        """
-        conv_quant = cls(in_channels=convbn.conv.in_channels,
-                         out_channels=convbn.conv.out_channels,
-                         kernel_size=convbn.conv.kernel_size,
-                         stride=convbn.conv.stride,
-                         pad_mode=convbn.conv.pad_mode,
-                         padding=convbn.conv.padding,
-                         dilation=convbn.conv.dilation,
-                         group=convbn.conv.group,
-                         eps=convbn.batchnorm.eps,
-                         momentum=convbn.batchnorm.momentum,
-                         has_bias=convbn.conv.has_bias,
-                         bias_init=convbn.conv.bias_init,
-                         weight_init=convbn.conv.weight_init,
-                         quant_config=quant_config)
-        conv_quant.batchnorm.gamma = convbn.batchnorm.gamma
-        conv_quant.batchnorm.beta = convbn.batchnorm.beta
-        conv_quant.batchnorm.moving_mean = convbn.batchnorm.moving_mean
-        conv_quant.batchnorm.moving_variance = convbn.batchnorm.moving_variance
-        conv_quant.weight = convbn.conv.weight
-        if convbn.conv.has_bias:
-            conv_quant.bias = convbn.conv.bias
-        return conv_quant
-
-    def construct(self, x):
-        """construct."""
-        weight = self.fake_quant_weight(self.weight)
-        out = self.conv(x, weight)
+        self.weight = handler.weight
+        self.bias_add = P.BiasAdd()
         if self.has_bias:
-            out = self.bias_add(out, self.bias)
-        out = self.batchnorm(out)
-        return out
+            self.bias = handler.bias
+
+        # initialize BatchNorm Parameter
+        self.gamma = handler.batchnorm.gamma
+        self.beta = handler.batchnorm.beta
+        self.moving_mean = handler.batchnorm.moving_mean
+        self.moving_variance = handler.batchnorm.moving_variance
+
+        # initialize fake ops
+        weight_perchannel_args = PerChannelArgs(self.out_channels, channel_axis)
+        self._weight_quantizer = policy.get_weight_quantizer(self.weight.name, weight_perchannel_args)
+        self.eps = handler.batchnorm.eps
+        self.batchnorm_fold = BatchNormFoldCell(epsilon=self.eps, momentum=handler.batchnorm.momentum,
+                                                freeze_bn=freeze_bn)
+        self.correct_mul = Q.CorrectionMul(channel_axis)
+        if context.get_context('device_target') == "Ascend":
+            self.batchnorm_fold2_train = Q.BatchNormFold2D(freeze_bn=freeze_bn)
+            self.batchnorm_fold2_infer = Q.BatchNormFold2D(freeze_bn=0)
+        elif context.get_context('device_target') == "GPU":
+            self.batchnorm_fold2_train = Q.BatchNormFold2(freeze_bn=freeze_bn)
+            self.batchnorm_fold2_infer = Q.BatchNormFold2(freeze_bn=0)
+        self.step = Parameter(initializer('normal', [1], dtype=mstype.int32), name='step', requires_grad=False)
+        self.one = Tensor(1, mstype.int32)
+        self.assignadd = P.AssignAdd()
+
+    def weight_quantizer(self):
+        return self._weight_quantizer
 
     def extend_repr(self):
         """Display instance object as string."""
         s = 'in_channels={}, out_channels={}, kernel_size={}, stride={}, ' \
-            'pad_mode={}, padding={}, dilation={}, group={}, ' \
-            'has_bias={}'.format(self.in_channels, self.out_channels, self.kernel_size, self.stride, self.pad_mode,
-                                 self.padding, self.dilation, self.group, self.has_bias)
+            'pad_mode={}, padding={}, dilation={}, group={}, fake={}, freeze_bn={}'\
+            .format(self.in_channels, self.out_channels, self.kernel_size, self.stride, self.pad_mode, self.padding,
+                    self.dilation, self.group, self.fake, self.freeze_bn)
         return s
+
+    def convert(self, backend: BackendTarget = BackendTarget.NONE, is_deploy=False):
+        if self._converted:
+            return
+        if backend is not BackendTarget.NONE:
+            raise ValueError("Only support convert to MS Backend now, got: ", backend)
+        if self.has_bias and self.bias:
+            raise ValueError("Only support conv2d with out bias.")
+        super(Conv2dBnFoldQuant, self).convert(backend, is_deploy)
+        self._weight_quantizer = self._weight_quantizer.convert_to_fakequantparam()
+        weight, bias = fold_batchnorm(self.weight.data.asnumpy(), self)
+        weight_tensor = Tensor(weight)
+        bias_tensor = Tensor(bias, mstype.float32)
+        self.weight = Parameter(weight_tensor, name=f"{self.weight.name}_bnfold")
+        bias_name = f"{self.weight.name}_bias_bnfold"
+        self.bias = Parameter(bias_tensor, name=bias_name)
+        self.has_bias = True
+
+    # pylint: disable=arguments-differ
+    def core_construct(self, x):
+        """construct."""
+        out_conv = self.conv(x, self.weight)
+        if self.has_bias:
+            out_conv = self.bias_add(out_conv, self.bias)
+        # BN fold1
+        batch_mean, batch_std, running_mean, running_std = self.batchnorm_fold(out_conv,
+                                                                               self.moving_mean,
+                                                                               self.moving_variance,
+                                                                               self.step)
+        # fake weight
+        weight = self.correct_mul(self.weight, self.gamma, running_std)
+        if self.fake:
+            weight = self._weight_quantizer(weight)
+        out = self.conv(x, weight)
+        if self.has_bias:
+            out = self.bias_add(out, self.bias)
+        # BN fold2
+        if self.is_gpu:
+            if self.training:
+                out = self.batchnorm_fold2_train(out, self.beta, self.gamma,
+                                                 batch_std, batch_mean, running_std, running_mean, self.step)
+                self.assignadd(self.step, self.one)
+            else:
+                out = self.batchnorm_fold2_infer(out, self.beta, self.gamma,
+                                                 batch_std, batch_mean, running_std, running_mean, self.step)
+        else:
+            if self.training:
+                out = self.batchnorm_fold2_train(out, self.beta, self.gamma, batch_std, batch_mean, running_std)
+                self.assignadd(self.step, self.one)
+            else:
+                out = self.batchnorm_fold2_infer(out, self.beta, self.gamma, running_std, running_mean, running_std)
+        return out
```

## Comparing `mindspore_gs/ops/nn/conv2d_quant.py` & `mindspore_gs/quantization/ops/nn/conv2d_bn_without_fold_quant.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,205 +8,156 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
-"""Conv2dQuant."""
+"""Conv2dBnWithoutFoldQuant."""
 from __future__ import absolute_import
 
+import mindspore.common.dtype as mstype
+from mindspore import Tensor
 from mindspore.ops import operations as P
 from mindspore.common.parameter import Parameter
-from mindspore.common.initializer import initializer
-from mindspore._checkparam import Validator, twice
-from mindspore.common.dtype import QuantDtype
-from mindspore.nn.cell import Cell
-from mindspore.nn.layer.conv import Conv2d
-from ...quantization.simulated_quantization.combined import Conv2dBn
-from .fake_quant_with_min_max_observer import quant_config_default, QuantConfig
+from mindspore.nn.layer.normalization import BatchNorm2d
+from mindspore_gs.common import BackendTarget
+from mindspore_gs.quantization.simulated_quantization.combined import Conv2dBn
+from mindspore_gs.quantization.quant_cell import QuantCell
+from mindspore_gs.quantization.layer_policy import LayerPolicy, PerChannelArgs
+from mindspore_gs.quantization.quant_utils import without_fold_batchnorm
 
 
-class Conv2dQuant(Cell):
+class Conv2dBnWithoutFoldQuant(QuantCell):
     r"""
-    2D convolution with fake quantized operation layer.
+    2D convolution and batchnorm without fold with fake quantized construct.
 
     This part is a more detailed overview of Conv2d operation. For more details about Quantization,
     please refer to the implementation of class of `FakeQuantWithMinMaxObserver`,
     :class:`mindspore.nn.FakeQuantWithMinMaxObserver`.
 
+    .. math::
+        y =x\times quant(w)+  b
+
+        y_{bn} =\frac{y-E[y] }{\sqrt{Var[y]+  \epsilon  } } *\gamma +  \beta
+
+    where :math:`quant` is the continuous execution of quant and dequant, you can refer to the implementation of
+    class of `FakeQuantWithMinMaxObserver`, :class:`mindspore.nn.FakeQuantWithMinMaxObserver`.
+
     Args:
         in_channels (int): The number of input channel :math:`C_{in}`.
         out_channels (int): The number of output channel :math:`C_{out}`.
         kernel_size (Union[int, tuple[int]]): Specifies the height and width of the 2D convolution window.
         stride (Union[int, tuple[int]]): Specifies stride for all spatial dimensions with the same value. Default: 1.
         pad_mode (str): Specifies padding mode. The optional values are "same", "valid", "pad". Default: "same".
         padding (Union[int, tuple[int]]): Implicit paddings on both sides of the `x`. Default: 0.
         dilation (Union[int, tuple[int]]): Specifies the dilation rate to use for dilated convolution. Default: 1.
         group (int): Splits filter into groups, `in_ channels` and `out_channels` must be
             divisible by the number of groups. Default: 1.
         has_bias (bool): Specifies whether the layer uses a bias vector. Default: False.
+        eps (float): Parameters for Batch Normalization. Default: 1e-5.
+        momentum (float): Parameters for Batch Normalization op. Default: 0.997.
         weight_init (Union[Tensor, str, Initializer, numbers.Number]): Initializer for the convolution kernel.
             Default: 'normal'.
         bias_init (Union[Tensor, str, Initializer, numbers.Number]): Initializer for the bias vector. Default: 'zeros'.
         quant_config (QuantConfig): Configures the types of quant observer and quant settings of weight and
             activation. Note that, QuantConfig is a special namedtuple, which is designed for quantization
             and can be generated by :func:`mindspore.compression.quant.create_quant_config` method.
             Default: QuantConfig with both items set to default :class:`FakeQuantWithMinMaxObserver`.
-        quant_dtype (QuantDtype): Specifies the FakeQuant datatype. Default: QuantDtype.INT8.
 
     Inputs:
         - **x** (Tensor) - Tensor of shape :math:`(N, C_{in}, H_{in}, W_{in})`.
-          The input dimension is preferably 2D or 4D.
 
     Outputs:
         Tensor of shape :math:`(N, C_{out}, H_{out}, W_{out})`.
 
+    Supported Platforms:
+        ``Ascend`` ``GPU``
+
     Raises:
         TypeError: If `in_channels`, `out_channels` or `group` is not an int.
         TypeError: If `kernel_size`, `stride`, `padding` or `dilation` is neither an int nor a tuple.
         TypeError: If `has_bias` is not a bool.
         ValueError: If `in_channels`, `out_channels`, `kernel_size`, `stride` or `dilation` is less than 1.
         ValueError: If `padding` is less than 0.
         ValueError: If `pad_mode` is not one of 'same', 'valid', 'pad'.
 
-    Supported Platforms:
-        ``Ascend`` ``GPU``
-
     Examples:
         >>> import numpy as np
         >>> import mindspore
-        >>> from mindspore.compression import quant
         >>> from mindspore import Tensor, nn
-        >>> qconfig = quant.create_quant_config()
-        >>> conv2d_quant = nn.Conv2dQuant(1, 1, kernel_size=(2, 2), stride=(1, 1), pad_mode="valid",
-        ...                               weight_init='ones', quant_config=qconfig)
+        >>> conv2d_no_bnfold = nn.Conv2dBnWithoutFoldQuant(1, 1, kernel_size=(2, 2), stride=(1, 1), pad_mode="valid",
+        ...                                                weight_init='ones')
         >>> x = Tensor(np.array([[[[1, 0, 3], [1, 4, 7], [2, 5, 2]]]]), mindspore.float32)
-        >>> result = conv2d_quant(x)
+        >>> result = conv2d_no_bnfold(x)
         >>> print(result)
-        [[[[5.9296875  13.8359375]
-           [11.859375  17.78125]]]]
+        [[[[5.929658  13.835868]
+           [11.859316  17.78116]]]]
     """
 
-    def __init__(self,
-                 in_channels,
-                 out_channels,
-                 kernel_size,
-                 stride=1,
-                 pad_mode='same',
-                 padding=0,
-                 dilation=1,
-                 group=1,
-                 has_bias=False,
-                 weight_init='normal',
-                 bias_init='zeros',
-                 quant_config=quant_config_default,
-                 quant_dtype=QuantDtype.INT8):
-        """Initialize Conv2dQuant."""
-        super(Conv2dQuant, self).__init__()
-        self.in_channels = Validator.check_positive_int(in_channels, "in_channels", self.cls_name)
-        self.out_channels = Validator.check_positive_int(out_channels, "out_channels", self.cls_name)
-        self.has_bias = has_bias
-        self.kernel_size = twice(kernel_size)
-        self.stride = twice(stride)
-        self.dilation = twice(dilation)
-        for kernel_size_elem in self.kernel_size:
-            Validator.check_positive_int(kernel_size_elem, 'kernel_size item', self.cls_name)
-        for stride_elem in self.stride:
-            Validator.check_positive_int(stride_elem, 'stride item', self.cls_name)
-        for dilation_elem in self.dilation:
-            Validator.check_positive_int(dilation_elem, 'dilation item', self.cls_name)
-        if pad_mode not in ('valid', 'same', 'pad'):
-            raise ValueError(f"For '{self.cls_name}', the 'pad_mode' must be one of values "
-                             f"in ('valid', 'same', 'pad'), but got {pad_mode}.")
-        self.pad_mode = pad_mode
-        if isinstance(padding, int):
-            Validator.check_non_negative_int(padding, 'padding', self.cls_name)
-            self.padding = padding
-        elif isinstance(padding, tuple):
-            for pad in padding:
-                Validator.check_non_negative_int(pad, 'padding item', self.cls_name)
-            self.padding = padding
-        else:
-            raise TypeError(f"For '{self.cls_name}', the type of 'padding' must be int/tuple(int), "
-                            f"but got {type(padding).__name__}!")
-        self.group = Validator.check_positive_int(group, "group", self.cls_name)
-        _ = quant_dtype  # for fix pylint unused-argument
-
-        weight_shape = [out_channels, in_channels // group, *self.kernel_size]
-        self.weight = Parameter(initializer(weight_init, weight_shape), name='weight')
-
+    def __init__(self, handler: Conv2dBn, policy: LayerPolicy):
+        """Initialize Conv2dBnWithoutFoldQuant."""
+        if not handler.has_bn:
+            raise ValueError(f"For '{self.cls_name}', input Conv2dBn should has batchnorm.")
+        super(Conv2dBnWithoutFoldQuant, self).__init__(handler, policy)
+        self.in_channels = handler.in_channels
+        self.out_channels = handler.out_channels
+        self.kernel_size = handler.kernel_size
+        self.stride = handler.stride
+        self.dilation = handler.dilation
+        self.pad_mode = handler.pad_mode
+        self.padding = handler.padding
+        self.group = handler.group
+        self.has_bias = handler.has_bias
         self.bias_add = P.BiasAdd()
-        if Validator.check_bool(has_bias, "has_bias", self.cls_name):
-            self.bias = Parameter(initializer(bias_init, [out_channels]), name='bias')
-        else:
-            self.bias = None
-
+        if self.has_bias:
+            self.bias = handler.bias
+        # initialize convolution op and Parameter
         self.conv = P.Conv2D(out_channel=self.out_channels,
                              kernel_size=self.kernel_size,
                              mode=1,
                              pad_mode=self.pad_mode,
                              pad=self.padding,
                              stride=self.stride,
                              dilation=self.dilation,
                              group=self.group)
+        self.weight = handler.weight
         channel_axis = 0
-        self.fake_quant_weight = quant_config.weight(channel_axis=channel_axis,
-                                                     num_channels=out_channels)
-
-    @classmethod
-    def from_conv2d(cls, conv: Conv2d, quant_config: QuantConfig):
-        """
-        A class method to create `Conv2dQuant` from `Conv2d`
-        """
-        conv_quant = cls(in_channels=conv.in_channels,
-                         out_channels=conv.out_channels,
-                         kernel_size=conv.kernel_size,
-                         stride=conv.stride,
-                         pad_mode=conv.pad_mode,
-                         padding=conv.padding,
-                         dilation=conv.dilation,
-                         group=conv.group,
-                         has_bias=conv.has_bias,
-                         bias_init=conv.bias_init,
-                         weight_init=conv.weight_init,
-                         quant_config=quant_config)
-        conv_quant.weight = conv.weight
-        if conv.has_bias:
-            conv_quant.bias = conv.bias
-        return conv_quant
-
-    @classmethod
-    def from_convbn(cls, convbn: Conv2dBn, quant_config: QuantConfig):
-        """
-        A class method to create `Conv2dQuant` from `Conv2dBn`
-        """
-        conv_quant = cls(in_channels=convbn.conv.in_channels,
-                         out_channels=convbn.conv.out_channels,
-                         kernel_size=convbn.conv.kernel_size,
-                         stride=convbn.conv.stride,
-                         pad_mode=convbn.conv.pad_mode,
-                         padding=convbn.conv.padding,
-                         dilation=convbn.conv.dilation,
-                         group=convbn.conv.group,
-                         has_bias=convbn.conv.has_bias,
-                         bias_init=convbn.conv.bias_init,
-                         weight_init=convbn.conv.weight_init,
-                         quant_config=quant_config)
-        conv_quant.weight = convbn.conv.weight
-        if convbn.conv.has_bias:
-            conv_quant.bias = convbn.conv.bias
-        return conv_quant
+        weight_perchannel_args = PerChannelArgs(self.out_channels, channel_axis)
+        self._weight_quantizer = policy.get_weight_quantizer(self.weight.name, weight_perchannel_args)
+        self.batchnorm = BatchNorm2d(self.out_channels, eps=handler.batchnorm.eps, momentum=handler.batchnorm.momentum)
+
+    def weight_quantizer(self):
+        return self._weight_quantizer
+
+    def convert(self, backend: BackendTarget = BackendTarget.NONE, is_deploy=False):
+        if self._converted:
+            return
+        if backend is not BackendTarget.NONE:
+            raise ValueError("Only support convert to MS Backend now, got: ", backend)
+        if self.has_bias and self.bias:
+            raise ValueError("Only support conv2d with out bias.")
+        super(Conv2dBnWithoutFoldQuant, self).convert(backend, is_deploy)
+        self._weight_quantizer = self._weight_quantizer.convert_to_fakequantparam()
+        weight, bias = without_fold_batchnorm(self.weight.data.asnumpy(), self)
+        weight_tensor = Tensor(weight)
+        bias_tensor = Tensor(bias, mstype.float32)
+        self.weight = Parameter(weight_tensor, name=f"{self.weight.name}_bnfold")
+        bias_name = f"{self.weight.name}_bias_bnfold"
+        self.bias = Parameter(bias_tensor, name=bias_name)
+        self.has_bias = True
 
-    def construct(self, x):
+    # pylint: disable=arguments-differ
+    def core_construct(self, x):
         """construct."""
-        weight = self.fake_quant_weight(self.weight)
+        weight = self._weight_quantizer(self.weight)
         out = self.conv(x, weight)
         if self.has_bias:
-            return self.bias_add(out, self.bias)
+            out = self.bias_add(out, self.bias)
+        out = self.batchnorm(out)
         return out
 
     def extend_repr(self):
         """Display instance object as string."""
         s = 'in_channels={}, out_channels={}, kernel_size={}, stride={}, ' \
             'pad_mode={}, padding={}, dilation={}, group={}, ' \
             'has_bias={}'.format(self.in_channels, self.out_channels, self.kernel_size, self.stride, self.pad_mode,
```

## Comparing `mindspore_gs/ops/nn/fake_quant_with_min_max_observer.py` & `mindspore_gs/quantization/ops/nn/fake_quant_with_min_max_observer.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,30 +8,33 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
-"""FakeQuantWithMinMaxObserver."""
+"""
+FakeQuantWithMinMaxObserver. Deprecated and not used, please refer to FakeQuantizers in quantization algorithms.
+"""
+
 from __future__ import absolute_import
 
 from functools import partial
 from collections import namedtuple
 import numpy as np
 
+import mindspore.context as context
 from mindspore.ops import operations as P
 from mindspore.common.parameter import Parameter
 from mindspore.common.tensor import Tensor
-from mindspore._checkparam import Validator
 from mindspore.common.dtype import QuantDtype
-import mindspore.context as context
 from mindspore.nn.cell import Cell
 from mindspore.ops.operations import _quant_ops as Q
-from mindspore_gs.ops.common.quant_op_utils import get_quant_dtype_num_bits
+from mindspore_gs.validator import Validator
+from mindspore_gs.quantization.quant_utils import get_quant_dtype_num_bits
 
 
 def _partial_init(cls_or_self, **kwargs):
     """
     Wrapper that allows creation of class factories.
 
     This can be useful when there is a need to create classes with the same
```

## Comparing `mindspore_gs/ops/nn/mul_quant.py` & `mindspore_gs/quantization/ops/nn/mul_quant.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,34 +12,33 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """MulQuant."""
 from __future__ import absolute_import
 
 from mindspore.ops import operations as P
-from mindspore.common.dtype import QuantDtype
-from mindspore.nn.cell import Cell
-from .fake_quant_with_min_max_observer import quant_config_default
+from mindspore.nn import Cell
+from mindspore_gs.quantization.quant_cell import QuantCell
+from mindspore_gs.quantization.layer_policy import LayerPolicy
 
 
-class MulQuant(Cell):
+class MulQuant(QuantCell):
     r"""
     Adds fake quantized operation after `Mul` operation.
 
     This part is a more detailed overview of `Mul` operation. For more details about Quantization,
     please refer to the implementation of class of `FakeQuantWithMinMaxObserver`,
     :class:`mindspore.nn.FakeQuantWithMinMaxObserver`.
 
     Args:
         ema_decay (float): Exponential Moving Average algorithm parameter. Default: 0.999.
         quant_config (QuantConfig): Configures the types of quant observer and quant settings of weight and
             activation. Note that, QuantConfig is a special namedtuple, which is designed for quantization
             and can be generated by :func:`mindspore.compression.quant.create_quant_config` method.
             Default: QuantConfig with both items set to default :class:`FakeQuantWithMinMaxObserver`.
-        quant_dtype (QuantDtype): Specifies the FakeQuant datatype. Default: QuantDtype.INT8.
 
     Inputs:
         - **x1** (Tensor) - The first tensor of MulQuant. The input dimension is preferably 2D or 4D.
         - **x2** (Tensor) - The second tensor of MulQuant. Has the same shape with `x1`.
 
     Outputs:
         Tensor, with the same type and shape as the `x1`.
@@ -50,37 +49,29 @@
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> import mindspore
-        >>> from mindspore.compression import quant
         >>> from mindspore import Tensor, nn
-        >>> qconfig = quant.create_quant_config()
-        >>> mul_quant = nn.MulQuant(quant_config=qconfig)
+        >>> mul_quant = nn.MulQuant()
         >>> x1 = Tensor(np.array([[1, 2, 1], [-2, 0, -1]]), mindspore.float32)
         >>> x2 = Tensor(np.ones((2, 3)) * 2, mindspore.float32)
         >>> output = mul_quant(x1, x2)
         >>> print(output)
         [[ 1.9764705  4.0000005  1.9764705]
          [-4.         0.        -1.9764705]]
     """
 
-    def __init__(self,
-                 ema_decay=0.999,
-                 quant_config=quant_config_default,
-                 quant_dtype=QuantDtype.INT8):
+    def weight_quantizer(self):
+        return None
+
+    def __init__(self, handler: Cell, policy: LayerPolicy):
         """Initialize MulQuant."""
-        super(MulQuant, self).__init__()
-        self.fake_quant_act = quant_config.activation(min_init=-6,
-                                                      max_init=6,
-                                                      ema=True,
-                                                      ema_decay=ema_decay,
-                                                      quant_dtype=quant_dtype)
+        super(MulQuant, self).__init__(handler, policy)
         self.mul = P.Mul()
 
-    def construct(self, x1, x2):
+    # pylint: disable=arguments-differ
+    def core_construct(self, x1, x2):
         """construct."""
-        x = self.mul(x1, x2)
-        x = self.fake_quant_act(x)
-        return x
+        return self.mul(x1, x2)
```

## Comparing `mindspore_gs/ops/operations/__init__.py` & `mindspore_gs/quantization/ops/operations/grad_operations/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,24 +9,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """
-MindSpore golden stick operations.
+MindSpore golden stick grad operations.
 """
 
-from .gs_custom import GSCustom, custom_op_attr_register
-from .fake_quant_perchannel import FakeQuantPerChannel
-from .fake_quant_perlayer import FakeQuantPerLayer
-from .min_max_update_perchannel import MinMaxUpdatePerChannel
-from .min_max_update_perlayer import MinMaxUpdatePerLayer
+from .fake_quant_perlayer_grad import FakeQuantPerLayerGrad
+from .fake_quant_perchannel_grad import FakeQuantPerChannelGrad
 
 __all__ = [
-    "MinMaxUpdatePerLayer",
-    "FakeQuantPerLayer",
-    "FakeQuantPerChannel",
-    "MinMaxUpdatePerChannel",
-    "GSCustom",
-    "custom_op_attr_register"
+    "FakeQuantPerLayerGrad",
+    "FakeQuantPerChannelGrad"
 ]
```

## Comparing `mindspore_gs/ops/operations/fake_quant_perchannel.py` & `mindspore_gs/quantization/ops/operations/fake_quant_perchannel.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,20 +11,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """
 MindSpore golden stick simulated-quantization ops FakeQuantPerChannel.
 """
+import os
+
 from mindspore.ops import DataType
+from mindspore import log as logger
 from mindspore.ops.functional import zeros_like
-from mindspore._checkparam import Validator as validator
-from mindspore._checkparam import Rel
-from mindspore_gs.ops.operations import GSCustom, custom_op_attr_register
-from mindspore_gs.ops.operations.grad_operations import FakeQuantPerChannelGrad
+from mindspore_gs.validator import Rel
+from mindspore_gs.validator import Validator as validator
+from mindspore_gs.ops import GSCustom, custom_op_attr_register
+from .grad_operations import FakeQuantPerChannelGrad
 
 
 class FakeQuantPerChannel(GSCustom):
     r"""
     Simulates the quantize and dequantize operations in training time base on per channel.
 
     Args:
@@ -118,7 +121,24 @@
     def _get_op_output_names(self) -> (str,):
         """set_op_output_names"""
         return ("y",)
 
     def _get_op_dtype_formats(self) -> [[DataType]]:
         """set_op_dtype_format"""
         return [[DataType.F32_Default, DataType.F32_Default, DataType.F32_Default, DataType.F32_Default]]
+
+    def _get_forward_func(self) -> str:
+        """
+        Automatically generate farward func according to class name.
+
+        Returns:
+            Farward func, a string represent '{dir_path}/{file_name}:{func_name}'.
+        """
+        dir_path = os.path.dirname(os.path.abspath(__file__))
+        func_path = os.path.join(dir_path, "../kernel/gpu/fake_quant_per_channel_impl.cu")
+        func_name = "Custom" + self._get_custom_op_name()
+        if not os.path.exists(func_path):
+            error_str = f"For {self._get_custom_op_name()}, cu file not exist, the path is {func_path}"
+            logger.error(error_str)
+            raise RuntimeError(error_str)
+        logger.info(f"Custom op {self._get_custom_op_name()} func: {func_path}:{func_name}")
+        return func_path + ":" + func_name
```

## Comparing `mindspore_gs/ops/operations/fake_quant_perlayer.py` & `mindspore_gs/quantization/ops/operations/fake_quant_perlayer.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,20 +11,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """
 MindSpore golden stick simulated-quantization ops FakeQuantPerLayer.
 """
+import os
+
 from mindspore.ops import DataType
+from mindspore import log as logger
 from mindspore.ops.functional import zeros_like
-from mindspore._checkparam import Validator as validator
-from mindspore._checkparam import Rel
-from mindspore_gs.ops.operations import GSCustom, custom_op_attr_register
-from mindspore_gs.ops.operations.grad_operations import FakeQuantPerLayerGrad
+from mindspore_gs.validator import Rel
+from mindspore_gs.validator import Validator as validator
+from mindspore_gs.ops import GSCustom, custom_op_attr_register
+from .grad_operations import FakeQuantPerLayerGrad
 
 
 class FakeQuantPerLayer(GSCustom):
     r"""
     Simulates the quantize and dequantize operations in training time.
 
     Args:
@@ -114,7 +117,24 @@
     def _get_op_output_names(self) -> (str,):
         """set_op_output_names"""
         return ("y",)
 
     def _get_op_dtype_formats(self) -> [[DataType]]:
         """set_op_dtype_format"""
         return [[DataType.F32_Default, DataType.F32_Default, DataType.F32_Default, DataType.F32_Default]]
+
+    def _get_forward_func(self) -> str:
+        """
+        Automatically generate farward func according to class name.
+
+        Returns:
+            Farward func, a string represent '{dir_path}/{file_name}:{func_name}'.
+        """
+        dir_path = os.path.dirname(os.path.abspath(__file__))
+        func_path = os.path.join(dir_path, "../kernel/gpu/fake_quant_per_layer_impl.cu")
+        func_name = "Custom" + self._get_custom_op_name()
+        if not os.path.exists(func_path):
+            error_str = f"For {self._get_custom_op_name()}, cu file not exist, the path is {func_path}"
+            logger.error(error_str)
+            raise RuntimeError(error_str)
+        logger.info(f"Custom op {self._get_custom_op_name()} func: {func_path}:{func_name}")
+        return func_path + ":" + func_name
```

## Comparing `mindspore_gs/ops/operations/gs_custom.py` & `mindspore_gs/ops/gs_custom.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """
 MindSpore golden stick base Custom op.
 """
-import os
+
 import functools
 import inspect
 import enum
 from typing import Union
 
 from mindspore.ops import Custom, DataType, CustomRegOp
 from mindspore import log as logger
@@ -246,26 +246,15 @@
     def _get_forward_func(self) -> str:
         """
         Automatically generate farward func according to class name.
 
         Returns:
             Farward func, a string represent '{dir_path}/{file_name}:{func_name}'.
         """
-        dir_path = os.path.dirname(os.path.abspath(__file__))
-        cu_file_name = GSCustom._get_lower_name(self._get_custom_op_name()) + "_impl.cu"
-        logger.info(f"Custom op {self._get_custom_op_name()} cu_file_name {cu_file_name}")
-        func_name = "Custom" + self._get_custom_op_name()
-        logger.info(f"Custom op {self._get_custom_op_name()} func_name {func_name}")
-        func_path = os.path.join(dir_path, "../kernel/gpu", cu_file_name)
-        logger.info(f"Custom op {self._get_custom_op_name()} func_path {func_path}")
-        if not os.path.exists(func_path):
-            error_str = f"For {self._get_custom_op_name()}, cu file not exist, the path is {func_path}"
-            logger.error(error_str)
-            raise RuntimeError(error_str)
-        return func_path + ":" + func_name
+        raise NotImplementedError
 
     @staticmethod
     def _get_lower_name(op_cls_name: str):
         """Get lower op cls name."""
         lower_name = ""
         for single_char in op_cls_name:
             if single_char.isupper():
@@ -290,15 +279,15 @@
 
     def _check_support_device_target(self, device_target_list: [str]):
         """check_support_device_target"""
         device_target = context.get_context('device_target')
         if device_target not in device_target_list:
             error_str = f"MindSpore Golden Stick op not support in current device {device_target}."
             logger.error(error_str)
-            raise NotImplementedError(error_str)
+            raise ValueError(error_str)
 
     def _get_custom_op_name(self) -> str:
         """_get_custom_op_name"""
         return self.__class__.__name__
 
     def _get_custom_attr(self, attr_name: str):
         """_get_custom_attr"""
```

## Comparing `mindspore_gs/ops/operations/min_max_update_perchannel.py` & `mindspore_gs/quantization/ops/operations/min_max_update_perchannel.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,19 +11,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """
 MindSpore golden stick simulated-quantization ops MinMaxUpdatePerChannel.
 """
+import os
+
 from mindspore.ops import DataType
+from mindspore import log as logger
 from mindspore.ops.functional import zeros_like
-from mindspore._checkparam import Validator as validator
-from mindspore._checkparam import Rel
-from mindspore_gs.ops.operations import GSCustom, custom_op_attr_register
+from mindspore_gs.validator import Rel
+from mindspore_gs.validator import Validator as validator
+from mindspore_gs.ops import GSCustom, custom_op_attr_register
 
 
 class MinMaxUpdatePerChannel(GSCustom):
     r"""
      Updates min and max per channel.
 
     Args:
@@ -88,7 +91,24 @@
         """set_op_output_names"""
         return "min_out", "max_out"
 
     def _get_op_dtype_formats(self) -> [[DataType]]:
         """set_op_dtype_format"""
         return [[DataType.F32_Default, DataType.F32_Default, DataType.F32_Default, DataType.F32_Default,
                  DataType.F32_Default]]
+
+    def _get_forward_func(self) -> str:
+        """
+        Automatically generate farward func according to class name.
+
+        Returns:
+            Farward func, a string represent '{dir_path}/{file_name}:{func_name}'.
+        """
+        dir_path = os.path.dirname(os.path.abspath(__file__))
+        func_path = os.path.join(dir_path, "../kernel/gpu/min_max_update_per_channel_impl.cu")
+        func_name = "Custom" + self._get_custom_op_name()
+        if not os.path.exists(func_path):
+            error_str = f"For {self._get_custom_op_name()}, cu file not exist, the path is {func_path}"
+            logger.error(error_str)
+            raise RuntimeError(error_str)
+        logger.info(f"Custom op {self._get_custom_op_name()} func: {func_path}:{func_name}")
+        return func_path + ":" + func_name
```

## Comparing `mindspore_gs/ops/operations/min_max_update_perlayer.py` & `mindspore_gs/quantization/ops/operations/grad_operations/fake_quant_perlayer_grad.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,83 +9,78 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """
-MindSpore golden stick simulated-quantization ops MinMaxUpdatePerLayer.
+MindSpore golden stick simulated-quantization ops FakeQuantPerLayerGrad.
 """
+import os
+
 from mindspore.ops import DataType
-from mindspore.ops.functional import zeros_like
-from mindspore._checkparam import Validator as validator
-from mindspore._checkparam import Rel
-from mindspore_gs.ops.operations import GSCustom, custom_op_attr_register
-
-
-class MinMaxUpdatePerLayer(GSCustom):
-    r"""
-    Updates min and max per layer.
-
-    Args:
-        ema (bool): Uses EMA algorithm update value min and max. Default: False.
-        ema_decay (int) : EMA algorithm decay parameter. Default: 0.999.
-
-    Inputs:
-        - **x** (Tensor) : float32 Tensor representing the shape of the output tensor.
-        - **min** (Tensor) : Value of the min range of the input data x.
-        - **max** (Tensor) : Value of the max range of the input data x.
-
-    Outputs:
-        - Tensor: Simulates quantize tensor of x.
-
-    Examples:
-        >>> import numpy as np
-        >>> from mindspore.common import dtype as mstype
-        >>> from mindspore import Tensor
-        >>> input_tensor = Tensor(np.random.rand(3, 16, 5, 5), mstype.float32)
-        >>> min_tensor = Tensor(np.array([-6]), mstype.float32)
-        >>> max_tensor = Tensor(np.array([6]), mstype.float32)
-        >>> output_tensor = MinMaxUpdatePerLayer(num_bits=8)(input_tensor, min_tensor, max_tensor)
+from mindspore import log as logger
+from mindspore_gs.validator import Validator as validator
+from mindspore_gs.ops import GSCustom, custom_op_attr_register
+
+
+class FakeQuantPerLayerGrad(GSCustom):
+    """
+    FakeQuantPerLayerGrad.
     """
     support_quant_bit = [4, 7, 8]
 
     @custom_op_attr_register
-    def __init__(self, ema=False, ema_decay=0.999):
-        """Initialize FakeQuantMinMaxPerLayerUpdate OP"""
+    def __init__(self,
+                 num_bits=8,
+                 quant_delay=0,
+                 symmetric=False,
+                 narrow_range=False):
+        """Initialize FakeQuantPerLayerGrad OP"""
         support_device = ["GPU"]
         self._check_support_device_target(support_device)
-        if ema and not ema_decay:
+        if num_bits not in self.support_quant_bit:
             raise ValueError(
-                f"For '{self._get_custom_op_name()}' attr \'ema\' and \'ema_decay\' should set together.")
+                f"For '{self._get_custom_op_name()}' attr \'num_bits\' is not support.")
 
-        validator.check_value_type('ema', ema, (bool,), self._get_custom_op_name())
-        validator.check_float_range(ema_decay, 0, 1, Rel.INC_BOTH, 'ema_decay', self._get_custom_op_name())
+        validator.check_value_type('symmetric', symmetric, (bool,), self._get_custom_op_name())
+        validator.check_value_type('narrow_range', narrow_range, (bool,), self._get_custom_op_name())
+        validator.check_positive_int(num_bits, 'num_bits', self._get_custom_op_name())
+        validator.check_non_negative_int(quant_delay, 'quant_delay', self._get_custom_op_name())
 
-    def _infer_shape(self, x, x_min, x_max):
+    def _infer_shape(self, dx, x, x_min, x_max):
         """infer_shape."""
-        return x_min, x_max
+        return x
 
-    def _infer_dtype(self, x, x_min, x_max):
+    def _infer_dtype(self, dx, x, x_min, x_max):
         """infer_dtype."""
-        return x_min, x_max
-
-    def _get_op_bprop(self):
-        """op_bprop."""
-
-        def bprop(x, x_min, x_max, out, dout):
-            """bprop."""
-            return zeros_like(x), zeros_like(x_min), zeros_like(x_max)
-        return bprop
+        return x
 
     def _get_op_input_names(self) -> (str,):
-        """set_op_input_names"""
-        return "x", "min_val", "max_val"
+        """_get_op_input_names"""
+        return "gradient", "x", "min_val", "max_val"
 
     def _get_op_output_names(self) -> (str,):
-        """set_op_output_names"""
-        return "min_out", "max_out"
+        """_get_op_output_names"""
+        return ("output",)
 
     def _get_op_dtype_formats(self) -> [[DataType]]:
         """set_op_dtype_format"""
-        return [[DataType.F32_Default, DataType.F32_Default, DataType.F32_Default, DataType.F32_Default,
-                 DataType.F32_Default]]
+        return [[DataType.F32_Default, DataType.F32_Default,
+                 DataType.F32_Default, DataType.F32_Default, DataType.F32_Default]]
+
+    def _get_forward_func(self) -> str:
+        """
+        Automatically generate farward func according to class name.
+
+        Returns:
+            Farward func, a string represent '{dir_path}/{file_name}:{func_name}'.
+        """
+        dir_path = os.path.dirname(os.path.abspath(__file__))
+        func_path = os.path.join(dir_path, "../../kernel/gpu/fake_quant_per_layer_grad_impl.cu")
+        func_name = "Custom" + self._get_custom_op_name()
+        if not os.path.exists(func_path):
+            error_str = f"For {self._get_custom_op_name()}, cu file not exist, the path is {func_path}"
+            logger.error(error_str)
+            raise RuntimeError(error_str)
+        logger.info(f"Custom op {self._get_custom_op_name()} func: {func_path}:{func_name}")
+        return func_path + ":" + func_name
```

## Comparing `mindspore_gs/ops/operations/grad_operations/__init__.py` & `mindspore_gs/datasets/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,20 @@
-# Copyright 2022 Huawei Technologies Co., Ltd
+# Copyright 2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """
-MindSpore golden stick grad operations.
+MindSpore golden stick datasets.
 """
 
-from .fake_quant_perlayer_grad import FakeQuantPerLayerGrad
-from .fake_quant_perchannel_grad import FakeQuantPerChannelGrad
-
-__all__ = [
-    "FakeQuantPerLayerGrad",
-    "FakeQuantPerChannelGrad"
-]
+from .wikitext2 import create_wikitext_dataset
+from .squad import create_squad_dataset
```

## Comparing `mindspore_gs/ops/operations/grad_operations/fake_quant_perchannel_grad.py` & `mindspore_gs/quantization/ops/operations/grad_operations/fake_quant_perchannel_grad.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,17 +11,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """
 MindSpore golden stick simulated-quantization ops FakeQuantPerChannelGrad.
 """
+import os
+
 from mindspore.ops import DataType
-from mindspore._checkparam import Validator as validator
-from mindspore_gs.ops.operations import GSCustom, custom_op_attr_register
+from mindspore import log as logger
+from mindspore_gs.validator import Validator as validator
+from mindspore_gs.ops import GSCustom, custom_op_attr_register
 
 
 class FakeQuantPerChannelGrad(GSCustom):
     """
     FakeQuantPerChannelGrad.
     """
     support_quant_bit = [4, 7, 8]
@@ -60,7 +63,24 @@
         """set_op_output_names"""
         return ("output",)
 
     def _get_op_dtype_formats(self) -> [[DataType]]:
         """set_op_dtype_format"""
         return [[DataType.F32_Default, DataType.F32_Default,
                  DataType.F32_Default, DataType.F32_Default, DataType.F32_Default]]
+
+    def _get_forward_func(self) -> str:
+        """
+        Automatically generate farward func according to class name.
+
+        Returns:
+            Farward func, a string represent '{dir_path}/{file_name}:{func_name}'.
+        """
+        dir_path = os.path.dirname(os.path.abspath(__file__))
+        func_path = os.path.join(dir_path, "../../kernel/gpu/fake_quant_per_channel_grad_impl.cu")
+        func_name = "Custom" + self._get_custom_op_name()
+        if not os.path.exists(func_path):
+            error_str = f"For {self._get_custom_op_name()}, cu file not exist, the path is {func_path}"
+            logger.error(error_str)
+            raise RuntimeError(error_str)
+        logger.info(f"Custom op {self._get_custom_op_name()} func: {func_path}:{func_name}")
+        return func_path + ":" + func_name
```

## Comparing `mindspore_gs-0.3.0.dist-info/LICENSE` & `mindspore_gs-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mindspore_gs-0.3.0.dist-info/METADATA` & `mindspore_gs-0.4.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: mindspore-gs
-Version: 0.3.0
+Version: 0.4.0
 Summary: A MindSpore model optimization algorithm set..
 Home-page: https://www.mindspore.cn
 Author: The MindSpore Authors
 Author-email: contact@mindspore.cn
 License: Apache 2.0
 Keywords: mindspore optimization quantization golden-stick
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
@@ -19,13 +18,12 @@
 Classifier: Programming Language :: C++
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
+License-File: LICENSE
+License-File: NOTICE
 Requires-Dist: numpy (>=1.17.0)
 Requires-Dist: scipy (>=1.5.2)
 
-UNKNOWN
-
-
```

## Comparing `mindspore_gs-0.3.0.dist-info/RECORD` & `mindspore_gs-0.4.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,84 +1,120 @@
-mindspore_gs/.commit_id,sha256=T3hNyQsnQhRc3JnMzHcobZeLvPag01tH92GDUttshRY,82
-mindspore_gs/__init__.py,sha256=IYkNOOMK4L0ql4U1BEZP7DL39Be0efV2YbnBBRtEc9w,1156
-mindspore_gs/comp_algo.py,sha256=Z9QNoI9iBwDtx5hTu0iOpHGzK1iuJkmLIaHAOqoO_0g,9205
-mindspore_gs/net_transform.py,sha256=bo4T_hO64NTWH0hxBVZ7lhtkJUXZmiHSK94RmS4cq5g,4088
-mindspore_gs/version.py,sha256=P73ttHZEtVRzXeTWbBl7kxGoVZaJ-D5jaexnHVlE8EI,2584
-mindspore_gs/ops/__init__.py,sha256=oeWSNOWUIR35LiPw_W4opqzOTFvzTy8Mbuu_ts0hIsw,703
-mindspore_gs/ops/common/__init__.py,sha256=R408mgnHOu4M5V7HhW2_EsVT85J6EgF9hyqXP5lSrd8,710
-mindspore_gs/ops/common/quant_op_utils.py,sha256=9gWn9t-m3BZ1RMj8tkSczUOIe7MBiC-yhHbtYh3Q3VA,1005
-mindspore_gs/ops/kernel/gpu/fake_quant_impl.cuh,sha256=F3siV5cesPO-A1rIVUig4tZ6gdTP3i-5dMrF03-PE8A,5210
-mindspore_gs/ops/kernel/gpu/fake_quant_per_channel_grad_impl.cu,sha256=EOWwjsyQjBSwMGfm67X6tTD4pX9hPHqR48pNjZ4CeKw,5032
-mindspore_gs/ops/kernel/gpu/fake_quant_per_channel_impl.cu,sha256=l5E6GkoEaH5vfvCtdHqmgDFz25y3uhLBQYT3BxBL_YQ,6210
-mindspore_gs/ops/kernel/gpu/fake_quant_per_layer_grad_impl.cu,sha256=McUnKDdCoNqRvbDLcHNrPoaK9VpkMhEMldld7w1xQUw,4650
-mindspore_gs/ops/kernel/gpu/fake_quant_per_layer_impl.cu,sha256=79OMyLffx7PPCck3XGieBeqdhvrLI0aFkAZzg1UFsEI,5350
-mindspore_gs/ops/kernel/gpu/min_max_update_per_channel_impl.cu,sha256=hOp3yX_8_6aDYsAGm_QmE_4-tIzsM_5HWdxFhD7pki4,4199
-mindspore_gs/ops/kernel/gpu/min_max_update_per_layer_impl.cu,sha256=T-1x1dS4wOw4jyRc7atpsi9017xrbEnaOsBzi11NSWc,4204
-mindspore_gs/ops/kernel/gpu/aot/custom_aot_extra.h,sha256=RgdyOewRgmwfNbDaJIm8Mttm3bRoHSYuv5sydGKew-E,2961
-mindspore_gs/ops/nn/__init__.py,sha256=mIh5_SP95UaoNiP6fCY946uglE0IEw8E1lHX7U1zq08,1433
-mindspore_gs/ops/nn/act_quant.py,sha256=or0gtXTJr0tRCk3QdtK-PTfd-Hh5TDbPjSArvMWGX4M,5519
-mindspore_gs/ops/nn/batchnorm_fold_cell.py,sha256=pZJL_T76mwn-gMz6vdG6AWB2D72IqHLkkQ4JwNvnakQ,3698
-mindspore_gs/ops/nn/conv2d_bn_fold_quant.py,sha256=kowUoaDqjmUFJ8qkl3JPGEFrSoL1pCbSZaoDprUPrSI,15276
-mindspore_gs/ops/nn/conv2d_bn_fold_quant_one_conv.py,sha256=R2N5aaN-Io84sWDcEXI-o1giE-X5fGjlu0jGAVtUh8o,14582
-mindspore_gs/ops/nn/conv2d_bn_without_fold_quant.py,sha256=QzLBY3bOJHwM48ucwZfjbjU8rPpoazGOUctwZcXkydU,10469
-mindspore_gs/ops/nn/conv2d_quant.py,sha256=s7UxmAZ2aiJTQPI51e029tjjcqrjH45GSlRB9FPrCKY,10454
-mindspore_gs/ops/nn/dense_quant.py,sha256=lsSPVKOK-kthXTWUcZEU6mLS30PFEYtZ8yIfytlSnhE,8550
-mindspore_gs/ops/nn/fake_quant_with_min_max_observer.py,sha256=6lO1pw54MdWjSGexPQCJu_oP9QbdFxMCdxXMU_i-iFY,21743
-mindspore_gs/ops/nn/mul_quant.py,sha256=pTxkfUcZjLZ7SNp1j3HgIVtFT_EUCPEYHhRQHIELAU8,3646
-mindspore_gs/ops/nn/tensor_add_quant.py,sha256=QabwYhAdFeEiGsgObDItrKXaUU5ghPBVWNjTSkuaeQU,3693
-mindspore_gs/ops/operations/__init__.py,sha256=-ZwraQbhv9cBJK5I_Yut0zqJumHwxvVsg6WzIZPDdK8,1165
-mindspore_gs/ops/operations/fake_quant_perchannel.py,sha256=FhcXgzoRnWaPUF8km824KAdZhUUnhLF1zQW_dUDdoEA,5702
-mindspore_gs/ops/operations/fake_quant_perlayer.py,sha256=PBN7uJtcKpOxBh4ZzpkdieilsxHgMk7W0VuPWSzWuXc,5350
-mindspore_gs/ops/operations/gs_custom.py,sha256=dvA1KxYFZtBJ3OCHDT8rsA18qU2pWn-y-CVTtTiZm4k,14042
-mindspore_gs/ops/operations/min_max_update_perchannel.py,sha256=29e9DyDPHBaLJKSGKfeq2eWmEdM38cJ39T4C4Z2cKZE,3821
-mindspore_gs/ops/operations/min_max_update_perlayer.py,sha256=N5nmOinUDugrxwXld5A-dXKJ1Qmf0JRYqwVU9L01M0k,3535
-mindspore_gs/ops/operations/grad_operations/__init__.py,sha256=l68Zs1VXQXvHKkoJbu_ha5oVg51HjdCjJPCVBhMJdQ0,914
-mindspore_gs/ops/operations/grad_operations/fake_quant_perchannel_grad.py,sha256=E8IOSACQ-yQtDohd7Hu_k6EB653gaZMoPp_-7m7px_U,2615
-mindspore_gs/ops/operations/grad_operations/fake_quant_perlayer_grad.py,sha256=EizzGJBfiGY31zDPHkKqAoozJnUaiRV5EVyQlkx_ET4,2575
-mindspore_gs/pruner/__init__.py,sha256=iVFATLTTsDU8TwNFPuHn3sGZZ-37JtcZq-5LmQ4e_fc,982
+mindspore_gs/.commit_id,sha256=6h4iykP6C8revc9ygDJVixjhJMa5K1yqjxw2yWfy4Pc,70
+mindspore_gs/__init__.py,sha256=SdJt3aMRCSSPHKO6pWz0HBX9_rvIzmSMKaOufpp13Y0,1412
+mindspore_gs/comp_algo.py,sha256=m3XTVklMHn09XdH61LfogpZ-C4JCR26fc2wTEk-w3sg,9365
+mindspore_gs/net_transform.py,sha256=I2qcrInTACpDobCuLdQLqEyPHGbVxTPsN5M9IpN_6cQ,6007
+mindspore_gs/validator.py,sha256=LSwxJ-RpqoWQh6lXtuCG1QYBKwfdeXQKEFUvuKQV_eY,916
+mindspore_gs/version.py,sha256=lzYNN87VNoUhWd_7X_BuESYNa8hGLQtgafdM37qRy0U,2627
+mindspore_gs/common/__init__.py,sha256=jOTYNhaNnhaGO6taawh3pwtHiRgiPHorGB38Ri2JiKM,774
+mindspore_gs/common/config.py,sha256=Uo9_O3wF2dNrG58q_YkFNYlGATDljNIE9QJovJTV6n4,2010
+mindspore_gs/common/gs_enum.py,sha256=P0oQcbA4oo7djbSplM-E_IKwBh0oWGt6a7BaqZ-itIY,1486
+mindspore_gs/common/register.py,sha256=VOAoYr8nIFr3D9Ah3FX8OKz8KnhKCqfmc99Vy0Dassg,2079
+mindspore_gs/common/utils.py,sha256=Sthr73TLGqv4JjpVUa5XHy5h8zcoVzw1tBVlE9yCP7o,1942
+mindspore_gs/datasets/__init__.py,sha256=DkG2DeaNfkLmeuEcaxGOVMH9cuqdiRoGFiBZ5B-Rzf0,796
+mindspore_gs/datasets/squad.py,sha256=7Hn1V1QOP18Qq8IhFGm1tsJXMC97E_qISo0g4RT92u8,6237
+mindspore_gs/datasets/wikitext2.py,sha256=2rVL2o2ebHBULnY_Iaqfi3oUJwaPmUQncg4B2Mrk_Ew,4230
+mindspore_gs/ghost/__init__.py,sha256=869WWV0yyA_XGFrSXQcHff7H4EzOuSokC_qsF9H5fwg,874
+mindspore_gs/ghost/ghost.py,sha256=DjVY68UnlkbJWXT7nVCkmskwppNJHQc9e1F74PFyomo,9654
+mindspore_gs/ops/__init__.py,sha256=SH9QmyFzUYKFz_CzuwPYybRkS18yxBSvGWDeBw5o04M,822
+mindspore_gs/ops/gs_custom.py,sha256=UFC1pOaC-9YnMCePPg7JqOS6j0Qis60_ZvUed9AudeM,13247
+mindspore_gs/pruner/__init__.py,sha256=FvvgQQB-gU5jMj87Ne24PzDaqLY3FQUcccEuO8-y53k,995
+mindspore_gs/pruner/heads/__init__.py,sha256=lp03VXdBdZKxOZZZPRe94q7hV8Aosob3tSmziWqphsw,843
+mindspore_gs/pruner/heads/abstract.py,sha256=WDk7Of_T0yPmIIXyfPpmOCjGWiBvOiGZ2pFRKNRHvvk,4351
+mindspore_gs/pruner/heads/factory.py,sha256=5D9nMCgQN1bL8IoOsgFw2uQCUMFBiCu7uhWpiR8Bru0,1860
+mindspore_gs/pruner/heads/supported.py,sha256=qpF3gWduAOxfnlQBlzAyuGl2tSP4geCtInJZYUIfrhY,837
+mindspore_gs/pruner/heads/type.py,sha256=jjGurRP7kLFB1yLWH9j1_9nZxcrfz8Ke5pCyPuQmNfU,806
+mindspore_gs/pruner/heads/lrp/__init__.py,sha256=6BnJBGZDFb0RAiSXrzj4FqErbq_-1D4jKjrScV4WxBo,763
+mindspore_gs/pruner/heads/lrp/abstract_lrp.py,sha256=sa6WBLlkKcJnmTD9iP5fp4iEH4LjZoCanmGyJLvFwuI,3095
+mindspore_gs/pruner/heads/lrp/utils.py,sha256=bNllrmwP00mfBOHzyqbspw64Em-SyznwxTtFqWfyuiQ,10973
+mindspore_gs/pruner/ops/__init__.py,sha256=32nhAjzXHh5EqX6fJRbO3sgw2NU1bNFQXCTpggDmyt4,892
+mindspore_gs/pruner/ops/masked_cell.py,sha256=Rc65_yryCjmkOhitIMpvmuivL4lw_-2Ose_yNDaEmUU,3732
+mindspore_gs/pruner/ops/masked_conv2d.py,sha256=pP7Jd4LvbatZVMlCIxz-5Zj-xhrbv6dHQVJ6pzsM1-o,2019
+mindspore_gs/pruner/ops/masked_dense.py,sha256=vaofNOsWetEr4_9jEPRb0l5ph-3ig5ZdMEz3J5HNtRA,2011
 mindspore_gs/pruner/scop/__init__.py,sha256=Rm6O-m7hMSQtPO5szc8jtcG4r8p1ZL1e0f1XcWsFBv8,833
-mindspore_gs/pruner/scop/scop_pruner.py,sha256=27RfFEOLLAseaOzbyVn0c5yPGqpImSVFsVYo_dJF4IU,22191
+mindspore_gs/pruner/scop/scop_pruner.py,sha256=AnCzjSlYRrTDBaIDD1iklnEraRw1sx87DzAn-gs_sTo,22203
 mindspore_gs/pruner/uni_pruning/__init__.py,sha256=h9R0IxJTlINhx2CN2qJy9-Q-GUNTkU5FLU7BjsRbHMk,768
-mindspore_gs/pruner/uni_pruning/graph_analyzer_mindir.py,sha256=3489DOD6fjHU7WivsP9igW2X4hqrO5-6SmRNObVYJDk,14990
-mindspore_gs/pruner/uni_pruning/uni_pruner.py,sha256=-co3V-wW5aCca6zSb6mxudWQS0ebl9TBDW8z8oatsjs,12909
+mindspore_gs/pruner/uni_pruning/uni_pruner.py,sha256=SLRUWNNjW5I-3dCETJITrabFmSEHkySjjfnkabXm4Po,15494
+mindspore_gs/pruner/uni_pruning/unipruning_masked_layer.py,sha256=tEa73hth5bdRWcDIFqtH_v6Q4QS6_DdPUuV4nZOr1gw,6558
+mindspore_gs/pruner/uni_pruning/graph_analyzer/__init__.py,sha256=jTMVbFt8UQCTTAy56n3yY1s1V98oZAIY3JnBmkYFxiA,766
+mindspore_gs/pruner/uni_pruning/graph_analyzer/equichannel_group.py,sha256=1edM6JwpYGn-c4smvNKQcqqMDlTIWieHJmMk7NI8aVA,4197
+mindspore_gs/pruner/uni_pruning/graph_analyzer/graph.py,sha256=TzxocvjZjM__V5zQTE1Yws4evS_U9monfCaRV8eVWIc,5044
+mindspore_gs/pruner/uni_pruning/graph_analyzer/graph_analyzer.py,sha256=l-DeXtKyToQ9H-pJSfOGdJzSZlZgohoyQDC1vFAjSFs,6559
 mindspore_gs/pruner/uni_pruning/utils/__init__.py,sha256=biu-VFm8VhmcpNNalBkgJspYUxBQt5dpe4ebabG1zhI,1092
-mindspore_gs/pruner/uni_pruning/utils/importance_criteria.py,sha256=6ig26ws71V9ZuDD4FBjmufFO5G4si4TWzLsgPG53Sk4,3497
+mindspore_gs/pruner/uni_pruning/utils/importance_criteria.py,sha256=yp8xlZ4rxcjdqBbAjjccclGtJNhV-kdX3Q-xf_1Q7Hg,3495
 mindspore_gs/pruner/uni_pruning/utils/mask.py,sha256=WbuDKorNf0lThTEsYMR1VQGUL86PQ5U18Krxq6CVSa4,5658
-mindspore_gs/pruner/uni_pruning/utils/model_utils.py,sha256=DO0dF9w8zJzrEVtQgMtW-qo_DhXyVk_Cu_iM0D5RqKw,4484
+mindspore_gs/pruner/uni_pruning/utils/model_utils.py,sha256=Tc4eaRrHmLuTOlRBOI9MU8NfX8dsdWKDo4hHDJyNom0,4482
 mindspore_gs/pruner/uni_pruning/utils/prune.py,sha256=DIyHGXt1rG2hvrcIFFT1CxPvwyU8VMrlwwg-Y81G6mg,3900
-mindspore_gs/quantization/__init__.py,sha256=siupk22MBuUSzGFX52zJINs6Agr-qgkozaMC8K8ah5A,1019
-mindspore_gs/quantization/fake_quantizer.py,sha256=W9z5dbv27jj-KOiGB37okTpUPA6ebLFfhQEJc1B8LXQ,808
-mindspore_gs/quantization/layer_policy.py,sha256=nC-GzTDKQKzd-MeVuOtxYN1bwSe1USIlSUmWVzTPdu0,4061
-mindspore_gs/quantization/net_policy.py,sha256=bl4Q6pT4Auazm8jTn3wmPM9nSZgUHYyssRCQxhOMtN4,1690
-mindspore_gs/quantization/quant_utils.py,sha256=xkfDQG_Wg1lTZJHLjfERATkSvCkzemImp8jDAEGHRcs,8947
-mindspore_gs/quantization/quantization_aware_training.py,sha256=oKBA7FeCtk-U-vjXSY7hszu8gkuxVPh6D6yTMnXRnb4,8793
-mindspore_gs/quantization/quantize_wrapper_cell.py,sha256=aU2yBLjwGu9y0CeSGbd7MYlz15ih6V2FwuxP0vO6pJI,2869
+mindspore_gs/ptq/__init__.py,sha256=jAkMLA8IpGpWXY5ONFoy_DgDjQd9v2JMsTrLkVUTw-w,803
+mindspore_gs/ptq/convert_utils.py,sha256=EjddlLmWTlNch2ZIAa6SMrLYwHuRkmcUP7f2gtWb4vs,9769
+mindspore_gs/ptq/fake_quantizer.py,sha256=cGNw4WMWkghHc73eIGZzTa-HGAh6zOTKatWuTnu8O-k,9712
+mindspore_gs/ptq/processor.py,sha256=tQGhwzC2CRdYZscGra3eHkFkIJQcMaZQuy9L4_o5uog,1521
+mindspore_gs/ptq/ptq_config.py,sha256=oMyOfZ6bMkCla1ageAvMuHsSMG5Ed6gH_soHWFN5TKo,8405
+mindspore_gs/ptq/quant_cells.py,sha256=TVA4pewrACBnN61oABHepoDalMqnV2coFt-Mk2zRlkQ,10320
+mindspore_gs/ptq/round_to_nearest/__init__.py,sha256=4cAb0_tOB-ZEP4NRcslXrLIGJb13P6JlRFem74bALIQ,765
+mindspore_gs/ptq/round_to_nearest/round_to_nearest.py,sha256=y1k9MADkweqVIsjqi3JfevPTD2SnjE89gdOeyOjU7Zk,8436
+mindspore_gs/ptq/round_to_nearest/rtn_layer_policy.py,sha256=XEpQ1PjECZT-jQsulLKQsz1HqfGAgYU9s6Luu_aKMdI,5308
+mindspore_gs/ptq/round_to_nearest/rtn_net_policy.py,sha256=GIKspGOaZCEE_8_94BwMSZ8k-O-oO0or6eRggJI-pA4,1728
+mindspore_gs/quantization/__init__.py,sha256=R_uJ8NuC0hSNKlwugl7IKM7_IG4IIYa8jZrGWH4sov8,1019
+mindspore_gs/quantization/fake_quantizer.py,sha256=jwctdaLS9xc-Nh049lRhDlqGXaH8xMv_gZzFuKBcAmY,4741
+mindspore_gs/quantization/layer_policy.py,sha256=72NxnbN5IHFOkyrEXlBMWn0tmcWn9kvB3F0UJy53QWw,5614
+mindspore_gs/quantization/net_policy.py,sha256=HEfzFCrXOX91gmb9aH7N-3leY3W4WEEav3AuYDxIwa0,1684
+mindspore_gs/quantization/quant_cell.py,sha256=ofHf_6RhGVE8yFZ2bE25EpYIs_EMuRHfeoXSnuyruu4,4039
+mindspore_gs/quantization/quant_utils.py,sha256=jls18rqjP3JiHrPTi2ELbGSu6KQv7epvt8LrF02VzCc,13203
+mindspore_gs/quantization/quantization_aware_training.py,sha256=lTUvggr2rPDmeMS76DAbjQt2uo4M4PwCBtbBrHDGJhQ,7994
 mindspore_gs/quantization/transformer.py,sha256=xR7Lx14Uy73GIhxOmFG3Xn92qfyHsCZH_nKfoyuHWUk,4671
 mindspore_gs/quantization/learned_step_size_quantization/__init__.py,sha256=vtCMN_lE6I1Z70G3m7Qe_e_CUfJv9GVax4Oq_JYKYQc,887
-mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_fake_quantizers.py,sha256=-td4u7J5s-WoKxmdxXgNZO_sPgucgrIMD97xVQ4DGDY,6775
-mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_quantization_aware_training.py,sha256=SZ1CJchjXL3oAZEE8IqXtxlB52-HLKYbeumleTcnfHc,21841
+mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_fake_quantizers.py,sha256=E_eeq9NZUJTi3o9L3_YjRFfxnNCHpvqJezQX1eha8yY,8168
+mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_quantization_aware_training.py,sha256=EELNzgqeBZcFLfEb33kGPDGseSBgGHCXCR1dpTdV2OM,21769
 mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_quantization_config.py,sha256=G1Nhb-u1O4MS49t0dQq57YBua-ru_H9EHoWSuv6AKfE,1367
-mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_quantization_layer_policy.py,sha256=tQYwTxubGKhBFvjE68H9adg3zqu4bx0z4FreMbRRkqw,5482
-mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_quantization_net_policy.py,sha256=XdPi0Ig0DG86dgx8g7y85HWYNUGnkTclwe93o5HsN2M,1859
+mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_quantization_layer_policy.py,sha256=R4RRunFpqtIffEmDzUhEZlCHtnO-JKjhwK7IPnS4dfQ,6733
+mindspore_gs/quantization/learned_step_size_quantization/learned_step_size_quantization_net_policy.py,sha256=_rcfAqBvLwNzXnzRd791S9eZTRSQg9U2bLxbNvLzqlY,1687
+mindspore_gs/quantization/ops/__init__.py,sha256=dXruTBCwNG6YJp0iRK1nEdOQkQS40WlddXX8OM1NL8Y,723
+mindspore_gs/quantization/ops/kernel/gpu/fake_quant_impl.cuh,sha256=F3siV5cesPO-A1rIVUig4tZ6gdTP3i-5dMrF03-PE8A,5210
+mindspore_gs/quantization/ops/kernel/gpu/fake_quant_per_channel_grad_impl.cu,sha256=EOWwjsyQjBSwMGfm67X6tTD4pX9hPHqR48pNjZ4CeKw,5032
+mindspore_gs/quantization/ops/kernel/gpu/fake_quant_per_channel_impl.cu,sha256=l5E6GkoEaH5vfvCtdHqmgDFz25y3uhLBQYT3BxBL_YQ,6210
+mindspore_gs/quantization/ops/kernel/gpu/fake_quant_per_layer_grad_impl.cu,sha256=McUnKDdCoNqRvbDLcHNrPoaK9VpkMhEMldld7w1xQUw,4650
+mindspore_gs/quantization/ops/kernel/gpu/fake_quant_per_layer_impl.cu,sha256=79OMyLffx7PPCck3XGieBeqdhvrLI0aFkAZzg1UFsEI,5350
+mindspore_gs/quantization/ops/kernel/gpu/min_max_update_per_channel_impl.cu,sha256=hOp3yX_8_6aDYsAGm_QmE_4-tIzsM_5HWdxFhD7pki4,4199
+mindspore_gs/quantization/ops/kernel/gpu/min_max_update_per_layer_impl.cu,sha256=T-1x1dS4wOw4jyRc7atpsi9017xrbEnaOsBzi11NSWc,4204
+mindspore_gs/quantization/ops/kernel/gpu/aot/custom_aot_extra.h,sha256=RgdyOewRgmwfNbDaJIm8Mttm3bRoHSYuv5sydGKew-E,2961
+mindspore_gs/quantization/ops/nn/__init__.py,sha256=zwg3O0xE_0KXMM86G-fidi9mAw-2yDEF9DwnSWibtS4,1432
+mindspore_gs/quantization/ops/nn/act_quant.py,sha256=AcYodbKWucMpQwTrDfs-gcpEO_qf9Y60vpd33jDVIao,2639
+mindspore_gs/quantization/ops/nn/batchnorm_fold_cell.py,sha256=c_qXRpbIsZ1nB99hzhZPpPXKDYWmuCYxxNKqSoVHOdk,3698
+mindspore_gs/quantization/ops/nn/conv2d_bn_fold_quant.py,sha256=6BedFVMGhvgfZz4winqD30DFUT5S6VgIMG5zHnVsmEU,10281
+mindspore_gs/quantization/ops/nn/conv2d_bn_fold_quant_one_conv.py,sha256=5gIlNvoN1puJ5Or6YdIh_bYvFYf4DUyCP1rI6rCqH9U,11957
+mindspore_gs/quantization/ops/nn/conv2d_bn_without_fold_quant.py,sha256=VouZipJTEIQY2UOgGFB7hRAgs4vxGmdJfIQ6Q9vjgeI,8377
+mindspore_gs/quantization/ops/nn/conv2d_quant.py,sha256=b3N0q9MYLXWkxRu7Tf5Hwqy53MScNFQ3eup2I_8w-_g,5654
+mindspore_gs/quantization/ops/nn/dense_quant.py,sha256=6nC_wD_Yxr1AMkSBcZTEB7KWl9XdE8BM5-uoejNPPSU,6220
+mindspore_gs/quantization/ops/nn/fake_quant_with_min_max_observer.py,sha256=KsrbuosRs1RetMNcd643mZ7CVOARfFUwXAeYux5MHKE,21830
+mindspore_gs/quantization/ops/nn/mul_quant.py,sha256=OMlHzRNenlHkVhhmudLwIbd6mD2gicYcCRmoiWThoiw,3055
+mindspore_gs/quantization/ops/nn/tensor_add_quant.py,sha256=IcNvUcyl5KIMtRiU_sAWG532w8ThNWWWaG5M9gPaYeo,3101
+mindspore_gs/quantization/ops/operations/__init__.py,sha256=7l-aq4sG46_nKlwPxXYTxJrQPOTSNyS2R9NoH8Ekf10,1062
+mindspore_gs/quantization/ops/operations/fake_quant_perchannel.py,sha256=h4tU_KQFa9vK43ca7TG7tooE6dR7zF0tz86zdq07do8,6519
+mindspore_gs/quantization/ops/operations/fake_quant_perlayer.py,sha256=3aDF9zaEi98xDFnCnPvYkZaEWQt9HzdNAAOMsAmFVXw,6165
+mindspore_gs/quantization/ops/operations/min_max_update_perchannel.py,sha256=AeJwcGN8wGeGLQxvHA2qFvKkFZLMbGhaUK_TmiKiAfA,4669
+mindspore_gs/quantization/ops/operations/min_max_update_perlayer.py,sha256=qKbXNTRl30GCbNXYSAHC3G_jiMBk92h9__Wsipg0CkA,4381
+mindspore_gs/quantization/ops/operations/grad_operations/__init__.py,sha256=l68Zs1VXQXvHKkoJbu_ha5oVg51HjdCjJPCVBhMJdQ0,914
+mindspore_gs/quantization/ops/operations/grad_operations/fake_quant_perchannel_grad.py,sha256=B2gKhoEP0_bSoqaXMQsc97G6YCBRIU-bpuaEM2kqKoY,3466
+mindspore_gs/quantization/ops/operations/grad_operations/fake_quant_perlayer_grad.py,sha256=dIjNOaFYatVEGHlYrEW_6Rjcj27nMFGTKxo6s9hpIPk,3424
 mindspore_gs/quantization/simulated_quantization/__init__.py,sha256=Tyn9wzHOo2HGYSbFeBhEidG5P_tzL9Xbqi0wcM-X2yo,859
-mindspore_gs/quantization/simulated_quantization/combined.py,sha256=h3XHcdRvkW8dpG8eH2WOebrqpoduI2qbh1YK9pqZraA,5959
-mindspore_gs/quantization/simulated_quantization/simulated_fake_quantizers.py,sha256=qV5RLnDZd9Oo8HJkc3p8PA2zepMji2oAyib6qeQgTOA,9067
-mindspore_gs/quantization/simulated_quantization/simulated_quantization_aware_training.py,sha256=-rOcovbwGymkmKishHrQ0am6Fvu06xM5M3EEcQpGCXM,25779
-mindspore_gs/quantization/simulated_quantization/simulated_quantization_config.py,sha256=tVsNV23hPmclY-E8gu2JglWukpKDHeW_UAd4JUpdtjk,1600
-mindspore_gs/quantization/simulated_quantization/simulated_quantization_convert.py,sha256=tYqaY5t2K4yYbfyHJAvsBeIDGkX2kvTZCNH7A7gpu1w,7586
-mindspore_gs/quantization/simulated_quantization/simulated_quantization_layer_policy.py,sha256=OwCd8lwI-WZa_lYfg-BOj8X0mRWQtWqAbZA_S8My1SQ,6668
-mindspore_gs/quantization/simulated_quantization/simulated_quantization_net_policy.py,sha256=TeKtWbYwxYG5VKKINL6Z6XOcndHqSop3Vwv1UZWDRWk,3052
+mindspore_gs/quantization/simulated_quantization/combined.py,sha256=ApgF-saxVUx7kzw2m7docnHWovlPWbEfk4sXKVOsTk0,5537
+mindspore_gs/quantization/simulated_quantization/simulated_fake_quantizers.py,sha256=ELxcXvU6lEHoYYDYWXwoW6K9grN7Ib-83h1BLmXbhKE,9049
+mindspore_gs/quantization/simulated_quantization/simulated_quantization_aware_training.py,sha256=TwcHdsOfZy6GfZ5QoTo-wYOdUShtOmlJRmP2lgdlHRg,26050
+mindspore_gs/quantization/simulated_quantization/simulated_quantization_config.py,sha256=jEvu_WVTvscfG2Guw_pt79_SJfYwNTSu-efC9WsK7Qc,1610
+mindspore_gs/quantization/simulated_quantization/simulated_quantization_convert.py,sha256=R2L1LvDZfEa371p6cvtFNn54ZMS9I6ULXaYD2VPddMM,1760
+mindspore_gs/quantization/simulated_quantization/simulated_quantization_layer_policy.py,sha256=PVxYBx5qHK7C-AGpo8g5K1mjlIyt25Qq6q-Mia58vaY,7372
+mindspore_gs/quantization/simulated_quantization/simulated_quantization_net_policy.py,sha256=XUoFYLWSBQ_ghJBEPg5jL5CGq6RsQENyzNmM6hCT1lw,2761
 mindspore_gs/quantization/simulated_quantization/simulated_quantization_transforms.py,sha256=CET5V8xJfKtEnZMaDZYVLQvM2CYIOrbvwmB9Kh3BZuM,9319
 mindspore_gs/quantization/slb/__init__.py,sha256=w5hDFU9VTsbMw3Wxh4xmjSMDPXORj-jQipUXbzeG-T0,847
-mindspore_gs/quantization/slb/slb_fake_quantizer.py,sha256=tjdTuV2qlnOdHyUy0tYX8tbygwLBagtnYrxUhVqbMcw,8428
-mindspore_gs/quantization/slb/slb_layer_policy.py,sha256=9m2Dm9ekB_cu8fOMdvh4XKgbk2CVDAz_OZvZ3rUAHQU,4499
-mindspore_gs/quantization/slb/slb_net_policy.py,sha256=wVYYi7Deaorx7ZZoKeymZRha67q-C-NbgUj6LmeULsU,1551
-mindspore_gs/quantization/slb/slb_quant.py,sha256=kZbaR3nmIxL-L0MHOaC8BjfHEPId9_3VdXnCX3gpicc,10802
-mindspore_gs/quantization/slb/slb_quant_aware_training.py,sha256=cIFkwNB_6_DGLUaDKh4t7ZwosusJALOIlTZ7QQ8C1Xc,28645
-mindspore_gs/quantization/slb/slb_quant_config.py,sha256=Q255F5bLF2XJUu8NwMSd1NH_2LTZZEkNo1BvgwRN_GU,1409
-mindspore_gs/quantization/slb/slb_quant_convert.py,sha256=PCfy907zUgRwpQbSD3w7Pex7raF6XOnPmrTXvGqcCGA,8421
-mindspore_gs-0.3.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mindspore_gs-0.3.0.dist-info/METADATA,sha256=4itoCHNYFilP7BCOGox_PNYNRZieMMxlKO8ivpN0mmo,1123
-mindspore_gs-0.3.0.dist-info/NOTICE,sha256=qNj_5bU31CQXBp2V38APtQ8WY2dsVPPz-qbJ97aQSk0,67
-mindspore_gs-0.3.0.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mindspore_gs-0.3.0.dist-info/top_level.txt,sha256=hymvg_un-AxnquXo_c8jQrerSv3WVgt3Ia0XqbzPals,13
-mindspore_gs-0.3.0.dist-info/RECORD,,
+mindspore_gs/quantization/slb/slb_fake_quantizer.py,sha256=Li-Uh22nl7-7wHdy599nuavH_KcxQLO75g3-nWWoFcA,9745
+mindspore_gs/quantization/slb/slb_layer_policy.py,sha256=J5o6t0tql03C67xGYHVkmm2y_gQOdMM57NYgQ01_AOI,3871
+mindspore_gs/quantization/slb/slb_net_policy.py,sha256=Y-Rxyg_gifQxZEDUp1hw5XTYsKXsx-BJrsmChyUwfQA,1575
+mindspore_gs/quantization/slb/slb_quant.py,sha256=ZStONEbsV3RYILyab3UQawDX39lSY3lLY7H2o6l_p2w,8986
+mindspore_gs/quantization/slb/slb_quant_aware_training.py,sha256=SeChxpi4G01h58LLLIihGjhHt8Ak5sAtxct3uwlpYZg,28708
+mindspore_gs/quantization/slb/slb_quant_config.py,sha256=6n_LnsZVyLUCG8Y3WL00SliRdQcIVuvRIAGc7xjp1MQ,1419
+mindspore_gs/quantization/slb/slb_quant_convert.py,sha256=Js5QHyNBSajK37yOdSA_2O6RMcGtmFdap0gxpXfVTbg,2065
+mindspore_gs-0.4.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mindspore_gs-0.4.0.dist-info/METADATA,sha256=9aTGFeuJIm94mpTMwG8O1MI0AVRbZBee_3bSABJik0g,1138
+mindspore_gs-0.4.0.dist-info/NOTICE,sha256=qNj_5bU31CQXBp2V38APtQ8WY2dsVPPz-qbJ97aQSk0,67
+mindspore_gs-0.4.0.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+mindspore_gs-0.4.0.dist-info/top_level.txt,sha256=hymvg_un-AxnquXo_c8jQrerSv3WVgt3Ia0XqbzPals,13
+mindspore_gs-0.4.0.dist-info/RECORD,,
```

