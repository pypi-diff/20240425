# Comparing `tmp/underactuated-2024.4.25.tar.gz` & `tmp/underactuated-2024.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "underactuated-2024.4.25.tar", max compression
+gzip compressed data, was "underactuated-2024.4.7.tar", max compression
```

## Comparing `underactuated-2024.4.25.tar` & `underactuated-2024.4.7.tar`

### file list

```diff
@@ -1,111 +1,108 @@
--rw-r--r--   0        0        0     1703 2024-02-22 14:55:42.076477 underactuated-2024.4.25/LICENSE.TXT
--rw-r--r--   0        0        0      550 2024-02-22 14:55:42.076477 underactuated-2024.4.25/README.md
--rw-r--r--   0        0        0     3111 2024-04-25 11:54:37.780915 underactuated-2024.4.25/pyproject.toml
--rw-r--r--   0        0        0      311 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/__init__.py
--rw-r--r--   0        0        0      846 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/_static/custom.css
--rw-r--r--   0        0        0      893 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/conf.py
--rw-r--r--   0        0        0     1692 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/double_integrator.py
--rw-r--r--   0        0        0    14061 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/exercises/acrobot/test_cartpole_balancing.py
--rw-r--r--   0        0        0    11827 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/exercises/acrobot/test_cartpoles_urdf.py
--rw-r--r--   0        0        0     7899 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/exercises/contact/test_compass_gait_limit_cycle.py
--rw-r--r--   0        0        0     3656 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/exercises/dp/J.npy
--rw-r--r--   0        0        0     5595 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/exercises/dp/minimum_time_utils.py
--rw-r--r--   0        0        0      796 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/exercises/dp/test_lp_dp.py
--rw-r--r--   0        0        0     1315 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/exercises/dp/test_minimum_time.py
--rw-r--r--   0        0        0     9657 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/exercises/dp/test_pendulum_cvi.py
--rw-r--r--   0        0        0     4498 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/exercises/grader.py
--rw-r--r--   0        0        0     2643 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/exercises/humanoids/footstep_planning_gcs_utils.py
--rw-r--r--   0        0        0     6496 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/exercises/humanoids/test_footstep_planning.py
--rw-r--r--   0        0        0     4279 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/exercises/humanoids/test_footstep_planning_gcs.py
--rw-r--r--   0        0        0     1754 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/exercises/intro/test_drake_systems.py
--rw-r--r--   0        0        0     5161 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/exercises/lqr/test_drake_diagrams.py
--rw-r--r--   0        0        0     7516 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/exercises/lyapunov/test_control.py
--rw-r--r--   0        0        0     1302 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/exercises/lyapunov/test_sos_and_psd.py
--rw-r--r--   0        0        0     5261 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/exercises/lyapunov/test_van_der_pol.py
--rw-r--r--   0        0        0     5992 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/exercises/pend/mnist.npz
--rw-r--r--   0        0        0     2590 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/exercises/pend/test_hopfield_network.py
--rw-r--r--   0        0        0     1127 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/exercises/pend/test_vibrating_pendulum.py
--rw-r--r--   0        0        0     5419 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/exercises/planning/test_rrt_planning.py
--rw-r--r--   0        0        0     6817 2024-02-22 14:55:42.180479 underactuated-2024.4.25/underactuated/exercises/simple_legs/test_one_d_hopper.py
--rw-r--r--   0        0        0     1803 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/exercises/sysid/test_glider_sysid.py
--rw-r--r--   0        0        0     2382 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/exercises/sysid/test_linear_sysid.py
--rw-r--r--   0        0        0     9519 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/exercises/trajopt/test_ilqr_driving.py
--rw-r--r--   0        0        0     4662 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/exercises/trajopt/test_orbital_transfer.py
--rw-r--r--   0        0        0     9898 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/exercises/trajopt/test_shooting_vs_transcription.py
--rw-r--r--   0        0        0      252 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/index.md
--rw-r--r--   0        0        0     5263 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/jupyter.py
--rw-r--r--   0        0        0      259 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/meshcat_cpp_utils.py
--rw-r--r--   0        0        0      104 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/meshcat_utils.md
--rw-r--r--   0        0        0    13260 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/meshcat_utils.py
--rw-r--r--   0        0        0     2331 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/cartpole.urdf
--rw-r--r--   0        0        0     2879 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/compass_gait_limit_cycle.urdf
--rw-r--r--   0        0        0     2151 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/double_pendulum.sdf
--rw-r--r--   0        0        0     2417 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/double_pendulum.urdf
--rw-r--r--   0        0        0     5943 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/glider/glider.urdf
--rw-r--r--   0        0        0     4411 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/glider/meshes/elevator.obj
--rw-r--r--   0        0        0     1192 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/glider/meshes/fuselageh_hstab.obj
--rw-r--r--   0        0        0    17609 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/glider/meshes/fuselageh_main.obj
--rw-r--r--   0        0        0    11270 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/glider/meshes/fuselagev_main.obj
--rw-r--r--   0        0        0     1664 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/glider/meshes/fuselagev_top.obj
--rw-r--r--   0        0        0     2316 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/glider/meshes/fuselagev_vstab.obj
--rw-r--r--   0        0        0     1460 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/glider/meshes/wing_left.obj
--rw-r--r--   0        0        0     1577 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/glider/meshes/wing_right.obj
--rw-r--r--   0        0        0      666 2024-04-09 13:18:23.087267 underactuated-2024.4.25/underactuated/models/ground.urdf
--rw-r--r--   0        0        0     5297 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/kneed_compass_gait.urdf
--rw-r--r--   0        0        0     1679 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/littledog/LICENSE.txt
--rw-r--r--   0        0        0    13333 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/littledog/LittleDog.urdf
--rw-r--r--   0        0        0      411 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/littledog/README.md
--rw-r--r--   0        0        0      666 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/littledog/ground.urdf
--rw-r--r--   0        0        0    50176 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/littledog/meshes/back_left_hip.obj
--rw-r--r--   0        0        0      200 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/littledog/meshes/back_left_hip.obj.mtl
--rw-r--r--   0        0        0   121081 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/littledog/meshes/back_left_lower.obj
--rw-r--r--   0        0        0      528 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/littledog/meshes/back_left_lower.obj.mtl
--rw-r--r--   0        0        0   104694 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/littledog/meshes/back_left_upper.obj
--rw-r--r--   0        0        0      512 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/littledog/meshes/back_left_upper.obj.mtl
--rw-r--r--   0        0        0    51166 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/littledog/meshes/back_right_hip.obj
--rw-r--r--   0        0        0      200 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/littledog/meshes/back_right_hip.obj.mtl
--rw-r--r--   0        0        0   120989 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/littledog/meshes/back_right_lower.obj
--rw-r--r--   0        0        0      528 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/littledog/meshes/back_right_lower.obj.mtl
--rw-r--r--   0        0        0   105531 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/littledog/meshes/back_right_upper.obj
--rw-r--r--   0        0        0      512 2024-02-22 14:55:42.184479 underactuated-2024.4.25/underactuated/models/littledog/meshes/back_right_upper.obj.mtl
--rw-r--r--   0        0        0  1036654 2024-02-22 14:55:42.188480 underactuated-2024.4.25/underactuated/models/littledog/meshes/body.obj
--rw-r--r--   0        0        0      357 2024-02-22 14:55:42.188480 underactuated-2024.4.25/underactuated/models/littledog/meshes/body.obj.mtl
--rw-r--r--   0        0        0    25320 2024-02-22 14:55:42.188480 underactuated-2024.4.25/underactuated/models/littledog/meshes/body2.jpg
--rw-r--r--   0        0        0    11322 2024-02-22 14:55:42.188480 underactuated-2024.4.25/underactuated/models/littledog/meshes/body3.jpg
--rw-r--r--   0        0        0    29266 2024-02-22 14:55:42.188480 underactuated-2024.4.25/underactuated/models/littledog/meshes/foot.jpg
--rw-r--r--   0        0        0    49151 2024-02-22 14:55:42.188480 underactuated-2024.4.25/underactuated/models/littledog/meshes/front_left_hip.obj
--rw-r--r--   0        0        0      200 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/models/littledog/meshes/front_left_hip.obj.mtl
--rw-r--r--   0        0        0   121747 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/models/littledog/meshes/front_left_lower.obj
--rw-r--r--   0        0        0      528 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/models/littledog/meshes/front_left_lower.obj.mtl
--rw-r--r--   0        0        0   104401 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/models/littledog/meshes/front_left_upper.obj
--rw-r--r--   0        0        0      512 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/models/littledog/meshes/front_left_upper.obj.mtl
--rw-r--r--   0        0        0    58904 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/models/littledog/meshes/front_right_hip.obj
--rw-r--r--   0        0        0      200 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/models/littledog/meshes/front_right_hip.obj.mtl
--rw-r--r--   0        0        0   121685 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/models/littledog/meshes/front_right_lower.obj
--rw-r--r--   0        0        0      528 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/models/littledog/meshes/front_right_lower.obj.mtl
--rw-r--r--   0        0        0   104294 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/models/littledog/meshes/front_right_upper.obj
--rw-r--r--   0        0        0      512 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/models/littledog/meshes/front_right_upper.obj.mtl
--rw-r--r--   0        0        0    21971 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/models/littledog/meshes/leg.jpg
--rw-r--r--   0        0        0     2820 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/models/one_d_hopper.urdf
--rw-r--r--   0        0        0      247 2024-04-09 13:40:34.295700 underactuated-2024.4.25/underactuated/models/planar_one_leg_hopper.dmd.yaml
--rw-r--r--   0        0        0     5185 2024-04-09 13:41:22.428583 underactuated-2024.4.25/underactuated/models/planar_one_leg_hopper.sdf
--rw-r--r--   0        0        0      177 2024-04-07 10:56:08.557440 underactuated-2024.4.25/underactuated/models/spot/README.md
--rw-r--r--   0        0        0      455 2024-04-07 10:56:08.557440 underactuated-2024.4.25/underactuated/models/spot/spot.dmd.yaml
--rw-r--r--   0        0        0    17320 2024-04-07 10:56:08.557440 underactuated-2024.4.25/underactuated/models/spot/spot.urdf
--rw-r--r--   0        0        0      515 2024-04-07 10:56:08.557440 underactuated-2024.4.25/underactuated/models/spot/spot_with_arm.dmd.yaml
--rw-r--r--   0        0        0    30975 2024-04-07 10:56:08.557440 underactuated-2024.4.25/underactuated/models/spot/spot_with_arm.urdf
--rw-r--r--   0        0        0     1723 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/models/undamped_cartpole.urdf
--rw-r--r--   0        0        0     1444 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/models/vibrating_pendulum.urdf
--rw-r--r--   0        0        0       96 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/multibody.md
--rw-r--r--   0        0        0     2343 2024-04-07 10:56:08.557440 underactuated-2024.4.25/underactuated/multibody.py
--rw-r--r--   0        0        0     2221 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/optimizers.py
--rw-r--r--   0        0        0      369 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/package.xml
--rw-r--r--   0        0        0     2238 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/pendulum.py
--rw-r--r--   0        0        0       98 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/plot_utils.md
--rw-r--r--   0        0        0     2056 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/plot_utils.py
--rw-r--r--   0        0        0      957 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/pyplot_visualizer.py
--rw-r--r--   0        0        0     5153 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/quadrotor2d.py
--rw-r--r--   0        0        0     3870 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/scenarios.py
--rw-r--r--   0        0        0       88 2024-02-22 14:55:42.192479 underactuated-2024.4.25/underactuated/utils.md
--rw-r--r--   0        0        0     3589 2024-04-07 10:56:08.557440 underactuated-2024.4.25/underactuated/utils.py
--rw-r--r--   0        0        0     1369 1970-01-01 00:00:00.000000 underactuated-2024.4.25/PKG-INFO
+-rw-r--r--   0        0        0     1703 2024-02-22 14:55:42.076477 underactuated-2024.4.7/LICENSE.TXT
+-rw-r--r--   0        0        0      550 2024-02-22 14:55:42.076477 underactuated-2024.4.7/README.md
+-rw-r--r--   0        0        0     3109 2024-04-07 10:56:58.002422 underactuated-2024.4.7/pyproject.toml
+-rw-r--r--   0        0        0      311 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/__init__.py
+-rw-r--r--   0        0        0      846 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/_static/custom.css
+-rw-r--r--   0        0        0      893 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/conf.py
+-rw-r--r--   0        0        0     1692 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/double_integrator.py
+-rw-r--r--   0        0        0    14061 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/exercises/acrobot/test_cartpole_balancing.py
+-rw-r--r--   0        0        0    11827 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/exercises/acrobot/test_cartpoles_urdf.py
+-rw-r--r--   0        0        0     7899 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/exercises/contact/test_compass_gait_limit_cycle.py
+-rw-r--r--   0        0        0     3656 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/exercises/dp/J.npy
+-rw-r--r--   0        0        0     5595 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/exercises/dp/minimum_time_utils.py
+-rw-r--r--   0        0        0      796 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/exercises/dp/test_lp_dp.py
+-rw-r--r--   0        0        0     1315 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/exercises/dp/test_minimum_time.py
+-rw-r--r--   0        0        0     9657 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/exercises/dp/test_pendulum_cvi.py
+-rw-r--r--   0        0        0     4498 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/exercises/grader.py
+-rw-r--r--   0        0        0     2643 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/exercises/humanoids/footstep_planning_gcs_utils.py
+-rw-r--r--   0        0        0     6496 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/exercises/humanoids/test_footstep_planning.py
+-rw-r--r--   0        0        0     4279 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/exercises/humanoids/test_footstep_planning_gcs.py
+-rw-r--r--   0        0        0     1754 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/exercises/intro/test_drake_systems.py
+-rw-r--r--   0        0        0     5161 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/exercises/lqr/test_drake_diagrams.py
+-rw-r--r--   0        0        0     7516 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/exercises/lyapunov/test_control.py
+-rw-r--r--   0        0        0     1302 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/exercises/lyapunov/test_sos_and_psd.py
+-rw-r--r--   0        0        0     5261 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/exercises/lyapunov/test_van_der_pol.py
+-rw-r--r--   0        0        0     5992 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/exercises/pend/mnist.npz
+-rw-r--r--   0        0        0     2590 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/exercises/pend/test_hopfield_network.py
+-rw-r--r--   0        0        0     1127 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/exercises/pend/test_vibrating_pendulum.py
+-rw-r--r--   0        0        0     5419 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/exercises/planning/test_rrt_planning.py
+-rw-r--r--   0        0        0     6817 2024-02-22 14:55:42.180479 underactuated-2024.4.7/underactuated/exercises/simple_legs/test_one_d_hopper.py
+-rw-r--r--   0        0        0     1803 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/exercises/sysid/test_glider_sysid.py
+-rw-r--r--   0        0        0     2382 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/exercises/sysid/test_linear_sysid.py
+-rw-r--r--   0        0        0     9519 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/exercises/trajopt/test_ilqr_driving.py
+-rw-r--r--   0        0        0     4662 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/exercises/trajopt/test_orbital_transfer.py
+-rw-r--r--   0        0        0     9898 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/exercises/trajopt/test_shooting_vs_transcription.py
+-rw-r--r--   0        0        0      252 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/index.md
+-rw-r--r--   0        0        0     5263 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/jupyter.py
+-rw-r--r--   0        0        0      259 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/meshcat_cpp_utils.py
+-rw-r--r--   0        0        0      104 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/meshcat_utils.md
+-rw-r--r--   0        0        0    13260 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/meshcat_utils.py
+-rw-r--r--   0        0        0     2331 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/cartpole.urdf
+-rw-r--r--   0        0        0     2879 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/compass_gait_limit_cycle.urdf
+-rw-r--r--   0        0        0     2151 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/double_pendulum.sdf
+-rw-r--r--   0        0        0     2417 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/double_pendulum.urdf
+-rw-r--r--   0        0        0     5943 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/glider/glider.urdf
+-rw-r--r--   0        0        0     4411 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/glider/meshes/elevator.obj
+-rw-r--r--   0        0        0     1192 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/glider/meshes/fuselageh_hstab.obj
+-rw-r--r--   0        0        0    17609 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/glider/meshes/fuselageh_main.obj
+-rw-r--r--   0        0        0    11270 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/glider/meshes/fuselagev_main.obj
+-rw-r--r--   0        0        0     1664 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/glider/meshes/fuselagev_top.obj
+-rw-r--r--   0        0        0     2316 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/glider/meshes/fuselagev_vstab.obj
+-rw-r--r--   0        0        0     1460 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/glider/meshes/wing_left.obj
+-rw-r--r--   0        0        0     1577 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/glider/meshes/wing_right.obj
+-rw-r--r--   0        0        0     5297 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/kneed_compass_gait.urdf
+-rw-r--r--   0        0        0     1679 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/littledog/LICENSE.txt
+-rw-r--r--   0        0        0    13333 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/littledog/LittleDog.urdf
+-rw-r--r--   0        0        0      411 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/littledog/README.md
+-rw-r--r--   0        0        0      666 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/littledog/ground.urdf
+-rw-r--r--   0        0        0    50176 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/littledog/meshes/back_left_hip.obj
+-rw-r--r--   0        0        0      200 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/littledog/meshes/back_left_hip.obj.mtl
+-rw-r--r--   0        0        0   121081 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/littledog/meshes/back_left_lower.obj
+-rw-r--r--   0        0        0      528 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/littledog/meshes/back_left_lower.obj.mtl
+-rw-r--r--   0        0        0   104694 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/littledog/meshes/back_left_upper.obj
+-rw-r--r--   0        0        0      512 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/littledog/meshes/back_left_upper.obj.mtl
+-rw-r--r--   0        0        0    51166 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/littledog/meshes/back_right_hip.obj
+-rw-r--r--   0        0        0      200 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/littledog/meshes/back_right_hip.obj.mtl
+-rw-r--r--   0        0        0   120989 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/littledog/meshes/back_right_lower.obj
+-rw-r--r--   0        0        0      528 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/littledog/meshes/back_right_lower.obj.mtl
+-rw-r--r--   0        0        0   105531 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/littledog/meshes/back_right_upper.obj
+-rw-r--r--   0        0        0      512 2024-02-22 14:55:42.184479 underactuated-2024.4.7/underactuated/models/littledog/meshes/back_right_upper.obj.mtl
+-rw-r--r--   0        0        0  1036654 2024-02-22 14:55:42.188480 underactuated-2024.4.7/underactuated/models/littledog/meshes/body.obj
+-rw-r--r--   0        0        0      357 2024-02-22 14:55:42.188480 underactuated-2024.4.7/underactuated/models/littledog/meshes/body.obj.mtl
+-rw-r--r--   0        0        0    25320 2024-02-22 14:55:42.188480 underactuated-2024.4.7/underactuated/models/littledog/meshes/body2.jpg
+-rw-r--r--   0        0        0    11322 2024-02-22 14:55:42.188480 underactuated-2024.4.7/underactuated/models/littledog/meshes/body3.jpg
+-rw-r--r--   0        0        0    29266 2024-02-22 14:55:42.188480 underactuated-2024.4.7/underactuated/models/littledog/meshes/foot.jpg
+-rw-r--r--   0        0        0    49151 2024-02-22 14:55:42.188480 underactuated-2024.4.7/underactuated/models/littledog/meshes/front_left_hip.obj
+-rw-r--r--   0        0        0      200 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/models/littledog/meshes/front_left_hip.obj.mtl
+-rw-r--r--   0        0        0   121747 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/models/littledog/meshes/front_left_lower.obj
+-rw-r--r--   0        0        0      528 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/models/littledog/meshes/front_left_lower.obj.mtl
+-rw-r--r--   0        0        0   104401 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/models/littledog/meshes/front_left_upper.obj
+-rw-r--r--   0        0        0      512 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/models/littledog/meshes/front_left_upper.obj.mtl
+-rw-r--r--   0        0        0    58904 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/models/littledog/meshes/front_right_hip.obj
+-rw-r--r--   0        0        0      200 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/models/littledog/meshes/front_right_hip.obj.mtl
+-rw-r--r--   0        0        0   121685 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/models/littledog/meshes/front_right_lower.obj
+-rw-r--r--   0        0        0      528 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/models/littledog/meshes/front_right_lower.obj.mtl
+-rw-r--r--   0        0        0   104294 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/models/littledog/meshes/front_right_upper.obj
+-rw-r--r--   0        0        0      512 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/models/littledog/meshes/front_right_upper.obj.mtl
+-rw-r--r--   0        0        0    21971 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/models/littledog/meshes/leg.jpg
+-rw-r--r--   0        0        0     2820 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/models/one_d_hopper.urdf
+-rw-r--r--   0        0        0      177 2024-04-07 10:56:08.557440 underactuated-2024.4.7/underactuated/models/spot/README.md
+-rw-r--r--   0        0        0      455 2024-04-07 10:56:08.557440 underactuated-2024.4.7/underactuated/models/spot/spot.dmd.yaml
+-rw-r--r--   0        0        0    17320 2024-04-07 10:56:08.557440 underactuated-2024.4.7/underactuated/models/spot/spot.urdf
+-rw-r--r--   0        0        0      515 2024-04-07 10:56:08.557440 underactuated-2024.4.7/underactuated/models/spot/spot_with_arm.dmd.yaml
+-rw-r--r--   0        0        0    30975 2024-04-07 10:56:08.557440 underactuated-2024.4.7/underactuated/models/spot/spot_with_arm.urdf
+-rw-r--r--   0        0        0     1723 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/models/undamped_cartpole.urdf
+-rw-r--r--   0        0        0     1444 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/models/vibrating_pendulum.urdf
+-rw-r--r--   0        0        0       96 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/multibody.md
+-rw-r--r--   0        0        0     2343 2024-04-07 10:56:08.557440 underactuated-2024.4.7/underactuated/multibody.py
+-rw-r--r--   0        0        0     2221 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/optimizers.py
+-rw-r--r--   0        0        0      369 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/package.xml
+-rw-r--r--   0        0        0     2238 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/pendulum.py
+-rw-r--r--   0        0        0       98 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/plot_utils.md
+-rw-r--r--   0        0        0     2056 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/plot_utils.py
+-rw-r--r--   0        0        0      957 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/pyplot_visualizer.py
+-rw-r--r--   0        0        0     5153 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/quadrotor2d.py
+-rw-r--r--   0        0        0     3870 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/scenarios.py
+-rw-r--r--   0        0        0       88 2024-02-22 14:55:42.192479 underactuated-2024.4.7/underactuated/utils.md
+-rw-r--r--   0        0        0     3589 2024-04-07 10:56:08.557440 underactuated-2024.4.7/underactuated/utils.py
+-rw-r--r--   0        0        0     1374 1970-01-01 00:00:00.000000 underactuated-2024.4.7/PKG-INFO
```

### Comparing `underactuated-2024.4.25/LICENSE.TXT` & `underactuated-2024.4.7/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/README.md` & `underactuated-2024.4.7/README.md`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/pyproject.toml` & `underactuated-2024.4.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "underactuated"
 # Use e.g. 2023.10.4.rc0 if I need to release a release candidate.
 # Use e.g. 2023.10.4.post1 if I need to rerelease on the same day.
-version = "2024.04.25"
+version = "2024.04.07"
 description = "MIT 6.821 - Underactuated Robotics"
 authors = ["Russ Tedrake <russt@mit.edu>"]
 license = "BSD License"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License"
@@ -46,41 +46,41 @@
 [[tool.poetry.source]]
 name = "drake-nightly"
 url = "https://drake-packages.csail.mit.edu/whl/nightly/"
 priority = "explicit"
 
 [tool.poetry.dependencies]
 python = "<4.0,>=3.10"
-#drake = { version = "==0.0.20240307", source = "drake-nightly" }
-drake = ">=1.28.0"
+drake = { version = "==0.0.20240307", source = "drake-nightly" }
+#drake = ">=1.23.0"
 gradescope-utils = ">=0.4.0"
 ipywidgets = ">7"
 mpld3 = ">=0.5.1"
 pandas = ">=2.0"
 pydot = ">=1.3.0"
 scipy = ">=1.10.0"  # From github dependabot
 timeout-decorator = ">=0.4.1"
 
 [tool.poetry.group.docs]
 optional = true
 
 # Must include all dependencies required to build the docs with sphinx + autodoc.
 [tool.poetry.group.docs.dependencies]
 # Should match drake version above.
-#drake = { version = "==0.0.20240307", source = "drake-nightly" }
-drake = ">=1.28.0"
+drake = { version = "==0.0.20240307", source = "drake-nightly" }
+#drake = ">=1.23.0"
 ipython = ">=7.8.0"
 sphinx = ">=7.2.6"
 myst-parser = ">=2.0.0"
 sphinx_rtd_theme = ">=2.0.0"
 
 [tool.poetry.group.dev.dependencies]
 beautifulsoup4 = ">=4.6.3"
 black = { version = ">=23.*", extras = ["jupyter"] }
-lxml = {version = ">=4.9.2", extras = ["html_clean"] }
+lxml = ">=4.9.2" # seems to be needed on python 3.11
 # Blocked on poetry known issue; see Developers.md
 #matplotlib = [ 
 #  {platform="darwin", version=">=3.7.0"}, # old versions don't build in XCode
 #  {platform="linux", version="3.5.1"}, # https://github.com/RobotLocomotion/drake/issues/14250 
 #]
 mysql-connector-python = ">=8.0.23"
 nbconvert = [
```

### Comparing `underactuated-2024.4.25/underactuated/_static/custom.css` & `underactuated-2024.4.7/underactuated/_static/custom.css`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/conf.py` & `underactuated-2024.4.7/underactuated/conf.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/double_integrator.py` & `underactuated-2024.4.7/underactuated/double_integrator.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/acrobot/test_cartpole_balancing.py` & `underactuated-2024.4.7/underactuated/exercises/acrobot/test_cartpole_balancing.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/acrobot/test_cartpoles_urdf.py` & `underactuated-2024.4.7/underactuated/exercises/acrobot/test_cartpoles_urdf.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/contact/test_compass_gait_limit_cycle.py` & `underactuated-2024.4.7/underactuated/exercises/contact/test_compass_gait_limit_cycle.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/dp/J.npy` & `underactuated-2024.4.7/underactuated/exercises/dp/J.npy`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/dp/minimum_time_utils.py` & `underactuated-2024.4.7/underactuated/exercises/dp/minimum_time_utils.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/dp/test_lp_dp.py` & `underactuated-2024.4.7/underactuated/exercises/dp/test_lp_dp.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/dp/test_minimum_time.py` & `underactuated-2024.4.7/underactuated/exercises/dp/test_minimum_time.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/dp/test_pendulum_cvi.py` & `underactuated-2024.4.7/underactuated/exercises/dp/test_pendulum_cvi.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/grader.py` & `underactuated-2024.4.7/underactuated/exercises/grader.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/humanoids/footstep_planning_gcs_utils.py` & `underactuated-2024.4.7/underactuated/exercises/humanoids/footstep_planning_gcs_utils.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/humanoids/test_footstep_planning.py` & `underactuated-2024.4.7/underactuated/exercises/humanoids/test_footstep_planning.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/humanoids/test_footstep_planning_gcs.py` & `underactuated-2024.4.7/underactuated/exercises/humanoids/test_footstep_planning_gcs.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/intro/test_drake_systems.py` & `underactuated-2024.4.7/underactuated/exercises/intro/test_drake_systems.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/lqr/test_drake_diagrams.py` & `underactuated-2024.4.7/underactuated/exercises/lqr/test_drake_diagrams.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/lyapunov/test_control.py` & `underactuated-2024.4.7/underactuated/exercises/lyapunov/test_control.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/lyapunov/test_sos_and_psd.py` & `underactuated-2024.4.7/underactuated/exercises/lyapunov/test_sos_and_psd.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/lyapunov/test_van_der_pol.py` & `underactuated-2024.4.7/underactuated/exercises/lyapunov/test_van_der_pol.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/pend/mnist.npz` & `underactuated-2024.4.7/underactuated/exercises/pend/mnist.npz`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/pend/test_hopfield_network.py` & `underactuated-2024.4.7/underactuated/exercises/pend/test_hopfield_network.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/pend/test_vibrating_pendulum.py` & `underactuated-2024.4.7/underactuated/exercises/pend/test_vibrating_pendulum.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/planning/test_rrt_planning.py` & `underactuated-2024.4.7/underactuated/exercises/planning/test_rrt_planning.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/simple_legs/test_one_d_hopper.py` & `underactuated-2024.4.7/underactuated/exercises/simple_legs/test_one_d_hopper.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/sysid/test_glider_sysid.py` & `underactuated-2024.4.7/underactuated/exercises/sysid/test_glider_sysid.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/sysid/test_linear_sysid.py` & `underactuated-2024.4.7/underactuated/exercises/sysid/test_linear_sysid.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/trajopt/test_ilqr_driving.py` & `underactuated-2024.4.7/underactuated/exercises/trajopt/test_ilqr_driving.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/trajopt/test_orbital_transfer.py` & `underactuated-2024.4.7/underactuated/exercises/trajopt/test_orbital_transfer.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/exercises/trajopt/test_shooting_vs_transcription.py` & `underactuated-2024.4.7/underactuated/exercises/trajopt/test_shooting_vs_transcription.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/jupyter.py` & `underactuated-2024.4.7/underactuated/jupyter.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/meshcat_utils.py` & `underactuated-2024.4.7/underactuated/meshcat_utils.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/cartpole.urdf` & `underactuated-2024.4.7/underactuated/models/cartpole.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/compass_gait_limit_cycle.urdf` & `underactuated-2024.4.7/underactuated/models/compass_gait_limit_cycle.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/double_pendulum.sdf` & `underactuated-2024.4.7/underactuated/models/double_pendulum.sdf`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/double_pendulum.urdf` & `underactuated-2024.4.7/underactuated/models/double_pendulum.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/glider/glider.urdf` & `underactuated-2024.4.7/underactuated/models/glider/glider.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/glider/meshes/elevator.obj` & `underactuated-2024.4.7/underactuated/models/glider/meshes/elevator.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/glider/meshes/fuselageh_hstab.obj` & `underactuated-2024.4.7/underactuated/models/glider/meshes/fuselageh_hstab.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/glider/meshes/fuselageh_main.obj` & `underactuated-2024.4.7/underactuated/models/glider/meshes/fuselageh_main.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/glider/meshes/fuselagev_main.obj` & `underactuated-2024.4.7/underactuated/models/glider/meshes/fuselagev_main.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/glider/meshes/fuselagev_top.obj` & `underactuated-2024.4.7/underactuated/models/glider/meshes/fuselagev_top.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/glider/meshes/fuselagev_vstab.obj` & `underactuated-2024.4.7/underactuated/models/glider/meshes/fuselagev_vstab.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/glider/meshes/wing_left.obj` & `underactuated-2024.4.7/underactuated/models/glider/meshes/wing_left.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/glider/meshes/wing_right.obj` & `underactuated-2024.4.7/underactuated/models/glider/meshes/wing_right.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/ground.urdf` & `underactuated-2024.4.7/underactuated/models/littledog/ground.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/kneed_compass_gait.urdf` & `underactuated-2024.4.7/underactuated/models/kneed_compass_gait.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/LICENSE.txt` & `underactuated-2024.4.7/underactuated/models/littledog/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/LittleDog.urdf` & `underactuated-2024.4.7/underactuated/models/littledog/LittleDog.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/back_left_hip.obj` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/back_left_hip.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/back_left_lower.obj` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/back_left_lower.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/back_left_lower.obj.mtl` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/back_left_lower.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/back_left_upper.obj` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/back_left_upper.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/back_left_upper.obj.mtl` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/back_left_upper.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/back_right_hip.obj` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/back_right_hip.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/back_right_lower.obj` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/back_right_lower.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/back_right_lower.obj.mtl` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/back_right_lower.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/back_right_upper.obj` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/back_right_upper.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/back_right_upper.obj.mtl` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/back_right_upper.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/body.obj` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/body.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/body2.jpg` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/body2.jpg`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/body3.jpg` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/body3.jpg`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/foot.jpg` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/foot.jpg`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/front_left_hip.obj` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/front_left_hip.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/front_left_lower.obj` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/front_left_lower.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/front_left_lower.obj.mtl` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/front_left_lower.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/front_left_upper.obj` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/front_left_upper.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/front_left_upper.obj.mtl` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/front_left_upper.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/front_right_hip.obj` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/front_right_hip.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/front_right_lower.obj` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/front_right_lower.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/front_right_lower.obj.mtl` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/front_right_lower.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/front_right_upper.obj` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/front_right_upper.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/front_right_upper.obj.mtl` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/front_right_upper.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/littledog/meshes/leg.jpg` & `underactuated-2024.4.7/underactuated/models/littledog/meshes/leg.jpg`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/one_d_hopper.urdf` & `underactuated-2024.4.7/underactuated/models/one_d_hopper.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/spot/spot.urdf` & `underactuated-2024.4.7/underactuated/models/spot/spot.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/spot/spot_with_arm.dmd.yaml` & `underactuated-2024.4.7/underactuated/models/spot/spot_with_arm.dmd.yaml`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/spot/spot_with_arm.urdf` & `underactuated-2024.4.7/underactuated/models/spot/spot_with_arm.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/undamped_cartpole.urdf` & `underactuated-2024.4.7/underactuated/models/undamped_cartpole.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/models/vibrating_pendulum.urdf` & `underactuated-2024.4.7/underactuated/models/vibrating_pendulum.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/multibody.py` & `underactuated-2024.4.7/underactuated/multibody.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/optimizers.py` & `underactuated-2024.4.7/underactuated/optimizers.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/pendulum.py` & `underactuated-2024.4.7/underactuated/pendulum.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/plot_utils.py` & `underactuated-2024.4.7/underactuated/plot_utils.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/pyplot_visualizer.py` & `underactuated-2024.4.7/underactuated/pyplot_visualizer.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/quadrotor2d.py` & `underactuated-2024.4.7/underactuated/quadrotor2d.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/scenarios.py` & `underactuated-2024.4.7/underactuated/scenarios.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/underactuated/utils.py` & `underactuated-2024.4.7/underactuated/utils.py`

 * *Files identical despite different names*

### Comparing `underactuated-2024.4.25/PKG-INFO` & `underactuated-2024.4.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: underactuated
-Version: 2024.4.25
+Version: 2024.4.7
 Summary: MIT 6.821 - Underactuated Robotics
 License: BSD License
 Author: Russ Tedrake
 Author-email: russt@mit.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: drake (>=1.28.0)
+Requires-Dist: drake (==0.0.20240307)
 Requires-Dist: gradescope-utils (>=0.4.0)
 Requires-Dist: ipywidgets (>7)
 Requires-Dist: mpld3 (>=0.5.1)
 Requires-Dist: pandas (>=2.0)
 Requires-Dist: pydot (>=1.3.0)
 Requires-Dist: scipy (>=1.10.0)
 Requires-Dist: timeout-decorator (>=0.4.1)
```

