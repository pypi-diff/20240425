# Comparing `tmp/clinica-0.8.0.tar.gz` & `tmp/clinica-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clinica-0.8.0.tar", max compression
+gzip compressed data, was "clinica-0.8.1.tar", max compression
```

## Comparing `clinica-0.8.0.tar` & `clinica-0.8.1.tar`

### file list

```diff
@@ -1,426 +1,426 @@
--rw-r--r--   0        0        0    11842 2024-03-25 19:30:02.749439 clinica-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0     8791 2024-03-25 19:30:02.749439 clinica-0.8.0/README.md
--rw-r--r--   0        0        0      175 2024-03-25 19:30:02.749439 clinica-0.8.0/clinica/__init__.py
--rw-r--r--   0        0        0     3020 2024-03-25 19:30:02.749439 clinica-0.8.0/clinica/cmdline.py
--rw-r--r--   0        0        0       67 2024-03-25 19:30:02.749439 clinica-0.8.0/clinica/compat.py
--rw-r--r--   0        0        0       33 2024-03-25 19:30:02.749439 clinica-0.8.0/clinica/engine/__init__.py
--rw-r--r--   0        0        0     5730 2024-03-25 19:30:02.749439 clinica-0.8.0/clinica/engine/cmdparser.py
--rw-r--r--   0        0        0     1908 2024-03-25 19:30:02.749439 clinica-0.8.0/clinica/engine/template.py
--rw-r--r--   0        0        0        0 2024-03-25 19:30:02.749439 clinica-0.8.0/clinica/iotools/__init__.py
--rw-r--r--   0        0        0      225 2024-03-25 19:30:02.749439 clinica-0.8.0/clinica/iotools/abstract_converter.py
--rw-r--r--   0        0        0     1405 2024-03-25 19:30:02.749439 clinica-0.8.0/clinica/iotools/bids_dataset_description.py
--rw-r--r--   0        0        0      636 2024-03-25 19:30:02.749439 clinica-0.8.0/clinica/iotools/bids_readme.py
--rw-r--r--   0        0        0    33186 2024-03-25 19:30:02.749439 clinica-0.8.0/clinica/iotools/bids_utils.py
--rw-r--r--   0        0        0    11818 2024-03-25 19:30:02.749439 clinica-0.8.0/clinica/iotools/converter_utils.py
--rw-r--r--   0        0        0        0 2024-03-25 19:30:02.749439 clinica-0.8.0/clinica/iotools/converters/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 19:30:02.749439 clinica-0.8.0/clinica/iotools/converters/adni_to_bids/__init__.py
--rw-r--r--   0        0        0    20529 2024-03-25 19:30:02.749439 clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_json.py
--rw-r--r--   0        0        0        0 2024-03-25 19:30:02.749439 clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_modalities/__init__.py
--rw-r--r--   0        0        0     5278 2024-03-25 19:30:02.749439 clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_av45_fbb_pet.py
--rw-r--r--   0        0        0     9191 2024-03-25 19:30:02.749439 clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_dwi.py
--rw-r--r--   0        0        0    10401 2024-03-25 19:30:02.749439 clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_fdg_pet.py
--rw-r--r--   0        0        0     7452 2024-03-25 19:30:02.749439 clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_flair.py
--rw-r--r--   0        0        0     8072 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_fmri.py
--rw-r--r--   0        0        0     4507 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_pib_pet.py
--rw-r--r--   0        0        0    21003 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_t1.py
--rw-r--r--   0        0        0     4941 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_tau_pet.py
--rw-r--r--   0        0        0    10543 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_to_bids.py
--rw-r--r--   0        0        0     2542 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_to_bids_cli.py
--rw-r--r--   0        0        0    55186 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_utils.py
--rw-r--r--   0        0        0        0 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/aibl_to_bids/__init__.py
--rw-r--r--   0        0        0     5381 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/aibl_to_bids/aibl_to_bids.py
--rw-r--r--   0        0        0     1203 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/aibl_to_bids/aibl_to_bids_cli.py
--rw-r--r--   0        0        0      354 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/aibl_to_bids/utils/__init__.py
--rw-r--r--   0        0        0    22165 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/aibl_to_bids/utils/bids.py
--rw-r--r--   0        0        0    14678 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/aibl_to_bids/utils/clinical.py
--rw-r--r--   0        0        0      833 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/cli.py
--rw-r--r--   0        0        0      875 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/cli_param.py
--rw-r--r--   0        0        0     5053 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/genfi_to_bids/genfi_to_bids.py
--rw-r--r--   0        0        0     1884 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/genfi_to_bids/genfi_to_bids_cli.py
--rw-r--r--   0        0        0    33214 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/genfi_to_bids/genfi_to_bids_utils.py
--rw-r--r--   0        0        0        0 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/habs_to_bids/__init__.py
--rw-r--r--   0        0        0     9029 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/habs_to_bids/habs_to_bids.py
--rw-r--r--   0        0        0     1040 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/habs_to_bids/habs_to_bids_cli.py
--rw-r--r--   0        0        0        0 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/nifd_to_bids/__init__.py
--rw-r--r--   0        0        0     1840 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/nifd_to_bids/nifd_to_bids.py
--rw-r--r--   0        0        0     1014 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/nifd_to_bids/nifd_to_bids_cli.py
--rw-r--r--   0        0        0    12134 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/nifd_to_bids/nifd_utils.py
--rw-r--r--   0        0        0        0 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/oasis3_to_bids/__init__.py
--rw-r--r--   0        0        0     2509 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/oasis3_to_bids/oasis3_to_bids.py
--rw-r--r--   0        0        0      885 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/oasis3_to_bids/oasis3_to_bids_cli.py
--rw-r--r--   0        0        0    11900 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/oasis3_to_bids/oasis3_utils.py
--rw-r--r--   0        0        0        0 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/oasis_to_bids/__init__.py
--rw-r--r--   0        0        0     7519 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/oasis_to_bids/oasis_to_bids.py
--rw-r--r--   0        0        0     1000 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/oasis_to_bids/oasis_to_bids_cli.py
--rw-r--r--   0        0        0        0 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/ukb_to_bids/__init__.py
--rw-r--r--   0        0        0     2094 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/ukb_to_bids/ukb_to_bids.py
--rw-r--r--   0        0        0     1086 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/ukb_to_bids/ukb_to_bids_cli.py
--rw-r--r--   0        0        0    16777 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/converters/ukb_to_bids/ukb_utils.py
--rw-r--r--   0        0        0     2383 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/data/clinical_specifications_adni_participant.tsv
--rw-r--r--   0        0        0      244 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/data/clinical_specifications_adni_scans.tsv
--rw-r--r--   0        0        0    89321 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/data/clinical_specifications_adni_sessions.tsv
--rw-r--r--   0        0        0     2708 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/data/clinical_specifications_participant.tsv
--rw-r--r--   0        0        0     1136 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/data/clinical_specifications_scans.tsv
--rw-r--r--   0        0        0    32532 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/data/clinical_specifications_sessions.tsv
--rw-r--r--   0        0        0    10872 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/data/genfi_data.tsv
--rw-r--r--   0        0        0    16189 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/data/genfi_data_mapping.tsv
--rw-r--r--   0        0        0     7777 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/data/genfi_ref.csv
--rw-r--r--   0        0        0      271 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/data/modality_equiv.tsv
--rw-r--r--   0        0        0      243 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/data/ukb_ref.csv
--rw-r--r--   0        0        0        0 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/utils/__init__.py
--rw-r--r--   0        0        0     8809 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/utils/cli.py
--rw-r--r--   0        0        0    56731 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/utils/data_handling.py
--rw-r--r--   0        0        0    14183 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/iotools/utils/pipeline_handling.py
--rw-r--r--   0        0        0        0 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/lib/__init__.py
--rw-r--r--   0        0        0       65 2024-03-25 19:30:02.753439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@random/char.m
--rw-r--r--   0        0        0      465 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@random/display.m
--rw-r--r--   0        0        0       67 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@random/double.m
--rw-r--r--   0        0        0     1135 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@random/image.m
--rw-r--r--   0        0        0       76 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@random/isempty.m
--rw-r--r--   0        0        0      671 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@random/minus.m
--rw-r--r--   0        0        0       85 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@random/mpower.m
--rw-r--r--   0        0        0     1873 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@random/mtimes.m
--rw-r--r--   0        0        0      732 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@random/plus.m
--rw-r--r--   0        0        0     5850 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@random/random.m
--rw-r--r--   0        0        0       92 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@random/size.m
--rw-r--r--   0        0        0       46 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@random/subsref.m
--rw-r--r--   0        0        0       30 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@term/char.m
--rw-r--r--   0        0        0      315 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@term/display.m
--rw-r--r--   0        0        0       33 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@term/double.m
--rw-r--r--   0        0        0      574 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@term/image.m
--rw-r--r--   0        0        0       43 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@term/isempty.m
--rw-r--r--   0        0        0      694 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@term/minus.m
--rw-r--r--   0        0        0      116 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@term/mpower.m
--rw-r--r--   0        0        0     1166 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@term/mtimes.m
--rw-r--r--   0        0        0      828 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@term/plus.m
--rw-r--r--   0        0        0       97 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@term/size.m
--rw-r--r--   0        0        0      178 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@term/subsref.m
--rw-r--r--   0        0        0     3878 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@term/term.m
--rw-r--r--   0        0        0      102 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/I.m
--rw-r--r--   0        0        0     1340 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatAvSurf.m
--rw-r--r--   0        0        0     1662 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatAvVol.m
--rw-r--r--   0        0        0      750 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatColLim.m
--rw-r--r--   0        0        0      567 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatColormap.m
--rw-r--r--   0        0        0     1491 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatCoord2Ind.m
--rw-r--r--   0        0        0      497 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatDataCursor.m
--rw-r--r--   0        0        0      692 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatDataCursorP.m
--rw-r--r--   0        0        0      636 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatDataCursorQ.m
--rw-r--r--   0        0        0     2172 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatDelete.m
--rw-r--r--   0        0        0     2384 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatEdg.m
--rw-r--r--   0        0        0     3989 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatF.m
--rw-r--r--   0        0        0     1099 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatInd2Coord.m
--rw-r--r--   0        0        0     2615 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatInflate.m
--rw-r--r--   0        0        0    10279 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatLinMod.m
--rw-r--r--   0        0        0      946 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatListDir.m
--rw-r--r--   0        0        0      995 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatMaskCut.m
--rw-r--r--   0        0        0     1925 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatNorm.m
--rw-r--r--   0        0        0     3891 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatP.m
--rw-r--r--   0        0        0     4053 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatPCA.m
--rw-r--r--   0        0        0     4282 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatPeakClus.m
--rw-r--r--   0        0        0     4388 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatPlot.m
--rw-r--r--   0        0        0     1687 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatQ.m
--rw-r--r--   0        0        0     1448 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatROI.m
--rw-r--r--   0        0        0     3855 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadData.m
--rw-r--r--   0        0        0     1599 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadData1.m
--rw-r--r--   0        0        0     4371 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadSurf.m
--rw-r--r--   0        0        0     6091 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadSurf1.m
--rw-r--r--   0        0        0     5816 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadVol.m
--rw-r--r--   0        0        0    17058 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadVol1.m
--rw-r--r--   0        0        0    17594 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatResels.m
--rw-r--r--   0        0        0     2202 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatSmooth.m
--rw-r--r--   0        0        0      860 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatStand.m
--rw-r--r--   0        0        0     3190 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatSurf2Vol.m
--rw-r--r--   0        0        0     5852 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatT.m
--rw-r--r--   0        0        0     5335 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatView.m
--rw-r--r--   0        0        0    11047 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatView1.m
--rw-r--r--   0        0        0     7015 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatViewData.m
--rw-r--r--   0        0        0     7036 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatViewData_backup.m
--rw-r--r--   0        0        0     6798 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatView_backup.m
--rw-r--r--   0        0        0     2751 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatViews.m
--rw-r--r--   0        0        0     1976 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatVol2Surf.m
--rw-r--r--   0        0        0     1196 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteData.m
--rw-r--r--   0        0        0     2395 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteSurf.m
--rw-r--r--   0        0        0     3385 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteSurf1.m
--rw-r--r--   0        0        0     1231 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteVol.m
--rw-r--r--   0        0        0    19785 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteVol1.m
--rw-r--r--   0        0        0      470 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/fac2var.m
--rw-r--r--   0        0        0     1588 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/gl.m
--rw-r--r--   0        0        0     1404 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/icbm_template_2.00mm+orig.HEAD
--rw-r--r--   0        0        0      348 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/icbm_template_2.00mm.hdr
--rw-r--r--   0        0        0     4096 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/icbm_template_2.00mm.mnc
--rw-r--r--   0        0        0     2021 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/redmod.m
--rw-r--r--   0        0        0      996 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/spectral.m
--rw-r--r--   0        0        0    27286 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/stat_threshold.m
--rw-r--r--   0        0        0      836 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/var2fac.m
--rwxr-xr-x   0        0        0    25158 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/lib/clinicasurfstat/clinicasurfstat.m
--rw-r--r--   0        0        0      886 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/option.py
--rw-r--r--   0        0        0      536 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/pipelines/__init__.py
--rw-r--r--   0        0        0      369 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/pipelines/cli.py
--rw-r--r--   0        0        0       45 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/pipelines/cli_param/__init__.py
--rw-r--r--   0        0        0     1362 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/pipelines/cli_param/argument.py
--rw-r--r--   0        0        0     5474 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/pipelines/cli_param/option.py
--rw-r--r--   0        0        0      538 2024-03-25 19:30:02.757439 clinica-0.8.0/clinica/pipelines/cli_param/option_group.py
--rw-r--r--   0        0        0       44 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/deeplearning_prepare_data/__init__.py
--rw-r--r--   0        0        0      584 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/deeplearning_prepare_data/deeplearning_prepare_data_cli.py
--rw-r--r--   0        0        0       45 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/__init__.py
--rw-r--r--   0        0        0       18 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/connectome/__init__.py
--rw-r--r--   0        0        0     1798 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/connectome/cli.py
--rw-r--r--   0        0        0      549 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/connectome/info.json
--rw-r--r--   0        0        0    23721 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/connectome/pipeline.py
--rw-r--r--   0        0        0     3939 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/connectome/utils.py
--rw-r--r--   0        0        0       18 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/dti/__init__.py
--rw-r--r--   0        0        0     1518 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/dti/cli.py
--rw-r--r--   0        0        0      523 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/dti/info.json
--rw-r--r--   0        0        0    21856 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/dti/pipeline.py
--rw-r--r--   0        0        0     1538 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/dti/tasks.py
--rw-r--r--   0        0        0     4700 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/dti/utils.py
--rw-r--r--   0        0        0       23 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/preprocessing/__init__.py
--rw-r--r--   0        0        0     1752 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/preprocessing/engine.py
--rw-r--r--   0        0        0       18 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/preprocessing/fmap/__init__.py
--rw-r--r--   0        0        0     2031 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/preprocessing/fmap/cli.py
--rw-r--r--   0        0        0      558 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/preprocessing/fmap/info.json
--rw-r--r--   0        0        0    16850 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/preprocessing/fmap/pipeline.py
--rw-r--r--   0        0        0     2583 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/preprocessing/fmap/tasks.py
--rw-r--r--   0        0        0    11217 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/preprocessing/fmap/utils.py
--rw-r--r--   0        0        0    20853 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/preprocessing/fmap/workflows.py
--rw-r--r--   0        0        0       18 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/preprocessing/t1/__init__.py
--rw-r--r--   0        0        0     2250 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/preprocessing/t1/cli.py
--rw-r--r--   0        0        0      693 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/preprocessing/t1/info.json
--rw-r--r--   0        0        0    15122 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/preprocessing/t1/pipeline.py
--rw-r--r--   0        0        0     3086 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/preprocessing/t1/tasks.py
--rw-r--r--   0        0        0    26157 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/preprocessing/t1/utils.py
--rw-r--r--   0        0        0    21662 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/preprocessing/t1/workflows.py
--rw-r--r--   0        0        0     1812 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/preprocessing/tasks.py
--rw-r--r--   0        0        0    10489 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/preprocessing/utils.py
--rw-r--r--   0        0        0     6907 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/preprocessing/workflows.py
--rw-r--r--   0        0        0     2445 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/dwi/utils.py
--rw-r--r--   0        0        0    32965 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/engine.py
--rw-r--r--   0        0        0       33 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/machine_learning/__init__.py
--rw-r--r--   0        0        0    48755 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/machine_learning/algorithm.py
--rw-r--r--   0        0        0     4219 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/machine_learning/base.py
--rw-r--r--   0        0        0     8371 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/machine_learning/classification_cli.py
--rw-r--r--   0        0        0    21613 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/machine_learning/input.py
--rw-r--r--   0        0        0     4103 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/machine_learning/ml_utils.py
--rw-r--r--   0        0        0    11503 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/machine_learning/ml_workflows.py
--rw-r--r--   0        0        0     2630 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/machine_learning/region_based_io.py
--rw-r--r--   0        0        0      934 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/machine_learning/tsv_based_io.py
--rw-r--r--   0        0        0    34650 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/machine_learning/validation.py
--rw-r--r--   0        0        0     1104 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/machine_learning/vertex_based_io.py
--rw-r--r--   0        0        0     2930 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/machine_learning/voxel_based_io.py
--rw-r--r--   0        0        0       30 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/machine_learning_spatial_svm/__init__.py
--rw-r--r--   0        0        0      190 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/machine_learning_spatial_svm/info.json
--rw-r--r--   0        0        0     3790 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_cli.py
--rw-r--r--   0        0        0    11930 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_pipeline.py
--rw-r--r--   0        0        0    27931 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_utils.py
--rw-r--r--   0        0        0       29 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/pet_linear/__init__.py
--rw-r--r--   0        0        0      283 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/pet_linear/info.json
--rw-r--r--   0        0        0     3065 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/pet_linear/pet_linear_cli.py
--rw-r--r--   0        0        0    19605 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/pet_linear/pet_linear_pipeline.py
--rw-r--r--   0        0        0     8904 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/pet_linear/pet_linear_utils.py
--rw-r--r--   0        0        0       60 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/pet_surface/__init__.py
--rw-r--r--   0        0        0     1050 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/pet_surface/applyInverseDeformationField.m
--rw-r--r--   0        0        0      549 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/pet_surface/info.json
--rw-r--r--   0        0        0     2673 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/pet_surface/pet_surface_cli.py
--rw-r--r--   0        0        0     2578 2024-03-25 19:30:02.761439 clinica-0.8.0/clinica/pipelines/pet_surface/pet_surface_longitudinal_cli.py
--rw-r--r--   0        0        0    16127 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/pet_surface/pet_surface_pipeline.py
--rw-r--r--   0        0        0    53041 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/pet_surface/pet_surface_utils.py
--rw-r--r--   0        0        0       29 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/pet_volume/__init__.py
--rw-r--r--   0        0        0      286 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/pet_volume/info.json
--rw-r--r--   0        0        0     4326 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/pet_volume/pet_volume_cli.py
--rw-r--r--   0        0        0    31184 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/pet_volume/pet_volume_pipeline.py
--rw-r--r--   0        0        0     7662 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/pet_volume/pet_volume_utils.py
--rw-r--r--   0        0        0       18 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_surface/__init__.py
--rw-r--r--   0        0        0    10409 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_surface/_utils.py
--rw-r--r--   0        0        0     5425 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_surface/cli.py
--rw-r--r--   0        0        0      346 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_surface/info.json
--rw-r--r--   0        0        0     9745 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_surface/pipeline.py
--rw-r--r--   0        0        0      173 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/__init__.py
--rw-r--r--   0        0        0     5435 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/_surfstat.py
--rw-r--r--   0        0        0     5161 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/_utils.py
--rw-r--r--   0        0        0      101 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/models/__init__.py
--rw-r--r--   0        0        0     7598 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/models/_base.py
--rw-r--r--   0        0        0     3329 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/models/_contrast.py
--rw-r--r--   0        0        0     1770 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/models/_correlation.py
--rw-r--r--   0        0        0     2897 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/models/_factory.py
--rw-r--r--   0        0        0     3526 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/models/_group.py
--rw-r--r--   0        0        0     3990 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/models/_utils.py
--rw-r--r--   0        0        0      246 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/models/results/__init__.py
--rw-r--r--   0        0        0     1962 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/models/results/_base.py
--rw-r--r--   0        0        0     2639 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/models/results/_plot.py
--rw-r--r--   0        0        0     3516 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/models/results/_serialize.py
--rw-r--r--   0        0        0     4780 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/models/results/_statistics.py
--rw-r--r--   0        0        0       36 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_volume/__init__.py
--rw-r--r--   0        0        0      287 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_volume/info.json
--rw-r--r--   0        0        0     5871 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_volume/statistics_volume_cli.py
--rw-r--r--   0        0        0    19061 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_volume/statistics_volume_pipeline.py
--rw-r--r--   0        0        0    34949 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_volume/statistics_volume_utils.py
--rw-r--r--   0        0        0      811 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_volume/template_model_contrast.m
--rw-r--r--   0        0        0     1106 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_volume/template_model_creation.m
--rw-r--r--   0        0        0      336 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_volume/template_model_estimation.m
--rw-r--r--   0        0        0      781 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_volume/template_model_results.m
--rw-r--r--   0        0        0       47 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_volume_correction/__init__.py
--rw-r--r--   0        0        0      180 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_volume_correction/info.json
--rw-r--r--   0        0        0     2633 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_cli.py
--rw-r--r--   0        0        0     9406 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_pipeline.py
--rw-r--r--   0        0        0     6317 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_utils.py
--rw-r--r--   0        0        0       32 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_freesurfer/__init__.py
--rw-r--r--   0        0        0      306 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_freesurfer/info.json
--rw-r--r--   0        0        0     2601 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_freesurfer/t1_freesurfer_cli.py
--rw-r--r--   0        0        0     9756 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_freesurfer/t1_freesurfer_pipeline.py
--rw-r--r--   0        0        0     4845 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_freesurfer/t1_freesurfer_utils.py
--rw-r--r--   0        0        0     5055 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_freesurfer/t1_freesurfer_visualizer.py
--rw-r--r--   0        0        0        0 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_freesurfer_atlas/__init__.py
--rw-r--r--   0        0        0      290 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_freesurfer_atlas/info.json
--rw-r--r--   0        0        0     7244 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_freesurfer_atlas/t1_freeesurfer_atlas_pipeline.py
--rw-r--r--   0        0        0     1181 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_freesurfer_atlas/t1_freesurfer_atlas_cli.py
--rw-r--r--   0        0        0     5242 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_freesurfer_atlas/t1_freesurfer_atlas_utils.py
--rw-r--r--   0        0        0      133 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_freesurfer_longitudinal/__init__.py
--rw-r--r--   0        0        0      324 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_freesurfer_longitudinal/info.json
--rw-r--r--   0        0        0     6126 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_freesurfer_longitudinal/longitudinal_utils.py
--rw-r--r--   0        0        0     2833 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_cli.py
--rw-r--r--   0        0        0     2091 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_cli.py
--rw-r--r--   0        0        0    11491 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_pipeline.py
--rw-r--r--   0        0        0    11905 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_utils.py
--rw-r--r--   0        0        0     1609 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_cli.py
--rw-r--r--   0        0        0    12260 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_pipeline.py
--rw-r--r--   0        0        0     8703 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_utils.py
--rw-r--r--   0        0        0       46 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_linear/__init__.py
--rw-r--r--   0        0        0    13679 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_linear/anat_linear_pipeline.py
--rw-r--r--   0        0        0     3522 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_linear/anat_linear_utils.py
--rw-r--r--   0        0        0     2148 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_linear/flair_linear_cli.py
--rw-r--r--   0        0        0      281 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_linear/info.json
--rw-r--r--   0        0        0     2137 2024-03-25 19:30:02.765439 clinica-0.8.0/clinica/pipelines/t1_linear/t1_linear_cli.py
--rw-r--r--   0        0        0       28 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume/__init__.py
--rw-r--r--   0        0        0      305 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume/info.json
--rw-r--r--   0        0        0     5055 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume/t1_volume_cli.py
--rw-r--r--   0        0        0       42 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_create_dartel/__init__.py
--rw-r--r--   0        0        0      300 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_create_dartel/info.json
--rw-r--r--   0        0        0     2110 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_create_dartel/t1_volume_create_dartel_cli.py
--rw-r--r--   0        0        0     9438 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_create_dartel/t1_volume_create_dartel_pipeline.py
--rw-r--r--   0        0        0       39 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_dartel2mni/__init__.py
--rw-r--r--   0        0        0      312 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_dartel2mni/info.json
--rw-r--r--   0        0        0     2407 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_dartel2mni/t1_volume_dartel2mni_cli.py
--rw-r--r--   0        0        0    13177 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_dartel2mni/t1_volume_dartel2mni_pipeline.py
--rw-r--r--   0        0        0      301 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_dartel2mni/t1_volume_dartel2mni_utils.py
--rw-r--r--   0        0        0       46 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_existing_template/__init__.py
--rw-r--r--   0        0        0      303 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_existing_template/info.json
--rw-r--r--   0        0        0     4524 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_existing_template/t1_volume_existing_template_cli.py
--rw-r--r--   0        0        0       41 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_parcellation/__init__.py
--rw-r--r--   0        0        0      178 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_parcellation/info.json
--rw-r--r--   0        0        0     1977 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_cli.py
--rw-r--r--   0        0        0     5735 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_pipeline.py
--rw-r--r--   0        0        0     1123 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_utils.py
--rw-r--r--   0        0        0       44 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_register_dartel/__init__.py
--rw-r--r--   0        0        0      301 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_register_dartel/info.json
--rw-r--r--   0        0        0     2093 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_cli.py
--rw-r--r--   0        0        0     8647 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_pipeline.py
--rw-r--r--   0        0        0     5603 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_utils.py
--rw-r--r--   0        0        0       48 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_tissue_segmentation/__init__.py
--rw-r--r--   0        0        0      343 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_tissue_segmentation/info.json
--rw-r--r--   0        0        0     2533 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_cli.py
--rw-r--r--   0        0        0    12806 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_pipeline.py
--rw-r--r--   0        0        0     5161 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_utils.py
--rw-r--r--   0        0        0      190 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/dwi/__init__.py
--rw-r--r--   0        0        0       94 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/dwi/_commons/__init__.py
--rw-r--r--   0        0        0      385 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/dwi/_commons/_tasks.py
--rw-r--r--   0        0        0     5110 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/dwi/_commons/_workflows.py
--rw-r--r--   0        0        0     5860 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/engine.py
--rw-r--r--   0        0        0     2583 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/engine_utils.py
--rw-r--r--   0        0        0     4943 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/interfaces.py
--rw-r--r--   0        0        0       30 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/machine_learning_spatial_svm/__init__.py
--rw-r--r--   0        0        0     4011 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/machine_learning_spatial_svm/pipeline.py
--rw-r--r--   0        0        0     3077 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/machine_learning_spatial_svm/spatial_svm_cli.py
--rw-r--r--   0        0        0     1731 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/machine_learning_spatial_svm/tasks.py
--rw-r--r--   0        0        0       29 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/pet_linear/__init__.py
--rw-r--r--   0        0        0     3020 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/pet_linear/pet_linear_cli.py
--rw-r--r--   0        0        0     6810 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/pet_linear/pipeline.py
--rw-r--r--   0        0        0     1718 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/pet_linear/tasks.py
--rw-r--r--   0        0        0       29 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/pet_volume/__init__.py
--rw-r--r--   0        0        0     3579 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/pet_volume/pet_volume_cli.py
--rw-r--r--   0        0        0    12200 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/pet_volume/pipeline.py
--rw-r--r--   0        0        0     4532 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/pet_volume/tasks.py
--rw-r--r--   0        0        0    11197 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/query.py
--rw-r--r--   0        0        0        0 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/shared_workflows/__init__.py
--rw-r--r--   0        0        0     1408 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/shared_workflows/smoothing.py
--rw-r--r--   0        0        0       36 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/statistics_volume/__init__.py
--rw-r--r--   0        0        0     7803 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/statistics_volume/pipeline.py
--rw-r--r--   0        0        0     4956 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/statistics_volume/statistics_volume_cli.py
--rw-r--r--   0        0        0     4336 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/statistics_volume/task.py
--rw-r--r--   0        0        0       47 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/statistics_volume_correction/__init__.py
--rw-r--r--   0        0        0     3211 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/statistics_volume_correction/pipeline.py
--rw-r--r--   0        0        0     2385 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/statistics_volume_correction/statistics_volume_correction_cli.py
--rw-r--r--   0        0        0     2441 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/statistics_volume_correction/task.py
--rw-r--r--   0        0        0       21 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/t1_freesurfer/__init__.py
--rw-r--r--   0        0        0      817 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/t1_freesurfer/cli.py
--rw-r--r--   0        0        0     2835 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/t1_freesurfer/pipeline.py
--rw-r--r--   0        0        0      886 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/t1_freesurfer/tasks.py
--rw-r--r--   0        0        0       28 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/t1_linear/__init__.py
--rw-r--r--   0        0        0     2769 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/t1_linear/t1_linear.py
--rw-r--r--   0        0        0     1339 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/t1_linear/t1_linear_cli.py
--rw-r--r--   0        0        0       78 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/t1_volume/__init__.py
--rw-r--r--   0        0        0       18 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/t1_volume/create_dartel/__init__.py
--rw-r--r--   0        0        0     1879 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/t1_volume/create_dartel/cli.py
--rw-r--r--   0        0        0     2301 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/t1_volume/create_dartel/pipeline.py
--rw-r--r--   0        0        0       18 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/t1_volume/dartel2mni/__init__.py
--rw-r--r--   0        0        0     1973 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/t1_volume/dartel2mni/cli.py
--rw-r--r--   0        0        0     3813 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/t1_volume/dartel2mni/pipeline.py
--rw-r--r--   0        0        0     2311 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/t1_volume/dartel2mni/tasks.py
--rw-r--r--   0        0        0       18 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/t1_volume/register_dartel/__init__.py
--rw-r--r--   0        0        0     2298 2024-03-25 19:30:02.769439 clinica-0.8.0/clinica/pydra/t1_volume/register_dartel/cli.py
--rw-r--r--   0        0        0     3964 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/pydra/t1_volume/register_dartel/pipeline.py
--rw-r--r--   0        0        0     2728 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/pydra/t1_volume/tasks.py
--rw-r--r--   0        0        0       18 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/pydra/t1_volume/tissue_segmentation/__init__.py
--rw-r--r--   0        0        0     2146 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/pydra/t1_volume/tissue_segmentation/cli.py
--rw-r--r--   0        0        0     2452 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/pydra/t1_volume/tissue_segmentation/pipeline.py
--rw-r--r--   0        0        0     1008 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/pydra/t1_volume/utils.py
--rw-r--r--   0        0        0     1377 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/pydra/tasks.py
--rw-r--r--   0        0        0     2628 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/pydra/utils.py
--rwxr-xr-x   0        0        0      966 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/atlases/atlas-AAL2.txt
--rw-r--r--   0        0        0    76312 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/atlases/atlas-AAL2_dseg.nii.gz
--rw-r--r--   0        0        0     2311 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/atlases/atlas-AAL2_dseg.tsv
--rwxr-xr-x   0        0        0     1779 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/atlases/atlas-AICHA.txt
--rw-r--r--   0        0        0    94631 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/atlases/atlas-AICHA_dseg.nii.gz
--rw-r--r--   0        0        0     8548 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/atlases/atlas-AICHA_dseg.tsv
--rw-r--r--   0        0        0     1873 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/atlases/atlas-Hammers_dseg.tsv
--rw-r--r--   0        0        0     1916 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/atlases/atlas-JHUDTI81_dseg.tsv
--rw-r--r--   0        0        0      684 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/atlases/atlas-JHUTract_dseg.tsv
--rw-r--r--   0        0        0     1535 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/atlases/atlas-LPBA40_dseg.tsv
--rw-r--r--   0        0        0     4151 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/atlases/atlas-Neuromorphometrics_dseg.tsv
--rw-r--r--   0        0        0      146 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/fmri/task-facesshapesemotion_events.tsv
--rw-r--r--   0        0        0     3872 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/label_conversion_gtmsegmentation.csv
--rw-r--r--   0        0        0        0 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/mappings/.emptyfile
--rw-r--r--   0        0        0     2661 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/masks/region-cerebellumPons_eroded-6mm_mask.nii.gz
--rw-r--r--   0        0        0     7028 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/masks/region-cerebellumPons_remove-extrabrain_eroded-3it_mask.nii.gz
--rw-r--r--   0        0        0     1194 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/masks/region-pons_eroded-6mm_mask.nii.gz
--rw-r--r--   0        0        0     4418 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/masks/region-pons_remove-extrabrain_eroded-2it_mask.nii.gz
--rw-r--r--   0        0        0     2774 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/templates/pipeline_template/README.md.j2
--rw-r--r--   0        0        0        0 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/templates/pipeline_template/__init__.py.j2
--rw-r--r--   0        0        0     2622 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/templates/pipeline_template/cli.py.j2
--rw-r--r--   0        0        0      295 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/templates/pipeline_template/info.json.j2
--rw-r--r--   0        0        0     5460 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/templates/pipeline_template/pipeline.py.j2
--rw-r--r--   0        0        0      713 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/templates/pipeline_template/utils.py.j2
--rw-r--r--   0        0        0      258 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/resources/templates/pipeline_template/visualizer.py.j2
--rw-r--r--   0        0        0        0 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/utils/__init__.py
--rw-r--r--   0        0        0    15002 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/utils/atlas.py
--rw-r--r--   0        0        0     5247 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/utils/bids.py
--rw-r--r--   0        0        0    11637 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/utils/check_dependency.py
--rw-r--r--   0        0        0     1438 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/utils/exceptions.py
--rw-r--r--   0        0        0    20324 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/utils/filemanip.py
--rw-r--r--   0        0        0    14440 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/utils/freesurfer.py
--rw-r--r--   0        0        0     2286 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/utils/group.py
--rw-r--r--   0        0        0     5552 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/utils/image.py
--rw-r--r--   0        0        0    24818 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/utils/input_files.py
--rw-r--r--   0        0        0    33603 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/utils/inputs.py
--rw-r--r--   0        0        0     4686 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/utils/longitudinal.py
--rw-r--r--   0        0        0     1585 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/utils/mri_registration.py
--rw-r--r--   0        0        0     1643 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/utils/nipype.py
--rw-r--r--   0        0        0     6337 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/utils/participant.py
--rw-r--r--   0        0        0     5995 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/utils/pet.py
--rw-r--r--   0        0        0     3626 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/utils/spm.py
--rw-r--r--   0        0        0     2828 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/utils/statistics.py
--rw-r--r--   0        0        0     1035 2024-03-25 19:30:02.773439 clinica-0.8.0/clinica/utils/stream.py
--rw-r--r--   0        0        0    12019 2024-03-25 19:30:02.777439 clinica-0.8.0/clinica/utils/testing_utils.py
--rw-r--r--   0        0        0     5537 2024-03-25 19:30:02.777439 clinica-0.8.0/clinica/utils/ux.py
--rw-r--r--   0        0        0     2399 2024-03-25 19:30:02.797439 clinica-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    11110 1970-01-01 00:00:00.000000 clinica-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11842 2024-04-25 06:57:47.702103 clinica-0.8.1/LICENSE.txt
+-rw-r--r--   0        0        0     8791 2024-04-25 06:57:47.702103 clinica-0.8.1/README.md
+-rw-r--r--   0        0        0      175 2024-04-25 06:57:47.702103 clinica-0.8.1/clinica/__init__.py
+-rw-r--r--   0        0        0     3020 2024-04-25 06:57:47.702103 clinica-0.8.1/clinica/cmdline.py
+-rw-r--r--   0        0        0       67 2024-04-25 06:57:47.702103 clinica-0.8.1/clinica/compat.py
+-rw-r--r--   0        0        0       33 2024-04-25 06:57:47.702103 clinica-0.8.1/clinica/engine/__init__.py
+-rw-r--r--   0        0        0     5730 2024-04-25 06:57:47.702103 clinica-0.8.1/clinica/engine/cmdparser.py
+-rw-r--r--   0        0        0     1908 2024-04-25 06:57:47.702103 clinica-0.8.1/clinica/engine/template.py
+-rw-r--r--   0        0        0        0 2024-04-25 06:57:47.702103 clinica-0.8.1/clinica/iotools/__init__.py
+-rw-r--r--   0        0        0      225 2024-04-25 06:57:47.702103 clinica-0.8.1/clinica/iotools/abstract_converter.py
+-rw-r--r--   0        0        0     1405 2024-04-25 06:57:47.702103 clinica-0.8.1/clinica/iotools/bids_dataset_description.py
+-rw-r--r--   0        0        0      636 2024-04-25 06:57:47.702103 clinica-0.8.1/clinica/iotools/bids_readme.py
+-rw-r--r--   0        0        0    33186 2024-04-25 06:57:47.702103 clinica-0.8.1/clinica/iotools/bids_utils.py
+-rw-r--r--   0        0        0    11818 2024-04-25 06:57:47.702103 clinica-0.8.1/clinica/iotools/converter_utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 06:57:47.702103 clinica-0.8.1/clinica/iotools/converters/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 06:57:47.702103 clinica-0.8.1/clinica/iotools/converters/adni_to_bids/__init__.py
+-rw-r--r--   0        0        0    20529 2024-04-25 06:57:47.702103 clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_json.py
+-rw-r--r--   0        0        0        0 2024-04-25 06:57:47.702103 clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_modalities/__init__.py
+-rw-r--r--   0        0        0     5278 2024-04-25 06:57:47.702103 clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_av45_fbb_pet.py
+-rw-r--r--   0        0        0     9191 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_dwi.py
+-rw-r--r--   0        0        0    10401 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_fdg_pet.py
+-rw-r--r--   0        0        0     7452 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_flair.py
+-rw-r--r--   0        0        0     8072 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_fmri.py
+-rw-r--r--   0        0        0     4507 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_pib_pet.py
+-rw-r--r--   0        0        0    21003 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_t1.py
+-rw-r--r--   0        0        0     4941 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_tau_pet.py
+-rw-r--r--   0        0        0    10543 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_to_bids.py
+-rw-r--r--   0        0        0     2542 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_to_bids_cli.py
+-rw-r--r--   0        0        0    55526 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/aibl_to_bids/__init__.py
+-rw-r--r--   0        0        0     5381 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/aibl_to_bids/aibl_to_bids.py
+-rw-r--r--   0        0        0     1203 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/aibl_to_bids/aibl_to_bids_cli.py
+-rw-r--r--   0        0        0      354 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/aibl_to_bids/utils/__init__.py
+-rw-r--r--   0        0        0    22165 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/aibl_to_bids/utils/bids.py
+-rw-r--r--   0        0        0    14678 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/aibl_to_bids/utils/clinical.py
+-rw-r--r--   0        0        0      833 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/cli.py
+-rw-r--r--   0        0        0      875 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/cli_param.py
+-rw-r--r--   0        0        0     5053 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/genfi_to_bids/genfi_to_bids.py
+-rw-r--r--   0        0        0     1884 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/genfi_to_bids/genfi_to_bids_cli.py
+-rw-r--r--   0        0        0    33214 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/genfi_to_bids/genfi_to_bids_utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/habs_to_bids/__init__.py
+-rw-r--r--   0        0        0     9029 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/habs_to_bids/habs_to_bids.py
+-rw-r--r--   0        0        0     1040 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/habs_to_bids/habs_to_bids_cli.py
+-rw-r--r--   0        0        0        0 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/nifd_to_bids/__init__.py
+-rw-r--r--   0        0        0     1840 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/nifd_to_bids/nifd_to_bids.py
+-rw-r--r--   0        0        0     1014 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/nifd_to_bids/nifd_to_bids_cli.py
+-rw-r--r--   0        0        0    12134 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/nifd_to_bids/nifd_utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/oasis3_to_bids/__init__.py
+-rw-r--r--   0        0        0     2509 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/oasis3_to_bids/oasis3_to_bids.py
+-rw-r--r--   0        0        0      885 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/oasis3_to_bids/oasis3_to_bids_cli.py
+-rw-r--r--   0        0        0    11900 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/oasis3_to_bids/oasis3_utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/oasis_to_bids/__init__.py
+-rw-r--r--   0        0        0     7519 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/oasis_to_bids/oasis_to_bids.py
+-rw-r--r--   0        0        0     1000 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/oasis_to_bids/oasis_to_bids_cli.py
+-rw-r--r--   0        0        0        0 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/ukb_to_bids/__init__.py
+-rw-r--r--   0        0        0     2094 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/ukb_to_bids/ukb_to_bids.py
+-rw-r--r--   0        0        0     1086 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/ukb_to_bids/ukb_to_bids_cli.py
+-rw-r--r--   0        0        0    16777 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/converters/ukb_to_bids/ukb_utils.py
+-rw-r--r--   0        0        0     2383 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/data/clinical_specifications_adni_participant.tsv
+-rw-r--r--   0        0        0      244 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/data/clinical_specifications_adni_scans.tsv
+-rw-r--r--   0        0        0    89321 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/data/clinical_specifications_adni_sessions.tsv
+-rw-r--r--   0        0        0     2708 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/data/clinical_specifications_participant.tsv
+-rw-r--r--   0        0        0     1136 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/data/clinical_specifications_scans.tsv
+-rw-r--r--   0        0        0    32532 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/data/clinical_specifications_sessions.tsv
+-rw-r--r--   0        0        0    10872 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/data/genfi_data.tsv
+-rw-r--r--   0        0        0    16189 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/data/genfi_data_mapping.tsv
+-rw-r--r--   0        0        0     7777 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/data/genfi_ref.csv
+-rw-r--r--   0        0        0      271 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/data/modality_equiv.tsv
+-rw-r--r--   0        0        0      243 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/data/ukb_ref.csv
+-rw-r--r--   0        0        0        0 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/utils/__init__.py
+-rw-r--r--   0        0        0     8809 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/utils/cli.py
+-rw-r--r--   0        0        0    56731 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/utils/data_handling.py
+-rw-r--r--   0        0        0    14183 2024-04-25 06:57:47.706103 clinica-0.8.1/clinica/iotools/utils/pipeline_handling.py
+-rw-r--r--   0        0        0        0 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@random/char.m
+-rw-r--r--   0        0        0      465 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@random/display.m
+-rw-r--r--   0        0        0       67 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@random/double.m
+-rw-r--r--   0        0        0     1135 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@random/image.m
+-rw-r--r--   0        0        0       76 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@random/isempty.m
+-rw-r--r--   0        0        0      671 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@random/minus.m
+-rw-r--r--   0        0        0       85 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@random/mpower.m
+-rw-r--r--   0        0        0     1873 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@random/mtimes.m
+-rw-r--r--   0        0        0      732 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@random/plus.m
+-rw-r--r--   0        0        0     5850 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@random/random.m
+-rw-r--r--   0        0        0       92 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@random/size.m
+-rw-r--r--   0        0        0       46 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@random/subsref.m
+-rw-r--r--   0        0        0       30 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@term/char.m
+-rw-r--r--   0        0        0      315 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@term/display.m
+-rw-r--r--   0        0        0       33 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@term/double.m
+-rw-r--r--   0        0        0      574 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@term/image.m
+-rw-r--r--   0        0        0       43 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@term/isempty.m
+-rw-r--r--   0        0        0      694 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@term/minus.m
+-rw-r--r--   0        0        0      116 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@term/mpower.m
+-rw-r--r--   0        0        0     1166 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@term/mtimes.m
+-rw-r--r--   0        0        0      828 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@term/plus.m
+-rw-r--r--   0        0        0       97 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@term/size.m
+-rw-r--r--   0        0        0      178 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@term/subsref.m
+-rw-r--r--   0        0        0     3878 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@term/term.m
+-rw-r--r--   0        0        0      102 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/I.m
+-rw-r--r--   0        0        0     1340 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatAvSurf.m
+-rw-r--r--   0        0        0     1662 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatAvVol.m
+-rw-r--r--   0        0        0      750 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatColLim.m
+-rw-r--r--   0        0        0      567 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatColormap.m
+-rw-r--r--   0        0        0     1491 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatCoord2Ind.m
+-rw-r--r--   0        0        0      497 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatDataCursor.m
+-rw-r--r--   0        0        0      692 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatDataCursorP.m
+-rw-r--r--   0        0        0      636 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatDataCursorQ.m
+-rw-r--r--   0        0        0     2172 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatDelete.m
+-rw-r--r--   0        0        0     2384 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatEdg.m
+-rw-r--r--   0        0        0     3989 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatF.m
+-rw-r--r--   0        0        0     1099 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatInd2Coord.m
+-rw-r--r--   0        0        0     2615 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatInflate.m
+-rw-r--r--   0        0        0    10279 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatLinMod.m
+-rw-r--r--   0        0        0      946 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatListDir.m
+-rw-r--r--   0        0        0      995 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatMaskCut.m
+-rw-r--r--   0        0        0     1925 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatNorm.m
+-rw-r--r--   0        0        0     3891 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatP.m
+-rw-r--r--   0        0        0     4053 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatPCA.m
+-rw-r--r--   0        0        0     4282 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatPeakClus.m
+-rw-r--r--   0        0        0     4388 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatPlot.m
+-rw-r--r--   0        0        0     1687 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatQ.m
+-rw-r--r--   0        0        0     1448 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatROI.m
+-rw-r--r--   0        0        0     3855 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadData.m
+-rw-r--r--   0        0        0     1599 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadData1.m
+-rw-r--r--   0        0        0     4371 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadSurf.m
+-rw-r--r--   0        0        0     6091 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadSurf1.m
+-rw-r--r--   0        0        0     5816 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadVol.m
+-rw-r--r--   0        0        0    17058 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadVol1.m
+-rw-r--r--   0        0        0    17594 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatResels.m
+-rw-r--r--   0        0        0     2202 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatSmooth.m
+-rw-r--r--   0        0        0      860 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatStand.m
+-rw-r--r--   0        0        0     3190 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatSurf2Vol.m
+-rw-r--r--   0        0        0     5852 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatT.m
+-rw-r--r--   0        0        0     5335 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatView.m
+-rw-r--r--   0        0        0    11047 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatView1.m
+-rw-r--r--   0        0        0     7015 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatViewData.m
+-rw-r--r--   0        0        0     7036 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatViewData_backup.m
+-rw-r--r--   0        0        0     6798 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatView_backup.m
+-rw-r--r--   0        0        0     2751 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatViews.m
+-rw-r--r--   0        0        0     1976 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatVol2Surf.m
+-rw-r--r--   0        0        0     1196 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteData.m
+-rw-r--r--   0        0        0     2395 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteSurf.m
+-rw-r--r--   0        0        0     3385 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteSurf1.m
+-rw-r--r--   0        0        0     1231 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteVol.m
+-rw-r--r--   0        0        0    19785 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteVol1.m
+-rw-r--r--   0        0        0      470 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/fac2var.m
+-rw-r--r--   0        0        0     1588 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/gl.m
+-rw-r--r--   0        0        0     1404 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/icbm_template_2.00mm+orig.HEAD
+-rw-r--r--   0        0        0      348 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/icbm_template_2.00mm.hdr
+-rw-r--r--   0        0        0     4096 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/icbm_template_2.00mm.mnc
+-rw-r--r--   0        0        0     2021 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/redmod.m
+-rw-r--r--   0        0        0      996 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/spectral.m
+-rw-r--r--   0        0        0    27286 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/stat_threshold.m
+-rw-r--r--   0        0        0      836 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/var2fac.m
+-rwxr-xr-x   0        0        0    25158 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/lib/clinicasurfstat/clinicasurfstat.m
+-rw-r--r--   0        0        0      886 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/option.py
+-rw-r--r--   0        0        0      536 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/pipelines/__init__.py
+-rw-r--r--   0        0        0      369 2024-04-25 06:57:47.710103 clinica-0.8.1/clinica/pipelines/cli.py
+-rw-r--r--   0        0        0       45 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/cli_param/__init__.py
+-rw-r--r--   0        0        0     1362 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/cli_param/argument.py
+-rw-r--r--   0        0        0     5474 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/cli_param/option.py
+-rw-r--r--   0        0        0      538 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/cli_param/option_group.py
+-rw-r--r--   0        0        0       44 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/deeplearning_prepare_data/__init__.py
+-rw-r--r--   0        0        0      584 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/deeplearning_prepare_data/deeplearning_prepare_data_cli.py
+-rw-r--r--   0        0        0       45 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/connectome/__init__.py
+-rw-r--r--   0        0        0     1798 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/connectome/cli.py
+-rw-r--r--   0        0        0      549 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/connectome/info.json
+-rw-r--r--   0        0        0    23721 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/connectome/pipeline.py
+-rw-r--r--   0        0        0     3939 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/connectome/utils.py
+-rw-r--r--   0        0        0       18 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/dti/__init__.py
+-rw-r--r--   0        0        0     1518 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/dti/cli.py
+-rw-r--r--   0        0        0      523 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/dti/info.json
+-rw-r--r--   0        0        0    21856 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/dti/pipeline.py
+-rw-r--r--   0        0        0     1538 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/dti/tasks.py
+-rw-r--r--   0        0        0     4700 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/dti/utils.py
+-rw-r--r--   0        0        0       23 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/preprocessing/__init__.py
+-rw-r--r--   0        0        0     1752 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/preprocessing/engine.py
+-rw-r--r--   0        0        0       18 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/preprocessing/fmap/__init__.py
+-rw-r--r--   0        0        0     2031 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/preprocessing/fmap/cli.py
+-rw-r--r--   0        0        0      558 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/preprocessing/fmap/info.json
+-rw-r--r--   0        0        0    16850 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/preprocessing/fmap/pipeline.py
+-rw-r--r--   0        0        0     2583 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/preprocessing/fmap/tasks.py
+-rw-r--r--   0        0        0    11217 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/preprocessing/fmap/utils.py
+-rw-r--r--   0        0        0    20853 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/preprocessing/fmap/workflows.py
+-rw-r--r--   0        0        0       18 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/preprocessing/t1/__init__.py
+-rw-r--r--   0        0        0     2250 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/preprocessing/t1/cli.py
+-rw-r--r--   0        0        0      693 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/preprocessing/t1/info.json
+-rw-r--r--   0        0        0    15113 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/preprocessing/t1/pipeline.py
+-rw-r--r--   0        0        0     3086 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/preprocessing/t1/tasks.py
+-rw-r--r--   0        0        0    26157 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/preprocessing/t1/utils.py
+-rw-r--r--   0        0        0    21662 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/preprocessing/t1/workflows.py
+-rw-r--r--   0        0        0     1812 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/preprocessing/tasks.py
+-rw-r--r--   0        0        0    10489 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/preprocessing/utils.py
+-rw-r--r--   0        0        0     6907 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/preprocessing/workflows.py
+-rw-r--r--   0        0        0     2445 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/dwi/utils.py
+-rw-r--r--   0        0        0    32965 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/engine.py
+-rw-r--r--   0        0        0       33 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/machine_learning/__init__.py
+-rw-r--r--   0        0        0    48755 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/machine_learning/algorithm.py
+-rw-r--r--   0        0        0     4219 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/machine_learning/base.py
+-rw-r--r--   0        0        0     8371 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/machine_learning/classification_cli.py
+-rw-r--r--   0        0        0    21613 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/machine_learning/input.py
+-rw-r--r--   0        0        0     4103 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/machine_learning/ml_utils.py
+-rw-r--r--   0        0        0    11503 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/machine_learning/ml_workflows.py
+-rw-r--r--   0        0        0     2630 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/machine_learning/region_based_io.py
+-rw-r--r--   0        0        0      934 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/machine_learning/tsv_based_io.py
+-rw-r--r--   0        0        0    34650 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/machine_learning/validation.py
+-rw-r--r--   0        0        0     1104 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/machine_learning/vertex_based_io.py
+-rw-r--r--   0        0        0     2930 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/machine_learning/voxel_based_io.py
+-rw-r--r--   0        0        0       30 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/machine_learning_spatial_svm/__init__.py
+-rw-r--r--   0        0        0      190 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/machine_learning_spatial_svm/info.json
+-rw-r--r--   0        0        0     3790 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_cli.py
+-rw-r--r--   0        0        0    11930 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_pipeline.py
+-rw-r--r--   0        0        0    27931 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_utils.py
+-rw-r--r--   0        0        0       29 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/pet_linear/__init__.py
+-rw-r--r--   0        0        0      283 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/pet_linear/info.json
+-rw-r--r--   0        0        0     3065 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/pet_linear/pet_linear_cli.py
+-rw-r--r--   0        0        0    19605 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/pet_linear/pet_linear_pipeline.py
+-rw-r--r--   0        0        0     8904 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/pet_linear/pet_linear_utils.py
+-rw-r--r--   0        0        0       60 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/pet_surface/__init__.py
+-rw-r--r--   0        0        0     1050 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/pet_surface/applyInverseDeformationField.m
+-rw-r--r--   0        0        0      549 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/pet_surface/info.json
+-rw-r--r--   0        0        0     2673 2024-04-25 06:57:47.714103 clinica-0.8.1/clinica/pipelines/pet_surface/pet_surface_cli.py
+-rw-r--r--   0        0        0     2578 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/pet_surface/pet_surface_longitudinal_cli.py
+-rw-r--r--   0        0        0    16127 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/pet_surface/pet_surface_pipeline.py
+-rw-r--r--   0        0        0    53041 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/pet_surface/pet_surface_utils.py
+-rw-r--r--   0        0        0       29 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/pet_volume/__init__.py
+-rw-r--r--   0        0        0      286 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/pet_volume/info.json
+-rw-r--r--   0        0        0     4326 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/pet_volume/pet_volume_cli.py
+-rw-r--r--   0        0        0    31184 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/pet_volume/pet_volume_pipeline.py
+-rw-r--r--   0        0        0     7662 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/pet_volume/pet_volume_utils.py
+-rw-r--r--   0        0        0       18 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_surface/__init__.py
+-rw-r--r--   0        0        0    10409 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_surface/_utils.py
+-rw-r--r--   0        0        0     5425 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_surface/cli.py
+-rw-r--r--   0        0        0      346 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_surface/info.json
+-rw-r--r--   0        0        0     9745 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_surface/pipeline.py
+-rw-r--r--   0        0        0      173 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/__init__.py
+-rw-r--r--   0        0        0     5435 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/_surfstat.py
+-rw-r--r--   0        0        0     5161 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/_utils.py
+-rw-r--r--   0        0        0      101 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/models/__init__.py
+-rw-r--r--   0        0        0     7598 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/models/_base.py
+-rw-r--r--   0        0        0     3329 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/models/_contrast.py
+-rw-r--r--   0        0        0     1770 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/models/_correlation.py
+-rw-r--r--   0        0        0     2897 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/models/_factory.py
+-rw-r--r--   0        0        0     3526 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/models/_group.py
+-rw-r--r--   0        0        0     3990 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/models/_utils.py
+-rw-r--r--   0        0        0      246 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/models/results/__init__.py
+-rw-r--r--   0        0        0     1962 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/models/results/_base.py
+-rw-r--r--   0        0        0     2639 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/models/results/_plot.py
+-rw-r--r--   0        0        0     3516 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/models/results/_serialize.py
+-rw-r--r--   0        0        0     4780 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/models/results/_statistics.py
+-rw-r--r--   0        0        0       36 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_volume/__init__.py
+-rw-r--r--   0        0        0      287 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_volume/info.json
+-rw-r--r--   0        0        0     5871 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_volume/statistics_volume_cli.py
+-rw-r--r--   0        0        0    19061 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_volume/statistics_volume_pipeline.py
+-rw-r--r--   0        0        0    34949 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_volume/statistics_volume_utils.py
+-rw-r--r--   0        0        0      811 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_volume/template_model_contrast.m
+-rw-r--r--   0        0        0     1106 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_volume/template_model_creation.m
+-rw-r--r--   0        0        0      336 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_volume/template_model_estimation.m
+-rw-r--r--   0        0        0      781 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_volume/template_model_results.m
+-rw-r--r--   0        0        0       47 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_volume_correction/__init__.py
+-rw-r--r--   0        0        0      180 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_volume_correction/info.json
+-rw-r--r--   0        0        0     2633 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_cli.py
+-rw-r--r--   0        0        0     9406 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_pipeline.py
+-rw-r--r--   0        0        0     6317 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_utils.py
+-rw-r--r--   0        0        0       32 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_freesurfer/__init__.py
+-rw-r--r--   0        0        0      306 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_freesurfer/info.json
+-rw-r--r--   0        0        0     2601 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_freesurfer/t1_freesurfer_cli.py
+-rw-r--r--   0        0        0     9756 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_freesurfer/t1_freesurfer_pipeline.py
+-rw-r--r--   0        0        0     4845 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_freesurfer/t1_freesurfer_utils.py
+-rw-r--r--   0        0        0     5055 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_freesurfer/t1_freesurfer_visualizer.py
+-rw-r--r--   0        0        0        0 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_freesurfer_atlas/__init__.py
+-rw-r--r--   0        0        0      290 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_freesurfer_atlas/info.json
+-rw-r--r--   0        0        0     7244 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_freesurfer_atlas/t1_freeesurfer_atlas_pipeline.py
+-rw-r--r--   0        0        0     1181 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_freesurfer_atlas/t1_freesurfer_atlas_cli.py
+-rw-r--r--   0        0        0     5242 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_freesurfer_atlas/t1_freesurfer_atlas_utils.py
+-rw-r--r--   0        0        0      133 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_freesurfer_longitudinal/__init__.py
+-rw-r--r--   0        0        0      324 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_freesurfer_longitudinal/info.json
+-rw-r--r--   0        0        0     6126 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_freesurfer_longitudinal/longitudinal_utils.py
+-rw-r--r--   0        0        0     2833 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_cli.py
+-rw-r--r--   0        0        0     2091 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_cli.py
+-rw-r--r--   0        0        0    11491 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_pipeline.py
+-rw-r--r--   0        0        0    11905 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_utils.py
+-rw-r--r--   0        0        0     1609 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_cli.py
+-rw-r--r--   0        0        0    12260 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_pipeline.py
+-rw-r--r--   0        0        0     8703 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_utils.py
+-rw-r--r--   0        0        0       46 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_linear/__init__.py
+-rw-r--r--   0        0        0    13679 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_linear/anat_linear_pipeline.py
+-rw-r--r--   0        0        0     3522 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_linear/anat_linear_utils.py
+-rw-r--r--   0        0        0     2148 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_linear/flair_linear_cli.py
+-rw-r--r--   0        0        0      281 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_linear/info.json
+-rw-r--r--   0        0        0     2137 2024-04-25 06:57:47.718103 clinica-0.8.1/clinica/pipelines/t1_linear/t1_linear_cli.py
+-rw-r--r--   0        0        0       28 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume/__init__.py
+-rw-r--r--   0        0        0      305 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume/info.json
+-rw-r--r--   0        0        0     5055 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume/t1_volume_cli.py
+-rw-r--r--   0        0        0       42 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_create_dartel/__init__.py
+-rw-r--r--   0        0        0      300 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_create_dartel/info.json
+-rw-r--r--   0        0        0     2110 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_create_dartel/t1_volume_create_dartel_cli.py
+-rw-r--r--   0        0        0     9438 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_create_dartel/t1_volume_create_dartel_pipeline.py
+-rw-r--r--   0        0        0       39 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_dartel2mni/__init__.py
+-rw-r--r--   0        0        0      312 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_dartel2mni/info.json
+-rw-r--r--   0        0        0     2407 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_dartel2mni/t1_volume_dartel2mni_cli.py
+-rw-r--r--   0        0        0    13177 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_dartel2mni/t1_volume_dartel2mni_pipeline.py
+-rw-r--r--   0        0        0      301 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_dartel2mni/t1_volume_dartel2mni_utils.py
+-rw-r--r--   0        0        0       46 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_existing_template/__init__.py
+-rw-r--r--   0        0        0      303 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_existing_template/info.json
+-rw-r--r--   0        0        0     4524 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_existing_template/t1_volume_existing_template_cli.py
+-rw-r--r--   0        0        0       41 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_parcellation/__init__.py
+-rw-r--r--   0        0        0      178 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_parcellation/info.json
+-rw-r--r--   0        0        0     1977 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_cli.py
+-rw-r--r--   0        0        0     5735 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_pipeline.py
+-rw-r--r--   0        0        0     1123 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_utils.py
+-rw-r--r--   0        0        0       44 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_register_dartel/__init__.py
+-rw-r--r--   0        0        0      301 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_register_dartel/info.json
+-rw-r--r--   0        0        0     2093 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_cli.py
+-rw-r--r--   0        0        0     8647 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_pipeline.py
+-rw-r--r--   0        0        0     5603 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_utils.py
+-rw-r--r--   0        0        0       48 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_tissue_segmentation/__init__.py
+-rw-r--r--   0        0        0      343 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_tissue_segmentation/info.json
+-rw-r--r--   0        0        0     2533 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_cli.py
+-rw-r--r--   0        0        0    12806 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_pipeline.py
+-rw-r--r--   0        0        0     5161 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_utils.py
+-rw-r--r--   0        0        0      190 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/dwi/__init__.py
+-rw-r--r--   0        0        0       94 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/dwi/_commons/__init__.py
+-rw-r--r--   0        0        0      385 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/dwi/_commons/_tasks.py
+-rw-r--r--   0        0        0     5110 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/dwi/_commons/_workflows.py
+-rw-r--r--   0        0        0     5860 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/engine.py
+-rw-r--r--   0        0        0     2583 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/engine_utils.py
+-rw-r--r--   0        0        0     4943 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/interfaces.py
+-rw-r--r--   0        0        0       30 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/machine_learning_spatial_svm/__init__.py
+-rw-r--r--   0        0        0     4011 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/machine_learning_spatial_svm/pipeline.py
+-rw-r--r--   0        0        0     3077 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/machine_learning_spatial_svm/spatial_svm_cli.py
+-rw-r--r--   0        0        0     1731 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/machine_learning_spatial_svm/tasks.py
+-rw-r--r--   0        0        0       29 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/pet_linear/__init__.py
+-rw-r--r--   0        0        0     3020 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/pet_linear/pet_linear_cli.py
+-rw-r--r--   0        0        0     6810 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/pet_linear/pipeline.py
+-rw-r--r--   0        0        0     1718 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/pet_linear/tasks.py
+-rw-r--r--   0        0        0       29 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/pet_volume/__init__.py
+-rw-r--r--   0        0        0     3579 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/pet_volume/pet_volume_cli.py
+-rw-r--r--   0        0        0    12200 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/pet_volume/pipeline.py
+-rw-r--r--   0        0        0     4532 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/pet_volume/tasks.py
+-rw-r--r--   0        0        0    11197 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/query.py
+-rw-r--r--   0        0        0        0 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/shared_workflows/__init__.py
+-rw-r--r--   0        0        0     1408 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/shared_workflows/smoothing.py
+-rw-r--r--   0        0        0       36 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/statistics_volume/__init__.py
+-rw-r--r--   0        0        0     7803 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/statistics_volume/pipeline.py
+-rw-r--r--   0        0        0     4956 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/statistics_volume/statistics_volume_cli.py
+-rw-r--r--   0        0        0     4336 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/statistics_volume/task.py
+-rw-r--r--   0        0        0       47 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/statistics_volume_correction/__init__.py
+-rw-r--r--   0        0        0     3211 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/statistics_volume_correction/pipeline.py
+-rw-r--r--   0        0        0     2385 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/statistics_volume_correction/statistics_volume_correction_cli.py
+-rw-r--r--   0        0        0     2441 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/statistics_volume_correction/task.py
+-rw-r--r--   0        0        0       21 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/t1_freesurfer/__init__.py
+-rw-r--r--   0        0        0      817 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/t1_freesurfer/cli.py
+-rw-r--r--   0        0        0     2835 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/t1_freesurfer/pipeline.py
+-rw-r--r--   0        0        0      886 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/t1_freesurfer/tasks.py
+-rw-r--r--   0        0        0       28 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/t1_linear/__init__.py
+-rw-r--r--   0        0        0     2769 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/t1_linear/t1_linear.py
+-rw-r--r--   0        0        0     1339 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/t1_linear/t1_linear_cli.py
+-rw-r--r--   0        0        0       78 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/t1_volume/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/t1_volume/create_dartel/__init__.py
+-rw-r--r--   0        0        0     1879 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/t1_volume/create_dartel/cli.py
+-rw-r--r--   0        0        0     2301 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/t1_volume/create_dartel/pipeline.py
+-rw-r--r--   0        0        0       18 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/t1_volume/dartel2mni/__init__.py
+-rw-r--r--   0        0        0     1973 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/t1_volume/dartel2mni/cli.py
+-rw-r--r--   0        0        0     3813 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/t1_volume/dartel2mni/pipeline.py
+-rw-r--r--   0        0        0     2311 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/t1_volume/dartel2mni/tasks.py
+-rw-r--r--   0        0        0       18 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/t1_volume/register_dartel/__init__.py
+-rw-r--r--   0        0        0     2298 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/t1_volume/register_dartel/cli.py
+-rw-r--r--   0        0        0     3964 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/t1_volume/register_dartel/pipeline.py
+-rw-r--r--   0        0        0     2728 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/t1_volume/tasks.py
+-rw-r--r--   0        0        0       18 2024-04-25 06:57:47.722103 clinica-0.8.1/clinica/pydra/t1_volume/tissue_segmentation/__init__.py
+-rw-r--r--   0        0        0     2146 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/pydra/t1_volume/tissue_segmentation/cli.py
+-rw-r--r--   0        0        0     2452 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/pydra/t1_volume/tissue_segmentation/pipeline.py
+-rw-r--r--   0        0        0     1008 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/pydra/t1_volume/utils.py
+-rw-r--r--   0        0        0     1377 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/pydra/tasks.py
+-rw-r--r--   0        0        0     2628 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/pydra/utils.py
+-rwxr-xr-x   0        0        0      966 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/atlases/atlas-AAL2.txt
+-rw-r--r--   0        0        0    76312 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/atlases/atlas-AAL2_dseg.nii.gz
+-rw-r--r--   0        0        0     2311 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/atlases/atlas-AAL2_dseg.tsv
+-rwxr-xr-x   0        0        0     1779 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/atlases/atlas-AICHA.txt
+-rw-r--r--   0        0        0    94631 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/atlases/atlas-AICHA_dseg.nii.gz
+-rw-r--r--   0        0        0     8548 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/atlases/atlas-AICHA_dseg.tsv
+-rw-r--r--   0        0        0     1873 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/atlases/atlas-Hammers_dseg.tsv
+-rw-r--r--   0        0        0     1916 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/atlases/atlas-JHUDTI81_dseg.tsv
+-rw-r--r--   0        0        0      684 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/atlases/atlas-JHUTract_dseg.tsv
+-rw-r--r--   0        0        0     1535 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/atlases/atlas-LPBA40_dseg.tsv
+-rw-r--r--   0        0        0     4151 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/atlases/atlas-Neuromorphometrics_dseg.tsv
+-rw-r--r--   0        0        0      146 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/fmri/task-facesshapesemotion_events.tsv
+-rw-r--r--   0        0        0     3872 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/label_conversion_gtmsegmentation.csv
+-rw-r--r--   0        0        0        0 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/mappings/.emptyfile
+-rw-r--r--   0        0        0     2661 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/masks/region-cerebellumPons_eroded-6mm_mask.nii.gz
+-rw-r--r--   0        0        0     7028 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/masks/region-cerebellumPons_remove-extrabrain_eroded-3it_mask.nii.gz
+-rw-r--r--   0        0        0     1194 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/masks/region-pons_eroded-6mm_mask.nii.gz
+-rw-r--r--   0        0        0     4418 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/masks/region-pons_remove-extrabrain_eroded-2it_mask.nii.gz
+-rw-r--r--   0        0        0     2774 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/templates/pipeline_template/README.md.j2
+-rw-r--r--   0        0        0        0 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/templates/pipeline_template/__init__.py.j2
+-rw-r--r--   0        0        0     2622 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/templates/pipeline_template/cli.py.j2
+-rw-r--r--   0        0        0      295 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/templates/pipeline_template/info.json.j2
+-rw-r--r--   0        0        0     5460 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/templates/pipeline_template/pipeline.py.j2
+-rw-r--r--   0        0        0      713 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/templates/pipeline_template/utils.py.j2
+-rw-r--r--   0        0        0      258 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/resources/templates/pipeline_template/visualizer.py.j2
+-rw-r--r--   0        0        0        0 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/utils/__init__.py
+-rw-r--r--   0        0        0    15002 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/utils/atlas.py
+-rw-r--r--   0        0        0     5247 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/utils/bids.py
+-rw-r--r--   0        0        0    11637 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/utils/check_dependency.py
+-rw-r--r--   0        0        0     1438 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/utils/exceptions.py
+-rw-r--r--   0        0        0    20324 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/utils/filemanip.py
+-rw-r--r--   0        0        0    14440 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/utils/freesurfer.py
+-rw-r--r--   0        0        0     2286 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/utils/group.py
+-rw-r--r--   0        0        0     5552 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/utils/image.py
+-rw-r--r--   0        0        0    24818 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/utils/input_files.py
+-rw-r--r--   0        0        0    33603 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/utils/inputs.py
+-rw-r--r--   0        0        0     4686 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/utils/longitudinal.py
+-rw-r--r--   0        0        0     1585 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/utils/mri_registration.py
+-rw-r--r--   0        0        0     1643 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/utils/nipype.py
+-rw-r--r--   0        0        0     6337 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/utils/participant.py
+-rw-r--r--   0        0        0     5995 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/utils/pet.py
+-rw-r--r--   0        0        0     3626 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/utils/spm.py
+-rw-r--r--   0        0        0     2828 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/utils/statistics.py
+-rw-r--r--   0        0        0     1035 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/utils/stream.py
+-rw-r--r--   0        0        0    12019 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/utils/testing_utils.py
+-rw-r--r--   0        0        0     5537 2024-04-25 06:57:47.726103 clinica-0.8.1/clinica/utils/ux.py
+-rw-r--r--   0        0        0     2399 2024-04-25 06:57:47.750103 clinica-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0    11110 1970-01-01 00:00:00.000000 clinica-0.8.1/PKG-INFO
```

### Comparing `clinica-0.8.0/LICENSE.txt` & `clinica-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/README.md` & `clinica-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/cmdline.py` & `clinica-0.8.1/clinica/cmdline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/engine/cmdparser.py` & `clinica-0.8.1/clinica/engine/cmdparser.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/engine/template.py` & `clinica-0.8.1/clinica/engine/template.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/bids_dataset_description.py` & `clinica-0.8.1/clinica/iotools/bids_dataset_description.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/bids_readme.py` & `clinica-0.8.1/clinica/iotools/bids_readme.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/bids_utils.py` & `clinica-0.8.1/clinica/iotools/bids_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converter_utils.py` & `clinica-0.8.1/clinica/iotools/converter_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_json.py` & `clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_json.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_av45_fbb_pet.py` & `clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_av45_fbb_pet.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_dwi.py` & `clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_dwi.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_fdg_pet.py` & `clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_fdg_pet.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_flair.py` & `clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_flair.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_fmri.py` & `clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_fmri.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_pib_pet.py` & `clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_pib_pet.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_t1.py` & `clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_t1.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_tau_pet.py` & `clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_modalities/adni_tau_pet.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_to_bids.py` & `clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_to_bids.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_to_bids_cli.py` & `clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_to_bids_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/adni_to_bids/adni_utils.py` & `clinica-0.8.1/clinica/iotools/converters/adni_to_bids/adni_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -627,17 +627,24 @@
 
     Returns:
         Corrected participants_df.
     """
     from clinica.utils.stream import cprint
 
     diagnosis_dict = {1: "CN", 2: "MCI", 3: "AD"}
-    dxsum_df = load_clinical_csv(clinical_data_dir, "DXSUM_PDXCONV_ADNIALL").set_index(
-        ["PTID", "VISCODE2"]
-    )
+    # DXSUM_PDXCONV_ADNIALL has been renamed to DXSUM_PDXCONV
+    # this ensures old ADNI downloads still work with recent versions of Clinica
+    try:
+        dxsum_df = load_clinical_csv(
+            clinical_data_dir, "DXSUM_PDXCONV_ADNIALL"
+        ).set_index(["PTID", "VISCODE2"])
+    except OSError:
+        dxsum_df = load_clinical_csv(clinical_data_dir, "DXSUM_PDXCONV").set_index(
+            ["PTID", "VISCODE2"]
+        )
     missing_sc = participants_df[participants_df.original_study == "ADNI3"]
     participants_df.set_index("alternative_id_1", drop=True, inplace=True)
     for alternative_id in missing_sc.alternative_id_1.values:
         try:
             diagnosis_sc = diagnosis_dict[
                 dxsum_df.loc[(alternative_id, "sc"), "DIAGNOSIS"].values[0]
             ]
@@ -856,14 +863,15 @@
     return "VISCODE"
 
 
 def _is_a_visit_code_2_type(csv_filename: str) -> bool:
     """If the csv file is among these files, then the visit code column is 'VISCODE2'."""
     return csv_filename in {
         "ADAS_ADNIGO2.csv",
+        "DXSUM_PDXCONV.csv",
         "DXSUM_PDXCONV_ADNIALL.csv",
         "CDR.csv",
         "NEUROBAT.csv",
         "GDSCALE.csv",
         "MODHACH.csv",
         "MOCA.csv",
         "NPIQ.csv",
```

### Comparing `clinica-0.8.0/clinica/iotools/converters/aibl_to_bids/aibl_to_bids.py` & `clinica-0.8.1/clinica/iotools/converters/aibl_to_bids/aibl_to_bids.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/aibl_to_bids/aibl_to_bids_cli.py` & `clinica-0.8.1/clinica/iotools/converters/aibl_to_bids/aibl_to_bids_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/aibl_to_bids/utils/bids.py` & `clinica-0.8.1/clinica/iotools/converters/aibl_to_bids/utils/bids.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/aibl_to_bids/utils/clinical.py` & `clinica-0.8.1/clinica/iotools/converters/aibl_to_bids/utils/clinical.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/cli.py` & `clinica-0.8.1/clinica/iotools/converters/cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/cli_param.py` & `clinica-0.8.1/clinica/iotools/converters/cli_param.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/genfi_to_bids/genfi_to_bids.py` & `clinica-0.8.1/clinica/iotools/converters/genfi_to_bids/genfi_to_bids.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/genfi_to_bids/genfi_to_bids_cli.py` & `clinica-0.8.1/clinica/iotools/converters/genfi_to_bids/genfi_to_bids_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/genfi_to_bids/genfi_to_bids_utils.py` & `clinica-0.8.1/clinica/iotools/converters/genfi_to_bids/genfi_to_bids_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/habs_to_bids/habs_to_bids.py` & `clinica-0.8.1/clinica/iotools/converters/habs_to_bids/habs_to_bids.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/habs_to_bids/habs_to_bids_cli.py` & `clinica-0.8.1/clinica/iotools/converters/habs_to_bids/habs_to_bids_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/nifd_to_bids/nifd_to_bids.py` & `clinica-0.8.1/clinica/iotools/converters/nifd_to_bids/nifd_to_bids.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/nifd_to_bids/nifd_to_bids_cli.py` & `clinica-0.8.1/clinica/iotools/converters/nifd_to_bids/nifd_to_bids_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/nifd_to_bids/nifd_utils.py` & `clinica-0.8.1/clinica/iotools/converters/nifd_to_bids/nifd_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/oasis3_to_bids/oasis3_to_bids.py` & `clinica-0.8.1/clinica/iotools/converters/oasis3_to_bids/oasis3_to_bids.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/oasis3_to_bids/oasis3_to_bids_cli.py` & `clinica-0.8.1/clinica/iotools/converters/oasis3_to_bids/oasis3_to_bids_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/oasis3_to_bids/oasis3_utils.py` & `clinica-0.8.1/clinica/iotools/converters/oasis3_to_bids/oasis3_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/oasis_to_bids/oasis_to_bids.py` & `clinica-0.8.1/clinica/iotools/converters/oasis_to_bids/oasis_to_bids.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/oasis_to_bids/oasis_to_bids_cli.py` & `clinica-0.8.1/clinica/iotools/converters/oasis_to_bids/oasis_to_bids_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/ukb_to_bids/ukb_to_bids.py` & `clinica-0.8.1/clinica/iotools/converters/ukb_to_bids/ukb_to_bids.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/ukb_to_bids/ukb_to_bids_cli.py` & `clinica-0.8.1/clinica/iotools/converters/ukb_to_bids/ukb_to_bids_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/converters/ukb_to_bids/ukb_utils.py` & `clinica-0.8.1/clinica/iotools/converters/ukb_to_bids/ukb_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/data/clinical_specifications_adni_participant.tsv` & `clinica-0.8.1/clinica/iotools/data/clinical_specifications_adni_participant.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/data/clinical_specifications_adni_sessions.tsv` & `clinica-0.8.1/clinica/iotools/data/clinical_specifications_adni_sessions.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/data/clinical_specifications_participant.tsv` & `clinica-0.8.1/clinica/iotools/data/clinical_specifications_participant.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/data/clinical_specifications_scans.tsv` & `clinica-0.8.1/clinica/iotools/data/clinical_specifications_scans.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/data/clinical_specifications_sessions.tsv` & `clinica-0.8.1/clinica/iotools/data/clinical_specifications_sessions.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/data/genfi_data.tsv` & `clinica-0.8.1/clinica/iotools/data/genfi_data.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/data/genfi_data_mapping.tsv` & `clinica-0.8.1/clinica/iotools/data/genfi_data_mapping.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/data/genfi_ref.csv` & `clinica-0.8.1/clinica/iotools/data/genfi_ref.csv`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/utils/cli.py` & `clinica-0.8.1/clinica/iotools/utils/cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/utils/data_handling.py` & `clinica-0.8.1/clinica/iotools/utils/data_handling.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/iotools/utils/pipeline_handling.py` & `clinica-0.8.1/clinica/iotools/utils/pipeline_handling.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@random/image.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@random/image.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@random/minus.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@random/minus.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@random/mtimes.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@random/mtimes.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@random/plus.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@random/plus.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@random/random.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@random/random.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@term/image.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@term/image.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@term/minus.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@term/minus.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@term/mtimes.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@term/mtimes.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@term/plus.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@term/plus.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/@term/term.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/@term/term.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatAvSurf.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatAvSurf.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatAvVol.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatAvVol.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatColLim.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatColLim.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatColormap.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatColormap.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatCoord2Ind.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatCoord2Ind.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatDataCursorP.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatDataCursorP.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatDataCursorQ.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatDataCursorQ.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatDelete.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatDelete.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatEdg.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatEdg.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatF.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatF.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatInd2Coord.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatInd2Coord.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatInflate.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatInflate.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatLinMod.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatLinMod.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatListDir.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatListDir.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatMaskCut.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatMaskCut.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatNorm.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatNorm.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatP.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatP.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatPCA.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatPCA.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatPeakClus.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatPeakClus.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatPlot.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatPlot.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatQ.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatQ.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatROI.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatROI.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadData.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadData.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadData1.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadData1.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadSurf.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadSurf.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadSurf1.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadSurf1.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadVol.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadVol.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadVol1.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatReadVol1.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatResels.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatResels.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatSmooth.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatSmooth.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatStand.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatStand.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatSurf2Vol.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatSurf2Vol.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatT.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatT.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatView.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatView.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatView1.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatView1.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatViewData.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatViewData.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatViewData_backup.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatViewData_backup.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatView_backup.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatView_backup.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatViews.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatViews.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatVol2Surf.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatVol2Surf.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteData.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteData.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteSurf.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteSurf.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteSurf1.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteSurf1.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteVol.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteVol.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteVol1.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/SurfStatWriteVol1.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/gl.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/gl.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/icbm_template_2.00mm+orig.HEAD` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/icbm_template_2.00mm+orig.HEAD`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/icbm_template_2.00mm.mnc` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/icbm_template_2.00mm.mnc`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/redmod.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/redmod.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/spectral.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/spectral.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/stat_threshold.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/stat_threshold.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/SurfStat/var2fac.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/SurfStat/var2fac.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/lib/clinicasurfstat/clinicasurfstat.m` & `clinica-0.8.1/clinica/lib/clinicasurfstat/clinicasurfstat.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/option.py` & `clinica-0.8.1/clinica/option.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/__init__.py` & `clinica-0.8.1/clinica/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/cli_param/argument.py` & `clinica-0.8.1/clinica/pipelines/cli_param/argument.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/cli_param/option.py` & `clinica-0.8.1/clinica/pipelines/cli_param/option.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/cli_param/option_group.py` & `clinica-0.8.1/clinica/pipelines/cli_param/option_group.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/deeplearning_prepare_data/deeplearning_prepare_data_cli.py` & `clinica-0.8.1/clinica/pipelines/deeplearning_prepare_data/deeplearning_prepare_data_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/connectome/cli.py` & `clinica-0.8.1/clinica/pipelines/dwi/connectome/cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/connectome/info.json` & `clinica-0.8.1/clinica/pipelines/dwi/connectome/info.json`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/connectome/pipeline.py` & `clinica-0.8.1/clinica/pipelines/dwi/connectome/pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/connectome/utils.py` & `clinica-0.8.1/clinica/pipelines/dwi/connectome/utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/dti/cli.py` & `clinica-0.8.1/clinica/pipelines/dwi/dti/cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/dti/info.json` & `clinica-0.8.1/clinica/pipelines/dwi/dti/info.json`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/dti/pipeline.py` & `clinica-0.8.1/clinica/pipelines/dwi/dti/pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/dti/tasks.py` & `clinica-0.8.1/clinica/pipelines/dwi/dti/tasks.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/dti/utils.py` & `clinica-0.8.1/clinica/pipelines/dwi/dti/utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/preprocessing/engine.py` & `clinica-0.8.1/clinica/pipelines/dwi/preprocessing/engine.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/preprocessing/fmap/cli.py` & `clinica-0.8.1/clinica/pipelines/dwi/preprocessing/fmap/cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/preprocessing/fmap/info.json` & `clinica-0.8.1/clinica/pipelines/dwi/preprocessing/fmap/info.json`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/preprocessing/fmap/pipeline.py` & `clinica-0.8.1/clinica/pipelines/dwi/preprocessing/fmap/pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/preprocessing/fmap/tasks.py` & `clinica-0.8.1/clinica/pipelines/dwi/preprocessing/fmap/tasks.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/preprocessing/fmap/utils.py` & `clinica-0.8.1/clinica/pipelines/dwi/preprocessing/fmap/utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/preprocessing/fmap/workflows.py` & `clinica-0.8.1/clinica/pipelines/dwi/preprocessing/fmap/workflows.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/preprocessing/t1/cli.py` & `clinica-0.8.1/clinica/pipelines/dwi/preprocessing/t1/cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/preprocessing/t1/info.json` & `clinica-0.8.1/clinica/pipelines/dwi/preprocessing/t1/info.json`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/preprocessing/t1/pipeline.py` & `clinica-0.8.1/clinica/pipelines/dwi/preprocessing/t1/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,24 +153,23 @@
                 input_names=["bids_or_caps_filename"],
                 output_names=["container"],
                 function=container_from_filename,
             ),
             name="container_path",
         )
         files_to_write_in_caps = [
-            "dwi_filename",
             "dwi_preproc_filename",
             "b_values_preproc_filename",
             "b_vectors_preproc_filename",
             "b0_brain_mask_filename",
         ]
 
         rename_into_caps = npe.Node(
             nutil.Function(
-                input_names=files_to_write_in_caps,
+                input_names=["dwi_filename"] + files_to_write_in_caps,
                 output_names=[f"{x}_caps" for x in files_to_write_in_caps],
                 function=rename_into_caps_task,
             ),
             name="rename_into_caps",
         )
 
         write_results = npe.Node(name="write_results", interface=nio.DataSink())
```

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/preprocessing/t1/tasks.py` & `clinica-0.8.1/clinica/pipelines/dwi/preprocessing/t1/tasks.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/preprocessing/t1/utils.py` & `clinica-0.8.1/clinica/pipelines/dwi/preprocessing/t1/utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/preprocessing/t1/workflows.py` & `clinica-0.8.1/clinica/pipelines/dwi/preprocessing/t1/workflows.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/preprocessing/tasks.py` & `clinica-0.8.1/clinica/pipelines/dwi/preprocessing/tasks.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/preprocessing/utils.py` & `clinica-0.8.1/clinica/pipelines/dwi/preprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/preprocessing/workflows.py` & `clinica-0.8.1/clinica/pipelines/dwi/preprocessing/workflows.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/dwi/utils.py` & `clinica-0.8.1/clinica/pipelines/dwi/utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/engine.py` & `clinica-0.8.1/clinica/pipelines/engine.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/machine_learning/algorithm.py` & `clinica-0.8.1/clinica/pipelines/machine_learning/algorithm.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/machine_learning/base.py` & `clinica-0.8.1/clinica/pipelines/machine_learning/base.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/machine_learning/classification_cli.py` & `clinica-0.8.1/clinica/pipelines/machine_learning/classification_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/machine_learning/input.py` & `clinica-0.8.1/clinica/pipelines/machine_learning/input.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/machine_learning/ml_utils.py` & `clinica-0.8.1/clinica/pipelines/machine_learning/ml_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/machine_learning/ml_workflows.py` & `clinica-0.8.1/clinica/pipelines/machine_learning/ml_workflows.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/machine_learning/region_based_io.py` & `clinica-0.8.1/clinica/pipelines/machine_learning/region_based_io.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/machine_learning/tsv_based_io.py` & `clinica-0.8.1/clinica/pipelines/machine_learning/tsv_based_io.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/machine_learning/validation.py` & `clinica-0.8.1/clinica/pipelines/machine_learning/validation.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/machine_learning/vertex_based_io.py` & `clinica-0.8.1/clinica/pipelines/machine_learning/vertex_based_io.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/machine_learning/voxel_based_io.py` & `clinica-0.8.1/clinica/pipelines/machine_learning/voxel_based_io.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_cli.py` & `clinica-0.8.1/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_pipeline.py` & `clinica-0.8.1/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_utils.py` & `clinica-0.8.1/clinica/pipelines/machine_learning_spatial_svm/spatial_svm_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/pet_linear/pet_linear_cli.py` & `clinica-0.8.1/clinica/pipelines/pet_linear/pet_linear_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/pet_linear/pet_linear_pipeline.py` & `clinica-0.8.1/clinica/pipelines/pet_linear/pet_linear_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/pet_linear/pet_linear_utils.py` & `clinica-0.8.1/clinica/pipelines/pet_linear/pet_linear_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/pet_surface/applyInverseDeformationField.m` & `clinica-0.8.1/clinica/pipelines/pet_surface/applyInverseDeformationField.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/pet_surface/info.json` & `clinica-0.8.1/clinica/pipelines/pet_surface/info.json`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/pet_surface/pet_surface_cli.py` & `clinica-0.8.1/clinica/pipelines/pet_surface/pet_surface_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/pet_surface/pet_surface_longitudinal_cli.py` & `clinica-0.8.1/clinica/pipelines/pet_surface/pet_surface_longitudinal_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/pet_surface/pet_surface_pipeline.py` & `clinica-0.8.1/clinica/pipelines/pet_surface/pet_surface_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/pet_surface/pet_surface_utils.py` & `clinica-0.8.1/clinica/pipelines/pet_surface/pet_surface_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/pet_volume/pet_volume_cli.py` & `clinica-0.8.1/clinica/pipelines/pet_volume/pet_volume_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/pet_volume/pet_volume_pipeline.py` & `clinica-0.8.1/clinica/pipelines/pet_volume/pet_volume_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/pet_volume/pet_volume_utils.py` & `clinica-0.8.1/clinica/pipelines/pet_volume/pet_volume_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_surface/_utils.py` & `clinica-0.8.1/clinica/pipelines/statistics_surface/_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_surface/cli.py` & `clinica-0.8.1/clinica/pipelines/statistics_surface/cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_surface/pipeline.py` & `clinica-0.8.1/clinica/pipelines/statistics_surface/pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/_surfstat.py` & `clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/_surfstat.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/_utils.py` & `clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/models/_base.py` & `clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/models/_base.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/models/_contrast.py` & `clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/models/_contrast.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/models/_correlation.py` & `clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/models/_correlation.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/models/_factory.py` & `clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/models/_factory.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/models/_group.py` & `clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/models/_group.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/models/_utils.py` & `clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/models/_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/models/results/_base.py` & `clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/models/results/_base.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/models/results/_plot.py` & `clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/models/results/_plot.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/models/results/_serialize.py` & `clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/models/results/_serialize.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_surface/surfstat/models/results/_statistics.py` & `clinica-0.8.1/clinica/pipelines/statistics_surface/surfstat/models/results/_statistics.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_volume/statistics_volume_cli.py` & `clinica-0.8.1/clinica/pipelines/statistics_volume/statistics_volume_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_volume/statistics_volume_pipeline.py` & `clinica-0.8.1/clinica/pipelines/statistics_volume/statistics_volume_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_volume/statistics_volume_utils.py` & `clinica-0.8.1/clinica/pipelines/statistics_volume/statistics_volume_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_volume/template_model_contrast.m` & `clinica-0.8.1/clinica/pipelines/statistics_volume/template_model_contrast.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_volume/template_model_creation.m` & `clinica-0.8.1/clinica/pipelines/statistics_volume/template_model_creation.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_volume/template_model_results.m` & `clinica-0.8.1/clinica/pipelines/statistics_volume/template_model_results.m`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_cli.py` & `clinica-0.8.1/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_pipeline.py` & `clinica-0.8.1/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_utils.py` & `clinica-0.8.1/clinica/pipelines/statistics_volume_correction/statistics_volume_correction_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_freesurfer/t1_freesurfer_cli.py` & `clinica-0.8.1/clinica/pipelines/t1_freesurfer/t1_freesurfer_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_freesurfer/t1_freesurfer_pipeline.py` & `clinica-0.8.1/clinica/pipelines/t1_freesurfer/t1_freesurfer_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_freesurfer/t1_freesurfer_utils.py` & `clinica-0.8.1/clinica/pipelines/t1_freesurfer/t1_freesurfer_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_freesurfer/t1_freesurfer_visualizer.py` & `clinica-0.8.1/clinica/pipelines/t1_freesurfer/t1_freesurfer_visualizer.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_freesurfer_atlas/t1_freeesurfer_atlas_pipeline.py` & `clinica-0.8.1/clinica/pipelines/t1_freesurfer_atlas/t1_freeesurfer_atlas_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_freesurfer_atlas/t1_freesurfer_atlas_cli.py` & `clinica-0.8.1/clinica/pipelines/t1_freesurfer_atlas/t1_freesurfer_atlas_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_freesurfer_atlas/t1_freesurfer_atlas_utils.py` & `clinica-0.8.1/clinica/pipelines/t1_freesurfer_atlas/t1_freesurfer_atlas_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_freesurfer_longitudinal/longitudinal_utils.py` & `clinica-0.8.1/clinica/pipelines/t1_freesurfer_longitudinal/longitudinal_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_cli.py` & `clinica-0.8.1/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_cli.py` & `clinica-0.8.1/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_pipeline.py` & `clinica-0.8.1/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_utils.py` & `clinica-0.8.1/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_longitudinal_correction_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_cli.py` & `clinica-0.8.1/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_pipeline.py` & `clinica-0.8.1/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_utils.py` & `clinica-0.8.1/clinica/pipelines/t1_freesurfer_longitudinal/t1_freesurfer_template_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_linear/anat_linear_pipeline.py` & `clinica-0.8.1/clinica/pipelines/t1_linear/anat_linear_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_linear/anat_linear_utils.py` & `clinica-0.8.1/clinica/pipelines/t1_linear/anat_linear_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_linear/flair_linear_cli.py` & `clinica-0.8.1/clinica/pipelines/t1_linear/flair_linear_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_linear/t1_linear_cli.py` & `clinica-0.8.1/clinica/pipelines/t1_linear/t1_linear_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_volume/t1_volume_cli.py` & `clinica-0.8.1/clinica/pipelines/t1_volume/t1_volume_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_volume_create_dartel/t1_volume_create_dartel_cli.py` & `clinica-0.8.1/clinica/pipelines/t1_volume_create_dartel/t1_volume_create_dartel_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_volume_create_dartel/t1_volume_create_dartel_pipeline.py` & `clinica-0.8.1/clinica/pipelines/t1_volume_create_dartel/t1_volume_create_dartel_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_volume_dartel2mni/t1_volume_dartel2mni_cli.py` & `clinica-0.8.1/clinica/pipelines/t1_volume_dartel2mni/t1_volume_dartel2mni_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_volume_dartel2mni/t1_volume_dartel2mni_pipeline.py` & `clinica-0.8.1/clinica/pipelines/t1_volume_dartel2mni/t1_volume_dartel2mni_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_volume_existing_template/t1_volume_existing_template_cli.py` & `clinica-0.8.1/clinica/pipelines/t1_volume_existing_template/t1_volume_existing_template_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_cli.py` & `clinica-0.8.1/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_pipeline.py` & `clinica-0.8.1/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_utils.py` & `clinica-0.8.1/clinica/pipelines/t1_volume_parcellation/t1_volume_parcellation_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_cli.py` & `clinica-0.8.1/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_pipeline.py` & `clinica-0.8.1/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_utils.py` & `clinica-0.8.1/clinica/pipelines/t1_volume_register_dartel/t1_volume_register_dartel_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_cli.py` & `clinica-0.8.1/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_pipeline.py` & `clinica-0.8.1/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_utils.py` & `clinica-0.8.1/clinica/pipelines/t1_volume_tissue_segmentation/t1_volume_tissue_segmentation_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/dwi/_commons/_workflows.py` & `clinica-0.8.1/clinica/pydra/dwi/_commons/_workflows.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/engine.py` & `clinica-0.8.1/clinica/pydra/engine.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/engine_utils.py` & `clinica-0.8.1/clinica/pydra/engine_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/interfaces.py` & `clinica-0.8.1/clinica/pydra/interfaces.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/machine_learning_spatial_svm/pipeline.py` & `clinica-0.8.1/clinica/pydra/machine_learning_spatial_svm/pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/machine_learning_spatial_svm/spatial_svm_cli.py` & `clinica-0.8.1/clinica/pydra/machine_learning_spatial_svm/spatial_svm_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/machine_learning_spatial_svm/tasks.py` & `clinica-0.8.1/clinica/pydra/machine_learning_spatial_svm/tasks.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/pet_linear/pet_linear_cli.py` & `clinica-0.8.1/clinica/pydra/pet_linear/pet_linear_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/pet_linear/pipeline.py` & `clinica-0.8.1/clinica/pydra/pet_linear/pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/pet_linear/tasks.py` & `clinica-0.8.1/clinica/pydra/pet_linear/tasks.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/pet_volume/pet_volume_cli.py` & `clinica-0.8.1/clinica/pydra/pet_volume/pet_volume_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/pet_volume/pipeline.py` & `clinica-0.8.1/clinica/pydra/pet_volume/pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/pet_volume/tasks.py` & `clinica-0.8.1/clinica/pydra/pet_volume/tasks.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/query.py` & `clinica-0.8.1/clinica/pydra/query.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/shared_workflows/smoothing.py` & `clinica-0.8.1/clinica/pydra/shared_workflows/smoothing.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/statistics_volume/pipeline.py` & `clinica-0.8.1/clinica/pydra/statistics_volume/pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/statistics_volume/statistics_volume_cli.py` & `clinica-0.8.1/clinica/pydra/statistics_volume/statistics_volume_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/statistics_volume/task.py` & `clinica-0.8.1/clinica/pydra/statistics_volume/task.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/statistics_volume_correction/pipeline.py` & `clinica-0.8.1/clinica/pydra/statistics_volume_correction/pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/statistics_volume_correction/statistics_volume_correction_cli.py` & `clinica-0.8.1/clinica/pydra/statistics_volume_correction/statistics_volume_correction_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/statistics_volume_correction/task.py` & `clinica-0.8.1/clinica/pydra/statistics_volume_correction/task.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/t1_freesurfer/cli.py` & `clinica-0.8.1/clinica/pydra/t1_freesurfer/cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/t1_freesurfer/pipeline.py` & `clinica-0.8.1/clinica/pydra/t1_freesurfer/pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/t1_freesurfer/tasks.py` & `clinica-0.8.1/clinica/pydra/t1_freesurfer/tasks.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/t1_linear/t1_linear.py` & `clinica-0.8.1/clinica/pydra/t1_linear/t1_linear.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/t1_linear/t1_linear_cli.py` & `clinica-0.8.1/clinica/pydra/t1_linear/t1_linear_cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/t1_volume/create_dartel/cli.py` & `clinica-0.8.1/clinica/pydra/t1_volume/create_dartel/cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/t1_volume/create_dartel/pipeline.py` & `clinica-0.8.1/clinica/pydra/t1_volume/create_dartel/pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/t1_volume/dartel2mni/cli.py` & `clinica-0.8.1/clinica/pydra/t1_volume/dartel2mni/cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/t1_volume/dartel2mni/pipeline.py` & `clinica-0.8.1/clinica/pydra/t1_volume/dartel2mni/pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/t1_volume/dartel2mni/tasks.py` & `clinica-0.8.1/clinica/pydra/t1_volume/dartel2mni/tasks.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/t1_volume/register_dartel/cli.py` & `clinica-0.8.1/clinica/pydra/t1_volume/register_dartel/cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/t1_volume/register_dartel/pipeline.py` & `clinica-0.8.1/clinica/pydra/t1_volume/register_dartel/pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/t1_volume/tasks.py` & `clinica-0.8.1/clinica/pydra/t1_volume/tasks.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/t1_volume/tissue_segmentation/cli.py` & `clinica-0.8.1/clinica/pydra/t1_volume/tissue_segmentation/cli.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/t1_volume/tissue_segmentation/pipeline.py` & `clinica-0.8.1/clinica/pydra/t1_volume/tissue_segmentation/pipeline.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/t1_volume/utils.py` & `clinica-0.8.1/clinica/pydra/t1_volume/utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/tasks.py` & `clinica-0.8.1/clinica/pydra/tasks.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/pydra/utils.py` & `clinica-0.8.1/clinica/pydra/utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/resources/atlases/atlas-AAL2.txt` & `clinica-0.8.1/clinica/resources/atlases/atlas-AAL2.txt`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/resources/atlases/atlas-AAL2_dseg.nii.gz` & `clinica-0.8.1/clinica/resources/atlases/atlas-AAL2_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/resources/atlases/atlas-AAL2_dseg.tsv` & `clinica-0.8.1/clinica/resources/atlases/atlas-AAL2_dseg.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/resources/atlases/atlas-AICHA.txt` & `clinica-0.8.1/clinica/resources/atlases/atlas-AICHA.txt`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/resources/atlases/atlas-AICHA_dseg.nii.gz` & `clinica-0.8.1/clinica/resources/atlases/atlas-AICHA_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/resources/atlases/atlas-AICHA_dseg.tsv` & `clinica-0.8.1/clinica/resources/atlases/atlas-AICHA_dseg.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/resources/atlases/atlas-Hammers_dseg.tsv` & `clinica-0.8.1/clinica/resources/atlases/atlas-Hammers_dseg.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/resources/atlases/atlas-JHUDTI81_dseg.tsv` & `clinica-0.8.1/clinica/resources/atlases/atlas-JHUDTI81_dseg.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/resources/atlases/atlas-JHUTract_dseg.tsv` & `clinica-0.8.1/clinica/resources/atlases/atlas-JHUTract_dseg.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/resources/atlases/atlas-LPBA40_dseg.tsv` & `clinica-0.8.1/clinica/resources/atlases/atlas-LPBA40_dseg.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/resources/atlases/atlas-Neuromorphometrics_dseg.tsv` & `clinica-0.8.1/clinica/resources/atlases/atlas-Neuromorphometrics_dseg.tsv`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/resources/label_conversion_gtmsegmentation.csv` & `clinica-0.8.1/clinica/resources/label_conversion_gtmsegmentation.csv`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/resources/masks/region-cerebellumPons_eroded-6mm_mask.nii.gz` & `clinica-0.8.1/clinica/resources/masks/region-cerebellumPons_eroded-6mm_mask.nii.gz`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/resources/masks/region-cerebellumPons_remove-extrabrain_eroded-3it_mask.nii.gz` & `clinica-0.8.1/clinica/resources/masks/region-cerebellumPons_remove-extrabrain_eroded-3it_mask.nii.gz`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/resources/masks/region-pons_eroded-6mm_mask.nii.gz` & `clinica-0.8.1/clinica/resources/masks/region-pons_eroded-6mm_mask.nii.gz`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/resources/masks/region-pons_remove-extrabrain_eroded-2it_mask.nii.gz` & `clinica-0.8.1/clinica/resources/masks/region-pons_remove-extrabrain_eroded-2it_mask.nii.gz`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/resources/templates/pipeline_template/README.md.j2` & `clinica-0.8.1/clinica/resources/templates/pipeline_template/README.md.j2`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/resources/templates/pipeline_template/cli.py.j2` & `clinica-0.8.1/clinica/resources/templates/pipeline_template/cli.py.j2`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/resources/templates/pipeline_template/pipeline.py.j2` & `clinica-0.8.1/clinica/resources/templates/pipeline_template/pipeline.py.j2`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/resources/templates/pipeline_template/utils.py.j2` & `clinica-0.8.1/clinica/resources/templates/pipeline_template/utils.py.j2`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/utils/atlas.py` & `clinica-0.8.1/clinica/utils/atlas.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/utils/bids.py` & `clinica-0.8.1/clinica/utils/bids.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/utils/check_dependency.py` & `clinica-0.8.1/clinica/utils/check_dependency.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/utils/exceptions.py` & `clinica-0.8.1/clinica/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/utils/filemanip.py` & `clinica-0.8.1/clinica/utils/filemanip.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/utils/freesurfer.py` & `clinica-0.8.1/clinica/utils/freesurfer.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/utils/group.py` & `clinica-0.8.1/clinica/utils/group.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/utils/image.py` & `clinica-0.8.1/clinica/utils/image.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/utils/input_files.py` & `clinica-0.8.1/clinica/utils/input_files.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/utils/inputs.py` & `clinica-0.8.1/clinica/utils/inputs.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/utils/longitudinal.py` & `clinica-0.8.1/clinica/utils/longitudinal.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/utils/mri_registration.py` & `clinica-0.8.1/clinica/utils/mri_registration.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/utils/nipype.py` & `clinica-0.8.1/clinica/utils/nipype.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/utils/participant.py` & `clinica-0.8.1/clinica/utils/participant.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/utils/pet.py` & `clinica-0.8.1/clinica/utils/pet.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/utils/spm.py` & `clinica-0.8.1/clinica/utils/spm.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/utils/statistics.py` & `clinica-0.8.1/clinica/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/utils/stream.py` & `clinica-0.8.1/clinica/utils/stream.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/utils/testing_utils.py` & `clinica-0.8.1/clinica/utils/testing_utils.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/clinica/utils/ux.py` & `clinica-0.8.1/clinica/utils/ux.py`

 * *Files identical despite different names*

### Comparing `clinica-0.8.0/pyproject.toml` & `clinica-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clinica"
-version = "0.8.0"
+version = "0.8.1"
 description = "Software platform for clinical neuroimaging studies"
 license = "MIT"
 authors = ["ARAMIS Lab"]
 maintainers = ["Clinica developers <clinica.run@gmail.com>"]
 readme = "README.md"
 homepage = "https://www.clinica.run"
 repository = "https://github.com/aramis-lab/clinica.git"
```

### Comparing `clinica-0.8.0/PKG-INFO` & `clinica-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clinica
-Version: 0.8.0
+Version: 0.8.1
 Summary: Software platform for clinical neuroimaging studies
 Home-page: https://www.clinica.run
 License: MIT
 Keywords: bids,image processing,machine learning,neuroimaging,neuroscience
 Author: ARAMIS Lab
 Maintainer: Clinica developers
 Maintainer-email: clinica.run@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clinica Version: 0.8.0 Summary: Software platform
+Metadata-Version: 2.1 Name: clinica Version: 0.8.1 Summary: Software platform
 for clinical neuroimaging studies Home-page: https://www.clinica.run License:
 MIT Keywords: bids,image processing,machine learning,neuroimaging,neuroscience
 Author: ARAMIS Lab Maintainer: Clinica developers Maintainer-email:
 clinica.run@gmail.com Requires-Python: >=3.9,<3.13 Classifier: Development
 Status :: 4 - Beta Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
```

