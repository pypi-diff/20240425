# Comparing `tmp/tinyrl-0.3.1.tar.gz` & `tmp/tinyrl-0.4.0.tar.gz`

## Comparing `tinyrl-0.3.1.tar` & `tinyrl-0.4.0.tar`

### file list

```diff
@@ -1,294 +1,299 @@
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/__init__.py
--rw-r--r--   0        0        0    10546 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers.h
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl_tools.h
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/version.h
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_arm.h
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu.h
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_blas.h
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_mkl.h
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_openblas.h
--rw-r--r--   0        0        0    13873 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cuda.h
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_dummy.h
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_esp32.h
--rw-r--r--   0        0        0    35055 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_generic.h
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/persist.h
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/persist_code.h
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/arm.h
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu.h
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_accelerate.h
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_blas.h
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_mkl.h
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_openblas.h
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_tensorboard.h
--rw-r--r--   0        0        0     4838 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cuda.h
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/devices.h
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/dummy.h
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/esp32.h
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/generic.h
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arduino.h
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arm.h
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu.h
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu_tensorboard.h
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cuda.h
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_dummy.h
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_arm.h
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_cpu.h
--rw-r--r--   0        0        0     9859 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_cuda.h
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_dummy.h
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_esp32.h
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_generic.h
--rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/activation_functions.h
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/nn.h
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu.h
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_accelerate.h
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_blas.h
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mkl.h
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mux.h
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_openblas.h
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cuda.h
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_dummy.h
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_generic.h
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/persist.h
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/layers.h
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu.h
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_accelerate.h
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_blas.h
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_mkl.h
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_openblas.h
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cuda.h
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_dummy.h
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_generic.h
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/layer.h
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/operations_generic.h
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/layer.h
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu.h
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_accelerate.h
--rw-r--r--   0        0        0    10729 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_blas.h
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_mkl.h
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_openblas.h
--rw-r--r--   0        0        0    25276 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cuda.h
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_dummy.h
--rw-r--r--   0        0        0    18492 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_generic.h
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist.h
--rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist_code.h
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/cuda/kernels.h
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/dsp.h
--rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/opt.h
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/dsp.h
--rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/opt.h
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/operations_generic.h
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/categorical_cross_entropy/operations_generic.h
--rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_cuda.h
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_generic.h
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/adam.h
--rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_cuda.h
--rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_generic.h
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist.h
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist_code.h
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/operations_generic.h
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/sgd.h
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_cuda.h
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_generic.h
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/parameters.h
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist.h
--rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist_code.h
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/models.h
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_cpu.h
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_cuda.h
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_dummy.h
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_generic.h
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/persist.h
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/persist_code.h
--rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/network.h
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_cpu.h
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_cuda.h
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_dummy.h
--rw-r--r--   0        0        0    21337 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_generic.h
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist.h
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist_code.h
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/network.h
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_cpu.h
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_generic.h
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/network.h
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_cpu.h
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_generic.h
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/output_view/model.h
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/model.h
--rw-r--r--   0        0        0    12487 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/operations_generic.h
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist.h
--rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist_code.h
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/arm.h
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu.h
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate.h
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl.h
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mux.h
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas.h
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard.h
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cuda.h
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/dummy.h
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/esp32.h
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_1.h
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_2.h
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_3.h
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_1.h
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_2.h
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_3.h
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_1.h
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_2.h
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_3.h
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_1.h
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_2.h
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_3.h
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_1.h
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_2.h
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_3.h
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_1.h
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_2.h
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_3.h
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_1.h
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_2.h
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_3.h
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_1.h
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_2.h
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_3.h
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_1.h
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_2.h
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_3.h
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/persist/code.h
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_arm.h
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_cpu.h
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_cuda.h
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_dummy.h
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_esp32.h
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_generic.h
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/operations_generic.h
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/rl.h
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/algorithms.h
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_cpu.h
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_cpu_mkl.h
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_generic.h
--rw-r--r--   0        0        0    19878 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic.h
--rw-r--r--   0        0        0    17846 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic_extensions.h
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/ppo.h
--rw-r--r--   0        0        0     5902 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/config.h
--rw-r--r--   0        0        0     5869 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/operations_generic.h
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/state.h
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu.h
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_accelerate.h
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_mkl.h
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_mux.h
--rw-r--r--   0        0        0     8159 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cuda.h
--rw-r--r--   0        0        0    34738 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_generic.h
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/sac.h
--rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/config.h
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_cpu.h
--rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_generic.h
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/state.h
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu.h
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_accelerate.h
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_mkl.h
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_mux.h
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cuda.h
--rw-r--r--   0        0        0    21772 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_generic.h
--rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/td3.h
--rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/config.h
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/operations_generic.h
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/state.h
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/components.h
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu.h
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu_accelerate.h
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu_mkl.h
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_generic.h
--rw-r--r--   0        0        0     8459 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/off_policy_runner.h
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu.h
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_accelerate.h
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_mkl.h
--rw-r--r--   0        0        0    10566 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cuda.h
--rw-r--r--   0        0        0    16438 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic.h
--rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic_per_env.h
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/on_policy_runner.h
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu.h
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_accelerate.h
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_mkl.h
--rw-r--r--   0        0        0    12759 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic.h
--rw-r--r--   0        0        0     8590 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_extensions.h
--rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_per_env.h
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/persist.h
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_cpu.h
--rw-r--r--   0        0        0     8285 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_generic.h
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/persist.h
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/replay_buffer.h
--rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/operations_generic.h
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/persist.h
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/running_normalizer.h
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/environments.h
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_cpu.h
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_generic.h
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/acrobot.h
--rw-r--r--   0        0        0    11900 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/operations_generic.h
--rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/ui.h
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/car.h
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_cpu.h
--rw-r--r--   0        0        0    10589 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_generic.h
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_json.h
--rw-r--r--   0        0        0    68731 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/track.h
--rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/ui.h
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/README.MD
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ant.h
--rw-r--r--   0        0        0    30495 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/model.h
--rw-r--r--   0        0        0     8075 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/operations_cpu.h
--rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ui.h
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_cpu.h
--rw-r--r--   0        0        0     6053 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_generic.h
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/pendulum.h
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui.h
--rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui_xeus.h
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/loop.h
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/config.h
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/operations_generic.h
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/state.h
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/config.h
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/operations_cpu.h
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/state.h
--rw-r--r--   0        0        0     8701 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/utils/evaluation.h
--rw-r--r--   0        0        0    12912 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation.h
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation_analysis.h
--rw-r--r--   0        0        0    16728 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/ui_server/server.h
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/client.h
--rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_boost.h
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_cpu.h
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/persist.h
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/declarations_cpu.h
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_arm.h
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cpu.h
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cuda.h
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_dummy.h
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_esp32.h
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_generic.h
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/generic/integrators.h
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/generic/memcpy.h
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/generic/typing.h
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/generic/vector_operations.h
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_cuda.h
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_generic.h
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/interface/algorithms/ppo/ppo.h
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/interface/algorithms/sac/default.h
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/interface/algorithms/sac/template.h
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/interface/inference/inference.cpp
--rw-r--r--   0        0        0     7596 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/interface/python_environment/operations_cpu.h
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/interface/python_environment/python_environment.h
--rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/interface/training/training.cpp
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/src/__init__.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/src/accelerate.py
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/src/compile.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/src/link_accelerate.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/src/link_mkl.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/src/load_checkpoint.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/src/load_module.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/src/render.py
--rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 tinyrl-0.3.1/tinyrl/src/sac.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tinyrl-0.3.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 tinyrl-0.3.1/LICENSE
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 tinyrl-0.3.1/README.md
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 tinyrl-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 tinyrl-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/__init__.py
+-rw-r--r--   0        0        0    10546 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers.h
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl_tools.h
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/version.h
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_arm.h
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu.h
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_blas.h
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_mkl.h
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_openblas.h
+-rw-r--r--   0        0        0    13873 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cuda.h
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_dummy.h
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_esp32.h
+-rw-r--r--   0        0        0    36524 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_generic.h
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/persist.h
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/persist_code.h
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/arm.h
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu.h
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_accelerate.h
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_blas.h
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_mkl.h
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_openblas.h
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_tensorboard.h
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cuda.h
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/devices.h
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/dummy.h
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/esp32.h
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/generic.h
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arduino.h
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arm.h
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu.h
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu_tensorboard.h
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cuda.h
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_dummy.h
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_arm.h
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_cpu.h
+-rw-r--r--   0        0        0     9859 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_cuda.h
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_dummy.h
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_esp32.h
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_generic.h
+-rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/activation_functions.h
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/nn.h
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu.h
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_blas.h
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mkl.h
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mux.h
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_openblas.h
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cuda.h
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_dummy.h
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_generic.h
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/persist.h
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/layers.h
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu.h
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_blas.h
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_mkl.h
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cpu_openblas.h
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_cuda.h
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_dummy.h
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/operations_generic.h
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/layer.h
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/operations_generic.h
+-rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/layer.h
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu.h
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0    11332 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_blas.h
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_mkl.h
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_openblas.h
+-rw-r--r--   0        0        0    25276 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cuda.h
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_dummy.h
+-rw-r--r--   0        0        0    18492 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_generic.h
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist.h
+-rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist_code.h
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/cuda/kernels.h
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/dsp.h
+-rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/opt.h
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/dsp.h
+-rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/opt.h
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/operations_generic.h
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/categorical_cross_entropy/operations_generic.h
+-rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_cuda.h
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_generic.h
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/adam.h
+-rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_cuda.h
+-rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_generic.h
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist.h
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist_code.h
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/operations_generic.h
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/sgd.h
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_cuda.h
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_generic.h
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/parameters.h
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist.h
+-rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist_code.h
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/models.h
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_cpu.h
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_cuda.h
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_dummy.h
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/operations_generic.h
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/persist.h
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/persist_code.h
+-rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/network.h
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_cpu.h
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_cuda.h
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_dummy.h
+-rw-r--r--   0        0        0    21337 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_generic.h
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist.h
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist_code.h
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/network.h
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_cpu.h
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_generic.h
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/network.h
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_cpu.h
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_generic.h
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/output_view/model.h
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/model.h
+-rw-r--r--   0        0        0    12487 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/operations_generic.h
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist.h
+-rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist_code.h
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/arm.h
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu.h
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate.h
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl.h
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mux.h
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas.h
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard.h
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cuda.h
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/dummy.h
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/esp32.h
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_1.h
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_2.h
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_3.h
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_1.h
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_2.h
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_3.h
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_1.h
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_2.h
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_3.h
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_1.h
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_2.h
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_3.h
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_1.h
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_2.h
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_3.h
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_1.h
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_2.h
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_3.h
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_1.h
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_2.h
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_3.h
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_1.h
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_2.h
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_3.h
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_1.h
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_2.h
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_3.h
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/persist/code.h
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_arm.h
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_cpu.h
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_cuda.h
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_dummy.h
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_esp32.h
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_generic.h
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/operations_generic.h
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/rl.h
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/algorithms.h
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_cpu.h
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_cpu_mkl.h
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/operations_generic.h
+-rw-r--r--   0        0        0    21201 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic.h
+-rw-r--r--   0        0        0    17846 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic_extensions.h
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/ppo.h
+-rw-r--r--   0        0        0     5902 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/config.h
+-rw-r--r--   0        0        0     5906 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/operations_generic.h
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/state.h
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu.h
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_mkl.h
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cpu_mux.h
+-rw-r--r--   0        0        0     8159 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cuda.h
+-rw-r--r--   0        0        0    36332 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_generic.h
+-rw-r--r--   0        0        0     8221 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/sac.h
+-rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/config.h
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_cpu.h
+-rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_generic.h
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/state.h
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu.h
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_mkl.h
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cpu_mux.h
+-rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cuda.h
+-rw-r--r--   0        0        0    21772 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_generic.h
+-rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/td3.h
+-rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/config.h
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/operations_generic.h
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/state.h
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/components.h
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu.h
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_cpu_mkl.h
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/operations_generic.h
+-rw-r--r--   0        0        0     8533 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/off_policy_runner.h
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu.h
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_mkl.h
+-rw-r--r--   0        0        0    10566 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cuda.h
+-rw-r--r--   0        0        0    16438 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic.h
+-rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic_per_env.h
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/on_policy_runner.h
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu.h
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_accelerate.h
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_mkl.h
+-rw-r--r--   0        0        0    12759 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic.h
+-rw-r--r--   0        0        0     8590 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_extensions.h
+-rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_per_env.h
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/persist.h
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_cpu.h
+-rw-r--r--   0        0        0     8285 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_generic.h
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/persist.h
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/replay_buffer.h
+-rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/operations_generic.h
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/persist.h
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/running_normalizer.h
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/environments.h
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_cpu.h
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_generic.h
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/acrobot.h
+-rw-r--r--   0        0        0    11982 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/operations_generic.h
+-rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/ui.h
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/car.h
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_cpu.h
+-rw-r--r--   0        0        0    10667 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_generic.h
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_json.h
+-rw-r--r--   0        0        0    68731 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/track.h
+-rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/ui.h
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/README.MD
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ant.h
+-rw-r--r--   0        0        0    30495 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/model.h
+-rw-r--r--   0        0        0     8075 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/operations_cpu.h
+-rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ui.h
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_cpu.h
+-rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_generic.h
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/pendulum.h
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui.h
+-rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui_xeus.h
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/loop.h
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/config.h
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/operations_generic.h
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/state.h
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/config.h
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/operations_cpu.h
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/state.h
+-rw-r--r--   0        0        0     8946 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/utils/evaluation.h
+-rw-r--r--   0        0        0    12912 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation.h
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation_analysis.h
+-rw-r--r--   0        0        0    16728 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/ui_server/server.h
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/client.h
+-rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_boost.h
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_cpu.h
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/persist.h
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/declarations_cpu.h
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_arm.h
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cpu.h
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cuda.h
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_dummy.h
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_esp32.h
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_generic.h
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/generic/integrators.h
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/generic/memcpy.h
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/generic/typing.h
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/generic/vector_operations.h
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_cuda.h
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_generic.h
+-rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/interface/algorithms/ppo/template.h
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/interface/algorithms/sac/template.h
+-rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/interface/algorithms/td3/template.h
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/interface/inference/inference.cpp
+-rw-r--r--   0        0        0     8007 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/interface/python_environment/operations_cpu.h
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/interface/python_environment/python_environment.h
+-rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/interface/training/training.cpp
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/__init__.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/accelerate.py
+-rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/compile.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/link_accelerate.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/link_blas.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/link_mkl.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/load_checkpoint.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/load_module.py
+-rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/ppo.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/render.py
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/sac.py
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/td3.py
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/training.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 tinyrl-0.4.0/tinyrl/src/utils.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 tinyrl-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 tinyrl-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 tinyrl-0.4.0/README.md
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 tinyrl-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 tinyrl-0.4.0/PKG-INFO
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl_tools.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl_tools.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/version.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/version.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_arm.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu.h`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #pragma once
 #define RL_TOOLS_CONTAINERS_OPERATIONS_CPU_H
 
 #include "operations_generic.h"
 
 #include <iostream>
 #include <iomanip>
+#include <cstdlib>
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
     template<typename DEVICE, typename SPEC>
     void print(DEVICE& device, const Matrix<SPEC>& m){
         for(typename DEVICE::index_t row_i = 0; row_i < SPEC::ROWS; row_i++){
             for(typename DEVICE::index_t col_i = 0; col_i < SPEC::COLS; col_i++){
                 std::cout << std::fixed << std::setw(12) << std::setprecision(6) << get(m, row_i, col_i) << " ";
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_blas.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_blas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_openblas.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cpu_openblas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cuda.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_dummy.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_esp32.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/operations_generic.h`

 * *Files 6% similar despite different names*

```diff
@@ -35,44 +35,70 @@
 #endif
     }
     template<typename DEVICE, typename SPEC>
     void free(DEVICE& device, MatrixStatic<SPEC>& matrix){
         // free is a no-op for statically allocated matrices
     }
 
-#ifndef RL_TOOLS_DISABLE_DYNAMIC_MEMORY_ALLOCATIONS
+#if !defined(RL_TOOLS_DISABLE_DYNAMIC_MEMORY_ALLOCATIONS)
     template<typename DEVICE, typename SPEC>
     void malloc(DEVICE& device, MatrixDynamic<SPEC>& matrix){
+        using TI = typename DEVICE::index_t;
 #ifdef RL_TOOLS_DEBUG_CONTAINER_CHECK_MALLOC
         utils::assert_exit(device, matrix._data == nullptr, "Matrix is already allocated");
 #endif
+#ifndef RL_TOOLS_DISABLE_ALIGNED_MEMORY_ALLOCATIONS
+        static constexpr TI POINTER_SIZE = sizeof(void*);
+        static constexpr TI BYTE_ALIGNMENT = 64;
+        static constexpr TI ALIGNED_SIZE = SPEC::SIZE_BYTES + BYTE_ALIGNMENT + POINTER_SIZE;
+#else
+        static constexpr TI ALIGNED_SIZE = SPEC::SIZE_BYTES;
+#endif
 #ifdef RL_TOOLS_CONTAINERS_USE_MALLOC
-        matrix._data = (typename SPEC::T*) ::malloc(SPEC::SIZE_BYTES);
+        void* original_pointer = ::malloc(ALIGNED_SIZE);
+#else
+        char* original_pointer = new char[ALIGNED_SIZE];
+#endif
+#ifndef RL_TOOLS_DISABLE_ALIGNED_MEMORY_ALLOCATIONS
+        char* byte_pointer = static_cast<char*>(original_pointer) + POINTER_SIZE;
+        static_assert(sizeof(TI) >= sizeof(void*), "TI must be at least as large as a pointer");
+        char* aligned_byte_pointer = reinterpret_cast<char*>((reinterpret_cast<TI>(byte_pointer) + BYTE_ALIGNMENT - 1) & ~(BYTE_ALIGNMENT - 1));
+        char* original_pointer_storage = aligned_byte_pointer - POINTER_SIZE;
+        *((decltype(original_pointer)*)original_pointer_storage) = original_pointer;
+        matrix._data = reinterpret_cast<typename SPEC::T*>(aligned_byte_pointer);
 #else
-        matrix._data = (typename SPEC::T*)new char[SPEC::SIZE_BYTES];
+        matrix._data = reinterpret_cast<typename SPEC::T*>(original_pointer);
 #endif
+
+
         count_malloc(device, SPEC::SIZE_BYTES);
 
 #ifdef RL_TOOLS_DEBUG_CONTAINER_MALLOC_INIT_NAN
         for(typename SPEC::TI i = 0; i < SPEC::SIZE; i++){
             if constexpr(utils::typing::is_same_v<typename SPEC::T, float> || utils::typing::is_same_v<typename SPEC::T, double>){
                 matrix._data[i] = math::nan<typename SPEC::T>(device.math);
             }
         }
 #endif
     }
     template<typename DEVICE, typename SPEC>
     void free(DEVICE& device, MatrixDynamic<SPEC>& matrix){
+        using TI = typename DEVICE::index_t;
 #ifdef RL_TOOLS_DEBUG_CONTAINER_CHECK_MALLOC
         utils::assert_exit(device, matrix._data != nullptr, "Matrix has not been allocated");
 #endif
+        char* aligned_byte_pointer = reinterpret_cast<char*>(matrix._data);
+        static constexpr TI POINTER_SIZE = sizeof(void*);
+        char* original_pointer_storage = aligned_byte_pointer - POINTER_SIZE;
 #ifdef RL_TOOLS_CONTAINERS_USE_MALLOC
-        ::free(matrix._data);
+        void* original_pointer = *((void**)original_pointer_storage);
+        ::free(original_pointer);
 #else
-        delete matrix._data;
+        char* original_pointer = *((char**)original_pointer_storage);
+        delete original_pointer;
 #endif
         matrix._data = nullptr;
     }
 #endif
 
     template<typename SPEC>
     RL_TOOLS_FUNCTION_PLACEMENT constexpr typename SPEC::TI rows(const Matrix<SPEC>& m){
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/persist.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/containers/persist_code.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/containers/persist_code.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/arm.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/arm.h`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     }
     namespace math{
         struct ARM: arm::Base{
             static constexpr Type TYPE = Type::math;
         };
     }
     namespace random{
-        struct ARM: arm::Base{
+        struct ARM: devices::random::Generic<typename math::ARM>, arm::Base{
             static constexpr Type TYPE = Type::random;
         };
     }
     namespace logging{
         struct ARM: arm::Base{
             static constexpr Type TYPE = Type::logging;
         };
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu.h`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     }
     namespace math{
         struct CPU: cpu::Base{
             static constexpr Type TYPE = Type::math;
         };
     }
     namespace random{
-        struct CPU: cpu::Base{
+        struct CPU: devices::random::Generic<devices::math::CPU>, cpu::Base{
             static constexpr Type TYPE = Type::random;
         };
     }
     namespace logging{
         struct CPU: cpu::Base{
             static constexpr Type TYPE = Type::logging;
         };
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_accelerate.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_accelerate.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_blas.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_blas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_mkl.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_mkl.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_openblas.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_openblas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_tensorboard.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cpu_tensorboard.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/cuda.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/cuda.h`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     }
     namespace math{
         struct CUDA: cuda::Base{
             static constexpr Type TYPE = Type::math;
         };
     }
     namespace random{
-        struct CUDA: cuda::Base{
+        struct CUDA:devices::random::Generic<devices::math::CUDA>, cuda::Base{
             static constexpr Type TYPE = Type::random;
         };
     }
     namespace logging{
         struct CUDA: cuda::Base{
             static constexpr Type TYPE = Type::logging;
         };
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/devices.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/devices.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/dummy.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/dummy.h`

 * *Files 4% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 #include "../utils/generic/typing.h"
 #include "devices.h"
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools::devices{
     namespace dummy{
         struct Base{
             static constexpr DeviceId DEVICE_ID = DeviceId::Dummy;
-            using index_t = unsigned;
+            using index_t = unsigned long long;
             static constexpr index_t MAX_INDEX = -1;
         };
     }
     namespace math{
         struct Dummy: dummy::Base{
             static constexpr Type TYPE = Type::math;
         };
     }
     namespace random{
-        struct Dummy: dummy::Base{
+        struct Dummy:devices::random::Generic<devices::math::Dummy>, dummy::Base{
             static constexpr Type TYPE = Type::random;
             using State = unsigned;
         };
     }
     namespace logging{
         struct Dummy: dummy::Base{
             static constexpr Type TYPE = Type::logging;
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/devices/esp32.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/devices/esp32.h`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     }
     namespace math{
         struct ESP32: esp32::Base{
             static constexpr Type TYPE = Type::math;
         };
     }
     namespace random{
-        struct ESP32: esp32::Base{
+        struct ESP32:devices::random::Generic<devices::math::ESP32>, esp32::Base{
             static constexpr Type TYPE = Type::random;
         };
     }
     namespace logging{
         struct ESP32: esp32::Base{
             static constexpr Type TYPE = Type::logging;
         };
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arduino.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arduino.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arm.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu_tensorboard.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cpu_tensorboard.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cuda.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/logging/operations_dummy.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/logging/operations_dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_arm.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_cpu.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_cuda.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_dummy.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_esp32.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/math/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/math/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/activation_functions.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/activation_functions.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mux.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/operations_cpu_mux.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/layer.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/layer.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/concat_constant/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/layer.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/layer.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_accelerate.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_accelerate.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_blas.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_blas.h`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 #pragma once
 #define RL_TOOLS_NN_LAYERS_DENSE_OPERATIONS_CPU_BLAS_H
 
 #include "operations_cpu.h"
 #include "../../../utils/generic/memcpy.h"
 #include "../../../devices/cpu_blas.h"
 
+// extern "C" {
+//     void cblas_sgemm(const enum CBLAS_ORDER Order, const enum CBLAS_TRANSPOSE TransA, const enum CBLAS_TRANSPOSE TransB, const int M, const int N, const int K, const float alpha, const float *A, const int lda, const float *B, const int ldb, const float beta, float *C, const int ldc);
+//     void cblas_dgemm(const enum CBLAS_ORDER Order, const enum CBLAS_TRANSPOSE TransA, const enum CBLAS_TRANSPOSE TransB, const int M, const int N, const int K, const double alpha, const double *A, const int lda, const double *B, const int ldb, const double beta, double *C, const int ldc);
+// }
+
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
     template<typename DEV_SPEC, typename LAYER_SPEC, typename INPUT_SPEC, typename OUTPUT_SPEC>
     void evaluate(devices::CPU_BLAS<DEV_SPEC>& device, const nn::layers::dense::Layer<LAYER_SPEC>& layer, const Matrix<INPUT_SPEC>& input, Matrix<OUTPUT_SPEC>& output) {
         static_assert(nn::layers::dense::check_input_output<LAYER_SPEC, INPUT_SPEC, OUTPUT_SPEC>);
 
         // Warning do not use the same buffer for input and output!
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_mkl.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_mkl.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_openblas.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cpu_openblas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cuda.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist_code.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/persist_code.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/cuda/kernels.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/cuda/kernels.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/dsp.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/dsp.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/opt.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_arm/opt.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/dsp.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/dsp.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/opt.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/layers/dense/operations_esp32/opt.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/categorical_cross_entropy/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/categorical_cross_entropy/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_cuda.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/loss_functions/mse/operations_generic.h`

 * *Files 3% similar despite different names*

```diff
@@ -22,19 +22,20 @@
     }
     template<typename DEVICE, typename SPEC_A, typename SPEC_B, typename SPEC_DA>
     void gradient(DEVICE& device, Matrix<SPEC_A> a, Matrix<SPEC_B> b, Matrix<SPEC_DA> d_a, typename SPEC_A::T loss_weight = 1) {
         static_assert(containers::check_structure<SPEC_A, SPEC_B>);
         static_assert(containers::check_structure<SPEC_A, SPEC_DA>);
         using T = typename SPEC_A::T;
         using TI = typename SPEC_A::TI;
+        T constant = (T)2/((T)SPEC_A::ROWS * SPEC_A::COLS) * loss_weight;
         for(TI row_i = 0; row_i < SPEC_A::ROWS; row_i++) {
             for(TI col_i = 0; col_i < SPEC_A::COLS; col_i++) {
 //                TI index = row_i * SPEC_A::COLS + col_i;
                 T diff = get(a, row_i, col_i) - get(b, row_i, col_i);
-                set(d_a, row_i, col_i, 2*diff/(SPEC_A::ROWS * SPEC_A::COLS) * loss_weight);
+                set(d_a, row_i, col_i, diff * constant);
             }
         }
     }
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 
 #endif
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/adam.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/adam.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_cuda.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist_code.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/adam/persist_code.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/sgd.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/optimizers/sgd/sgd.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/parameters.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/parameters.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist_code.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn/parameters/persist_code.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/network.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/network.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist_code.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp/persist_code.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/network.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/network.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_normalized_unconditional_stddev/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/network.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/network.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/mlp_unconditional_stddev/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/output_view/model.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/output_view/model.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/model.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/model.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist_code.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/nn_models/sequential/persist_code.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/arm.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mux.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mux.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cuda.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/dummy.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/esp32.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_1.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/arm/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_1.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_1.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_2.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_accelerate/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_1.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_2.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_mkl/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_1.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_2.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 #include "../../version.h"
-#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_OPERATIONS_CPU_OPENBLAS_GROUP_1_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
+#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_OPERATIONS_CPU_OPENBLAS_GROUP_2_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
-#define RL_TOOLS_OPERATIONS_CPU_OPENBLAS_GROUP_1_H
-#if defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_OPERATIONS_CPU_OPENBLAS_GROUP_1)
-    #define RL_TOOLS_OPERATIONS_CPU_OPENBLAS_GROUP_1
-    #include <cblas.h>
-    #include "../../devices/cpu_openblas.h"
-    #include "../../utils/assert/declarations_cpu.h"
-    #include "../../math/operations_cpu.h"
-    #include "../../logging/operations_cpu.h"
+#define RL_TOOLS_OPERATIONS_CPU_OPENBLAS_GROUP_2_H
+#if defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_OPERATIONS_CPU_OPENBLAS_GROUP_2)
+    #define RL_TOOLS_OPERATIONS_CPU_OPENBLAS_GROUP_2
+    #include "../../utils/assert/operations_cpu.h"
+    #include "../../random/operations_cpu.h"
 #else
-    #error "Group 1 already imported"
+    #error "Group 2 already imported"
 #endif
 #endif
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_openblas/group_2.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_1.h`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #include "../../version.h"
-#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_OPERATIONS_CPU_OPENBLAS_GROUP_2_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
+#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_OPERATIONS_DUMMY_GROUP_1_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
-#define RL_TOOLS_OPERATIONS_CPU_OPENBLAS_GROUP_2_H
-#if defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_OPERATIONS_CPU_OPENBLAS_GROUP_2)
-    #define RL_TOOLS_OPERATIONS_CPU_OPENBLAS_GROUP_2
-    #include "../../utils/assert/operations_cpu.h"
-    #include "../../random/operations_cpu.h"
+#define RL_TOOLS_OPERATIONS_DUMMY_GROUP_1_H
+#if defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_OPERATIONS_DUMMY_GROUP_1)
+    #define RL_TOOLS_OPERATIONS_DUMMY_GROUP_1
+    #include "../../devices/dummy.h"
+    #include "../../math/operations_dummy.h"
+    #include "../../logging/operations_dummy.h"
 #else
-    #error "Group 2 already imported"
+    #error "Group 1 already imported"
 #endif
 #endif
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_1.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_2.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cpu_tensorboard/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_1.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/cuda/group_1.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_1.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_1.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #include "../../version.h"
-#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_OPERATIONS_DUMMY_GROUP_1_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
+#if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_OPERATIONS_ESP32_GROUP_1_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
-#define RL_TOOLS_OPERATIONS_DUMMY_GROUP_1_H
-#if defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_OPERATIONS_DUMMY_GROUP_1)
-    #define RL_TOOLS_OPERATIONS_DUMMY_GROUP_1
-    #include "../../devices/dummy.h"
-    #include "../../math/operations_dummy.h"
-    #include "../../logging/operations_dummy.h"
+#define RL_TOOLS_OPERATIONS_ESP32_GROUP_1_H
+#if defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_OPERATIONS_ESP32_GROUP_1)
+    #define RL_TOOLS_OPERATIONS_ESP32_GROUP_1
+    #include "../../devices/esp32.h"
+//    #include "../../utils/assert/declarations_esp32.h"
+    #include "../../math/operations_esp32.h"
+//    #include "../../logging/operations_esp32.h"
 #else
     #error "Group 1 already imported"
 #endif
 #endif
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_2.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/dummy/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_2.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/operations/esp32/group_2.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/persist/code.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/persist/code.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_arm.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_arm.h`

 * *Files 18% similar despite different names*

```diff
@@ -44,29 +44,12 @@
         return uniform_real_distribution(devices::random::Generic<devices::math::ARM>{}, low, high, rng);
     }
     namespace normal_distribution{
         template<typename T, typename RNG>
         T sample(const devices::random::ARM& dev, T mean, T std, RNG& rng){
             return sample(devices::random::Generic<devices::math::ARM>{}, mean, std, rng);
         }
-        template<typename DEVICE, typename T>
-        T log_prob(const devices::random::ARM& dev, T mean, T log_std, T value){
-            static_assert(utils::typing::is_same_v<T, float> || utils::typing::is_same_v<T, double>);
-            return log_prob(devices::random::Generic<devices::math::ARM>{}, mean, log_std, value);
-        }
-        template<typename DEVICE, typename T>
-        T d_log_prob_d_mean(const devices::random::ARM& dev, T mean, T log_std, T value){
-            return d_log_prob_d_mean(devices::random::Generic<devices::math::ARM>{}, mean, log_std, value);
-        }
-        template<typename DEVICE, typename T>
-        T d_log_prob_d_log_std(const devices::random::ARM& dev, T mean, T log_std, T value){
-            return d_log_prob_d_log_std(devices::random::Generic<devices::math::ARM>{}, mean, log_std, value);
-        }
-        template<typename DEVICE, typename T>
-        T d_log_prob_d_sample(const devices::random::ARM& dev, T mean, T log_std, T value){
-            return d_log_prob_d_sample(devices::random::Generic<devices::math::ARM>{}, mean, log_std, value);
-        }
     }
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 
 #endif
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_dummy.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_dummy.h`

 * *Files 9% similar despite different names*

```diff
@@ -33,19 +33,14 @@
     }
     namespace normal_distribution{
         template<typename T, typename RNG>
         T sample(const devices::random::Dummy& dev, T mean, T std, RNG& rng){
             static_assert(utils::typing::is_same_v<T, float> || utils::typing::is_same_v<T, double>);
             return 0;
         }
-        template<typename DEVICE, typename T>
-        T log_prob(const devices::random::Dummy& dev, T mean, T log_std, T value){
-            static_assert(utils::typing::is_same_v<T, float> || utils::typing::is_same_v<T, double>);
-            return 0;
-        }
     }
 //        static_assert(utils::typing::is_same_v<RNG, typename DEVICE::index_t>);
 //        //
 //        T x, y, r, res;
 //        x = 0;
 //        y = 0;
 //        r = 0;
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_esp32.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/random/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/random/operations_generic.h`

 * *Files 7% similar despite different names*

```diff
@@ -50,39 +50,43 @@
             next(dev, rng);
             T u2 = rng / static_cast<T>(next_max(dev));
             T x = math::sqrt(MATH_DEV{}, -2.0 * math::log(MATH_DEV{}, u1));
             T y = 2.0 * math::PI<T> * u2;
             T z = x * math::cos(MATH_DEV{}, y);
             return z * std + mean;
         }
-        template<typename MATH_DEV, typename T>
-        RL_TOOLS_FUNCTION_PLACEMENT T log_prob(const devices::random::Generic<MATH_DEV>& dev, T mean, T log_std, T value){
+        template<typename RANDOM_DEVICE, typename T>
+        RL_TOOLS_FUNCTION_PLACEMENT T log_prob(const RANDOM_DEVICE& dev, T mean, T log_std, T value){
             static_assert(utils::typing::is_same_v<T, float> || utils::typing::is_same_v<T, double>);
+            using MATH_DEV = typename RANDOM_DEVICE::MATH_DEVICE;
             T neg_log_sqrt_pi = -0.5 * math::log(MATH_DEV{}, 2 * math::PI<T>);
             T diff = (value - mean);
             T std = math::exp(MATH_DEV{}, log_std);
             T pre_square = diff/std;
             return neg_log_sqrt_pi - log_std - 0.5 * pre_square * pre_square;
         }
-        template<typename MATH_DEV, typename T>
-        RL_TOOLS_FUNCTION_PLACEMENT T d_log_prob_d_mean(const devices::random::Generic<MATH_DEV>& dev, T mean, T log_std, T value){
+        template<typename RANDOM_DEVICE, typename T>
+        RL_TOOLS_FUNCTION_PLACEMENT T d_log_prob_d_mean(RANDOM_DEVICE& dev, T mean, T log_std, T value){
+            using MATH_DEV = typename RANDOM_DEVICE::MATH_DEVICE;
             T diff = (value - mean);
             T std = math::exp(MATH_DEV{}, log_std);
             T pre_square = diff/std;
             return pre_square / std;
         }
-        template<typename MATH_DEV, typename T>
-        RL_TOOLS_FUNCTION_PLACEMENT T d_log_prob_d_log_std(const devices::random::Generic<MATH_DEV>& dev, T mean, T log_std, T value){
+        template<typename RANDOM_DEVICE, typename T>
+        RL_TOOLS_FUNCTION_PLACEMENT T d_log_prob_d_log_std(RANDOM_DEVICE& dev, T mean, T log_std, T value){
+            using MATH_DEV = typename RANDOM_DEVICE::MATH_DEVICE;
             T diff = (value - mean);
             T std = math::exp(MATH_DEV{}, log_std);
             T pre_square = diff/std;
             return - 1 + pre_square * pre_square;
         }
-        template<typename MATH_DEV, typename T>
-        RL_TOOLS_FUNCTION_PLACEMENT T d_log_prob_d_sample(const devices::random::Generic<MATH_DEV>& dev, T mean, T log_std, T value){
+        template<typename RANDOM_DEVICE, typename T>
+        RL_TOOLS_FUNCTION_PLACEMENT T d_log_prob_d_sample(RANDOM_DEVICE& dev, T mean, T log_std, T value){
+            using MATH_DEV = typename RANDOM_DEVICE::MATH_DEVICE;
             T diff = (value - mean);
             T std = math::exp(MATH_DEV{}, log_std);
             T pre_square = diff/std;
             return - pre_square / std;
         }
     }
 }
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic.h`

 * *Files 8% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 #ifdef RL_TOOLS_DEBUG_RL_ALGORITHMS_PPO_CHECK_INIT
         utils::assert_exit(device, ppo.initialized, "PPO not initialized");
 #endif
         using T = typename PPO_SPEC::T;
         using TI = typename PPO_SPEC::TI;
         static_assert(utils::typing::is_same_v<typename PPO_SPEC::ENVIRONMENT, typename OPR_SPEC::ENVIRONMENT>, "environment mismatch");
         using DATASET = rl::components::on_policy_runner::Dataset<rl::components::on_policy_runner::DatasetSpecification<OPR_SPEC, STEPS_PER_ENV>>;
-        static_assert(DATASET::STEPS_TOTAL > 0);
+        static_assert(DATASET::STEPS_TOTAL > 1);
         constexpr TI N_EPOCHS = PPO_SPEC::PARAMETERS::N_EPOCHS;
         constexpr TI BATCH_SIZE = PPO_SPEC::BATCH_SIZE;
         constexpr TI N_BATCHES = DATASET::STEPS_TOTAL/BATCH_SIZE;
         static_assert(N_BATCHES > 0);
         constexpr TI ACTION_DIM = OPR_SPEC::ENVIRONMENT::ACTION_DIM;
         constexpr TI OBSERVATION_DIM = OPR_SPEC::ENVIRONMENT::OBSERVATION_DIM;
         constexpr bool NORMALIZE_OBSERVATIONS = PPO_SPEC::PARAMETERS::NORMALIZE_OBSERVATIONS;
@@ -182,53 +182,65 @@
                             kl += (current_action_std * current_action_std + action_mean_diff * action_mean_diff)/(2 * rollout_action_std * rollout_action_std + PPO_SPEC::PARAMETERS::POLICY_KL_EPSILON);
                             kl += (T)-0.5;
                             kl = math::max(device.math, kl, (T)0);
                             policy_kl_divergence += kl;
                             batch_policy_kl_divergence += kl;
                         }
 
-                        T action_diff_by_action_std = (current_action - rollout_action) / current_action_std;
-                        action_log_prob += -0.5 * action_diff_by_action_std * action_diff_by_action_std - current_action_log_std - 0.5 * math::log(device.math, 2 * math::PI<T>);
-                        set(ppo_buffers.d_action_log_prob_d_action, batch_step_i, action_i, - action_diff_by_action_std / current_action_std);
+//                        T action_diff_by_action_std = (current_action - rollout_action) / current_action_std;
+//                        action_log_prob += -0.5 * action_diff_by_action_std * action_diff_by_action_std - current_action_log_std - 0.5 * math::log(device.math, 2 * math::PI<T>);
+                        // probability of the old actions under the new policy
+                        action_log_prob += random::normal_distribution::log_prob(device.random, current_action, current_action_log_std, rollout_action);
+//                        set(ppo_buffers.d_action_log_prob_d_action, batch_step_i, action_i, - action_diff_by_action_std / current_action_std);
+                        set(ppo_buffers.d_action_log_prob_d_action, batch_step_i, action_i, random::normal_distribution::d_log_prob_d_mean(device.random, current_action, current_action_log_std, rollout_action));
+
                         T current_entropy = current_action_log_std + math::log(device.math, 2 * math::PI<T>)/(T)2 + (T)1/(T)2;
                         T current_entropy_loss = -(T)1/BATCH_SIZE * PPO_SPEC::PARAMETERS::ACTION_ENTROPY_COEFFICIENT * current_entropy;
                         // todo: think about possible implementation detail: clipping entropy bonus as well (because it changes the distribution)
                         if(PPO_SPEC::PARAMETERS::LEARN_ACTION_STD){
                             T d_entropy_loss_d_current_action_log_std = -(T)1/BATCH_SIZE * PPO_SPEC::PARAMETERS::ACTION_ENTROPY_COEFFICIENT;
                             increment(ppo.actor.log_std.gradient, 0, action_i, d_entropy_loss_d_current_action_log_std);
 //                          derivation: d_current_action_log_prob_d_action_log_std
 //                          d_current_action_log_prob_d_action_std =  (-action_diff_by_action_std) * (-action_diff_by_action_std)      / action_std - 1 / action_std)
 //                          d_current_action_log_prob_d_action_std = ((-action_diff_by_action_std) * (-action_diff_by_action_std) - 1) / action_std)
 //                          d_current_action_log_prob_d_action_std = (action_diff_by_action_std * action_diff_by_action_std - 1) / action_std
 //                          d_current_action_log_prob_d_action_log_std = (action_diff_by_action_std * action_diff_by_action_std - 1) / action_std * exp(action_log_std)
 //                          d_current_action_log_prob_d_action_log_std = (action_diff_by_action_std * action_diff_by_action_std - 1) / action_std * action_std
 //                          d_current_action_log_prob_d_action_log_std =  action_diff_by_action_std * action_diff_by_action_std - 1
-                            T d_current_action_log_prob_d_action_log_std = action_diff_by_action_std * action_diff_by_action_std - 1;
-                            set(ppo_buffers.d_action_log_prob_d_action_log_std, batch_step_i, action_i, d_current_action_log_prob_d_action_log_std);
+//                            T d_current_action_log_prob_d_action_log_std = action_diff_by_action_std * action_diff_by_action_std - 1;
+                            T d_action_log_prob_d_current_action_log_std = random::normal_distribution::d_log_prob_d_log_std(device.random, current_action, current_action_log_std, rollout_action);
+                            set(ppo_buffers.d_action_log_prob_d_action_log_std, batch_step_i, action_i, d_action_log_prob_d_current_action_log_std);
                         }
                     }
                     T rollout_action_log_prob = get(batch_action_log_probs, batch_step_i, 0);
                     T advantage = get(batch_advantages, batch_step_i, 0);
                     if(PPO_SPEC::PARAMETERS::NORMALIZE_ADVANTAGE){
                         advantage = (advantage - advantage_mean) / (advantage_std + PPO_SPEC::PARAMETERS::ADVANTAGE_EPSILON);
                     }
                     T log_ratio = action_log_prob - rollout_action_log_prob;
                     T ratio = math::exp(device.math, log_ratio);
                     // todo: test relative clipping (clipping in log space makes more sense thatn clipping in exp space)
                     T clipped_ratio = math::clamp(device.math, ratio, 1 - PPO_SPEC::PARAMETERS::EPSILON_CLIP, 1 + PPO_SPEC::PARAMETERS::EPSILON_CLIP);
+                    bool clipped = ratio != clipped_ratio;
                     T normal_advantage = ratio * advantage;
                     T clipped_advantage = clipped_ratio * advantage;
                     T slippage = 0.0;
                     bool ratio_min_switch = normal_advantage - clipped_advantage <= slippage;
-                    T clipped_surrogate = ratio_min_switch ? normal_advantage : clipped_advantage;
+                    T pessimistic_surrogate = ratio_min_switch ? normal_advantage : clipped_advantage;
 
-                    T d_loss_d_clipped_surrogate = -(T)1/BATCH_SIZE;
-                    T d_clipped_surrogate_d_ratio = ratio_min_switch ? advantage : 0;
+                    T d_loss_d_pessimistic_surrogate = -(T)1/BATCH_SIZE;
+                    T d_pessimistic_surrogate_d_normal_advantage = ratio_min_switch ? 1 : 0;
+                    T d_pessimistic_surrogate_d_clipped_advantage = ratio_min_switch ? 0 : 1;
+                    T d_normal_advantage_d_ratio = advantage;
+                    T d_clipped_advantage_d_clipped_ratio = advantage;
+                    T d_clipped_ratio_d_ratio = clipped ? 0 : 1;
+                    T d_pessimistic_surrogate_d_ratio = d_pessimistic_surrogate_d_normal_advantage * d_normal_advantage_d_ratio + d_pessimistic_surrogate_d_clipped_advantage * d_clipped_advantage_d_clipped_ratio * d_clipped_ratio_d_ratio;
+                    T d_loss_d_ratio = d_loss_d_pessimistic_surrogate * d_pessimistic_surrogate_d_ratio;
                     T d_ratio_d_action_log_prob = ratio;
-                    T d_loss_d_action_log_prob = d_loss_d_clipped_surrogate * d_clipped_surrogate_d_ratio * d_ratio_d_action_log_prob;
+                    T d_loss_d_action_log_prob = d_loss_d_ratio * d_ratio_d_action_log_prob;
                     for(TI action_i = 0; action_i < ACTION_DIM; action_i++){
                         multiply(ppo_buffers.d_action_log_prob_d_action, batch_step_i, action_i, d_loss_d_action_log_prob);
                         if(PPO_SPEC::PARAMETERS::LEARN_ACTION_STD){
                             T current_d_action_log_prob_d_action_log_std = get(ppo_buffers.d_action_log_prob_d_action_log_std, batch_step_i, action_i);
                             increment(ppo.actor.log_std.gradient, 0, action_i, d_loss_d_action_log_prob * current_d_action_log_prob_d_action_log_std);
                         }
                     }
@@ -242,15 +254,15 @@
                         actor_optimizer.parameters.alpha = math::min(device.math, actor_optimizer.parameters.alpha / PPO_SPEC::PARAMETERS::ADAPTIVE_LEARNING_RATE_DECAY, PPO_SPEC::PARAMETERS::ADAPTIVE_LEARNING_RATE_MAX);
                     }
                 }
                 backward(device, ppo.actor, batch_observations, ppo_buffers.d_action_log_prob_d_action, actor_buffers);
 //                forward_backward_mse(device, ppo.critic, batch_observations, batch_target_values, critic_buffers);
                 {
                     forward(device, ppo.critic, batch_observations);
-                    nn::loss_functions::mse::gradient(device, output(ppo.critic), batch_target_values, ppo_buffers.d_critic_output);
+                    nn::loss_functions::mse::gradient(device, output(ppo.critic), batch_target_values, ppo_buffers.d_critic_output, 0.5);
                     backward(device, ppo.critic, batch_observations, ppo_buffers.d_critic_output, critic_buffers);
                 }
                 T critic_loss = nn::loss_functions::mse::evaluate(device, output(ppo.critic), batch_target_values);
                 add_scalar(device, device.logger, "ppo/critic_loss", critic_loss);
                 step(device, actor_optimizer, ppo.actor);
                 step(device, actor_optimizer, ppo.critic); // todo: evaluate switch to critic_optimizer
             }
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic_extensions.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/operations_generic_extensions.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/ppo.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/ppo.h`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 namespace rl_tools::rl::algorithms{
     namespace ppo{
         template<typename T, typename TI>
         struct DefaultParameters {
             static constexpr T GAMMA = 0.99;
             static constexpr T LAMBDA = 0.95;
             static constexpr T EPSILON_CLIP = 0.2;
-            static constexpr T INITIAL_ACTION_STD = 0.5;
+            static constexpr T INITIAL_ACTION_STD = 0.5; // note this is NOT log(std) but actual std (log is applied at init)
             static constexpr bool LEARN_ACTION_STD = true;
             static constexpr T ACTION_ENTROPY_COEFFICIENT = 0.01;
             static constexpr T ADVANTAGE_EPSILON = 1e-8;
             static constexpr bool NORMALIZE_ADVANTAGE = true;
             static constexpr bool ADAPTIVE_LEARNING_RATE = false;
             static constexpr T ADAPTIVE_LEARNING_RATE_POLICY_KL_THRESHOLD = 0.008;
             static constexpr T POLICY_KL_EPSILON = 1e-5;
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/config.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/config.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/operations_generic.h`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     template <typename DEVICE, typename T_CONFIG>
     void free(DEVICE& device, rl::algorithms::ppo::loop::core::State<T_CONFIG>& ts){
         free(device, ts.ppo);
         free(device, ts.ppo_buffers);
         free(device, ts.on_policy_runner_dataset);
         free(device, ts.on_policy_runner);
         free(device, ts.actor_eval_buffers);
-        free(device, ts.actor_deterministic_eval_buffers);
         free(device, ts.actor_buffers);
         free(device, ts.critic_buffers);
         free(device, ts.critic_buffers_gae);
         free(device, ts.observation_normalizer);
         for(auto& env: ts.envs){
             free(device, env);
         }
@@ -80,14 +79,16 @@
         bool finished = false;
         collect(device, ts.on_policy_runner_dataset, ts.on_policy_runner, ts.ppo.actor, ts.actor_eval_buffers, ts.observation_normalizer.mean, ts.observation_normalizer.std, ts.rng);
         auto on_policy_runner_dataset_all_observations = CONFIG::PPO_SPEC::PARAMETERS::NORMALIZE_OBSERVATIONS ? ts.on_policy_runner_dataset.all_observations_normalized : ts.on_policy_runner_dataset.all_observations;
         evaluate(device, ts.ppo.critic, on_policy_runner_dataset_all_observations, ts.on_policy_runner_dataset.all_values, ts.critic_buffers_gae);
         estimate_generalized_advantages(device, ts.on_policy_runner_dataset, typename CONFIG::PPO_TYPE::SPEC::PARAMETERS{});
         train(device, ts.ppo, ts.on_policy_runner_dataset, ts.actor_optimizer, ts.critic_optimizer, ts.ppo_buffers, ts.actor_buffers, ts.critic_buffers, ts.rng);
 
+//        log(device, device.logger, "log_std: ", get(ts.ppo.actor.log_std.parameters, 0, 0));
+
         ts.step++;
         if(ts.step > CONFIG::CORE_PARAMETERS::STEP_LIMIT){
             return true;
         }
         else{
             return finished;
         }
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/state.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/ppo/loop/core/state.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #include "../../../../../version.h"
 #if (defined(RL_TOOLS_DISABLE_INCLUDE_GUARDS) || !defined(RL_TOOLS_RL_ALGORITHMS_PPO_LOOP_CORE_STATE_H)) && (RL_TOOLS_USE_THIS_VERSION == 1)
 #pragma once
 #define RL_TOOLS_RL_ALGORITHMS_PPO_LOOP_CORE_STATE_H
 
 #include "../../../../../rl/algorithms/ppo/ppo.h"
 #include "../../../../../rl/components/off_policy_runner/off_policy_runner.h"
+#include "../../../../../rl/environments/environments.h"
 
 RL_TOOLS_NAMESPACE_WRAPPER_START
 namespace rl_tools{
     namespace rl::algorithms::ppo::loop::core{
         // Config State (Init/Step)
         template<typename T_CONFIG>
         struct State{
@@ -26,15 +27,15 @@
             typename CONFIG::PPO_TYPE::SPEC::ACTOR_TYPE::template Buffer<1> actor_deterministic_evaluation_buffers;
             typename CONFIG::ACTOR_BUFFERS actor_buffers;
             typename CONFIG::CRITIC_BUFFERS critic_buffers;
             typename CONFIG::CRITIC_BUFFERS_GAE critic_buffers_gae;
             rl::components::RunningNormalizer<rl::components::running_normalizer::Specification<T, TI, CONFIG::ENVIRONMENT::OBSERVATION_DIM>> observation_normalizer;
             typename CONFIG::ENVIRONMENT envs[CONFIG::CORE_PARAMETERS::N_ENVIRONMENTS];
             MatrixDynamic<matrix::Specification<typename CONFIG::T, TI, 1, CONFIG::ENVIRONMENT::OBSERVATION_DIM>> observations_mean, observations_std;
-            bool ui = false;
+            environments::DummyUI ui;
             TI next_checkpoint_id = 0;
             TI next_evaluation_id = 0;
             TI step;
         };
     }
     template <typename T_CONFIG>
     constexpr auto& get_actor(rl::algorithms::ppo::loop::core::State<T_CONFIG>& ts){
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cuda.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/operations_generic.h`

 * *Files 7% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         critic_training_buffers.next_actions_log_std          = view(device, critic_training_buffers.next_state_action_value_input_full, matrix::ViewSpec<BUFFERS::BATCH_SIZE, BUFFERS::ACTION_DIM>{}, 0, BUFFERS::CRITIC_OBSERVATION_DIM + BUFFERS::ACTION_DIM);
         malloc(device, critic_training_buffers.action_value);
         malloc(device, critic_training_buffers.target_action_value);
         malloc(device, critic_training_buffers.next_state_action_value_critic_1);
         malloc(device, critic_training_buffers.next_state_action_value_critic_2);
         malloc(device, critic_training_buffers.d_output);
         malloc(device, critic_training_buffers.d_input);
-        malloc(device, critic_training_buffers.action_log_probs);
+        malloc(device, critic_training_buffers.next_action_log_probs);
     }
 
     template <typename DEVICE, typename SPEC>
     void free(DEVICE& device, rl::algorithms::sac::CriticTrainingBuffers<SPEC>& critic_training_buffers){
         free(device, critic_training_buffers.next_state_action_value_input_full);
         critic_training_buffers.next_state_action_value_input._data = nullptr;
         critic_training_buffers.next_observations._data = nullptr;
@@ -93,15 +93,15 @@
         critic_training_buffers.next_actions_log_std._data = nullptr;
         free(device, critic_training_buffers.action_value);
         free(device, critic_training_buffers.target_action_value);
         free(device, critic_training_buffers.next_state_action_value_critic_1);
         free(device, critic_training_buffers.next_state_action_value_critic_2);
         free(device, critic_training_buffers.d_output);
         free(device, critic_training_buffers.d_input);
-        free(device, critic_training_buffers.action_log_probs);
+        free(device, critic_training_buffers.next_action_log_probs);
     }
 
     template <typename DEVICE, typename SPEC, typename RNG>
     void init(DEVICE& device, rl::algorithms::sac::ActorCritic<SPEC>& actor_critic, RNG& rng){
         init_weights(device, actor_critic.actor   , rng);
         init_weights(device, actor_critic.critic_1, rng);
         init_weights(device, actor_critic.critic_2, rng);
@@ -127,17 +127,18 @@
         static_assert(BATCH_SIZE == BUFFERS::BATCH_SIZE);
         T min_next_state_action_value = math::min(device.math,
                                                   get(training_buffers.next_state_action_value_critic_1, batch_step_i, 0),
                                                   get(training_buffers.next_state_action_value_critic_2, batch_step_i, 0)
         );
         T reward = get(batch.rewards, 0, batch_step_i);
         bool terminated = get(batch.terminated, 0, batch_step_i);
-        T future_value = SPEC::PARAMETERS::IGNORE_TERMINATION || !terminated ? SPEC::PARAMETERS::GAMMA * min_next_state_action_value : 0;
-        T entropy_bonus = -alpha * get(training_buffers.action_log_probs, batch_step_i, 0);
-        T current_target_action_value = reward + future_value + entropy_bonus;
+        T entropy_bonus = -alpha * get(training_buffers.next_action_log_probs, batch_step_i, 0);
+        T min_next_state_action_value_entropy_bonus = min_next_state_action_value + entropy_bonus;
+        T future_value = SPEC::PARAMETERS::IGNORE_TERMINATION || !terminated ? SPEC::PARAMETERS::GAMMA * min_next_state_action_value_entropy_bonus : 0;
+        T current_target_action_value = reward + future_value;
         set(training_buffers.target_action_value, batch_step_i, 0, current_target_action_value); // todo: improve pitch of target action values etc. (by transformig it into row vectors instead of column vectors)
     }
     template <typename DEVICE, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE, typename SPEC, typename ALPHA_PARAMETER>
     void target_actions(DEVICE& device, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, rl::algorithms::sac::CriticTrainingBuffers<SPEC>& training_buffers, ALPHA_PARAMETER& log_alpha) {
         using T = typename SPEC::T;
         using TI = typename DEVICE::index_t;
         using BUFFERS = rl::algorithms::sac::CriticTrainingBuffers<SPEC>;
@@ -154,22 +155,27 @@
         constexpr TI ACTION_DIM = SPEC::ENVIRONMENT::ACTION_DIM;
         constexpr TI BATCH_SIZE = rl::algorithms::sac::ActorTrainingBuffers<SPEC>::BATCH_SIZE;
         static_assert(BATCH_SIZE == ACTION_NOISE_SPEC::ROWS);
         static_assert(ACTION_DIM == ACTION_NOISE_SPEC::COLS);
         T action_log_prob = 0;
         for(TI action_i = 0; action_i < ACTION_DIM; action_i++){
             T mean = get(training_buffers.next_actions_mean, sample_i, action_i);
-            T log_std = get(training_buffers.next_actions_log_std, sample_i, action_i);
-            T std = math::exp(typename DEVICE::SPEC::MATH{}, log_std);
+            T log_std_pre_clamp = get(training_buffers.next_actions_log_std, sample_i, action_i);
+            T log_std_clamped = math::clamp(device.math, log_std_pre_clamp, (T)SPEC::PARAMETERS::ACTION_LOG_STD_LOWER_BOUND, (T)SPEC::PARAMETERS::ACTION_LOG_STD_UPPER_BOUND);
+            T std = math::exp(typename DEVICE::SPEC::MATH{}, log_std_clamped);
 //            T action_sampled = random::normal_distribution::sample(typename DEVICE::SPEC::RANDOM{}, mean, std, rng);
             T action_sampled = mean + get(action_noise, sample_i, action_i) * std;
-            set(training_buffers.next_actions_mean, sample_i, action_i, action_sampled);
-            action_log_prob += random::normal_distribution::log_prob<DEVICE, T>(typename DEVICE::SPEC::RANDOM{}, mean, log_std, action_sampled);
+            T action_squashed = math::tanh(device.math, action_sampled);
+//            action_log_prob += random::normal_distribution::log_prob<DEVICE, T>(typename DEVICE::SPEC::RANDOM{}, mean, log_std_clamped, action_sampled);
+            T eps = 1e-6;
+            T one_minus_action_square_plus_eps = (1-action_squashed*action_squashed + eps);
+            action_log_prob += random::normal_distribution::log_prob(device.random, mean, log_std_clamped, action_sampled) - math::log(typename DEVICE::SPEC::MATH{}, one_minus_action_square_plus_eps);
+            set(training_buffers.next_actions_mean, sample_i, action_i, action_squashed);
         }
-        set(training_buffers.action_log_probs, sample_i, 0, action_log_prob);
+        set(training_buffers.next_action_log_probs, sample_i, 0, action_log_prob);
     }
     template <typename DEVICE, typename SPEC, typename ACTION_NOISE_SPEC>
     void sample_actions_critic(DEVICE& device, rl::algorithms::sac::CriticTrainingBuffers<SPEC>& training_buffers, Matrix<ACTION_NOISE_SPEC>& action_noise) {
         using T = typename SPEC::T;
         using TI = typename DEVICE::index_t;
         constexpr TI ACTION_DIM = SPEC::ENVIRONMENT::ACTION_DIM;
         constexpr TI BATCH_SIZE = rl::algorithms::sac::ActorTrainingBuffers<SPEC>::BATCH_SIZE;
@@ -196,15 +202,15 @@
         sample_actions_critic(device, training_buffers, action_noise);
         copy(device, device, batch.next_observations_privileged, training_buffers.next_observations);
         evaluate(device, actor_critic.critic_target_1, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_1, critic_buffers);
         evaluate(device, actor_critic.critic_target_2, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_2, critic_buffers);
 
         target_actions(device, batch, training_buffers, actor_critic.log_alpha);
         forward(device, critic, batch.observations_and_actions);
-        nn::loss_functions::mse::gradient(device, output(critic), training_buffers.target_action_value, training_buffers.d_output);
+        nn::loss_functions::mse::gradient(device, output(critic), training_buffers.target_action_value, training_buffers.d_output, 0.5);
         backward(device, critic, batch.observations_and_actions, training_buffers.d_output, critic_buffers);
         step(device, optimizer, critic);
     }
     template <typename DEVICE, typename SPEC, typename CRITIC_TYPE, typename OFF_POLICY_RUNNER_SPEC, auto BATCH_SIZE>
     typename SPEC::T critic_loss(DEVICE& device, const rl::algorithms::sac::ActorCritic<SPEC>& actor_critic, CRITIC_TYPE& critic, rl::components::off_policy_runner::Batch<rl::components::off_policy_runner::BatchSpecification<OFF_POLICY_RUNNER_SPEC, BATCH_SIZE>>& batch, typename SPEC::ACTOR_NETWORK_TYPE::template Buffers<BATCH_SIZE>& actor_buffers, typename CRITIC_TYPE::template Buffers<BATCH_SIZE>& critic_buffers, rl::algorithms::sac::CriticTrainingBuffers<SPEC>& training_buffers) {
         using T = typename SPEC::T;
         using TI = typename DEVICE::index_t;
@@ -215,23 +221,25 @@
         evaluate(device, actor_critic.critic_target_1, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_1, critic_buffers);
         evaluate(device, actor_critic.critic_target_2, training_buffers.next_state_action_value_input, training_buffers.next_state_action_value_critic_2, critic_buffers);
 
         T log_alpha = get(actor_critic.log_alpha, 0, 0);
         T alpha = math::exp(typename DEVICE::SPEC::MATH{}, log_alpha);
         target_actions(device, batch, training_buffers, alpha);
         evaluate(device, critic, batch.observations_and_actions, training_buffers.action_value, critic_buffers);
-        return nn::loss_functions::mse::evaluate(device, training_buffers.action_value, training_buffers.target_action_value);
+        return nn::loss_functions::mse::evaluate(device, training_buffers.action_value, training_buffers.target_action_value, 0.5);
     }
     template <typename DEVICE, typename OUTPUT_SPEC, typename SPEC, typename ACTION_NOISE_SPEC, typename TI_SAMPLE>
     RL_TOOLS_FUNCTION_PLACEMENT void sample_actions_actor_per_sample(DEVICE& device, Matrix<OUTPUT_SPEC>& output, rl::algorithms::sac::ActorTrainingBuffers<SPEC>& training_buffers, Matrix<ACTION_NOISE_SPEC>& action_noise, TI_SAMPLE batch_i) {
         using T = typename SPEC::T;
         using TI = typename DEVICE::index_t;
         constexpr TI ACTION_DIM = SPEC::ENVIRONMENT::ACTION_DIM;
         for(TI action_i = 0; action_i < ACTION_DIM; action_i++){
-            T std = math::exp(typename DEVICE::SPEC::MATH{}, get(output, batch_i, action_i + ACTION_DIM));
+            T log_std_pre_clip = get(output, batch_i, action_i + ACTION_DIM);
+            T log_std_clip = math::clamp(device.math, log_std_pre_clip, (T)SPEC::PARAMETERS::ACTION_LOG_STD_LOWER_BOUND, (T)SPEC::PARAMETERS::ACTION_LOG_STD_UPPER_BOUND);
+            T std = math::exp(typename DEVICE::SPEC::MATH{}, log_std_pre_clip);
             // action_sample = noise * std + mean
 //            T noise = random::normal_distribution::sample(typename DEVICE::SPEC::RANDOM{}, (T)0, (T)1, rng);
             T noise = get(action_noise, batch_i, action_i);
             set(training_buffers.action_noise, batch_i, action_i, noise);
             T action_sample = get(output, batch_i, action_i) + std * noise;
             set(training_buffers.action_sample, batch_i, action_i, action_sample);
             T action = math::tanh(typename DEVICE::SPEC::MATH{}, action_sample);
@@ -262,56 +270,64 @@
         action_prob = gaussian::prob(mu, std, action_sample) * | d/d_action tanh^{-1}(action) |
                     = gaussian::prob(mu, std, action_sample) * | (d/d_action_sample tanh(action_sample))^{-1} |
                     = gaussian::prob(mu, std, action_sample) * | (d/d_action_sample tanh(action_sample))|^{-1}
                     = gaussian::prob(mu, std, action_sample) * ((1-tanh(action_sample)^2))^{-1}
         action_log_prob = gaussian::log_prob(mu, std, action_sample) - log(1-tanh(action_sample)^2))
         actor_loss = alpha  * action_log_prob - min(Q_1, Q_2);
         d/d_mu _actor_loss = alpha * d/d_mu action_log_prob - d/d_mu min(Q_1, Q_2)
-        d/d_mu action_log_prob = d/d_mu gaussian::log_prob(mu, std, action_sample) + d/d_action_sample gaussian::log_prob(mu, std, action_sample) * d/d_mu action_sample + 1/(1-tanh(action_sample)^2) * 2*tanh(action_sample) * d/d_mu action_sample
+        d/d_mu action_log_prob = d/d_mu gaussian::log_prob(mu, std, action_sample) + d/d_action_sample gaussian::log_prob(mu, std, action_sample) * d/d_mu action_sample - 1/(1-tanh(action_sample)^2) * (-2*tanh(action_sample))*(1-tanh(action_sample)^2) * d/d_mu action_sample)
+                               = d/d_mu gaussian::log_prob(mu, std, action_sample) + d/d_action_sample gaussian::log_prob(mu, std, action_sample) * d/d_mu action_sample + 2*tanh(action_sample)) * d/d_mu action_sample)
         d/d_mu action_sample = 1
         d/d_std action_sample = noise
         d/d_mu min(Q_1, Q_2) = d/d_action min(Q_1, Q_2) * d/d_mu action
         d/d_mu action = d/d_action_sample tanh(action_sample) * d/d_mu action_sample
 */
         bool critic_1_value = get(critic_1_output, batch_i, 0) < get(critic_2_output, batch_i, 0);
         T entropy = 0;
-        for(TI action_i = 0; action_i < ACTION_DIM; action_i++) {
+        for(TI action_i = 0; action_i < ACTION_DIM; action_i++){
             T action = get(training_buffers.actions, batch_i, action_i);
             T d_mu = 0;
             T d_std = 0;
             {
                 T d_input = 0;
                 if(critic_1_value) {
                     d_input = get(training_buffers.d_critic_1_input, batch_i, SPEC::CRITIC_NETWORK_TYPE::INPUT_DIM - ACTION_DIM + action_i);
                 }
                 else{
                     d_input = get(training_buffers.d_critic_2_input, batch_i, SPEC::CRITIC_NETWORK_TYPE::INPUT_DIM - ACTION_DIM + action_i);
                 }
-                d_mu  = d_input * (1-action*action);
-                d_std = d_input * (1-action*action) * get(training_buffers.action_noise, batch_i, action_i);
+                T d_tanh_pre_activation = d_input * (1-action*action);
+                d_mu = d_tanh_pre_activation/BATCH_SIZE;
+                d_std = d_tanh_pre_activation * get(training_buffers.action_noise, batch_i, action_i)/BATCH_SIZE;
             }
-            T log_std = get(actions, batch_i, action_i + ACTION_DIM);
-            T std = math::exp(typename DEVICE::SPEC::MATH{}, log_std);
+            T log_std_pre_clamp = get(actions, batch_i, action_i + ACTION_DIM);
+            T log_std_clamped = math::clamp(device.math, log_std_pre_clamp, (T)SPEC::PARAMETERS::ACTION_LOG_STD_LOWER_BOUND, (T)SPEC::PARAMETERS::ACTION_LOG_STD_UPPER_BOUND);
+            T std = math::exp(typename DEVICE::SPEC::MATH{}, log_std_clamped);
 
-            T d_log_std = std * d_std;
+            T d_log_std_clamped = std * d_std;
+            T d_log_std = log_std_pre_clamp < SPEC::PARAMETERS::ACTION_LOG_STD_LOWER_BOUND || log_std_pre_clamp > SPEC::PARAMETERS::ACTION_LOG_STD_UPPER_BOUND ? 0 : d_log_std_clamped;
 
+            // Entropy bonus
             T mu = get(actions, batch_i, action_i);
             T action_sample = get(training_buffers.action_sample, batch_i, action_i);
             T eps = 1e-6;
-            T one_minus_action_square_plus_eps = (1-action*action + eps);
-            T one_over_one_minus_action_square_plus_eps = 1/one_minus_action_square_plus_eps;
-            d_mu += alpha/BATCH_SIZE * (random::normal_distribution::d_log_prob_d_mean<DEVICE, T>(typename DEVICE::SPEC::RANDOM{}, mu, log_std, action_sample) + random::normal_distribution::d_log_prob_d_sample<DEVICE, T>(typename DEVICE::SPEC::RANDOM{}, mu, log_std, action_sample) + one_over_one_minus_action_square_plus_eps * 2*action);
+//            T one_over_one_minus_action_square_plus_eps = 1/one_minus_action_square_plus_eps;
+            T d_log_prob_d_mean = random::normal_distribution::d_log_prob_d_mean(device.random, mu, log_std_clamped, action_sample);
+            T d_log_prob_d_sample = random::normal_distribution::d_log_prob_d_sample(device.random, mu, log_std_clamped, action_sample);
+            d_mu += alpha/BATCH_SIZE * (d_log_prob_d_mean + d_log_prob_d_sample + 2*action);
 
             T noise = get(training_buffers.action_noise, batch_i, action_i);
-            d_log_std += alpha/BATCH_SIZE * (random::normal_distribution::d_log_prob_d_log_std<DEVICE, T>(typename DEVICE::SPEC::RANDOM{}, mu, log_std, action_sample) + random::normal_distribution::d_log_prob_d_sample<DEVICE, T>(typename DEVICE::SPEC::RANDOM{}, mu, log_std, action_sample) * noise * std + one_over_one_minus_action_square_plus_eps * 2*action * noise * std);
+            T d_log_prob_d_log_std = random::normal_distribution::d_log_prob_d_log_std(device.random, mu, log_std_clamped, action_sample);
+            d_log_std += alpha/BATCH_SIZE * (d_log_prob_d_log_std + d_log_prob_d_sample * noise * std + 2*action * noise * std);
 
             set(training_buffers.d_actor_output, batch_i, action_i, d_mu);
             set(training_buffers.d_actor_output, batch_i, action_i + ACTION_DIM, d_log_std);
 
-            T action_log_prob = random::normal_distribution::log_prob<DEVICE, T>(typename DEVICE::SPEC::RANDOM{}, mu, log_std, action_sample) - math::log(typename DEVICE::SPEC::MATH{}, one_minus_action_square_plus_eps);
+            T one_minus_action_square_plus_eps = (1-action*action + eps);
+            T action_log_prob = random::normal_distribution::log_prob(device.random, mu, log_std_clamped, action_sample) - math::log(typename DEVICE::SPEC::MATH{}, one_minus_action_square_plus_eps);
             entropy += -action_log_prob;
         }
         T d_alpha = entropy - SPEC::PARAMETERS::TARGET_ENTROPY;
         return d_alpha;
     }
     template <typename DEVICE, typename SPEC>
     void d_action_d_action_distribution(DEVICE& device, rl::algorithms::sac::ActorCritic<SPEC>& actor_critic, rl::algorithms::sac::ActorTrainingBuffers<SPEC>& training_buffers){
@@ -446,13 +462,13 @@
         copy(source_device, target_device, source.next_state_action_value_input_full, target.next_state_action_value_input_full);
         copy(source_device, target_device, source.action_value, target.action_value);
         copy(source_device, target_device, source.target_action_value, target.target_action_value);
         copy(source_device, target_device, source.next_state_action_value_critic_1, target.next_state_action_value_critic_1);
         copy(source_device, target_device, source.next_state_action_value_critic_2, target.next_state_action_value_critic_2);
         copy(source_device, target_device, source.d_input, target.d_input);
         copy(source_device, target_device, source.d_output, target.d_output);
-        copy(source_device, target_device, source.action_log_probs, target.action_log_probs);
+        copy(source_device, target_device, source.next_action_log_probs, target.next_action_log_probs);
     }
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
 
 #endif
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/sac.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/sac.h`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
         static constexpr TI N_WARMUP_STEPS_CRITIC = 0;
         static constexpr TI N_WARMUP_STEPS_ACTOR = 0;
         static constexpr TI CRITIC_TRAINING_INTERVAL = 1;
         static constexpr TI ACTOR_TRAINING_INTERVAL = 1;
         static constexpr TI CRITIC_TARGET_UPDATE_INTERVAL = 1;
         static constexpr T ACTOR_POLYAK = 1.0 - 0.005;
         static constexpr T CRITIC_POLYAK = 1.0 - 0.005;
-//        static constexpr T TARGET_NEXT_ACTION_NOISE_STD = 0.2;
-//        static constexpr T TARGET_NEXT_ACTION_NOISE_CLIP = 0.5;
         static constexpr bool IGNORE_TERMINATION = false; // ignoring the termination flag is useful for training on environments with negative rewards, where the agent would try to terminate the episode as soon as possible otherwise
         static constexpr T TARGET_ENTROPY = -((T)ACTION_DIM);
         static constexpr bool ADAPTIVE_ALPHA = true;
+        static constexpr T ACTION_LOG_STD_LOWER_BOUND = -20;
+        static constexpr T ACTION_LOG_STD_UPPER_BOUND = 2;
     };
 
     template<
         typename T_T,
         typename T_TI,
         typename T_ENVIRONMENT,
         typename T_ACTOR_NETWORK_TYPE,
@@ -103,15 +103,15 @@
         typename CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, BATCH_SIZE, 1>> action_value;
         typename CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, BATCH_SIZE, 1>> target_action_value;
         typename CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, BATCH_SIZE, 1>> next_state_action_value_critic_1;
         typename CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, BATCH_SIZE, 1>> next_state_action_value_critic_2;
 
         typename CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, BATCH_SIZE, CRITIC_OBSERVATION_DIM + ACTION_DIM>> d_input;
         typename CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, BATCH_SIZE, 1>> d_output;
-        typename CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, BATCH_SIZE, 1>> action_log_probs;
+        typename CONTAINER_TYPE_TAG::template type<matrix::Specification<T, TI, BATCH_SIZE, 1>> next_action_log_probs;
     };
 
     template<typename T_SPEC>
     struct ActorCritic {
         using SPEC = T_SPEC;
         using T = typename SPEC::T;
         using TI = typename SPEC::TI;
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/config.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/config.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_cpu.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/state.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/sac/loop/core/state.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cuda.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/td3.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/td3.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/config.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/config.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/state.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/algorithms/td3/loop/core/state.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/off_policy_runner.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/off_policy_runner.h`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         static constexpr bool COLLECT_EPISODE_STATS = T_COLLECT_EPISODE_STATS;
         static constexpr TI EPISODE_STATS_BUFFER_SIZE = T_EPISODE_STATS_BUFFER_SIZE;
         using CONTAINER_TYPE_TAG = T_CONTAINER_TYPE_TAG;
         static constexpr bool ASYMMETRIC_OBSERVATIONS = T_ASYMMETRIC_OBSERVATIONS && ENVIRONMENT::OBSERVATION_DIM_PRIVILEGED > 0;
         static_assert(ASYMMETRIC_OBSERVATIONS == T_ASYMMETRIC_OBSERVATIONS, "ASYMMETRIC_OBSERVATIONS requested but not available in the environment");
         static constexpr TI OBSERVATION_DIM_PRIVILEGED = ASYMMETRIC_OBSERVATIONS ? ENVIRONMENT::OBSERVATION_DIM_PRIVILEGED : ENVIRONMENT::OBSERVATION_DIM;
         static constexpr TI OBSERVATION_DIM_PRIVILEGED_ACTUAL = ASYMMETRIC_OBSERVATIONS ? ENVIRONMENT::OBSERVATION_DIM_PRIVILEGED : 0;
+        static constexpr bool ACTION_CLAMPING_TANH = T_STOCHASTIC_POLICY;
     };
 
     template<typename SPEC>
     struct Buffers{
         // todo: make the buffer exploit the observation = observation_priviliged to save memory in the case of symmetric observations
         using T = typename SPEC::T;
         using TI = typename SPEC::TI;
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_accelerate.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_accelerate.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_mkl.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cpu_mkl.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cuda.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic_per_env.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/off_policy_runner/operations_generic_per_env.h`

 * *Files 5% similar despite different names*

```diff
@@ -46,17 +46,26 @@
     template<typename DEVICE, typename SPEC, typename RNG>
     RL_TOOLS_FUNCTION_PLACEMENT auto process_and_get_action(DEVICE& device, rl::components::OffPolicyRunner<SPEC>& runner, RNG &rng, typename DEVICE::index_t env_i) {
         using T = typename SPEC::T;
         using TI = typename SPEC::TI;
         using ENVIRONMENT = typename SPEC::ENVIRONMENT;
         if constexpr(SPEC::STOCHASTIC_POLICY){
             for (TI i = 0; i < ENVIRONMENT::ACTION_DIM; i++){
-                T std = math::exp(typename DEVICE::SPEC::MATH{}, get(runner.buffers.actions, env_i, ENVIRONMENT::ACTION_DIM+i));
-                T action_noisy = random::normal_distribution::sample(typename DEVICE::SPEC::RANDOM(), get(runner.buffers.actions, env_i, i), std, rng);
-                set(runner.buffers.actions, env_i, i, math::clamp<T>(device.math, action_noisy, -1, 1));
+                T log_std = get(runner.buffers.actions, env_i, ENVIRONMENT::ACTION_DIM+i);
+                T log_std_clip = math::clamp<T>(device.math, log_std, -20, 2); // todo: absorb this into the policy
+                T std = math::exp(typename DEVICE::SPEC::MATH{}, log_std_clip);
+                T mu = get(runner.buffers.actions, env_i, i);
+                T action_noisy = random::normal_distribution::sample(typename DEVICE::SPEC::RANDOM(), mu, std, rng);
+                static_assert(SPEC::ACTION_CLAMPING_TANH);
+                if constexpr(SPEC::ACTION_CLAMPING_TANH){
+                    set(runner.buffers.actions, env_i, i, math::tanh<T>(device.math, action_noisy));
+                }
+                else{
+                    set(runner.buffers.actions, env_i, i, math::clamp<T>(device.math, action_noisy, -1, 1));
+                }
             }
             return view(device, runner.buffers.actions, matrix::ViewSpec<1, SPEC::ENVIRONMENT::ACTION_DIM>{}, env_i, 0);
         }
         else{
             for (TI i = 0; i < ENVIRONMENT::ACTION_DIM; i++){
                 T action_noisy = get(runner.buffers.actions, env_i, i) + random::normal_distribution::sample(typename DEVICE::SPEC::RANDOM(), (T) 0, runner.parameters.exploration_noise, rng);
                 set(runner.buffers.actions, env_i, i, math::clamp<T>(device.math, action_noisy, -1, 1));
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/on_policy_runner.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/on_policy_runner.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_accelerate.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_accelerate.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_mkl.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_cpu_mkl.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_extensions.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_extensions.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_per_env.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/operations_generic_per_env.h`

 * *Files 12% similar despite different names*

```diff
@@ -32,18 +32,20 @@
         using TI = typename SPEC::TI;
         T action_log_prob = 0;
         for(TI action_i = 0; action_i < SPEC::ENVIRONMENT::ACTION_DIM; action_i++) {
             T action_mean = get(actions_mean, env_i, action_i);
 //                    std::stringstream topic;
 //                    topic << "action/" << action_i;
 //                    add_scalar(device, device.logger, topic.str(), action_mu);
-            T action_std = math::exp(device.math, get(action_log_std, 0, action_i));
+            static_assert(SPEC::ENVIRONMENT::ACTION_DIM == ACTION_LOG_STD_SPEC::COLS);
+            static_assert(ACTION_LOG_STD_SPEC::ROWS == 1);
+            T current_action_log_std = get(action_log_std, 0, action_i);
+            T action_std = math::exp(device.math, current_action_log_std);
             T action_noisy = random::normal_distribution::sample(typename DEVICE::SPEC::RANDOM(), action_mean, action_std, rng);
-            T action_by_action_std = (action_noisy-action_mean) / action_std;
-            action_log_prob += -0.5 * action_by_action_std * action_by_action_std - math::log(device.math, action_std) - 0.5 * math::log(device.math, 2 * math::PI<T>);
+            action_log_prob += random::normal_distribution::log_prob(device.random, action_mean, current_action_log_std, action_noisy);
             set(actions, env_i, action_i, action_noisy);
         }
         set(dataset.action_log_probs, pos, 0, action_log_prob);
         auto& env = get(runner.environments, 0, env_i);
         auto& state = get(runner.states, 0, env_i);
         typename SPEC::ENVIRONMENT::State next_state;
         auto action = row(device, actions, env_i);
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/persist.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/on_policy_runner/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/persist.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/replay_buffer.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/replay_buffer/replay_buffer.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/persist.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/running_normalizer.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/components/running_normalizer/running_normalizer.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/acrobot.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/acrobot.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/operations_generic.h`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,16 @@
         static_assert(ACTION_SPEC::COLS == 1);
         using namespace rl::environments::acrobot;
         using T = typename SPEC::T;
         using PARAMS = typename SPEC::PARAMETERS;
 
         T state_flat[4] = {state.theta_0, state.theta_1, state.theta_0_dot, state.theta_1_dot};
         T next_state_flat[4];
-        T action_scaled = (get(action, 0, 0) + 1.0) / 2.0 * (PARAMS::MAX_TORQUE - (PARAMS::MIN_TORQUE)) + (PARAMS::MIN_TORQUE);
+        T action_clamped = math::clamp(device.math, get(action, 0, 0), (T)-1, (T)1);
+        T action_scaled = (action_clamped + 1.0) / 2.0 * (PARAMS::MAX_TORQUE - (PARAMS::MIN_TORQUE)) + (PARAMS::MIN_TORQUE);
         rl::environments::acrobot::rk4(state_flat, action_scaled, next_state_flat, PARAMS::DT, PARAMS{});
 
         next_state_flat[0] = angle_normalize(device.math, next_state_flat[0]);
         next_state_flat[1] = angle_normalize(device.math, next_state_flat[1]);
         next_state_flat[2] = math::clamp(    device.math, next_state_flat[2], -PARAMS::MAX_VEL_1, PARAMS::MAX_VEL_1);
         next_state_flat[3] = math::clamp(    device.math, next_state_flat[3], -PARAMS::MAX_VEL_2, PARAMS::MAX_VEL_2);
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/ui.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/acrobot/ui.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/car.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/car.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_cpu.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_generic.h`

 * *Files 5% similar despite different names*

```diff
@@ -55,16 +55,16 @@
     RL_TOOLS_FUNCTION_PLACEMENT typename SPEC::T step(DEVICE& device, const rl::environments::Car<SPEC>& env, const typename rl::environments::Car<SPEC>::State& s, const Matrix<ACTION_SPEC>& action, typename rl::environments::Car<SPEC>::State& next_state, RNG& rng) {
         using ENVIRONMENT = rl::environments::Car<SPEC>;
         static_assert(ACTION_SPEC::ROWS == 1);
         static_assert(ACTION_SPEC::COLS == ENVIRONMENT::ACTION_DIM);
         using namespace rl::environments::car;
         using T = typename SPEC::T;
 
-        T throttle_break = get(action, 0, 0);
-        T delta = get(action, 0, 1);
+        T throttle_break = math::clamp(device.math, get(action, 0, 0), (T)-1, (T)1);
+        T delta = math::clamp(device.math, get(action, 0, 1), (T)-1, (T)1);
         
         auto& p = env.parameters;
         
         T alpha_f = math::atan2(device.math, (s.vy + p.lf * s.omega), s.vx) - delta;
         T alpha_r = math::atan2(device.math, (s.vy - p.lr * s.omega), s.vx);
         T FnF = p.lr / (p.lf + p.lr) * p.m * p.g;
         T FnR = p.lf / (p.lf + p.lr) * p.m * p.g;
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_json.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/operations_json.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/track.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/track.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/ui.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/car/ui.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ant.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ant.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/model.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/model.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/operations_cpu.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ui.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/mujoco/ant/ui.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/operations_generic.h`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     template<typename DEVICE, typename SPEC, typename ACTION_SPEC, typename RNG>
     RL_TOOLS_FUNCTION_PLACEMENT typename SPEC::T step(DEVICE& device, const rl::environments::Pendulum<SPEC>& env, const typename rl::environments::Pendulum<SPEC>::State& state, const Matrix<ACTION_SPEC>& action, typename rl::environments::Pendulum<SPEC>::State& next_state, RNG& rng) {
         static_assert(ACTION_SPEC::ROWS == 1);
         static_assert(ACTION_SPEC::COLS == 1);
         using namespace rl::environments::pendulum;
         typedef typename SPEC::T T;
         typedef typename SPEC::PARAMETERS PARAMS;
-        T u_normalised = get(action, 0, 0);
+        T u_normalised = math::clamp(device.math, get(action, 0, 0), (T)-1, (T)1);
         T u = PARAMS::max_torque * u_normalised;
         T g = PARAMS::g;
         T m = PARAMS::m;
         T l = PARAMS::l;
         T dt = PARAMS::dt;
 
         u = clip(u, -PARAMS::max_torque, PARAMS::max_torque);
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/pendulum.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/pendulum.h`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         using T = typename SPEC::T;
         using TI = typename SPEC::TI;
         using State = pendulum::State<T, TI>;
         using PARAMETERS = typename SPEC::PARAMETERS;
         static constexpr TI OBSERVATION_DIM = 3;
         static constexpr TI OBSERVATION_DIM_PRIVILEGED = OBSERVATION_DIM;
         static constexpr TI ACTION_DIM = 1;
+        static constexpr TI EPISODE_STEP_LIMIT = 200;
     };
 }
 RL_TOOLS_NAMESPACE_WRAPPER_END
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui_xeus.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/environments/pendulum/ui_xeus.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/config.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/config.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/state.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/evaluation/state.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/operations_cpu.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/state.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/loop/steps/timing/state.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/utils/evaluation.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/utils/evaluation.h`

 * *Files 4% similar despite different names*

```diff
@@ -59,16 +59,18 @@
         malloc(device, action_full);
         observe(device, env, state, observation, rng);
         normalize(device, observation_mean, observation_std, observation, observation_normalized);
 
         auto action = view(device, action_full, matrix::ViewSpec<1, ENVIRONMENT::ACTION_DIM>{});
         evaluate(device, policy, observation_normalized, action_full, policy_eval_buffers);
 
-        for(TI action_i=0; action_i<ENVIRONMENT::ACTION_DIM; action_i++){
-            set(action, 0, action_i, math::clamp<T>(device.math, get(action, 0, action_i), -1, 1));
+        if constexpr(STOCHASTIC_POLICY){ // todo: This is a special case for SAC, will be uneccessary once (https://github.com/rl-tools/rl-tools/blob/72a59eabf4038502c3be86a4f772bd72526bdcc8/TODO.md?plain=1#L22) is implemented
+            for(TI action_i=0; action_i<ENVIRONMENT::ACTION_DIM; action_i++){
+                    set(action, 0, action_i, math::tanh<T>(device.math, get(action, 0, action_i)));
+            }
         }
         typename ENVIRONMENT::State next_state;
         T dt = step(device, env, state, action, next_state, rng);
         set_state(device, env, ui, state);
         set_action(device, env, ui, action);
         render(device, env, ui);
         T r = reward(device, env, state, action, next_state, rng);
```

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation_analysis.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/rl/utils/validation_analysis.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/ui_server/server.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/ui_server/server.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_boost.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_boost.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_cpu.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/ui_server/client/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/persist.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/persist.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_arm.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_arm.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cpu.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cpu.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cuda.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_dummy.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_dummy.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_esp32.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_esp32.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/assert/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/generic/integrators.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/generic/integrators.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/generic/typing.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/generic/typing.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/generic/vector_operations.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/generic/vector_operations.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_cuda.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_cuda.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_generic.h` & `tinyrl-0.4.0/tinyrl/external/rl_tools/include/rl_tools/utils/polyak/operations_generic.h`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/interface/algorithms/sac/template.h` & `tinyrl-0.4.0/tinyrl/interface/algorithms/sac/template.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 #include <rl_tools/rl/algorithms/sac/loop/core/config.h>
 #include <rl_tools/rl/loop/steps/evaluation/config.h>
 #include <rl_tools/rl/loop/steps/timing/config.h>
 #include <rl_tools/rl/algorithms/sac/loop/core/operations_cpu.h>
 #include <rl_tools/rl/loop/steps/evaluation/operations_generic.h>
 #include <rl_tools/rl/loop/steps/timing/operations_cpu.h>
 
+namespace TINYRL_MODULE_NAME{
 
-namespace rlt = rl_tools;
+    namespace rlt = rl_tools;
 
-template <typename T, typename TI, typename ENVIRONMENT, TI T_EPISODE_STEP_LIMIT>
-struct SAC_LOOP_CORE_PARAMETERS: rlt::rl::algorithms::sac::loop::core::DefaultParameters<T, TI, ENVIRONMENT>{
-    struct SAC_PARAMETERS {
-        static constexpr T GAMMA = $GAMMA;
-        static constexpr T ALPHA = $ALPHA;
-        static constexpr TI ACTOR_BATCH_SIZE = $ACTOR_BATCH_SIZE;
-        static constexpr TI CRITIC_BATCH_SIZE = $CRITIC_BATCH_SIZE;
-        static constexpr TI N_WARMUP_STEPS_CRITIC = 0;
-        static constexpr TI N_WARMUP_STEPS_ACTOR = 0;
-        static constexpr TI CRITIC_TRAINING_INTERVAL = $CRITIC_TRAINING_INTERVAL;
-        static constexpr TI ACTOR_TRAINING_INTERVAL = $ACTOR_TRAINING_INTERVAL;
-        static constexpr TI CRITIC_TARGET_UPDATE_INTERVAL = $CRITIC_TARGET_UPDATE_INTERVAL;
-        static constexpr T ACTOR_POLYAK = $ACTOR_POLYAK;
-        static constexpr T CRITIC_POLYAK = $CRITIC_POLYAK;
-        static constexpr bool IGNORE_TERMINATION = $IGNORE_TERMINATION; 
-        static constexpr T TARGET_ENTROPY = $TARGET_ENTROPY;
-        static constexpr bool ADAPTIVE_ALPHA = $ADAPTIVE_ALPHA;
+    // This should stay in sync with the parameters in https://github.com/rl-tools/rl-tools/blob/a98bc461f7ebfed0ba71c653216edec6d9334b78/include/rl_tools/rl/algorithms/sac/loop/core/config.h#L18
+    template <typename T, typename TI, typename ENVIRONMENT, TI T_EPISODE_STEP_LIMIT>
+    struct SAC_LOOP_CORE_PARAMETERS: rlt::rl::algorithms::sac::loop::core::DefaultParameters<T, TI, ENVIRONMENT>{
+        struct SAC_PARAMETERS{
+            static constexpr T GAMMA = $GAMMA;
+            static constexpr T ALPHA = $ALPHA;
+            static constexpr TI ACTOR_BATCH_SIZE = $ACTOR_BATCH_SIZE;
+            static constexpr TI CRITIC_BATCH_SIZE = $CRITIC_BATCH_SIZE;
+            static constexpr TI N_WARMUP_STEPS_CRITIC = 0;
+            static constexpr TI N_WARMUP_STEPS_ACTOR = 0;
+            static constexpr TI CRITIC_TRAINING_INTERVAL = $CRITIC_TRAINING_INTERVAL;
+            static constexpr TI ACTOR_TRAINING_INTERVAL = $ACTOR_TRAINING_INTERVAL;
+            static constexpr TI CRITIC_TARGET_UPDATE_INTERVAL = $CRITIC_TARGET_UPDATE_INTERVAL;
+            static constexpr T ACTOR_POLYAK = $ACTOR_POLYAK;
+            static constexpr T CRITIC_POLYAK = $CRITIC_POLYAK;
+            static constexpr bool IGNORE_TERMINATION = $IGNORE_TERMINATION; 
+            static constexpr T TARGET_ENTROPY = $TARGET_ENTROPY;
+            static constexpr bool ADAPTIVE_ALPHA = $ADAPTIVE_ALPHA;
+            static constexpr T ACTION_LOG_STD_LOWER_BOUND = $ACTION_LOG_STD_LOWER_BOUND;
+            static constexpr T ACTION_LOG_STD_UPPER_BOUND = $ACTION_LOG_STD_UPPER_BOUND;
+        };
+        static constexpr TI N_ENVIRONMENTS = $N_ENVIRONMENTS;
+        static constexpr TI N_WARMUP_STEPS = $N_WARMUP_STEPS;
+        static constexpr TI STEP_LIMIT = $STEP_LIMIT;
+        static constexpr TI REPLAY_BUFFER_CAP = $REPLAY_BUFFER_CAP;
+        static constexpr TI EPISODE_STEP_LIMIT = T_EPISODE_STEP_LIMIT;
+        static constexpr TI ACTOR_HIDDEN_DIM = $ACTOR_HIDDEN_DIM;
+        static constexpr TI ACTOR_NUM_LAYERS = $ACTOR_NUM_LAYERS;
+        static constexpr auto ACTOR_ACTIVATION_FUNCTION = rlt::nn::activation_functions::ActivationFunction::$ACTOR_ACTIVATION_FUNCTION;
+        static constexpr TI CRITIC_HIDDEN_DIM = $CRITIC_HIDDEN_DIM;
+        static constexpr TI CRITIC_NUM_LAYERS = $CRITIC_NUM_LAYERS;
+        static constexpr auto CRITIC_ACTIVATION_FUNCTION = rlt::nn::activation_functions::ActivationFunction::$CRITIC_ACTIVATION_FUNCTION;
+        static constexpr bool COLLECT_EPISODE_STATS = $COLLECT_EPISODE_STATS;
+        static constexpr TI EPISODE_STATS_BUFFER_SIZE = $EPISODE_STATS_BUFFER_SIZE;
+        struct OPTIMIZER_PARAMETERS: rlt::nn::optimizers::adam::DEFAULT_PARAMETERS_TENSORFLOW<T>{
+            static constexpr T ALPHA = $OPTIMIZER_ALPHA;
+            static constexpr T BETA_1 = $OPTIMIZER_BETA_1;
+            static constexpr T BETA_2 = $OPTIMIZER_BETA_2;
+            static constexpr T EPSILON = $OPTIMIZER_EPSILON;
+        };
     };
-    static constexpr TI N_ENVIRONMENTS = $N_ENVIRONMENTS;
-    static constexpr TI N_WARMUP_STEPS = $N_WARMUP_STEPS;
-    static constexpr TI STEP_LIMIT = $STEP_LIMIT;
-    static constexpr TI REPLAY_BUFFER_CAP = $REPLAY_BUFFER_CAP;
-    static constexpr TI EPISODE_STEP_LIMIT = $EPISODE_STEP_LIMIT;
-    static constexpr TI ACTOR_HIDDEN_DIM = $ACTOR_HIDDEN_DIM;
-    static constexpr TI ACTOR_NUM_LAYERS = $ACTOR_NUM_LAYERS;
-    static constexpr auto ACTOR_ACTIVATION_FUNCTION = rlt::nn::activation_functions::ActivationFunction::$ACTOR_ACTIVATION_FUNCTION;
-    static constexpr TI CRITIC_HIDDEN_DIM = $CRITIC_HIDDEN_DIM;
-    static constexpr TI CRITIC_NUM_LAYERS = $CRITIC_NUM_LAYERS;
-    static constexpr auto CRITIC_ACTIVATION_FUNCTION = rlt::nn::activation_functions::ActivationFunction::$CRITIC_ACTIVATION_FUNCTION;
-    static constexpr bool COLLECT_EPISODE_STATS = $COLLECT_EPISODE_STATS;
-    static constexpr TI EPISODE_STATS_BUFFER_SIZE = $EPISODE_STATS_BUFFER_SIZE;
-    struct OPTIMIZER_PARAMETERS: rlt::nn::optimizers::adam::DEFAULT_PARAMETERS_TENSORFLOW<T>{
-        static constexpr T ALPHA = $OPTIMIZER_ALPHA;
-        static constexpr T BETA_1 = $OPTIMIZER_BETA_1;
-        static constexpr T BETA_2 = $OPTIMIZER_BETA_2;
-        static constexpr T EPSILON = $OPTIMIZER_EPSILON;
-    };
-};
 
-template <typename T, typename TI, typename RNG, typename ENVIRONMENT, TI T_EPISODE_STEP_LIMIT>
-using LOOP_CORE_CONFIG_FACTORY = rlt::rl::algorithms::sac::loop::core::Config<T, TI, RNG, ENVIRONMENT, SAC_LOOP_CORE_PARAMETERS<T, TI, ENVIRONMENT, T_EPISODE_STEP_LIMIT>>;
+    template <typename T, typename TI, typename RNG, typename ENVIRONMENT, TI T_EPISODE_STEP_LIMIT>
+    using LOOP_CORE_CONFIG_FACTORY = rlt::rl::algorithms::sac::loop::core::Config<T, TI, RNG, ENVIRONMENT, SAC_LOOP_CORE_PARAMETERS<T, TI, ENVIRONMENT, T_EPISODE_STEP_LIMIT>>;
+}
```

### Comparing `tinyrl-0.3.1/tinyrl/interface/inference/inference.cpp` & `tinyrl-0.4.0/tinyrl/interface/inference/inference.cpp`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/interface/python_environment/operations_cpu.h` & `tinyrl-0.4.0/tinyrl/interface/python_environment/operations_cpu.h`

 * *Files 8% similar despite different names*

```diff
@@ -48,19 +48,22 @@
         }
         if(low.shape(0) != SPEC::ACTION_DIM || high.shape(0) != SPEC::ACTION_DIM){
             throw std::runtime_error("Incompatible action space dimension. Limits: low " + std::to_string(low.shape(0)) + ", high " + std::to_string(high.shape(0)) + " (expected " + std::to_string(SPEC::ACTION_DIM) + "). Check the action space dimension returned by env.action_space and the one configured when building the TinyRL interface");
         }
         for(TI action_i=0; action_i<SPEC::ACTION_DIM; action_i++){
             T current_low = low.at(action_i);
             T current_high = high.at(action_i);
-            env.action_space_offset[action_i] = (current_high + current_low)/2;
-            env.action_space_range[action_i] = (current_high - current_low)/2;
-#ifdef TINYRL_VERBOSE
-            std::cout << "Action dim: " << action_i << " low: " << current_low << " high: " << current_high << std::endl;
-#endif
+//             env.action_space_offset[action_i] = (current_high + current_low)/2;
+//             env.action_space_range[action_i] = (current_high - current_low)/2;
+// #ifdef TINYRL_VERBOSE
+//             std::cout << "Action dim: " << action_i << " low: " << current_low << " high: " << current_high << std::endl;
+// #endif
+            if(math::abs(device.math, current_low - (-1.0)) > 1e-6 || math::abs(device.math, current_high - 1.0) > 1e-6){
+                throw std::runtime_error("Incompatible action space limits. Limits: low " + std::to_string(current_low) + ", high " + std::to_string(current_high) + " (expected -1.0 and 1.0). You should use a RescaleActionV0(env, -1, 1) or equivalent.");
+            };
         }
     }
     template<typename DEVICE, typename SPEC>
     static void init(DEVICE& device, PythonEnvironment<SPEC>& env){}
     template<typename DEVICE, typename SPEC>
     static void initial_state(DEVICE& device, const PythonEnvironment<SPEC>& env, typename PythonEnvironment<SPEC>::State& state){
         using T = typename SPEC::T;
@@ -83,15 +86,15 @@
         static_assert(ACTION_SPEC::COLS == SPEC::ACTION_DIM);
         using T = typename SPEC::T;
 
         pybind11::array_t<T> action_array(SPEC::ACTION_DIM);
         pybind11::buffer_info action_info = action_array.request();
         auto action_data_ptr = static_cast<T*>(action_info.ptr);
         for(size_t i=0; i<SPEC::ACTION_DIM; i++){
-            action_data_ptr[i] = get(action, 0, i) * env.action_space_range[i] + env.action_space_offset[i];
+            action_data_ptr[i] = get(action, 0, i); // * env.action_space_range[i] + env.action_space_offset[i];
         }
         auto result = env.environment->attr("step")(action_array);
         pybind11::tuple result_tuple = pybind11::cast<pybind11::tuple>(result);
         auto observation = result_tuple[0];
         auto reward = result_tuple[1];
         auto terminated = result_tuple[2];
         auto truncated = result_tuple[3];
```

### Comparing `tinyrl-0.3.1/tinyrl/interface/python_environment/python_environment.h` & `tinyrl-0.4.0/tinyrl/interface/python_environment/python_environment.h`

 * *Files 16% similar despite different names*

```diff
@@ -28,10 +28,10 @@
     using T = typename SPEC::T;
     using TI = typename SPEC::TI;
     using State = PythonEnvironmentState<T, TI, SPEC::OBSERVATION_DIM>;
     static constexpr TI OBSERVATION_DIM = SPEC::OBSERVATION_DIM;
     static constexpr TI OBSERVATION_DIM_PRIVILEGED = SPEC::OBSERVATION_DIM;
     static constexpr TI ACTION_DIM = SPEC::ACTION_DIM;
     pybind11::object* environment;
-    T action_space_range[ACTION_DIM];
-    T action_space_offset[ACTION_DIM];
+    // T action_space_range[ACTION_DIM];
+    // T action_space_offset[ACTION_DIM];
 };
```

### Comparing `tinyrl-0.3.1/tinyrl/interface/training/training.cpp` & `tinyrl-0.4.0/tinyrl/interface/training/training.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -2,18 +2,14 @@
 #error "TINYRL_MODULE_NAME not defined"
 #endif
 
 #ifndef TINYRL_DTYPE
 #define TINYRL_DTYPE float
 #endif
 
-#ifndef TINYRL_EPISODE_STEP_LIMIT
-#define TINYRL_EPISODE_STEP_LIMIT 200
-#endif
-
 #include <rl_tools/operations/cpu_mux.h>
 #include <rl_tools/nn/operations_cpu_mux.h>
 
 #ifdef TINYRL_USE_PYTHON_ENVIRONMENT
 #include "../python_environment/operations_cpu.h"
 #else
 #include <environment.h>
@@ -21,136 +17,153 @@
 
 #include <rl_tools/nn_models/sequential/operations_generic.h>
 #include <rl_tools/nn/optimizers/adam/persist_code.h>
 #include <rl_tools/nn/layers/dense/persist_code.h>
 #include <rl_tools/nn/parameters/persist_code.h>
 #include <rl_tools/nn_models/sequential/persist_code.h>
 #include <rl_tools/nn_models/mlp_unconditional_stddev/operations_generic.h>
+#include <rl_tools/nn_models/mlp/persist_code.h>
+// #include <rl_tools/nn_models/mlp/persist_code.h>
 
 #include "loop_core_config.h"
 
 namespace rlt = rl_tools;
 
 #include <pybind11/pybind11.h>
 #include <pybind11/functional.h>
 #include <pybind11/numpy.h>
 #include <pybind11/stl.h>
 
-using DEVICE = rlt::devices::DEVICE_FACTORY<>;
-using RNG = decltype(rlt::random::default_engine(typename DEVICE::SPEC::RANDOM{}));
-using TI = typename DEVICE::index_t;
-
-using T = TINYRL_DTYPE;
-
-
-#ifdef TINYRL_USE_PYTHON_ENVIRONMENT
-constexpr TI OBSERVATION_DIM = TINYRL_OBSERVATION_DIM;
-constexpr TI ACTION_DIM = TINYRL_ACTION_DIM;
-using ENVIRONMENT_SPEC = PythonEnvironmentSpecification<T, TI, OBSERVATION_DIM, ACTION_DIM>;
-using ENVIRONMENT = PythonEnvironment<ENVIRONMENT_SPEC>;
-#else
-using ENVIRONMENT = ENVIRONMENT_FACTORY<T, TI>;
-#endif
-
-#ifdef TINYRL_ENABLE_EVALUATION
-constexpr bool ENABLE_EVALUATION = true;
-#else
-constexpr bool ENABLE_EVALUATION = false;
-#endif
-constexpr TI EPISODE_STEP_LIMIT = TINYRL_EPISODE_STEP_LIMIT;
-
-
-
-// #ifdef TINYRL_USE_PPO
-// using LOOP_CORE_CONFIG = PPO_LOOP_CORE_CONFIG<T, TI, RNG, ENVIRONMENT, EPISODE_STEP_LIMIT>;
-// #else
-using LOOP_CORE_CONFIG = LOOP_CORE_CONFIG_FACTORY<T, TI, RNG, ENVIRONMENT, EPISODE_STEP_LIMIT>;
-// #endif
-
-
-template <typename NEXT>
-struct LOOP_EVAL_PARAMETERS: rlt::rl::loop::steps::evaluation::Parameters<T, TI, NEXT>{
-    static constexpr TI EVALUATION_INTERVAL = 1000;
-    static constexpr TI NUM_EVALUATION_EPISODES = 10;
-    static constexpr TI N_EVALUATIONS = NEXT::CORE_PARAMETERS::STEP_LIMIT / EVALUATION_INTERVAL;
-};
 
-DEVICE device;
-
-using LOOP_EVAL_CONFIG = rlt::utils::typing::conditional_t<ENABLE_EVALUATION, rlt::rl::loop::steps::evaluation::Config<LOOP_CORE_CONFIG, LOOP_EVAL_PARAMETERS<LOOP_CORE_CONFIG>>, LOOP_CORE_CONFIG>;
-using LOOP_TIMING_CONFIG = rlt::rl::loop::steps::timing::Config<LOOP_EVAL_CONFIG>;
-using LOOP_CONFIG = LOOP_TIMING_CONFIG;
-using LOOP_STATE = typename LOOP_CONFIG::template State<LOOP_CONFIG>;
-
-#ifdef TINYRL_USE_PYTHON_ENVIRONMENT
-void set_environment_factory(std::function<pybind11::object()> p_environment_factory){
-    environment_factory = p_environment_factory;
-    auto python_atexit = pybind11::module_::import("atexit");
-    python_atexit.attr("register")(pybind11::cpp_function([]() {
-        environment_factory = nullptr;
-    }));
-}
-#endif
-
-struct State: LOOP_STATE{
-    State(TI seed){
-        rlt::malloc(device, static_cast<LOOP_STATE&>(*this));
-        rlt::init(device, static_cast<LOOP_STATE&>(*this), seed);
-// #ifdef TINYRL_USE_PPO
-//         state.actor_optimizer.parameters.alpha = 1e-3;
-//         state.critic_optimizer.parameters.alpha = 1e-3;
-// #endif
+namespace TINYRL_MODULE_NAME{
+    using DEVICE = rlt::devices::DEVICE_FACTORY<>;
+#ifdef TINYRL_FORCE_BLAS
+    static_assert(DEVICE::DEVICE_ID == rlt::devices::DeviceId::CPU_MKL || DEVICE::DEVICE_ID == rlt::devices::DeviceId::CPU_ACCELERATE || DEVICE::DEVICE_ID == rlt::devices::DeviceId::CPU_OPENBLAS);
+#endif
+    using RNG = decltype(rlt::random::default_engine(typename DEVICE::SPEC::RANDOM{}));
+    using TI = typename DEVICE::index_t;
+
+    using T = TINYRL_DTYPE;
+
+
+    #ifdef TINYRL_USE_PYTHON_ENVIRONMENT
+    constexpr TI OBSERVATION_DIM = TINYRL_OBSERVATION_DIM;
+    constexpr TI ACTION_DIM = TINYRL_ACTION_DIM;
+    using ENVIRONMENT_SPEC = PythonEnvironmentSpecification<T, TI, OBSERVATION_DIM, ACTION_DIM>;
+    using ENVIRONMENT = PythonEnvironment<ENVIRONMENT_SPEC>;
+    #else
+    using ENVIRONMENT = ENVIRONMENT_FACTORY<T, TI>;
+    #endif
+
+    #ifdef TINYRL_EPISODE_STEP_LIMIT
+    constexpr TI EPISODE_STEP_LIMIT = TINYRL_EPISODE_STEP_LIMIT;
+    #else
+    constexpr TI EPISODE_STEP_LIMIT = ENVIRONMENT::EPISODE_STEP_LIMIT;
+    #endif
+
+
+
+    // #ifdef TINYRL_USE_PPO
+    // using LOOP_CORE_CONFIG = PPO_LOOP_CORE_CONFIG<T, TI, RNG, ENVIRONMENT, EPISODE_STEP_LIMIT>;
+    // #else
+    using LOOP_CORE_CONFIG = LOOP_CORE_CONFIG_FACTORY<T, TI, RNG, ENVIRONMENT, EPISODE_STEP_LIMIT>;
+    // #endif
+
+
+
+    DEVICE device;
+
+    #ifdef TINYRL_ENABLE_EVALUATION
+    constexpr bool ENABLE_EVALUATION = true;
+    #ifndef TINYRL_EVALUATION_INTERVAL
+    #error "TINYRL_EVALUATION_INTERVAL not defined"
+    #else
+    constexpr TI PARAMETER_EVALUATION_INTERVAL = TINYRL_EVALUATION_INTERVAL;
+    constexpr TI PARAMETER_NUM_EVALUATION_EPISODES = TINYRL_NUM_EVALUATION_EPISODES;
+
+    template <typename NEXT>
+    struct LOOP_EVAL_PARAMETERS: rlt::rl::loop::steps::evaluation::Parameters<T, TI, NEXT>{
+        static constexpr TI EVALUATION_INTERVAL = PARAMETER_EVALUATION_INTERVAL;
+        static constexpr TI NUM_EVALUATION_EPISODES = PARAMETER_NUM_EVALUATION_EPISODES;
+        static constexpr TI N_EVALUATIONS = NEXT::CORE_PARAMETERS::STEP_LIMIT / EVALUATION_INTERVAL;
+    };
+    using LOOP_EVAL_CONFIG = rlt::rl::loop::steps::evaluation::Config<LOOP_CORE_CONFIG, LOOP_EVAL_PARAMETERS<LOOP_CORE_CONFIG>>;
+    #endif
+    #else
+    constexpr bool ENABLE_EVALUATION = false;
+    using LOOP_EVAL_CONFIG = LOOP_CORE_CONFIG;
+    #endif
+    using LOOP_TIMING_CONFIG = rlt::rl::loop::steps::timing::Config<LOOP_EVAL_CONFIG>;
+    using LOOP_CONFIG = LOOP_TIMING_CONFIG;
+    using LOOP_STATE = typename LOOP_CONFIG::template State<LOOP_CONFIG>;
+
+    #ifdef TINYRL_USE_PYTHON_ENVIRONMENT
+    void set_environment_factory(std::function<pybind11::object()> p_environment_factory){
+        environment_factory = p_environment_factory;
+        auto python_atexit = pybind11::module_::import("atexit");
+        python_atexit.attr("register")(pybind11::cpp_function([]() {
+            environment_factory = nullptr;
+        }));
     }
-    bool step(){
-        return rlt::step(device, static_cast<LOOP_STATE&>(*this));
-    }
-    pybind11::array_t<T> action(const pybind11::array_t<T>& observation){
-        pybind11::buffer_info observation_info = observation.request();
-        if (observation_info.format != pybind11::format_descriptor<T>::format() || observation_info.ndim != 1) {
-            throw std::runtime_error("Incompatible buffer format. Check the floating point type of the observation returned by env.step() and the one configured when building the TinyRL interface");
-        }
-        auto observation_data_ptr = static_cast<T*>(observation_info.ptr);
-        size_t num_elements = observation_info.shape[0];
-        if(num_elements != ENVIRONMENT::OBSERVATION_DIM){
-            throw std::runtime_error("Incompatible observation dimension. Check the dimension of the observation returned by env.step() and the one configured when building the TinyRL interface");
+    #endif
+    struct State: LOOP_STATE{
+        State(TI seed){
+            rlt::malloc(device, static_cast<LOOP_STATE&>(*this));
+            rlt::init(device, static_cast<LOOP_STATE&>(*this), seed);
         }
-        rlt::MatrixStatic<rlt::matrix::Specification<T, TI, 1, ENVIRONMENT::OBSERVATION_DIM>> observation_rlt;
-        rlt::malloc(device, observation_rlt);
-        for(TI observation_i=0; observation_i<num_elements; observation_i++){
-            rlt::set(observation_rlt, 0, observation_i, observation_data_ptr[observation_i]);
+        bool step(){
+            return rlt::step(device, static_cast<LOOP_STATE&>(*this));
         }
-        rlt::MatrixStatic<rlt::matrix::Specification<T, TI, 1, 2*ENVIRONMENT::ACTION_DIM>> action_distribution; //2x for mean and std
-        rlt::malloc(device, action_distribution);
-        rlt::evaluate(device, rlt::get_actor(*this), observation_rlt, action_distribution, this->actor_deterministic_evaluation_buffers);
-        rlt::free(device, observation_rlt);
+        pybind11::array_t<T> action(const pybind11::array_t<T>& observation){
+            pybind11::buffer_info observation_info = observation.request();
+            if (observation_info.format != pybind11::format_descriptor<T>::format() || observation_info.ndim != 1) {
+                throw std::runtime_error("Incompatible buffer format. Check the floating point type of the observation returned by env.step() and the one configured when building the TinyRL interface");
+            }
+            auto observation_data_ptr = static_cast<T*>(observation_info.ptr);
+            size_t num_elements = observation_info.shape[0];
+            if(num_elements != ENVIRONMENT::OBSERVATION_DIM){
+                throw std::runtime_error("Incompatible observation dimension. Check the dimension of the observation returned by env.step() and the one configured when building the TinyRL interface");
+            }
+            rlt::MatrixStatic<rlt::matrix::Specification<T, TI, 1, ENVIRONMENT::OBSERVATION_DIM>> observation_rlt;
+            rlt::malloc(device, observation_rlt);
+            for(TI observation_i=0; observation_i<num_elements; observation_i++){
+                rlt::set(observation_rlt, 0, observation_i, observation_data_ptr[observation_i]);
+            }
+            using ACTOR_TYPE = rlt::utils::typing::remove_reference<decltype(rlt::get_actor(*this))>::type;
+            rlt::MatrixStatic<rlt::matrix::Specification<T, TI, 1, ACTOR_TYPE::OUTPUT_DIM>> action_distribution; //2x for mean and std
+            rlt::malloc(device, action_distribution);
+            rlt::evaluate(device, rlt::get_actor(*this), observation_rlt, action_distribution, this->actor_deterministic_evaluation_buffers);
+            rlt::free(device, observation_rlt);
+
+            auto action_rlt = rlt::view(device, action_distribution, rlt::matrix::ViewSpec<1, ENVIRONMENT::ACTION_DIM>{});
+
+            std::vector<T> action(ENVIRONMENT::ACTION_DIM);
+
+            for (TI action_i = 0; action_i < ENVIRONMENT::ACTION_DIM; action_i++){
+                action[action_i] = rlt::get(action_rlt, 0, action_i);
+            }
 
-        auto action_rlt = rlt::view(device, action_distribution, rlt::matrix::ViewSpec<1, ENVIRONMENT::ACTION_DIM>{});
-
-        std::vector<T> action(ENVIRONMENT::ACTION_DIM);
-
-        for (TI action_i = 0; action_i < ENVIRONMENT::ACTION_DIM; action_i++){
-            action[action_i] = rlt::get(action_rlt, 0, action_i);
+            return pybind11::array_t<T>(ENVIRONMENT::ACTION_DIM, action.data());
+        }
+        std::string export_policy(){
+            return rlt::save_code(device, rlt::get_actor(*this), "policy");
+        }
+        ~State(){
+            rlt::free(device, static_cast<LOOP_STATE&>(*this));
         }
+    };
+}
 
-        return pybind11::array_t<T>(ENVIRONMENT::ACTION_DIM, action.data());
-    }
-    std::string export_policy(){
-        return rlt::save_code(device, rlt::get_actor(*this), "policy");
-    }
-    ~State(){
-        rlt::free(device, static_cast<LOOP_STATE&>(*this));
-    }
-};
 
 
 
 PYBIND11_MODULE(TINYRL_MODULE_NAME, m){
-    m.doc() = "TinyRL SAC Training Loop";
-    pybind11::class_<State>(m, "State")
-            .def(pybind11::init<TI>())
-            .def("step", &State::step, "Step the loop")
-            .def("action", &State::action, "Get the action for the given observation")
-            .def("export_policy", &State::export_policy, "Export the policy to a python file");
+    m.doc() = "TinyRL Training Loop";
+    pybind11::class_<TINYRL_MODULE_NAME::State>(m, "State")
+            .def(pybind11::init<TINYRL_MODULE_NAME::TI>())
+            .def("step", &TINYRL_MODULE_NAME::State::step, "Step the loop")
+            .def("action", &TINYRL_MODULE_NAME::State::action, "Get the action for the given observation")
+            .def("export_policy", &TINYRL_MODULE_NAME::State::export_policy, "Export the policy to a python file");
 #ifdef TINYRL_USE_PYTHON_ENVIRONMENT
-    m.def("set_environment_factory", &set_environment_factory, "Set the environment factory");
+    m.def("set_environment_factory", &TINYRL_MODULE_NAME::set_environment_factory, "Set the environment factory");
 #endif
 }
```

### Comparing `tinyrl-0.3.1/tinyrl/src/render.py` & `tinyrl-0.4.0/tinyrl/src/render.py`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/tinyrl/src/sac.py` & `tinyrl-0.4.0/tinyrl/src/sac.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,100 +1,88 @@
-import os, sys, importlib
-
-from .compile import compile
-from .load_module import load_module
+import os
 from .render import render, sanitize_values
-from .accelerate import acceleration_flags
+from .training import compile_training
+from .compile import compile_option
 
 from .. import CACHE_PATH
 
 
 absolute_path = os.path.dirname(os.path.abspath(__file__))
 
-
 def SAC(env_factory, # can be either a lambda that creates a new Gym-like environment, or a dict with a specification of a C++ environment: {"path": "path/to/environment", "action_dim": xx, "observation_dim": yy}
+    verbose=False,
     force_recompile=False,
     enable_evaluation=True,
+    evaluation_interval=1000,
+    num_evaluation_episodes=10,
+    interface_name="default", # this is the namespace used for the compilation of the TinyRL interface (in a temporary directory) and should be unique if run in parallel. We don't choose a random uuid because it would invalidate the cache and require a re-compilation every time
     # Compile-time parameters:
+    # Same set of parameters as: rl::algorithms::td3::DefaultParameters
     GAMMA = 0.99,
     ALPHA = 0.5,
     ACTOR_BATCH_SIZE = 100, #32,
     CRITIC_BATCH_SIZE = 100, #32,
     CRITIC_TRAINING_INTERVAL = 1,
     ACTOR_TRAINING_INTERVAL = 1,
     CRITIC_TARGET_UPDATE_INTERVAL = 1,
     ACTOR_POLYAK = 1.0 - 0.005,
     CRITIC_POLYAK = 1.0 - 0.005,
     IGNORE_TERMINATION = False,
     TARGET_ENTROPY = None,
     ADAPTIVE_ALPHA = True,
+    ACTION_LOG_STD_LOWER_BOUND=-20,
+    ACTION_LOG_STD_UPPER_BOUND=2,
+    # Same set of parameters as rl::algorithms::sac::loop::core::DefaultParameters
     N_ENVIRONMENTS = 1,
     N_WARMUP_STEPS = None,
     STEP_LIMIT = 10000,
     REPLAY_BUFFER_CAP = None,
-    EPISODE_STEP_LIMIT = 200,
+    EPISODE_STEP_LIMIT = None,
     ACTOR_HIDDEN_DIM = 64,
     ACTOR_NUM_LAYERS = 3,
     ACTOR_ACTIVATION_FUNCTION = "RELU",
     CRITIC_HIDDEN_DIM = 64,
     CRITIC_NUM_LAYERS = 3,
     CRITIC_ACTIVATION_FUNCTION = "RELU",
     COLLECT_EPISODE_STATS = True,
     EPISODE_STATS_BUFFER_SIZE = 1000,
     # optimizer
     OPTIMIZER_ALPHA=1e-3,
     OPTIMIZER_BETA_1=0.9,
     OPTIMIZER_BETA_2=0.999,
     OPTIMIZER_EPSILON=1e-7,
+    **kwargs
     ):
+    verbose = verbose or "TINYRL_VERBOSE" in os.environ
 
-    use_python_environment = type(env_factory) != dict
-    custom_environment_header_search_path = None if use_python_environment else env_factory["path"]
-    custom_environment_flag = '-I' + custom_environment_header_search_path if custom_environment_header_search_path is not None else ''
 
+    # The action dim is needed to set the default target entropy
+    use_python_environment = type(env_factory) != dict
     if use_python_environment:
         example_env = env_factory()
         ACTION_DIM = example_env.action_space.shape[0]
     else:
         ACTION_DIM = env_factory["action_dim"]
 
     TARGET_ENTROPY = TARGET_ENTROPY if TARGET_ENTROPY is not None else -ACTION_DIM
     REPLAY_BUFFER_CAP = REPLAY_BUFFER_CAP if REPLAY_BUFFER_CAP is not None else STEP_LIMIT
     N_WARMUP_STEPS = N_WARMUP_STEPS if N_WARMUP_STEPS is not None else max(ACTOR_BATCH_SIZE, CRITIC_BATCH_SIZE)
 
     compile_time_parameters = sanitize_values(locals())
 
-    module_name = 'tinyrl_sac'
-
-    use_python_environment_flag = '-DTINYRL_USE_PYTHON_ENVIRONMENT' if use_python_environment else ''
-    observation_dim_flag = f'-DTINYRL_OBSERVATION_DIM={example_env.observation_space.shape[0]}' if use_python_environment else ''
-    action_dim_flag = f'-DTINYRL_ACTION_DIM={ACTION_DIM}' if use_python_environment else ''
-    enable_evaluation_flag = '-DTINYRL_ENABLE_EVALUATION' if enable_evaluation else ''
-    module_flag = f'-DTINYRL_MODULE_NAME={module_name}'
-
-    flags = [use_python_environment_flag, custom_environment_flag, observation_dim_flag, action_dim_flag, enable_evaluation_flag, module_flag]
+    module_name = f'tinyrl_sac_{interface_name}'
 
-
-    flags += acceleration_flags()
-
-    source = os.path.join(absolute_path, '../interface/training/training.cpp')
     config_template = os.path.join(absolute_path, '../interface/algorithms/sac/template.h')
 
+    print('TinyRL Cache Path: ', CACHE_PATH, flush=True) if verbose else None
     render_output_directory = os.path.join(CACHE_PATH, 'template', module_name)
     
     os.makedirs(render_output_directory, exist_ok=True)
     render_output_path = os.path.join(render_output_directory, 'loop_core_config.h')
     new_config = render(config_template, render_output_path, **compile_time_parameters)
     if new_config:
         print('New SAC config detected, forcing recompilation...')
     
-    loop_core_config_search_path_flag = f'-I{render_output_directory}'
-    loop_core_config_flag = "-DTINYRL_USE_LOOP_CORE_CONFIG"
-
-    flags += [loop_core_config_search_path_flag, loop_core_config_flag]
-
-    output_path = compile(source, module_name, flags, force_recompile=force_recompile or new_config, **compile_time_parameters)
-
-    module = load_module(module_name, output_path)
-    if use_python_environment:
-        module.set_environment_factory(env_factory)
-    return module
+    loop_core_config_search_path_flag = compile_option("header_search_path", render_output_directory)
+    loop_core_config_flag = compile_option("macro_definition", "TINYRL_USE_LOOP_CORE_CONFIG")
+    flags = [loop_core_config_search_path_flag, loop_core_config_flag]
+    return compile_training(module_name, env_factory, flags, verbose=verbose, force_recompile=(force_recompile or new_config), enable_evaluation=enable_evaluation, evaluation_interval=evaluation_interval, num_evaluation_episodes=num_evaluation_episodes, **kwargs)
```

### Comparing `tinyrl-0.3.1/LICENSE` & `tinyrl-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyrl-0.3.1/README.md` & `tinyrl-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -63,7 +63,11 @@
 
 # Acceleration
 
 On macOS TinyRL automatically uses Accelerate. To use MKL on linux you can install TinyRL with the `mkl` option:
 ```
 pip install tinyrl[mkl]
 ```
+
+# Windows
+
+TinyRL also works on Windows but MKL is not integrated, yet. Please make sure to install Python from the installer from the Python website and not using the Windows Store Python version. The latter resides in a directory that requires admin privileges even for read access. Due to the just-in-time compilation of RLtools we need to be able to read the Python header and library files. After installing the right Python version the easies way to run TinyRL is by opening the cloned folder in Visual Studio Code and launching the preconfigured targets. Make sure to start Visual Studio Code from the Visual Studio Prompt (e.g. `Developer Command Prompt for VS 2022`) by running `code` so that `cl.exe` (MSVC) is available in the environment.
```

### Comparing `tinyrl-0.3.1/pyproject.toml` & `tinyrl-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tinyrl"
-version = "0.3.1"
+version = "0.4.0"
 authors = [
   { name="Jonas Eschmann", email="jonas.eschmann@gmail.com" },
 ]
 description = "A Python wrapper for RLtools"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -29,14 +29,19 @@
 onnx = [
   "onnx"
 ]
 tests = [
   "onnx",
   "torch"
 ]
+learning-curves = [
+  "stable-baselines3==2.3.0",
+  "torch==2.2.1",
+  "gymnasium[mujoco]==0.29.1",
+]
 
 [tool.hatch.build]
 include = [
   "tinyrl/__init__.py",
   "tinyrl/interface/**",
   "tinyrl/src/**",
   "tinyrl/external/rl_tools/include/**"
```

