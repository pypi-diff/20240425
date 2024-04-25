# Comparing `tmp/comet_toolbox-0.3.0.tar.gz` & `tmp/comet_toolbox-0.3.2.tar.gz`

## Comparing `comet_toolbox-0.3.0.tar` & `comet_toolbox-0.3.2.tar`

### file list

```diff
@@ -1,229 +1,233 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/.gitattributes
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/__init__.py
--rwxr-xr-x   0        0        0     3821 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/cifti.py
--rwxr-xr-x   0        0        0     3968 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/data.py
--rw-r--r--   0        0        0    29936 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/graph.py
--rw-r--r--   0        0        0   105766 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/gui.py
--rwxr-xr-x   0        0        0    44939 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/methods.py
--rwxr-xr-x   0        0        0    26011 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/multiverse.py
--rw-r--r--   0        0        0    96617 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/simulation.pkl
--rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/simulation.txt
--rw-r--r--   0        0        0   192811 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/single_state.txt
--rwxr-xr-x   0        0        0  1038952 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/atlas/Q1-Q6_RelatedValidation210.CorticalAreas_dil_Final_Final_Areas_Group_Colors_with_Atlas_ROIs2.32k_fs_LR.dlabel.nii
--rwxr-xr-x   0        0        0      531 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/atlas/README.md
--rwxr-xr-x   0        0        0  1029992 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/atlas/Schaefer2018_200Parcels_17Networks_order_Tian_Subcortex_S4.dlabel.nii
--rwxr-xr-x   0        0        0   655904 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/atlas/Schaefer2018_200Parcels_Kong2022_17Networks_order.dlabel.nii
--rwxr-xr-x   0        0        0     1047 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/atlas/fs_LR_32k_medial_mask.mat
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/img/badge.svg
--rw-r--r--   0        0        0    40910 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/img/content.drawio
--rw-r--r--   0        0        0   175918 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/img/content.png
--rw-r--r--   0        0        0   202431 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/img/gui.png
--rw-r--r--   0        0        0   724684 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/img/logo.png
--rw-r--r--   0        0        0   185059 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/example_analysis.ipynb
--rw-r--r--   0        0        0   450982 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/example_dfc.ipynb
--rw-r--r--   0        0        0  1311678 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/example_graph.ipynb
--rw-r--r--   0        0        0   114703 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/example_multiverse.ipynb
--rw-r--r--   0        0        0   804479 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/example_data/abide_50008.txt
--rw-r--r--   0        0        0   969955 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/example_data/aomic_multi.pkl
--rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/example_data/simulation.txt
--rw-r--r--   0        0        0  1564386 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/example_data/xcpd.tsv
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_1.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_10.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_11.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_12.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_13.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_14.py
--rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_15.py
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_16.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_17.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_18.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_19.py
--rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_2.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_20.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_21.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_22.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_23.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_24.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_25.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_26.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_27.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_28.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_29.py
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_3.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_30.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_31.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_32.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_33.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_34.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_35.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_36.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_37.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_38.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_39.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_4.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_40.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_41.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_42.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_43.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_44.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_45.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_46.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_47.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_48.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_49.py
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_5.py
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_50.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_51.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_52.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_53.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_54.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_55.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_56.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_57.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_58.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_59.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_6.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_60.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_61.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_62.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_63.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_64.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_65.py
--rw-r--r--   0        0        0     4642 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_66.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_67.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_68.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_69.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_7.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_70.py
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_71.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_72.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_73.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_74.py
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_75.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_76.py
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_77.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_78.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_79.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_8.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_80.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_81.py
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_82.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_83.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_84.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_85.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_86.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_87.py
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_88.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_89.py
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_9.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_90.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_91.py
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_92.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_93.py
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_94.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_95.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_96.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/forking_paths.pkl
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/multiverse_summary.csv
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/pipelines.csv
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_1.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_10.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_11.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_12.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_13.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_14.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_15.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_16.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_17.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_18.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_19.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_2.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_20.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_21.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_22.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_23.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_24.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_25.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_26.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_27.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_28.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_29.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_3.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_30.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_31.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_32.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_33.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_34.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_35.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_36.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_37.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_38.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_39.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_4.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_40.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_41.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_42.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_43.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_44.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_45.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_46.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_47.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_48.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_49.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_5.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_50.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_51.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_52.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_53.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_54.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_55.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_56.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_57.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_58.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_59.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_6.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_60.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_61.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_62.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_63.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_64.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_65.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_66.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_67.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_68.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_69.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_7.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_70.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_71.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_72.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_73.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_74.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_75.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_76.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_77.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_78.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_79.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_8.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_80.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_81.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_82.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_83.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_84.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_85.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_86.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_87.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_88.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_89.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_9.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_90.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_91.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_92.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_93.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_94.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_95.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_96.pkl
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/LICENSE
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/README.md
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/.gitattributes
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/adj.mat
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/adj_bin.mat
+-rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/simulation.txt
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/__init__.py
+-rwxr-xr-x   0        0        0     3821 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/cifti.py
+-rwxr-xr-x   0        0        0     3968 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/data.py
+-rw-r--r--   0        0        0    29936 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/graph.py
+-rw-r--r--   0        0        0   135519 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/gui.py
+-rwxr-xr-x   0        0        0    47496 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/methods.py
+-rwxr-xr-x   0        0        0    26011 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/multiverse.py
+-rw-r--r--   0        0        0    96617 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/simulation.pkl
+-rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/simulation.txt
+-rw-r--r--   0        0        0   192811 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/single_state.txt
+-rwxr-xr-x   0        0        0  1038952 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/atlas/Q1-Q6_RelatedValidation210.CorticalAreas_dil_Final_Final_Areas_Group_Colors_with_Atlas_ROIs2.32k_fs_LR.dlabel.nii
+-rwxr-xr-x   0        0        0      531 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/atlas/README.md
+-rwxr-xr-x   0        0        0  1029992 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/atlas/Schaefer2018_200Parcels_17Networks_order_Tian_Subcortex_S4.dlabel.nii
+-rwxr-xr-x   0        0        0   655904 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/atlas/Schaefer2018_200Parcels_Kong2022_17Networks_order.dlabel.nii
+-rwxr-xr-x   0        0        0     1047 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/atlas/fs_LR_32k_medial_mask.mat
+-rw-r--r--   0        0        0    40910 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/img/content.drawio
+-rw-r--r--   0        0        0   175918 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/img/content.png
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/img/doi.svg
+-rw-r--r--   0        0        0   202431 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/img/gui.png
+-rw-r--r--   0        0        0   724684 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/img/logo.png
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/img/pypi.svg
+-rw-r--r--   0        0        0   185059 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/example_analysis.ipynb
+-rw-r--r--   0        0        0   450982 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/example_dfc.ipynb
+-rw-r--r--   0        0        0  1311678 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/example_graph.ipynb
+-rw-r--r--   0        0        0   114703 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/example_multiverse.ipynb
+-rw-r--r--   0        0        0   804479 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/example_data/abide_50008.txt
+-rw-r--r--   0        0        0   969955 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/example_data/aomic_multi.pkl
+-rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/example_data/simulation.txt
+-rw-r--r--   0        0        0  1564386 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/example_data/xcpd.tsv
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_1.py
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_10.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_11.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_12.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_13.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_14.py
+-rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_15.py
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_16.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_17.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_18.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_19.py
+-rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_2.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_20.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_21.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_22.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_23.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_24.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_25.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_26.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_27.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_28.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_29.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_3.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_30.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_31.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_32.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_33.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_34.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_35.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_36.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_37.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_38.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_39.py
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_4.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_40.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_41.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_42.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_43.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_44.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_45.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_46.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_47.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_48.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_49.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_5.py
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_50.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_51.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_52.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_53.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_54.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_55.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_56.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_57.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_58.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_59.py
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_6.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_60.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_61.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_62.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_63.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_64.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_65.py
+-rw-r--r--   0        0        0     4642 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_66.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_67.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_68.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_69.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_7.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_70.py
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_71.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_72.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_73.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_74.py
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_75.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_76.py
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_77.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_78.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_79.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_8.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_80.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_81.py
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_82.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_83.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_84.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_85.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_86.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_87.py
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_88.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_89.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_9.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_90.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_91.py
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_92.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_93.py
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_94.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_95.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_96.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/forking_paths.pkl
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/multiverse_summary.csv
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/pipelines.csv
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_1.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_10.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_11.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_12.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_13.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_14.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_15.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_16.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_17.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_18.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_19.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_2.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_20.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_21.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_22.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_23.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_24.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_25.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_26.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_27.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_28.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_29.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_3.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_30.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_31.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_32.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_33.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_34.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_35.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_36.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_37.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_38.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_39.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_4.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_40.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_41.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_42.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_43.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_44.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_45.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_46.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_47.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_48.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_49.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_5.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_50.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_51.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_52.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_53.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_54.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_55.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_56.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_57.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_58.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_59.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_6.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_60.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_61.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_62.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_63.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_64.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_65.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_66.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_67.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_68.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_69.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_7.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_70.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_71.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_72.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_73.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_74.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_75.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_76.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_77.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_78.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_79.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_8.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_80.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_81.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_82.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_83.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_84.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_85.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_86.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_87.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_88.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_89.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_9.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_90.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_91.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_92.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_93.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_94.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_95.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_96.pkl
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/README.md
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5004 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/PKG-INFO
```

### Comparing `comet_toolbox-0.3.0/src/comet/cifti.py` & `comet_toolbox-0.3.2/src/comet/cifti.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/src/comet/data.py` & `comet_toolbox-0.3.2/src/comet/data.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/src/comet/graph.py` & `comet_toolbox-0.3.2/src/comet/graph.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/src/comet/gui.py` & `comet_toolbox-0.3.2/src/comet/gui.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 import sys
 import copy
+import json
 import pickle
 import inspect
 import numpy as np
 import pandas as pd
 import nibabel as nib
 from scipy.io import loadmat, savemat
 from dataclasses import dataclass, field
@@ -21,20 +22,19 @@
 
 # Qt imports
 import qdarkstyle
 from PyQt6.QtCore import Qt, QPoint, QThread, pyqtSignal, QObject
 from PyQt6.QtGui import QEnterEvent, QFontMetrics
 from PyQt6.QtWidgets import QApplication, QMainWindow, QPushButton, QVBoxLayout, QHBoxLayout, \
     QSlider, QToolTip, QWidget, QLabel, QFileDialog, QComboBox, QLineEdit, QSizePolicy, \
-    QSpacerItem, QCheckBox, QTabWidget, QSpinBox, QDoubleSpinBox, QTextEdit
+    QSpacerItem, QCheckBox, QTabWidget, QSpinBox, QDoubleSpinBox, QTextEdit, QMessageBox
 
 # Comet imports and state-based dFC methods from pydfc
 from . import cifti, methods, graph
 import pydfc
-import bct
 
 class Worker(QObject):
     # Worker class for calculations (runs in a separate thread)
     finished = pyqtSignal()
     error = pyqtSignal(str)
     result = pyqtSignal(object)
 
@@ -64,35 +64,40 @@
         tooltip_pos = self.mapToGlobal(QPoint(self.width(), 0)) # Tooltip position can be adjusted here
         QToolTip.showText(tooltip_pos, self.info_text)
         super().enterEvent(event)
 
 @dataclass
 class Data:
     # File variables
-    file_name:    str        = field(default=None)         # data file name
-    file_data:    np.ndarray = field(default=None)         # input time series data  
+    file_name:     str        = field(default=None)         # data file name
+    file_data:     np.ndarray = field(default=None)         # input time series data  
 
     # DFC variables
-    dfc_instance: Any        = field(default=None)         # instance of the dFC class
-    dfc_name:     str        = field(default=None)         # method class name
-    dfc_params:   Dict       = field(default_factory=dict) # input parameters
-    dfc_data:     np.ndarray = field(default=None)         # dfc data
-    dfc_states:   Dict       = field(default_factory=dict) # dfc states
-    dfc_state_tc: np.ndarray = field(default=None)         # dfc state time course
-    dfc_edge_ts:  np.ndarray = field(default=None)         # dfc edge time series
+    dfc_instance:  Any        = field(default=None)         # instance of the dFC class
+    dfc_name:      str        = field(default=None)         # method class name
+    dfc_params:    Dict       = field(default_factory=dict) # input parameters
+    dfc_data:      np.ndarray = field(default=None)         # dfc data
+    dfc_states:    Dict       = field(default_factory=dict) # dfc states
+    dfc_state_tc:  np.ndarray = field(default=None)         # dfc state time course
+    dfc_edge_ts:   np.ndarray = field(default=None)         # dfc edge time series
 
     # Graph variables
-    graph_file:   str        = field(default=None)         # graph file name
-    graph_raw:    np.ndarray = field(default=None)         # raw input data for graph (dFC matrix)
-    graph_data:   np.ndarray = field(default=None)         # working data for graph (while processing)
-    graph_out:    Any = field(default=None)                # output graph measure data
+    graph_file:    str        = field(default=None)         # graph file name
+    graph_raw:     np.ndarray = field(default=None)         # raw input data for graph (dFC matrix)
+    graph_data:    np.ndarray = field(default=None)         # working data for graph (while processing)
+    graph_out:     Any = field(default=None)                # output graph measure data
+
+    # Multiverse variables
+    forking_paths: Dict      = field(default_factory=dict) # Decision points for multiverse analysis
+    invalid_paths: list      = field(default_factory=list) # Invalid paths for multiverse analysis
 
     # Misc variables
-    cifti_data:   np.ndarray = field(default=None)         # input cifti data (for .dtseries files)
-    roi_names:    np.ndarray = field(default=None)         # input roi data (for .tsv files)
+    cifti_data:    np.ndarray = field(default=None)         # input cifti data (for .dtseries files)
+    roi_names:     np.ndarray = field(default=None)         # input roi data (for .tsv files)
+    mv_containers: list       = field(default_factory=list) # decision containers for multiverse analysis
 
     def clear_dfc_data(self):
         self.dfc_params   = {}
         self.dfc_data     = None
         self.dfc_states   = {}
         self.dfc_state_tc = None
         self.dfc_edge_ts  = None
@@ -134,15 +139,14 @@
         # Get data for the last calculation with a given method
         for data_obj in reversed(list(self.storage.values())):
             if data_obj.dfc_name == methodName and data_obj.dfc_data is not None:
                 return copy.deepcopy(data_obj) # IMPORTANT: deep copy
         return None
 
 class App(QMainWindow):
-
     """
     Initialization and GUI setup functions
     """
     def __init__(self, init_dfc_data=None, init_dfc_instance=None):
         super().__init__()
         self.title = 'Comet Toolbox'
         self.init_flag = True
@@ -150,14 +154,15 @@
         self.data = Data()
         self.data_storage = DataStorage()
 
         self.currentSliderValue = 0
         self.currentTabIndex = 0
         self.graphStepCounter = 1
 
+        # Parameter names for the GUI
         self.param_names = {
             "self":                 "self", 
             "time_series":          "Time series",
             "windowsize":           "Window size",
             "shape":                "Window shape",
             "std":                  "Window sigma",
             "diagonal":             "Main diagonal",
@@ -198,14 +203,72 @@
             "dhmm_obs_state_ratio": "State ratio",
             "vlim":                 "Color axis limit",
             "parcellation":         "Parcellation"
 
         }
         self.reverse_param_names = {v: k for k, v in self.param_names.items()}
         
+        # All availble connectivity methods
+        self.connectivityMethods = {
+            'SlidingWindow':                'CONT Sliding Window',
+            'Jackknife':                    'CONT Jackknife Correlation',
+            'FlexibleLeastSquares':         'CONT Flexible Least Squares',
+            'SpatialDistance':              'CONT Spatial Distance', 
+            'TemporalDerivatives':          'CONT Multiplication of Temporal Derivatives',
+            'DCC':                          'CONT Dynamic Conditional Correlation',
+            'PhaseSynchrony':               'CONT Phase Synchronization',
+            'LeiDA':                        'CONT Leading Eigenvector Dynamics',
+            'WaveletCoherence':             'CONT Wavelet Coherence',
+            'Edge_centric_connectivity':    'CONT Edge-centric Connectivity',
+            
+            'Sliding_Window_Clustr':        'STATE Sliding Window Clustering',
+            'Cap':                          'STATE Co-activation patterns',
+            'HMM_Disc':                     'STATE Discrete Hidden Markov Model',
+            'HM_Cont':                      'STATE Continuous Hidden Markov Model',
+            'Windowless':                   'STATE Windowless',
+
+            'Static_Pearson':               'STATIC Pearson Correlation',
+            'Static_Partial':               'STATIC Partial Correlation',
+            'Static_Mutual_Info':           'STATIC Mutual Information'
+        }
+
+        self.reverse_connectivityMethods = {v: k for k, v in self.connectivityMethods.items()}
+        
+        
+        # All availble graph analysis functions
+        self.graphOptions = {
+            "handle_negative_weights":      "PREP Negative weights",
+            "threshold":                    "PREP Threshold",
+            "binarise":                     "PREP Binarise",
+            "normalise":                    "PREP Normalise",
+            "invert":                       "PREP Invert",
+            "logtransform":                 "PREP Log-transform",
+            "symmetrise":                   "PREP Symmetrise",
+            "randomise":                    "PREP Randomise",
+            "postproc":                     "PREP Post-processing",
+            
+            "efficiency":                   "COMET Efficiency",
+            "matching_ind_und":             "COMET Matching index",
+            "small_world_propensity":       "COMET Small world propensity",
+
+            "backbone_wu":                  "BCT Backbone (weighted)",
+            "betweenness":                  "BCT Betweenness centrality",
+            "clustering_coef":              "BCT Clustering coefficient",
+            "degrees_und":                  "BCT Degrees",
+            "density_und":                  "BCT Density",
+            "eigenvector_centrality_und":   "BCT Eigenvector centrality",
+            "gateway_coef_sign":            "BCT Gateway coefficient (sign)",
+            "pagerank_centrality":          "BCT Pagerank centrality",
+            "participation_coef":           "BCT Participation coef",
+            "participation_coef_sign":      "BCT Participation coef (sign)",
+            "transitivity":                 "BCT Transitivity",
+        }
+        self.reverse_graphOptions = {v: k for k, v in self.graphOptions.items()}
+
+        # Init the UI
         self.initUI()
 
         if init_dfc_data is not None:
             self.initFromData(init_dfc_data, init_dfc_instance)
 
     def initUI(self):
         self.setWindowTitle(self.title)
@@ -214,15 +277,15 @@
         topLayout = QVBoxLayout()
         self.topTabWidget = QTabWidget()
         topLayout.addWidget(self.topTabWidget)
 
         # Setup the individual tabs
         self.connectivityTab()
         self.graphTab()
-        #self.multiverseTab()
+        self.multiverseTab()
 
         # Set main window layout to the top-level layout
         centralWidget = QWidget()
         centralWidget.setLayout(topLayout)
         self.setCentralWidget(centralWidget)
 
     def initFromData(self, init_dfc_data=None, init_dfc_instance=None):
@@ -305,17 +368,22 @@
 
         ###############################
         #  Left section for settings  #
         ###############################
         self.leftLayout = QVBoxLayout()
 
         # Create button and label for file loading
-        self.fileButton = QPushButton('Load File')
-        self.fileNameLabel = QLabel('No file loaded')
-        self.leftLayout.addWidget(self.fileButton)
+        loadLayout = QHBoxLayout()
+        self.fileButton = QPushButton('Load time series')
+        self.bidsButton = QPushButton('Load BIDS dataset')
+        self.fileNameLabel = QLabel('No file loaded yet')
+        
+        loadLayout.addWidget(self.fileButton)
+        loadLayout.addWidget(self.bidsButton)
+        self.leftLayout.addLayout(loadLayout)
         self.leftLayout.addWidget(self.fileNameLabel)
         self.fileButton.clicked.connect(self.loadConnectivityFile)
 
         # Create a checkbox for reshaping the data
         self.transposeCheckbox = QCheckBox("Transpose data (time has to be the first dimension)")
         self.leftLayout.addWidget(self.transposeCheckbox)
         self.transposeCheckbox.setEnabled(False)
@@ -544,60 +612,29 @@
         self.loadGraphFileButton.clicked.connect(self.loadGraphFile)
 
         self.takeCurrentButton = QPushButton('From current dFC')
         self.takeCurrentButton.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Preferred)
         buttonsLayout.addWidget(self.takeCurrentButton, 1)
         self.takeCurrentButton.clicked.connect(self.takeCurrentData)
         
-        self.graphFileNameLabel = QLabel('No file loaded')
+        self.graphFileNameLabel = QLabel('No file loaded yet')
 
         leftLayout.addLayout(buttonsLayout)
         leftLayout.addWidget(self.graphFileNameLabel)
         leftLayout.addItem(QSpacerItem(0, 20, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Fixed))
 
         # Graph analysis options
         graphTabLabel = QLabel("Graph analysis options:")
         leftLayout.addWidget(graphTabLabel)
 
         # Checkboxes for method types
         self.preprocessingCheckBox = QCheckBox("Preprocessing")
         self.graphCheckBox = QCheckBox("Comet")
         self.BCTCheckBox = QCheckBox("BCT")
 
-        # Populate the combo box with options
-        self.graphOptions = {
-            "handle_negative_weights":      "PREP Negative weights",
-            "threshold":                    "PREP Threshold",
-            "binarise":                     "PREP Binarise",
-            "normalise":                    "PREP Normalise",
-            "invert":                       "PREP Invert",
-            "logtransform":                 "PREP Log-transform",
-            "symmetrise":                   "PREP Symmetrise",
-            "randomise":                    "PREP Randomise",
-            "postproc":                     "PREP Post-processing",
-            
-            "efficiency":                   "COMET Efficiency",
-            "matching_ind_und":             "COMET Matching index",
-            "small_world_propensity":       "COMET Small world propensity",
-
-            "backbone_wu":                  "BCT Backbone (weighted)",
-            "betweenness":                  "BCT Betweenness centrality",
-            "clustering_coef":              "BCT Clustering coefficient",
-            "degrees_und":                  "BCT Degrees",
-            "density_und":                  "BCT Density",
-            "eigenvector_centrality_und":   "BCT Eigenvector centrality",
-            "gateway_coef_sign":            "BCT Gateway coefficient (sign)",
-            "pagerank_centrality":          "BCT Pagerank centrality",
-            "participation_coef":           "BCT Participation coef",
-            "participation_coef_sign":      "BCT Participation coef (sign)",
-            "transitivity":                 "BCT Transitivity",
-        }
- 
-        self.reverse_graphOptions = {v: k for k, v in self.graphOptions.items()}
-
         # Checkboxes for function types
         checkboxLayout = QHBoxLayout()
         checkboxLayout.addWidget(self.preprocessingCheckBox)
         checkboxLayout.addWidget(self.graphCheckBox)
         checkboxLayout.addWidget(self.BCTCheckBox)
         checkboxLayout.setSpacing(10)
         checkboxLayout.addStretch()
@@ -654,15 +691,14 @@
         leftLayout.addWidget(self.optionsTextbox)
 
         # "Save" button
         saveButton = QPushButton('Save')
         leftLayout.addWidget(saveButton)
         saveButton.clicked.connect(self.saveGraphFile)
 
-
         ################################
         #  Right section for plotting  #
         ################################
         rightLayout = QVBoxLayout()
         
         # Different plotting tabs
         graphTabWidget = QTabWidget()
@@ -731,76 +767,744 @@
         multiverseTab.setLayout(multiverseLayout)
         
         ###############################
         #  Left section for settings  #
         ###############################
         leftLayout = QVBoxLayout()
 
-        # Section for defining decision points
-        decisionPointLabel = QLabel('Define Decision Points:')
-        leftLayout.addWidget(decisionPointLabel)
-
-        # Container for dynamic input fields based on decision type
-        self.decisionFieldsContainer = QVBoxLayout()
-        self.decisionTypeDropdown = QComboBox()
-        self.decisionTypeDropdown.addItems(['Select Decision Type', 'strings', 'numbers', 'booleans', 'dfc_measures', 'graph_measures'])
-        self.decisionTypeDropdown.currentIndexChanged.connect(self.updateDecisionFields)  # Implement this method
-        leftLayout.addWidget(self.decisionTypeDropdown)
-        leftLayout.addLayout(self.decisionFieldsContainer)
-
-        addDecisionButton = QPushButton('Add Decision Point')
-        addDecisionButton.clicked.connect(self.addDecisionPoint)  # Implement this method
-        leftLayout.addWidget(addDecisionButton)
-
-        # Section for defining invalid paths
-        invalidPathsLabel = QLabel('Define Invalid Paths:')
-        self.invalidPathsEditor = QTextEdit()
-        leftLayout.addWidget(invalidPathsLabel)
-        leftLayout.addWidget(self.invalidPathsEditor)
+        loadLabel = QLabel('Create multiverse analysis template script:')
+        leftLayout.addWidget(loadLabel)
+
+        # Creating a first decision container
+        decisionWidget = self.addDecisionContainer()
+        leftLayout.addWidget(decisionWidget)
+
+        # Horizontal layout for add/collapse buttons
+        buttonLayout = QHBoxLayout()
+
+        newDecisionButton = QPushButton("\u2795")
+        newDecisionButton.clicked.connect(lambda: self.addNewDecision(leftLayout, buttonLayout))
+        buttonLayout.addWidget(newDecisionButton, 5)
+        buttonLayout.addStretch(21)
+
+        leftLayout.addLayout(buttonLayout)
 
         leftLayout.addStretch()
 
+
+        #########################
+        #  Bottom left section  #
+        #########################
+
+        # Perform multiverse analysis
+        loadLabel = QLabel('Perform multiverse analysis:')
+        leftLayout.addWidget(loadLabel)
+
+        loadLayout = QHBoxLayout()
+        loadScriptButton = QPushButton('Load Script')
+        loadLayout.addWidget(loadScriptButton, 1)
+
+        # Textbox to display the loaded script path
+        self.loadedScriptDisplay = QLineEdit()
+        self.loadedScriptDisplay.setPlaceholderText("No script loaded yet")
+        self.loadedScriptDisplay.setReadOnly(True)
+        loadLayout.addWidget(self.loadedScriptDisplay, 3)
+
+        # Add the horizontal layout to the main left layout
+        leftLayout.addLayout(loadLayout)
+
+        # Connect the button to the method that handles file loading
+        loadScriptButton.clicked.connect(self.loadScript)
+
+        executeButton = QPushButton('Run multiverse analysis')
+        leftLayout.addWidget(executeButton)
+        executeButton.clicked.connect(self.executeScript)
+
+
         ################################
         #  Right section for plotting  #
         ################################
         rightLayout = QVBoxLayout()
-        
-        # Different plotting tabs
-        multiverseTabWidget = QTabWidget()
 
-        # Tab 1: Imshow plot
-        imshowTab = QWidget()
-        imshowLayout = QVBoxLayout()
-        imshowTab.setLayout(imshowLayout)
+        # Creating a tab widget for different purposes
+        multiverseTabWidget = QTabWidget()
 
+        # Tab 1: Template textbox for script display
+        templateTab = QWidget()
+        templateLayout = QVBoxLayout()
+        templateTab.setLayout(templateLayout)
+
+        self.scriptDisplay = QTextEdit()
+        self.scriptDisplay.setReadOnly(True)
+        templateLayout.addWidget(self.scriptDisplay)
+
+        # Create and add the save button
+        saveScriptButton = QPushButton('Save template script')
+        saveScriptButton.clicked.connect(self.saveScript)
+        templateLayout.addWidget(saveScriptButton)
+
+        # Add the complete tab to the multiverseTabWidget
+        multiverseTabWidget.addTab(templateTab, "Template")
+        self.generateScript(init_template=True) # Generate the template script
+
+        # Tab 2: Plot for visualizations
+        plotTab = QWidget()
+        plotTab.setLayout(QVBoxLayout())
         self.multiverseFigure = Figure()
         self.multiverseCanvas = FigureCanvas(self.multiverseFigure)
         self.multiverseFigure.patch.set_facecolor('#E0E0E0')
-        imshowLayout.addWidget(self.multiverseCanvas)
-        multiverseTabWidget.addTab(imshowTab, "Imshow Plot")
-        rightLayout.addWidget(multiverseTabWidget)
+        plotTab.layout().addWidget(self.multiverseCanvas)
+        multiverseTabWidget.addTab(plotTab, "Multiverse Plot")
 
-        # Draw default plot (logo)
+        # Draw default plot (logo) on the canvas
         self.plotLogo(self.multiverseFigure)
         self.multiverseCanvas.draw()
 
+        # Add the tab widget to the right layout
+        rightLayout.addWidget(multiverseTabWidget)
+
         #####################
         #  Combine layouts  #
         #####################
         mainLayout = QHBoxLayout()
         mainLayout.addLayout(leftLayout, 1)
-        mainLayout.addLayout(rightLayout, 2)
+        mainLayout.addLayout(rightLayout, 1)
         multiverseLayout.addLayout(mainLayout)
 
         self.topTabWidget.addTab(multiverseTab, "Multiverse Analysis")
 
     """
+    Multiverse functions
+    """
+    # Adds a combined container widget for all things related to creating decisions and options
+    def addDecisionContainer(self):
+        decisionWidget = QWidget()  # Widget that holds the entire container
+        mainLayout = QVBoxLayout(decisionWidget)  # Vertical layout: contains decision layout and function layout
+        mainLayout.setContentsMargins(0, 0, 0, 0) # Remove space to remove excessive space between widgets
+
+        functionLayout = QHBoxLayout()  # Controls layout for functions and properties
+
+        # Create the dropdown menu
+        categoryComboBox = QComboBox()
+        categoryComboBox.addItems(["General", "FC", "Graph", "Other"])
+
+        # Decision name input field
+        decisionNameInput = QLineEdit()
+        decisionNameInput.setPlaceholderText("Decision name")
+
+        # Decision options input field
+        decisionOptionsInput = QLineEdit()
+        decisionOptionsInput.setPlaceholderText("Options (comma-separated)")
+
+        # Collapse button to hide/show the function and parameter widgets
+        collapseButton = QPushButton(" \u25B2 ")
+        collapseButton.setObjectName("collapseButton")
+        collapseButton.hide()
+
+        # Add option button to add a new option to the decision
+        addOptionButton = QPushButton(' \u25B6 ')
+        addOptionButton.hide()
+
+        # Include button to confirm the decision
+        includeButton = QPushButton(' \u2714 ')
+
+        # Remove button to delete the decision
+        removeButton = QPushButton(' \u2718 ')
+
+        # Add widgets to the layout with appropriate stretch factors
+        functionLayout.addWidget(categoryComboBox, 6)
+        functionLayout.addWidget(decisionNameInput, 7)
+        functionLayout.addWidget(decisionOptionsInput, 12)
+        functionLayout.addWidget(collapseButton, 1)
+        functionLayout.addWidget(addOptionButton, 1)
+        functionLayout.addWidget(includeButton, 1)
+        functionLayout.addWidget(removeButton, 1)
+
+        # Combo box for selecting specific functions or methods (will be inside the parameterContainer widget)
+        functionComboBox = QComboBox()
+        functionComboBox.currentIndexChanged.connect(lambda _: self.updateFunctionParameters(functionComboBox, parameterContainer))
+        functionComboBox.setObjectName("functionComboBox")
+        
+        # Parameter container widget
+        parameterContainer = QWidget()
+        parameterContainer.setObjectName("parameterContainer")
+        parameterLayout = QVBoxLayout()
+        parameterContainer.setLayout(parameterLayout)
+        parameterContainer.hide()
+
+        # Connect category combo box change
+        categoryComboBox.currentIndexChanged.connect(lambda _: self.onCategoryComboBoxChanged(categoryComboBox, functionComboBox, parameterContainer, addOptionButton, collapseButton, decisionNameInput, decisionOptionsInput))
+
+        # Connect the signals for the buttons, done here so all widgets are available
+        includeButton.clicked.connect(lambda: self.includeDecision(categoryComboBox, decisionNameInput, decisionOptionsInput))
+        removeButton.clicked.connect(lambda: self.removeDecision(decisionNameInput, decisionWidget, decisionOptionsInput))
+        collapseButton.clicked.connect(lambda: self.collapseOption(collapseButton, parameterContainer))
+        addOptionButton.clicked.connect(lambda: self.addOption(functionComboBox, parameterContainer, decisionNameInput, decisionOptionsInput))
+
+        # Adding the controls layout to the main layout
+        mainLayout.addLayout(functionLayout)
+        mainLayout.addWidget(parameterContainer)
+
+        # Add the widget to a list so we can keep track of individual items
+        self.data.mv_containers.append(decisionWidget)
+
+        return decisionWidget
+
+    # Handles if the type of the decision is changed
+    def onCategoryComboBoxChanged(self, categoryComboBox, functionComboBox, parameterContainer, addOptionButton, collapseButton, decisionNameInput, decisionOptionsInput):
+        selected_category = categoryComboBox.currentText()
+        self.clearLayout(parameterContainer.layout())
+
+        functionComboBox.clear()
+        decisionNameInput.clear()
+        decisionOptionsInput.clear()
+
+        functionComboBox.hide()
+        parameterContainer.hide()
+        addOptionButton.hide()
+        collapseButton.hide()
+
+        """
+        # Re-populate fields based on the last entry in forking_paths for the selected category
+        last_key, last_entry = None, None
+        if selected_category in ['FC', 'Graph']:
+            # Filter entries by prefix in "Option" within args dict
+            prefix = 'PREP' if selected_category == 'Graph' else 'CONT'
+            for key, entries in reversed(list(self.data.forking_paths.items())):
+                if isinstance(entries, list) and any(isinstance(d, dict) and 'args' in d and 'Option' in d['args'] and prefix in d['args']['Option'] for d in entries):
+                    last_key, last_entry = key, entries
+                    break
+        elif selected_category == 'General':
+            # General is simply the last key in the dictionary where value is a list of ints
+            for key, value in reversed(list(self.data.forking_paths.items())):
+                if isinstance(value, list) and all(isinstance(x, int) for x in value):
+                    last_key, last_entry = key, value
+                    break
+
+        # Set the inputs if there was an entry found
+        if last_key:
+            decisionNameInput.setText(last_key)
+            if isinstance(last_entry, list) and all(isinstance(x, dict) for x in last_entry):
+                decisionOptionsInput.setText(', '.join(d['name'] for d in last_entry if 'name' in d))
+            elif isinstance(last_entry, list):
+                decisionOptionsInput.setText(', '.join(map(str, last_entry)))"""
+
+        # Sets up the layout and input fields for the new category/options
+        decisionOptionsInput.setPlaceholderText("Enter options, comma-separated" if selected_category == "General" else "Define options below")
+        decisionOptionsInput.setReadOnly(selected_category != "General")
+
+        if selected_category in ["FC", "Graph"]:
+            methods = self.graphOptions if selected_category == "Graph" else self.connectivityMethods
+            for name, description in methods.items():
+                functionComboBox.addItem(description, name)
+
+            functionComboBox.show()
+            parameterContainer.show()
+            addOptionButton.show()
+            collapseButton.show()
+
+        elif selected_category == "Other":
+            parameterContainer.show()
+            addOptionButton.show()
+            collapseButton.show()
+            self.otherOptionCategory(parameterContainer)
+
+        self.update()
+
+        return
+    
+    # Gets a dict with the current function parameters
+    def getFunctionParameters(self, parameterContainer):
+        params_dict = {}
+        paramLayout = parameterContainer.layout()
+
+        # Iterate over all layout items in the parameter layout
+        for i in range(paramLayout.count()):
+            layout_item = paramLayout.itemAt(i)
+
+            # Ensure the layout item is a QHBoxLayout (each parameter is in its own QHBoxLayout)
+            if isinstance(layout_item.layout(), QHBoxLayout):
+                param_layout = layout_item.layout()
+
+                # The parameter name is in the QLabel, and the value is in the second widget (QLineEdit, QComboBox, etc.)
+                if param_layout.count() >= 2:
+                    # Extract the parameter name from the QLabel
+                    param_name_label = param_layout.itemAt(0).widget()
+                    if isinstance(param_name_label, QLabel):
+                        param_name = param_name_label.text().rstrip(':')  # Remove the colon at the end
+
+                        # Extract the parameter value from the appropriate widget type
+                        param_widget = param_layout.itemAt(1).widget()
+                        if isinstance(param_widget, QLineEdit):
+                            param_value = param_widget.text()
+                        elif isinstance(param_widget, QComboBox):
+                            param_value = param_widget.currentText()
+                        elif isinstance(param_widget, QSpinBox) or isinstance(param_widget, QDoubleSpinBox):
+                            param_value = param_widget.value()
+
+                        # Convert to appropriate boolean type if necessary (LineEdit and QComboBox return strings)
+                        if param_value == "True":
+                            param_value = True
+                        elif param_value == "False":
+                            param_value = False
+
+                        # Add the parameter name and value to the dictionary
+                        params_dict[param_name] = param_value
+
+        return params_dict
+
+    # Creates and updates all the parameter widgets based on the selected function
+    def updateFunctionParameters(self, functionComboBox, parameterContainer):
+        if functionComboBox.currentData() is None:
+            return
+
+        func_key = functionComboBox.currentData()
+        try:
+            method_name = self.connectivityMethods[func_key]
+        except:
+            method_name = self.graphOptions[func_key]
+        prefix = method_name.strip().split(' ')[0]
+
+        if prefix == "COMET" or prefix == "PREP" or prefix == "BCT":
+            func = getattr(graph, functionComboBox.currentData())
+        elif prefix == "CONT" or prefix == "STATE" or prefix == "STATIC":
+            dfc_class_ = getattr(methods, functionComboBox.currentData())
+            func = dfc_class_.__init__
+        else:
+            QMessageBox.warning(self, "Error", "Function is not recognized")
+        
+        # Retrieve the signature of the function
+        func_signature = inspect.signature(func)
+        type_hints = get_type_hints(func)
+
+        # Clear previous parameters
+        self.clearLayout(parameterContainer.layout())
+
+        # Calculate the maximum label width
+        max_label_width = 0
+        font_metrics = QFontMetrics(self.font())
+        for name, param in func_signature.parameters.items():
+            if name not in ['self', 'args', 'kwargs']:  # Skip unwanted parameters
+                label_width = font_metrics.boundingRect(f"{name}:").width()
+                max_label_width = max(max_label_width, label_width)
+
+        # Add the function combobox
+        func_layout = QHBoxLayout()
+        func_label = QLabel("Option:")
+        func_label.setFixedWidth(max_label_width + 20)
+        func_layout.addWidget(func_label)
+        func_layout.addWidget(functionComboBox)
+        parameterContainer.layout().addLayout(func_layout)
+
+        # Add the 'Name' QLineEdit before other parameters
+        name_layout = QHBoxLayout()
+        name_label = QLabel("Name:")
+        name_label.setFixedWidth(max_label_width + 20)
+        name_edit = QLineEdit()
+        name_edit.setPlaceholderText("Option name")
+        name_layout.addWidget(name_label)
+        name_layout.addWidget(name_edit)
+        parameterContainer.layout().addLayout(name_layout)
+
+        is_first_parameter = True  # Flag to identify the first parameter
+
+        # Iterate over parameters in the function signature
+        temp_widgets = {}
+        for name, param in func_signature.parameters.items():
+        
+            if name not in ['self', 'copy', 'args', 'kwargs']:  # Skip unwanted parameters
+                # Horizontal layout for each parameter
+                param_layout = QHBoxLayout()
+                param_type = type_hints.get(name)
+                print(name, param_type)
+                param_default = 1 if isinstance(param.default, inspect._empty) else param.default
+                
+                if param_default == None:
+                    if param_type == bool:
+                        param_default = False
+                    elif param_type == int or param_type == float:
+                        param_default = 1
+                    else:
+                        param_default = "empty"
+
+                # Create a label for the parameter and set its fixed width
+                param_label = QLabel(f"{name}:")
+                param_label.setFixedWidth(max_label_width + 20)  # Add some padding
+                param_layout.addWidget(param_label)
+
+                # For the first parameter, set its value based on the data source and lock it
+                if is_first_parameter:
+                    param_widget = QLineEdit()
+                    param_widget.setPlaceholderText("Input data (name of the variable in the script)")
+                    is_first_parameter = False  # Update the flag so this block runs only for the first parameter
+                else:
+                    # Bool
+                    if param_type == bool:
+                        param_widget = QComboBox()
+                        param_widget.addItems(["False", "True"])
+                        param_widget.setCurrentIndex(int(param_default))
+                    # Int                  
+                    elif param_type == int:
+                        param_widget = QSpinBox()
+                        param_widget.setValue(param_default)
+                        param_widget.setMaximum(10000)
+                        param_widget.setMinimum(-10000)
+                        param_widget.setSingleStep(1)
+                    # Float 
+                    elif param_type == float:    
+                        param_widget = QDoubleSpinBox()
+                        if name == "threshold":
+                            param_widget.setValue(0.0)
+                        else:
+                            param_widget.setValue(param_default)
+
+                        if prefix == "COMET" or prefix == "PREP" or prefix == "BCT":
+                            param_widget.setMaximum(1.0)
+                            param_widget.setMinimum(0.0)
+                        else:
+                            param_widget.setMaximum(10000.0)
+                            param_widget.setMinimum(-10000.0)
+
+                        param_widget.setSingleStep(0.01)
+
+                    # String
+                    elif get_origin(type_hints.get(name)) is Literal:
+                        options = type_hints.get(name).__args__ 
+                        param_widget = QComboBox()
+                        param_widget.addItems([str(option) for option in options])
+                    # Fallback
+                    else:
+                        param_widget = QLineEdit(str(param.default) if param.default != inspect.Parameter.empty else "")
+
+                temp_widgets[name] = (param_label, param_widget)
+                param_layout.addWidget(param_widget)
+                parameterContainer.layout().addLayout(param_layout)
+
+        # Adjust visibility based on 'type' parameter
+        type_widget = None
+        if 'type' in temp_widgets:
+            _, type_widget = temp_widgets['type']
+
+        if type_widget:
+            # Function to update parameter visibility
+            def updateVisibility():
+                selected_type = type_widget.currentText()
+                if selected_type == 'absolute':
+                    if 'threshold' in temp_widgets:
+                        temp_widgets['threshold'][0].show()
+                        temp_widgets['threshold'][1].show()
+                    if 'density' in temp_widgets:
+                        temp_widgets['density'][0].hide()
+                        temp_widgets['density'][1].hide()
+                elif selected_type == 'density':
+                    if 'threshold' in temp_widgets:
+                        temp_widgets['threshold'][0].hide()
+                        temp_widgets['threshold'][1].hide()
+                    if 'density' in temp_widgets:
+                        temp_widgets['density'][0].show()
+                        temp_widgets['density'][1].show()
+            
+            # Connect the signal from the type_widget to the updateVisibility function
+            type_widget.currentIndexChanged.connect(updateVisibility)
+            updateVisibility()
+            
+            return
+
+    # "Other" category for custom functions
+    def otherOptionCategory(self, parameterContainer):
+        # Clear the parameter container
+        self.clearLayout(parameterContainer.layout())
+
+        # Add a single QLineEdit for the user to input the option
+        font_metrics = QFontMetrics(self.font())
+        label_width = font_metrics.boundingRect(f"Parameters:").width()
+
+        option_layout = QHBoxLayout()
+        option_label = QLabel("Function:")
+        option_label.setFixedWidth(label_width + 20)
+        option_edit = QLineEdit()
+        option_edit.setPlaceholderText("Name of the function (e.g. np.mean)")
+        option_layout.addWidget(option_label)
+        option_layout.addWidget(option_edit)
+        parameterContainer.layout().addLayout(option_layout)
+
+        param_layout = QHBoxLayout()
+        param_label = QLabel("Parameters:")
+        param_label.setFixedWidth(label_width + 20)
+        param_edit = QLineEdit()
+        param_edit.setPlaceholderText("Function parameters as dict (e.g. {'axis': 0})")
+        param_layout.addWidget(param_label)
+        param_layout.addWidget(param_edit)
+        parameterContainer.layout().addLayout(param_layout)
+
+        return  
+
+    # Adds a new decision widget to the layout
+    def addNewDecision(self, layout, buttonLayout):
+        # Collapse all existing parameter containers before adding a new one
+        for container in self.data.mv_containers:
+            parameterContainer = container.findChild(QWidget, "parameterContainer")
+            collapseButton = container.findChild(QPushButton, "collapseButton")
+            if parameterContainer and collapseButton and parameterContainer.isVisible():
+                self.collapseOption(collapseButton, parameterContainer)
+
+        # Add new decision container
+        newDecisionWidget = self.addDecisionContainer()
+        buttonLayoutIndex = layout.indexOf(buttonLayout)
+        layout.insertWidget(buttonLayoutIndex, newDecisionWidget)
+
+        return
+
+    # Add option to a decision
+    def addOption(self, functionComboBox, parameterContainer, nameInputField, optionsInputField):
+        # Retrieve the selected function key and determine its module prefix
+        func_key = functionComboBox.currentData()
+
+        try:
+            method_name = self.connectivityMethods[func_key]
+        except:
+            method_name = self.graphOptions[func_key]
+        prefix = method_name.strip().split(' ')[0]
+
+        if prefix == "COMET" or prefix == "PREP":
+            module_prefix = "comet.graph"
+        elif prefix == "BCT":
+            module_prefix = "bct"
+        elif prefix == "CONT" or prefix == "STATE" or prefix == "STATIC":
+            module_prefix = "comet.methods"
+        else:
+            QMessageBox.warning(self, "Error", "Function is not recognized")
+
+        # Construct the full function path
+        func = f"{module_prefix}.{func_key}"
+
+        params = self.getFunctionParameters(parameterContainer)
+        option_name = params.get('Name', '').strip()
+
+        if not option_name:
+            QMessageBox.warning(self, "Error", "Please provide a name for the option")
+            return
+
+        # Get current values from name and options input fields
+        currentName = nameInputField.text().strip()
+        currentOptions = optionsInputField.text().strip()
+
+        # Prepare the new options string by appending the new option name
+        newOptions = f"{currentOptions}, {option_name}" if currentOptions else option_name
+        optionsInputField.setText(newOptions)
+
+        # Construct the dict for the new option
+        option_dict = {
+            "name": option_name,
+            "func": func,
+            "args": {k: v for k, v in params.items() if k != 'Name'}
+        }
+
+        # Append the new option to the existing list in the data dictionary
+        if currentName not in self.data.forking_paths:
+            self.data.forking_paths[currentName] = []
+
+        # Add to forking paths
+        self.data.forking_paths[currentName].append(option_dict)
+        return
+    
+    # Collapse the option layout
+    def collapseOption(self, collapseButton, parameterContainer):
+        if collapseButton.text() == " \u25B2 ":
+            parameterContainer.hide()
+            collapseButton.setText(" \u25BC ")
+            return
+            
+        if collapseButton.text() == " \u25BC ":
+            parameterContainer.show()
+            collapseButton.setText(" \u25B2 ")
+            return
+        
+        return
+
+    # Adds decision to the script
+    def includeDecision(self, categoryComboBox, nameInput, optionsInput):
+        category = categoryComboBox.currentText()
+        name = nameInput.text().strip()
+
+        if category == "General":
+            options = [self.setDtypeForOption(option.strip()) for option in optionsInput.text().split(',') if option.strip()]
+            self.data.forking_paths[name] = options
+        else: 
+            options = self.data.forking_paths[name]
+
+        if name and options:
+            self.generateScript()
+        else:
+            QMessageBox.warning(self, "Input Error", "Please ensure a name and at least one option are provided.")
+        return
+    
+    # Handles data conversion based on the input
+    def setDtypeForOption(self, option):
+        # Try to convert to integer
+        try:
+            return int(option)
+        except ValueError:
+            pass
+
+        # Try to convert to float
+        try:
+            return float(option)
+        except ValueError:
+            pass
+
+        # Check for boolean values
+        if option.lower() in ['true', 'false']:
+            return option.lower() == 'true'
+
+        return option
+
+    # Removes one option with each click and finally the entire decision
+    def removeDecision(self, decisionNameInput, decisionWidget, optionsInputField):
+        key = decisionNameInput.text().strip()
+
+        # No key means the decision widget is empty, so clear and delete everything
+        if key == "":
+            if decisionWidget.layout():
+                self.clearLayout(decisionWidget.layout())
+                decisionWidget.deleteLater()
+                optionsInputField.clear()
+                self.data.mv_containers.remove(decisionWidget)
+                return
+            
+        if key in self.data.forking_paths:
+            options = self.data.forking_paths[key]
+
+            # Remove the last option and update the input field
+            if options:
+                options.pop()  # Remove the last option
+                options_str = ', '.join(opt['name'] if isinstance(opt, dict) else str(opt) for opt in options)
+                optionsInputField.setText(options_str)  # Update the input field
+
+            # If all options are removed or there are no options, clear and delete everything
+            if not options:
+                del self.data.forking_paths[key]
+                if decisionWidget.layout():
+                    self.clearLayout(decisionWidget.layout())  # Clear all child widgets and sub-layouts
+                decisionWidget.deleteLater()  # Delete the decision widget
+                optionsInputField.clear()  # Clear the options input field
+                self.data.mv_containers.remove(decisionWidget)
+
+        self.generateScript()
+        return
+
+    # Clears the entire decisionWidget layout
+    def clearLayout(self, layout):
+        # Recursively delete all items in a layout. This method handles both widgets and sub-layouts.
+        while layout.count():
+            item = layout.takeAt(0)  # Take the first item in the layout
+            if item.widget():
+                if item.widget().objectName() != "functionComboBox":  # Ensure it's not the functionComboBox
+                    item.widget().deleteLater()  # Delete the widget if the item is a widget
+            elif item.layout():
+                self.clearLayout(item.layout())  # Recursively clear if the item is a layout
+                item.layout().deleteLater()  # Delete the sub-layout after clearing it
+            elif item.spacerItem():
+                # No need to delete spacer items as Qt does it automatically
+                pass
+    
+    # Generates the template script
+    def generateScript(self, init_template=False):
+        if init_template:
+            script_content = (
+                "\"\"\"\n"
+                "Running Multiverse analysis\n"
+                "\n"
+                "Multiverse analysis requires a Python script to be created by the user.\n"
+                "An initial template for this can be created through the GUI, with forking paths being stored in a dict and later used through double curly braces in the template function.\n\n"
+                "This example shows how one would create and run a multiverse analysis which will generate 3 Python scripts (universes) printing the numbers 1, 2, and 3, respectively.\n"
+                "\"\"\"\n"
+                "\n"
+                "from comet.multiverse import Multiverse\n"
+                "\n"
+                "forking_paths = {\n"
+                "    \"numbers\": [1, 2, 3]\n"
+                "}\n"
+                "\n"
+                "def analysis_template():\n"
+                "    print({{numbers}})\n"
+                "\n"
+                "multiverse = Multiverse(name=\"multiverse_example\")\n"
+                "multiverse.create(analysis_template, forking_paths)\n"
+                "multiverse.summary()\n"
+                "#multiverse.run()\n"
+            )
+        
+        else:
+            script_content = (
+                "from comet.multiverse import Multiverse\n"
+                "\n"
+                "forking_paths = {\n"
+            )
+            for name, options in self.data.forking_paths.items():
+                if isinstance(options, list) and all(isinstance(item, dict) for item in options):
+                    # Format as JSON only if it's a list of dictionaries
+                    formatted_options = json.dumps(options, indent=4)
+                    formatted_options = formatted_options.replace('true', 'True').replace('false', 'False').replace('null', 'None')
+                    script_content += f'    "{name}": {formatted_options},\n'
+                else:
+                    # Simple list of primitives or a single dictionary
+                    script_content += f'    "{name}": {options},\n'
+
+            script_content += (
+                "}\n\n"
+                "def analysis_template():\n"
+                "    # The following forking paths are available for multiverse analysis:\n"
+            )
+
+            for name in self.data.forking_paths:
+                script_content += f"    {{{{{name}}}}}\n"  # placeholder variables are in double curly braces {{variable}}
+
+            script_content += (
+                "\nmultiverse = Multiverse(name=\"example_multiverse\")\n"
+                "multiverse.create(analysis_template, forking_paths)\n"
+                "multiverse.summary()\n"
+                "#multiverse.run()\n"
+            )
+
+        self.scriptDisplay.setText(script_content)
+
+    # Loads a multiverse script
+    def loadScript(self):
+        fileName, _ = QFileDialog.getOpenFileName(self, "Load Script", "", "Python Files (*.py);;All Files (*)")
+        if fileName:
+            self.loadedScriptDisplay.setText(f"Loaded: {fileName}")
+            self.loadedScriptPath = fileName
+
+    # Saves the current template script
+    def saveScript(self):
+        script_text = self.scriptDisplay.toPlainText()
+        fileName, _ = QFileDialog.getSaveFileName(self, "Save Script", "", "Python Files (*.py);;All Files (*)")
+
+        if fileName:
+            # Ensure the file has the correct extension
+            if not fileName.endswith('.py'):
+                fileName += '.py'
+            
+            with open(fileName, 'w') as file:
+                file.write(script_text)
+
+    # Runs the script/multiverse analysis
+    def executeScript(self):
+        if hasattr(self, 'loadedScriptPath') and self.loadedScriptPath:
+            with open(self.loadedScriptPath, "r") as file:
+                exec(file.read(), {})
+            QMessageBox.information(self, "Execution", "Script executed successfully.")
+        else:
+            QMessageBox.warning(self, "Load Script", "No script file is loaded.")
+
+    """
     I/O and data related functions
     """
-    # dFC functions
+    # dFC tab
     def loadConnectivityFile(self):
         fileFilter = "All Supported Files (*.mat *.txt *.npy *.pkl *.tsv *.dtseries.nii *.ptseries.nii);;MAT files (*.mat);;Text files (*.txt);;NumPy files (*.npy);;Pickle files (*.pkl);;TSV files (*.tsv);;CIFTI files (*.dtseries.nii *.ptseries.nii)"
         file_path, _ = QFileDialog.getOpenFileName(self, "Load File", "", fileFilter)
         file_name = file_path.split('/')[-1]
         self.data.file_name = file_name
         self.getParameters() # Get current UI parameters
 
@@ -909,15 +1613,15 @@
         self.methodComboBox.setEnabled(True)
         self.calculateButton.setEnabled(True)
         self.clearMemoryButton.setEnabled(True)
         self.keepInMemoryCheckbox.setEnabled(True)
 
     def saveConnectivityFile(self):
         if self.data.dfc_data is None:
-            print("No dFC data available to save.")
+            QMessageBox.warning(self, "Output Error", "No dFC data available to save.")
             return
 
         # Open a file dialog to specify where to save the file
         filePath, _ = QFileDialog.getSaveFileName(self, "Save File", "", "MAT Files (*.mat)")
 
         if filePath:
             # Ensure the file has the correct extension
@@ -951,16 +1655,16 @@
                         pass
                     else:
                         data_dict[field] = value
 
                 savemat(filePath, data_dict)
 
             except Exception as e:
-                print(f"Error saving data: {e}")
-            
+                QMessageBox.warning(self, "Output Error", f"Error saving data: {e}")
+
         return
 
     def onTransposeChecked(self, state):
         if self.data.file_data is None:
             return  # No data loaded, so do nothing
 
         if state == Qt.CheckState.Checked:
@@ -970,15 +1674,15 @@
             # Transpose it back to original
             self.data.file_data = self.data.file_data.transpose()
 
         # Update the labels
         self.fileNameLabel.setText(f"Loaded {self.time_series_textbox.text()} with shape: {self.data.file_data.shape}")
         self.time_series_textbox.setText(self.data.file_name)
 
-    # Graph functions
+    # Graph tab
     def loadGraphFile(self):
         fileFilter = "All Supported Files (*.mat *.txt *.npy *.pkl *.tsv *.dtseries.nii *.ptseries.nii);;MAT files (*.mat);;Text files (*.txt);;NumPy files (*.npy);;Pickle files (*.pkl);;TSV files (*.tsv);;CIFTI files (*.dtseries.nii *.ptseries.nii)"
         file_path, _ = QFileDialog.getOpenFileName(self, "Load File", "", fileFilter)
         file_name = file_path.split('/')[-1]
         self.data.graph_file = file_name
 
         if not file_path:
@@ -1005,15 +1709,15 @@
         self.graphFileNameLabel.setText(f"Loaded {self.data.graph_file} with shape {self.data.graph_data.shape}")
         
         self.plotGraph()
         self.onGraphCombobox()
 
     def saveGraphFile(self):
         if self.data.graph_data is None:
-            print("No graph data available to save.")
+            QMessageBox.warning(self, "Output Error", "No graph data available to save.")
             return
 
         # Open a file dialog to specify where to save the file
         filePath, _ = QFileDialog.getSaveFileName(self, "Save File", "", "MAT Files (*.mat)")
 
         if filePath:
             # Ensure the file has the correct extension
@@ -1047,95 +1751,36 @@
                         pass
                     else:
                         data_dict[field] = value
 
                 savemat(filePath, data_dict)
             
             except Exception as e:
-                print(f"Error saving data: {e}")
+                QMessageBox.warning(self, "Output Error", f"Error saving data: {e}")
             
             return
 
     def takeCurrentData(self):
         if self.data.dfc_data is None:
-            print("No current dFC data available.")
+            QMessageBox.warning(self, "Output Error", "No current dFC data available.")
             return
         
         self.data.graph_data = self.data.dfc_data[:,:,self.currentSliderValue]
         self.data.graph_raw = self.data.graph_data
         
         print(f"Used current dFC data with shape {self.data.graph_data.shape}")
         self.graphFileNameLabel.setText(f"Used current dFC data with shape {self.data.graph_data.shape}")
         self.data.graph_file = f"dfC from {self.data.file_name}" #with {self.data.dfc_name} at t={self.currentSliderValue}"
         self.plotGraph()
         self.onGraphCombobox()
 
     """
-    multiverse functions
-    """
-    def updateDecisionFields(self):
-        # First, clear existing fields in the decisionFieldsContainer layout
-        for i in reversed(range(self.decisionFieldsContainer.count())): 
-            self.decisionFieldsContainer.itemAt(i).widget().deleteLater()
-
-        # Check which decision type is selected and create corresponding input fields
-        decision_type = self.decisionTypeDropdown.currentText()
-        if decision_type == "strings" or decision_type == "numbers":
-            inputField = QLineEdit()
-            self.decisionFieldsContainer.addWidget(QLabel(f"Enter {decision_type}:"))
-            self.decisionFieldsContainer.addWidget(inputField)
-        elif decision_type == "booleans":
-            inputField = QComboBox()
-            inputField.addItems(["True", "False"])
-            self.decisionFieldsContainer.addWidget(QLabel("Select boolean value:"))
-            self.decisionFieldsContainer.addWidget(inputField)
-        elif decision_type in ["dfc_measures", "graph_measures"]:
-            # For complex types like dfc_measures, you might need multiple fields
-            nameField = QLineEdit()
-            connectivityField = QLineEdit()
-            inputDataField = QLineEdit()
-            self.decisionFieldsContainer.addWidget(QLabel("Name:"))
-            self.decisionFieldsContainer.addWidget(nameField)
-            self.decisionFieldsContainer.addWidget(QLabel("Connectivity:"))
-            self.decisionFieldsContainer.addWidget(connectivityField)
-            self.decisionFieldsContainer.addWidget(QLabel("Input Data:"))
-            self.decisionFieldsContainer.addWidget(inputDataField)
-            # Add more fields as needed for args etc.
-        # Add more decision types as needed
-
-    def addDecisionPoint(self):
-        decision_type = self.decisionTypeDropdown.currentText()
-        decision_data = {}
-
-        if decision_type == "strings" or decision_type == "numbers":
-            value = self.decisionFieldsContainer.itemAt(1).widget().text()  # Assuming the second widget is the input field
-            decision_data[decision_type] = [value]  # Wrap value in a list to mimic the structure
-        elif decision_type == "booleans":
-            value = self.decisionFieldsContainer.itemAt(1).widget().currentText()
-            decision_data[decision_type] = [value == "True"]  # Convert to boolean
-        elif decision_type in ["dfc_measures", "graph_measures"]:
-            # Assuming the first, third, and fifth widgets are the input fields
-            name = self.decisionFieldsContainer.itemAt(1).widget().text()
-            connectivity = self.decisionFieldsContainer.itemAt(3).widget().text()
-            input_data = self.decisionFieldsContainer.itemAt(5).widget().text()
-            # Collect more fields as needed and construct the decision data
-            decision_data[decision_type] = [{
-                "name": name,
-                "connectivity": connectivity,
-                "input_data": input_data,
-                # Include "args" and other fields as needed
-            }]
-
-        print("Added decision point:", decision_data)
-        # Here, instead of printing, you would add decision_data to your forking_paths structure
-
-    """
     dFC/graph functions
     """
-    # dFC functions
+    # dFC tab
     def onMethodCombobox(self, methodName=None):
         # Clear old variables and data
         self.clearParameters(self.parameterLayout)
 
         # Return if no methods are available
         if methodName == None or methodName == "Use checkboxes to get available methods":
             return
@@ -1337,15 +1982,15 @@
             "Schaefer Tian 254": "schaefer_tian"
         }
         atlas_name = atlas_map.get(atlas_name, None)
 
         self.data.file_data = cifti.parcellate(self.data.cifti_data, atlas=atlas_name)
         self.fileNameLabel.setText(f"Loaded and parcellated {self.data.file_name} with shape {self.data.file_data.shape}")
 
-    # Graph functios
+    # Graph tab
     def onGraphCombobox(self):
         self.setGraphParameters()
 
     def updateGraphComboBox(self):
         def shouldIncludeFunc(funcName):
             if self.preprocessingCheckBox.isChecked() and funcName.startswith("PREP"):
                 return True
@@ -1378,15 +2023,15 @@
             self.onGraphCombobox()
 
         return
 
     """
     Parameters
     """
-    # dFC functions
+    # dFC tab
     def initParameters(self, class_instance):
         # Now the parameter labels and boxes are set up    
         labels = []
 
         # Calculate the maximum label width (just a visual thing)
         max_label_width = 0
         init_signature = inspect.signature(class_instance.__init__)
@@ -1398,15 +2043,17 @@
         # Special case for 'time_series' parameter as this is created from the loaded file
         # Add label for time_series
         time_series_label = QLabel("Time series:")
         time_series_label.setSizePolicy(QSizePolicy.Policy.Preferred, QSizePolicy.Policy.Preferred)
         time_series_label.setMinimumSize(time_series_label.sizeHint())
         labels.append(time_series_label)
         
-        self.time_series_textbox.setText(self.data.file_name)
+        self.time_series_textbox.setPlaceholderText("No data loaded yet")
+        if self.data.file_name:
+            self.time_series_textbox.setText(self.data.file_name)
         self.time_series_textbox.setEnabled(True)
 
         # Create info button for time_series
         time_series_info_text = "2D time series loaded from file. Time has to be the first dimension."
         time_series_info_button = InfoButton(time_series_info_text)
 
         time_series_layout = QHBoxLayout()
@@ -1617,15 +2264,15 @@
             elif item.layout():  # If the item is a layout
                 self.clearParameters(item.layout())  # Recursively clear the layout
                 item.layout().deleteLater()  # Delete the layout itself
             elif item.spacerItem():  # If the item is a spacer
                 # No need to delete spacer items; they are automatically handled by Qt
                 pass
     
-    # Graph functions
+    # Graph tab
     def setGraphParameters(self):
         # Clear parameters
         self.clearParameters(self.graphParameterLayout)
         
         # Retrieve the selected function from the graph module
         if self.graphAnalysisComboBox.currentData() == None:
             return
@@ -1668,15 +2315,18 @@
                 # Create a label for the parameter and set its fixed width
                 param_label = QLabel(f"{name}:")
                 param_label.setFixedWidth(max_label_width + 20)  # Add some padding
                 param_layout.addWidget(param_label)
 
                 # For the first parameter, set its value based on the data source and lock it
                 if is_first_parameter:
-                    param_widget = QLineEdit("as shown in plot" if self.data.graph_file else "")
+                    param_widget = QLineEdit()
+                    param_widget.setPlaceholderText("No data loaded yet")
+                    if self.data.graph_file:
+                        param_widget = QLineEdit("as shown in plot")
                     param_widget.setReadOnly(True)  # Make the widget read-only
                     is_first_parameter = False  # Update the flag so this block runs only for the first parameter
                 else:
                     # Bool
                     if param_type == bool:
                         param_widget = QComboBox()
                         param_widget.addItems(["False", "True"])
@@ -1790,15 +2440,15 @@
         self.optionsTextbox.clear()
         self.graphTextbox.clear()
         self.graphStepCounter = 1
 
     """
     Calculation
     """
-    # dFC functions
+    # dFC tab
     def onCalculateButton(self):
         # Check if ts_data is available
         if self.data.file_data is None:
             self.calculatingLabel.setText(f"Error. No time series data has been loaded.")
             return
         
         # Get the current parameters from the UI for the upcoming calculation
@@ -1897,22 +2547,22 @@
 
         self.calculateButton.setEnabled(True)
         self.onTabChanged()
         self.update()
 
     def handleError(self, error):
         # Handles errors in the worker thread
-        print(f"Error occurred: {error}")
+        QMessageBox.warning(self, "Calculation Error", f"Error occurred furing calculation: {error}")
         self.calculateButton.setEnabled(True)
         self.data.clear_dfc_data()
         self.positionLabel.setText("no data available")
         self.plotLogo(self.figure)
         self.canvas.draw()
 
-    # Graph functions
+    # Graph tab
     def onAddGraphOption(self):
 
         # Start worker thread for graph calculations
         self.workerThread = QThread()
         self.worker = Worker(self.calculateGraph, None)
         self.worker.moveToThread(self.workerThread)
 
@@ -1979,20 +2629,20 @@
         updated_text = '\n'.join(lines)
         self.optionsTextbox.setPlainText(updated_text)
 
         self.graphStepCounter += 1
 
     def handleGraphError(self, error):
         # Handles errors in the worker thread
-        print(f"Error occurred: {error}")
+        QMessageBox.warning(self, "Calculation Error", f"Error occurred furing calculation: {error}")
 
     """
     Memory functions
     """
-    # dFC functions
+    # dFC tab
     def onKeepInMemoryChecked(self, state):
         if state == 2 and self.data.dfc_data is not None:
             self.data_storage.add_data(self.data)
                 
     def onClearMemory(self):
         self.data_storage = DataStorage()
         
@@ -2004,20 +2654,20 @@
         self.calculatingLabel.setText(f"Cleared memory")
         print("Cleared memory")
         return
 
     """
     Plotting functions
     """
-    # dFC functions
+    # dFC tab
     def plotConnectivity(self):
         current_data = self.data.dfc_data
         
         if current_data is None:
-            print("No calculated data available for plotting")
+            QMessageBox.warning(self, "No calculated data available for plotting")
             return
 
         self.figure.clear()
         ax = self.figure.add_subplot(111)
 
         try:
             current_slice = current_data[:, :, self.currentSliderValue] if len(current_data.shape) == 3 else current_data
@@ -2027,14 +2677,21 @@
             current_slice = current_data[:, :, 0] if len(current_data.shape) == 3 else current_data
             vmax = np.max(np.abs(current_slice))
             self.im = ax.imshow(current_slice, cmap='coolwarm', vmin=-vmax, vmax=vmax)
 
         ax.set_xlabel("ROI")
         ax.set_ylabel("ROI")
 
+        # If we have roi names and less than 100 ROIS, we can plot the names
+        if self.data.roi_names is not None and len(self.data.roi_names) < 100:
+            ax.set_xticks(np.arange(len(self.data.roi_names)))
+            ax.set_yticks(np.arange(len(self.data.roi_names)))
+            ax.set_xticklabels(self.data.roi_names, rotation=45, fontsize=120/len(self.data.roi_names) + 2)
+            ax.set_yticklabels(self.data.roi_names,              fontsize=120/len(self.data.roi_names) + 2)
+
         # Create the colorbar
         divider = make_axes_locatable(ax)
         cax = divider.append_axes("right", size="5%", pad=0.15)
         cbar = self.figure.colorbar(self.im, cax=cax)
         cbar.ax.yaxis.set_major_formatter(FuncFormatter(lambda x, _: f'{x:.1f}'))
 
         self.slider.setMaximum(current_data.shape[2] - 1 if len(current_data.shape) == 3 else 0)
@@ -2304,20 +2961,20 @@
         self.currentSliderValue = max(0, min(self.slider.value() + delta, self.slider.maximum()))
         self.slider.setValue(self.currentSliderValue)
         self.slider.update()
         
         self.plotConnectivity()
         self.plotDistribution()
 
-    # Graph functions
+    # Graph tab
     def plotGraph(self):
         current_data = self.data.graph_data
         
         if current_data is None:
-            print("No data available for plotting")
+            QMessageBox.warning(self, "No calculated data available for plotting")
             return
 
         self.matrixFigure.clear()
         ax = self.matrixFigure.add_subplot(111)
 
         vmax = np.max(np.abs(current_data))
         self.im = ax.imshow(current_data, cmap='coolwarm', vmin=-vmax, vmax=vmax)
@@ -2422,15 +3079,15 @@
         # Draw the plot
         self.graphFigure.set_facecolor('#E0E0E0')
         self.graphFigure.tight_layout()
         self.graphCanvas.draw()
         
         return
     
-    # Shared functions
+    # Shared tab
     def plotLogo(self, figure=None):
         with pkg_resources.path("comet.resources.img", "logo.png") as file_path:
             logo = imread(file_path)
 
         figure.clear()
         ax = figure.add_subplot(111)
         ax.set_axis_off()
```

### Comparing `comet_toolbox-0.3.0/src/comet/methods.py` & `comet_toolbox-0.3.2/src/comet/methods.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from scipy.signal import windows, hilbert
 from scipy.linalg import eigh, solve, inv
 from scipy.optimize import minimize
 from sklearn.metrics import mutual_info_score
 from statsmodels.stats.weightstats import DescrStatsW
 from pycwt import cwt, Morlet
 from pydfc.dfc_methods import *
+from typing import Literal
 
 from joblib import Parallel, delayed
 os.environ["OPENBLAS_NUM_THREADS"] = "1"
 os.environ["OMP_NUM_THREADS"] = "1"
 
 '''
 Abstract class template for all dynamic functional connectivity methods
@@ -71,15 +72,24 @@
     options = {"shape": ["rectangular", "gaussian", "hamming"]}
 
     '''
     Sliding Window
         Most widely used method, which involves sliding a window over the data.
         Cavariance is estimated for each windowed section.
     '''
-    def __init__(self, time_series, windowsize=29, shape="rectangular", std=10, diagonal=0, standardize=False, fisher_z=False, tril=False):
+    def __init__(self,
+                 time_series: np.ndarray,
+                 windowsize: int = 29,
+                 shape: Literal["rectangular", "gaussian", "hamming"] = "rectangular",
+                 std: float = 10,
+                 diagonal: int = 0,
+                 standardize: bool = False,
+                 fisher_z: bool = False,
+                 tril: bool = False):
+        
         super().__init__(time_series, diagonal, standardize, fisher_z, tril)
         self.windowsize = windowsize
         self.shape = shape
         self.std = std
         
         self.N_estimates = self.T - self.windowsize + 1 # N possible estimates given the window size
         self.R_mat = np.full((self.P,self.P, self.N_estimates), np.nan)
@@ -131,15 +141,22 @@
     options = {}
     '''
     Jackknife correlation:
         Richter CG, Thompson WH, Bosman CA, Fries P. A jackknife approach to quantifying single-trial 
         correlation between covariance-based metrics undefined on a single-trial basis.
         https://doi.org/10.1016/j.neuroimage.2015.04.040
     '''
-    def __init__(self, time_series, windowsize=1, diagonal=0, standardize=False, fisher_z=False, tril=False):
+    def __init__(self,
+                 time_series: np.ndarray,
+                 windowsize: int = 1,
+                 diagonal: int = 0,
+                 standardize: bool = False,
+                 fisher_z: bool = False,
+                 tril: bool = False):
+        
         super().__init__(time_series, diagonal, standardize, fisher_z, tril)
         self.windowsize = windowsize
 
         self.N_estimates = self.T - self.windowsize + 1 # N possible estimates given the window size
         self.R_mat = np.full((self.P,self.P, self.N_estimates), np.nan)
 
         assert self.windowsize <= self.T, "windowsize is larger than time series"
@@ -174,15 +191,22 @@
     options = {"dist": ["euclidean"]}
     '''
     Spatial Distance:
         William Hedley Thompson, Per Brantefors, Peter Fransson. From static 
         to temporal network theory: Applications to functional brain connectivity. 
         https://doi.org/10.1162/NETN_a_00011
     '''
-    def __init__(self, time_series, dist='euclidean', diagonal=0, standardize=False, fisher_z=True, tril=False):
+    def __init__(self,
+                 time_series: np.ndarray,
+                 dist: Literal["euclidean", "cosine", "cityblock"] = "euclidean",
+                 diagonal: int = 0,
+                 standardize: bool = False,
+                 fisher_z: bool = False,
+                 tril: bool = False):
+        
         super().__init__(time_series, diagonal, standardize, fisher_z, tril)
         self.distance = self._distance_functions(dist)
 
         self.N_estimates = self.T
         self.R_mat = np.full((self.P,self.P, self.N_estimates), np.nan)
     
     def _distance_functions(self, dist):
@@ -222,15 +246,22 @@
     options = {}
     '''
     Multiplication of temporal derivatives:
         Shine JM, Koyejo O, Bell PT, Gorgolewski KJ, Gilat M, Poldrack RA. Estimation of
         dynamic functional connectivity using Multiplication of Temporal Derivatives.
         https://doi.org/10.1016/j.neuroimage.2015.07.064.
     '''
-    def __init__(self, time_series, windowsize=7, diagonal=0, standardize=False, fisher_z=False, tril=False):
+    def __init__(self,
+                 time_series: np.ndarray,
+                 windowsize: int = 7,
+                 diagonal: int = 0,
+                 standardize: bool = False,
+                 fisher_z: bool = False,
+                 tril: bool = False):
+        
         super().__init__(time_series, diagonal, standardize, fisher_z, tril)
         self.windowsize = windowsize
         
         self.N_estimates = self.T - self.windowsize
         self.R_mat = np.full((self.P,self.P, self.N_estimates), np.nan)
 
         assert self.windowsize <= self.T, "windowsize is larger than time series"
@@ -261,15 +292,24 @@
     options = {}
     '''
     Flexible Least Squares:
         Liao, W., Wu, G. R., Xu, Q., Ji, G. J., Zhang, Z., Zang, Y. F., & Lu, G. (2014). 
         DynamicBC: a MATLAB toolbox for dynamic brain connectome analysis. Brain connectivity, 4(10), 780-790.
         https://doi.org/10.1089/brain.2014.0253
     '''
-    def __init__(self, time_series, standardizeData=True, mu=100, num_cores=16, diagonal=0, standardize=False, fisher_z=False, tril=False):
+    def __init__(self,
+                 time_series: np.ndarray,
+                 standardizeData: bool = True,
+                 mu: float = 100,
+                 num_cores: int = 16,
+                 diagonal: int = 0,
+                 standardize: bool = False,
+                 fisher_z: bool = False,
+                 tril: bool = False):
+        
         super().__init__(time_series, diagonal, standardize, fisher_z, tril)
         self.N_estimates = self.T
         self.R_mat = np.full((self.P,self.P, self.N_estimates), np.nan)
         self.standardizeData = standardizeData
         self.mu = mu
         self.num_cores = num_cores
 
@@ -337,15 +377,22 @@
     name = "CONT Phase Synchronization"
     options = {"method": ["crp", "pcoh", "teneto"]}
     '''
     Instantaneous Phase Synchrony:
         Honari, H., Choe, A. S., & Lindquist, M. A. (2021). Evaluating phase synchronization methods in fMRI: 
         A comparison study and new approaches. NeuroImage, 228, 117704. https://doi.org/10.1016/j.neuroimage.2020.117704
     '''
-    def __init__(self, time_series, method="crp", diagonal=0, standardize=False, fisher_z=False, tril=False):
+    def __init__(self,
+                 time_series: np.ndarray,
+                 method: Literal["crp", "pcoh", "teneto"] = "crp",
+                 diagonal: int = 0,
+                 standardize: bool = False,
+                 fisher_z: bool = False,
+                 tril: bool = False):
+        
         super().__init__(time_series, diagonal, standardize, fisher_z, tril)
         self.N_estimates = self.T
         self.R_mat = np.full((self.P,self.P, self.N_estimates), np.nan)
         self.method = method
 
     def connectivity(self):
         '''
@@ -383,15 +430,22 @@
         of time-varying functional connectivity is associated with plasma psilocin and subjective effects. Neuroimage, 264, 119716.
         https://doi.org/10.1016/j.neuroimage.2022.119716
 
         Vohryzek, J., Deco, G., Cessac, B., Kringelbach, M. L., & Cabral, J. (2020). Ghost attractors in spontaneous brain activity: 
         Recurrent excursions into functionally-relevant BOLD phase-locking states. Frontiers in systems neuroscience, 14, 20.
         https://doi.org/10.3389/fnsys.2020.00020
     '''
-    def __init__(self, time_series, flip_eigenvectors=False, diagonal=0, standardize=False, fisher_z=False, tril=False):
+    def __init__(self,
+                 time_series: np.ndarray,
+                 flip_eigenvectors: bool = False,
+                 diagonal: int = 0,
+                 standardize: bool = False,
+                 fisher_z: bool = False,
+                 tril: bool = False):
+        
         super().__init__(time_series, diagonal, standardize, fisher_z, tril)
 
         self.N_estimates = self.T
         self.R_mat = np.full((self.P,self.P, self.N_estimates), np.nan)
         self.flip_eigenvectors = flip_eigenvectors
         self.res = []
 
@@ -427,15 +481,28 @@
     options = {"method": ["weighted"]}
     '''
     Instantaneous Wavelet Coherence:
         Jacob Billings, Manish Saggar, Jaroslav Hlinka, Shella Keilholz, Giovanni Petri; Simplicial and 
         topological descriptions of human brain dynamics. Network Neuroscience 2021; 5 (2): 549–568. 
         https://doi.org/10.1162/netn_a_00190
     '''
-    def __init__(self, time_series, method="weighted", TR=0.72, fmin=0.007, fmax=0.15, n_scales=15, drop_scales=2, drop_timepoints=50, diagonal=0, standardize=False, fisher_z=False, tril=False):
+    def __init__(self,
+                 time_series: np.ndarray,
+                 method: Literal["weighted"] = "weighted",
+                 TR: float = 0.72,
+                 fmin: float = 0.007,
+                 fmax: float = 0.15,
+                 n_scales: int = 15,
+                 drop_scales: int = 2,
+                 drop_timepoints: int = 50,
+                 diagonal: int = 0,
+                 standardize: bool = False,
+                 fisher_z: bool = False,
+                 tril: bool = False):
+        
         super().__init__(time_series, diagonal, standardize, fisher_z, tril)
 
         self.N_estimates = self.T
         self.R_mat = np.full((self.P,self.P, self.N_estimates), np.nan)
         self.method = method
         self.TR = TR
         self.fmin = fmin
@@ -516,15 +583,23 @@
     '''
     Dynamic Conditional Correlation:
         Lindquist, M. A., Xu, Y., Nebel, M. B., & Caffo, B. S. (2014). Evaluating dynamic bivariate correlations 
         in resting-state fMRI: a comparison study and a new approach. NeuroImage, 101, 531-546.
         https://doi.org/10.1016/j.neuroimage.2014.06.052
     '''
 
-    def __init__(self, time_series, num_cores=16, standardizeData=True, diagonal=0, standardize=False, fisher_z=False, tril=False):
+    def __init__(self,
+                 time_series: np.ndarray,
+                 num_cores: int = 16,
+                 standardizeData: bool = True,
+                 diagonal: int = 0,
+                 standardize: bool = False,
+                 fisher_z: bool = False,
+                 tril: bool = False):
+        
         super().__init__(time_series, diagonal, standardize, fisher_z, tril)
 
         self.N_estimates = self.T
         self.R_mat = np.full((self.P,self.P, self.N_estimates), np.nan)
         self.standardizeData = standardizeData
         self.num_cores = num_cores
 
@@ -725,15 +800,23 @@
         #return H, R, Theta, X
         return R
 
 class Edge_centric_connectivity(ConnectivityMethod):
     name = "CONT Edge-centric Connectivity"
     options = {}
 
-    def __init__(self, time_series, standardizeData=True, vlim=3, diagonal=0, standardize=False, fisher_z=False, tril=False):
+    def __init__(self,
+                 time_series: np.ndarray,
+                 standardizeData: bool = True,
+                 vlim: float = 3, # for plotting in the GUI, not used in the method itself
+                 diagonal: int = 0,
+                 standardize: bool = False,
+                 fisher_z: bool = False,
+                 tril: bool = False):
+        
         super().__init__(time_series, diagonal, standardize, fisher_z, tril)
         self.standardizeData = standardizeData
     
     def connectivity(self):
         
         z = zscore(self.time_series, axis=0, ddof=1) if self.standardizeData else self.time_series
         u, v = np.triu_indices(self.time_series.shape[1], k=1)
@@ -1066,41 +1149,60 @@
 '''
 Static FC methods
 '''
 class Static_Pearson(ConnectivityMethod):
     name = "STATIC Pearson Correlation"
     options = {}
 
-    def __init__(self, time_series, diagonal=0, standardize=False, fisher_z=False, tril=False):
+    def __init__(self,
+                 time_series: np.ndarray,
+                 diagonal: int = 0,
+                 standardize: bool = False,
+                 fisher_z: bool = False,
+                 tril: bool = False):
+        
         super().__init__(time_series, diagonal, standardize, fisher_z, tril)
 
     def connectivity(self):
         fc = np.corrcoef(self.time_series.T) 
         fc = self.postproc(fc)
         return fc  
 
 class Static_Partial(ConnectivityMethod):
     name = "STATIC Partial Correlation"
     options = {}
 
-    def __init__(self, time_series, diagonal=0, standardize=False, fisher_z=False, tril=False):
+    def __init__(self,
+                 time_series: np.ndarray,
+                 diagonal: int = 0,
+                 standardize: bool = False,
+                 fisher_z: bool = False,
+                 tril: bool = False):
+        
         super().__init__(time_series, diagonal, standardize, fisher_z, tril)
 
     def connectivity(self):
         corr = np.corrcoef(self.time_series.T)
         precision = inv(corr)
         fc = -precision / np.sqrt(np.outer(np.diag(precision), np.diag(precision)))
         fc = self.postproc(fc)
         return fc
     
 class Static_Mutual_Info(ConnectivityMethod):
     name = "STATIC Mutual Information"
     options = {}
 
-    def __init__(self, time_series, num_bins=10, diagonal=0, standardize=False, fisher_z=False, tril=False):
+    def __init__(self, 
+                 time_series: np.ndarray,
+                 num_bins: int = 10,
+                 diagonal: int = 0,
+                 standardize: bool = False,
+                 fisher_z: bool = False,
+                 tril: bool = False):
+        
         super().__init__(time_series, diagonal, standardize, fisher_z, tril)
         self.num_bins = num_bins
 
     def connectivity(self):
         assert self.num_bins is not None, "Number of bins must be specified for mutual information method"
 
         binned_data = np.zeros_like(self.time_series, dtype=int)
@@ -1116,8 +1218,7 @@
             for j in range(i + 1, self.P):
                 mi = mutual_info_score(binned_data[:, i], binned_data[:, j])
                 fc[i, j] = mi
                 fc[j, i] = mi
 
         fc = self.postproc(fc)
         return fc
-
```

### Comparing `comet_toolbox-0.3.0/src/comet/multiverse.py` & `comet_toolbox-0.3.2/src/comet/multiverse.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/src/comet/resources/simulation.pkl` & `comet_toolbox-0.3.2/src/comet/resources/simulation.pkl`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/src/comet/resources/simulation.txt` & `comet_toolbox-0.3.2/simulation.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/src/comet/resources/single_state.txt` & `comet_toolbox-0.3.2/src/comet/resources/single_state.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/src/comet/resources/atlas/Q1-Q6_RelatedValidation210.CorticalAreas_dil_Final_Final_Areas_Group_Colors_with_Atlas_ROIs2.32k_fs_LR.dlabel.nii` & `comet_toolbox-0.3.2/src/comet/resources/atlas/Q1-Q6_RelatedValidation210.CorticalAreas_dil_Final_Final_Areas_Group_Colors_with_Atlas_ROIs2.32k_fs_LR.dlabel.nii`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/src/comet/resources/atlas/README.md` & `comet_toolbox-0.3.2/src/comet/resources/atlas/README.md`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/src/comet/resources/atlas/Schaefer2018_200Parcels_17Networks_order_Tian_Subcortex_S4.dlabel.nii` & `comet_toolbox-0.3.2/src/comet/resources/atlas/Schaefer2018_200Parcels_17Networks_order_Tian_Subcortex_S4.dlabel.nii`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/src/comet/resources/atlas/Schaefer2018_200Parcels_Kong2022_17Networks_order.dlabel.nii` & `comet_toolbox-0.3.2/src/comet/resources/atlas/Schaefer2018_200Parcels_Kong2022_17Networks_order.dlabel.nii`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/src/comet/resources/atlas/fs_LR_32k_medial_mask.mat` & `comet_toolbox-0.3.2/src/comet/resources/atlas/fs_LR_32k_medial_mask.mat`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/src/comet/resources/img/content.drawio` & `comet_toolbox-0.3.2/src/comet/resources/img/content.drawio`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/src/comet/resources/img/content.png` & `comet_toolbox-0.3.2/src/comet/resources/img/content.png`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/src/comet/resources/img/gui.png` & `comet_toolbox-0.3.2/src/comet/resources/img/gui.png`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/src/comet/resources/img/logo.png` & `comet_toolbox-0.3.2/src/comet/resources/img/logo.png`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/example_analysis.ipynb` & `comet_toolbox-0.3.2/tutorials/example_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/example_dfc.ipynb` & `comet_toolbox-0.3.2/tutorials/example_dfc.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/example_graph.ipynb` & `comet_toolbox-0.3.2/tutorials/example_graph.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/example_multiverse.ipynb` & `comet_toolbox-0.3.2/tutorials/example_multiverse.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/example_data/abide_50008.txt` & `comet_toolbox-0.3.2/tutorials/example_data/abide_50008.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/example_data/aomic_multi.pkl` & `comet_toolbox-0.3.2/tutorials/example_data/aomic_multi.pkl`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/example_data/simulation.txt` & `comet_toolbox-0.3.2/src/comet/resources/simulation.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/example_data/xcpd.tsv` & `comet_toolbox-0.3.2/tutorials/example_data/xcpd.tsv`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_1.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_1.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_10.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_10.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_11.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_11.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_12.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_12.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_13.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_13.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_14.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_14.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_15.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_15.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_16.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_16.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_17.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_17.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_18.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_18.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_19.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_19.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_2.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_2.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_20.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_20.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_21.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_21.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_22.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_22.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_23.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_23.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_24.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_24.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_25.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_25.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_26.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_26.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_27.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_27.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_28.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_28.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_29.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_29.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_3.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_3.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_30.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_30.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_31.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_31.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_32.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_32.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_33.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_33.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_34.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_34.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_35.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_35.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_36.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_36.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_37.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_37.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_38.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_38.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_39.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_39.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_4.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_4.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_40.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_40.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_41.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_41.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_42.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_42.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_43.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_43.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_44.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_44.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_45.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_45.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_46.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_46.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_47.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_47.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_48.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_48.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_49.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_49.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_5.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_5.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_50.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_50.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_51.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_51.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_52.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_52.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_53.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_53.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_54.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_54.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_55.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_55.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_56.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_56.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_57.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_57.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_58.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_58.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_59.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_59.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_6.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_6.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_60.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_60.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_61.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_61.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_62.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_62.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_63.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_63.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_64.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_64.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_65.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_65.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_66.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_66.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_67.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_67.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_68.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_68.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_69.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_69.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_7.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_7.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_70.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_70.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_71.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_71.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_72.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_72.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_73.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_73.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_74.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_74.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_75.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_75.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_76.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_76.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_77.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_77.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_78.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_78.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_79.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_79.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_8.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_8.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_80.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_80.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_81.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_81.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_82.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_82.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_83.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_83.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_84.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_84.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_85.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_85.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_86.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_86.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_87.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_87.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_88.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_88.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_89.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_89.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_9.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_9.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_90.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_90.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_91.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_91.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_92.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_92.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_93.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_93.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_94.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_94.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_95.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_95.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/universe_96.py` & `comet_toolbox-0.3.2/tutorials/multiverse/universe_96.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/results/forking_paths.pkl` & `comet_toolbox-0.3.2/tutorials/multiverse/results/forking_paths.pkl`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/results/multiverse_summary.csv` & `comet_toolbox-0.3.2/tutorials/multiverse/results/multiverse_summary.csv`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/tutorials/multiverse/results/pipelines.csv` & `comet_toolbox-0.3.2/tutorials/multiverse/results/pipelines.csv`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/.gitignore` & `comet_toolbox-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/LICENSE` & `comet_toolbox-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.0/README.md` & `comet_toolbox-0.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 ## Comet - A dynamic functional connectivity toolbox for multiverse analysis
-[![DOI](src/comet/resources/img/badge.svg)](https://doi.org/10.1101/2024.01.21.576546)
+[![DOI](src/comet/resources/img/doi.svg)](https://doi.org/10.1101/2024.01.21.576546) [![PyPI](src/comet/resources/img/pypi.svg)](https://pypi.org/project/comet-toolbox/)
 
 **Important notes:**
 
 * This package is at an early stage of development, with frequent changes being made. If you intend to use this package at this stage, I kindly ask that you contact me via the email address in the [pyproject.toml](https://github.com/mibur1/dfc-multiverse/blob/main/pyproject.toml) file.
 * Many features are not yet tested, so there will be bugs (the question is just how many). A comprehensive testing suite and documentation will be added in the near future
 
 ### Current Features
 
 ![Features_image](src/comet/resources/img/content.png)
 
 ### Installation
 
-Installation is possible through the Python Package Index (PyPI) with the pip or pip3 command, depending on your system:
+It is recommended to use a dedicated [Anaconda](https://www.anaconda.com/download) or [Miniconda](https://conda.io/projects/conda/en/latest/index.html) environment to mitigate the risk of potential version conflicts:
 
 ```
-pip install comet-toolbox
+conda create -n comet python==3.11
+conda activate comet
 ```
-We further recommend using a dedicated [Anaconda](https://www.anaconda.com/download) or [Miniconda](https://conda.io/projects/conda/en/latest/index.html) environment to mitigate the risk of potential version conflicts.
 
+Installation is then possible through the Python Package Index (PyPI) with the pip or pip3 command, depending on your system:
+
+```
+pip install comet-toolbox
+```
 
 Installation from the source code of this repository is also possible:
 
 1. Download/clone the repository
 2. Open a terminal in the folder which contains the pyproject.toml file
-3. Install the package via pip (or pip3, depending on your environment)
-4. If you intend to implement your own modification, installing in editable mode (-e) is a helpful approach
+3. Install the package via pip (installing in editable mode (-e) is a helpful approach if you intend to modify the source code):
 
 ```
 pip install -e .
 ```
 
 ### Usage
 
 **General** 
 
 The toolbox is designed in a modular way, which means you can use the individual parts in combination with others, but also by themselves.
 
 * continuous and static dFC measures require 2D time series data (n_timepoints x n_regions) as input
-* state-based dFC methods require a TIME_SERIES object (as used in the pydfc package) containing data for multiple subjects as input
+* state-based dFC methods require a TIME_SERIES object (as used in the [pydfc toolbox](https://github.com/neurodatascience/dFC)) containing data for multiple subjects as input
 * Graph measures need 2D adjacency/connectivity matrices as input
-* Multiverse analysis needs decision/option pairs of any kind to create forking paths in the analysis
+* Multiverse analysis needs decision/option pairs of any kind to create forking paths in the analysis as well as a template script for the analysis
 
 
 **GUI** 
 
 After installation, you can use the graphical user interface through the terminal by typing:
 
 ```
```

### Comparing `comet_toolbox-0.3.0/pyproject.toml` & `comet_toolbox-0.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "comet-toolbox"
-version = "0.3.0"
+version = "0.3.2"
 authors = [
   {name="Micha Burkhardt", email="micha.burkhardt@uol.de"},
 ]
 description = "Dynamic functional connectivity toolbox for multiverse analysis"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 dependencies = [
   "numpy >=1.26.2",
```

### Comparing `comet_toolbox-0.3.0/PKG-INFO` & `comet_toolbox-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: comet-toolbox
-Version: 0.3.0
+Version: 0.3.2
 Summary: Dynamic functional connectivity toolbox for multiverse analysis
 Project-URL: Homepage, https://github.com/mibur1/dfc-multiverse
 Project-URL: Issues, https://github.com/mibur1/dfc-multiverse/issues
 Author-email: Micha Burkhardt <micha.burkhardt@uol.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Requires-Dist: bctpy>=0.6.1
 Requires-Dist: ipykernel>=6.29.3
 Requires-Dist: jinja2>=3.1.2
 Requires-Dist: joblib>=1.3.2
 Requires-Dist: matplotlib>=3.8.2
 Requires-Dist: networkx>=3.2.1
 Requires-Dist: nibabel>=5.1.0
@@ -30,56 +30,60 @@
 Requires-Dist: scipy>=1.11.4
 Requires-Dist: seaborn>=0.13.0
 Requires-Dist: statsmodels>=0.14.0
 Requires-Dist: tqdm>=4.66.1
 Description-Content-Type: text/markdown
 
 ## Comet - A dynamic functional connectivity toolbox for multiverse analysis
-[![DOI](src/comet/resources/img/badge.svg)](https://doi.org/10.1101/2024.01.21.576546)
+[![DOI](src/comet/resources/img/doi.svg)](https://doi.org/10.1101/2024.01.21.576546) [![PyPI](src/comet/resources/img/pypi.svg)](https://pypi.org/project/comet-toolbox/)
 
 **Important notes:**
 
 * This package is at an early stage of development, with frequent changes being made. If you intend to use this package at this stage, I kindly ask that you contact me via the email address in the [pyproject.toml](https://github.com/mibur1/dfc-multiverse/blob/main/pyproject.toml) file.
 * Many features are not yet tested, so there will be bugs (the question is just how many). A comprehensive testing suite and documentation will be added in the near future
 
 ### Current Features
 
 ![Features_image](src/comet/resources/img/content.png)
 
 ### Installation
 
-Installation is possible through the Python Package Index (PyPI) with the pip or pip3 command, depending on your system:
+It is recommended to use a dedicated [Anaconda](https://www.anaconda.com/download) or [Miniconda](https://conda.io/projects/conda/en/latest/index.html) environment to mitigate the risk of potential version conflicts:
 
 ```
-pip install comet-toolbox
+conda create -n comet python==3.11
+conda activate comet
 ```
-We further recommend using a dedicated [Anaconda](https://www.anaconda.com/download) or [Miniconda](https://conda.io/projects/conda/en/latest/index.html) environment to mitigate the risk of potential version conflicts.
 
+Installation is then possible through the Python Package Index (PyPI) with the pip or pip3 command, depending on your system:
+
+```
+pip install comet-toolbox
+```
 
 Installation from the source code of this repository is also possible:
 
 1. Download/clone the repository
 2. Open a terminal in the folder which contains the pyproject.toml file
-3. Install the package via pip (or pip3, depending on your environment)
-4. If you intend to implement your own modification, installing in editable mode (-e) is a helpful approach
+3. Install the package via pip (installing in editable mode (-e) is a helpful approach if you intend to modify the source code):
 
 ```
 pip install -e .
 ```
 
 ### Usage
 
 **General** 
 
 The toolbox is designed in a modular way, which means you can use the individual parts in combination with others, but also by themselves.
 
 * continuous and static dFC measures require 2D time series data (n_timepoints x n_regions) as input
-* state-based dFC methods require a TIME_SERIES object (as used in the pydfc package) containing data for multiple subjects as input
+* state-based dFC methods require a TIME_SERIES object (as used in the [pydfc toolbox](https://github.com/neurodatascience/dFC)) containing data for multiple subjects as input
 * Graph measures need 2D adjacency/connectivity matrices as input
-* Multiverse analysis needs decision/option pairs of any kind to create forking paths in the analysis
+* Multiverse analysis needs decision/option pairs of any kind to create forking paths in the analysis as well as a template script for the analysis
 
 
 **GUI** 
 
 After installation, you can use the graphical user interface through the terminal by typing:
 
 ```
```

