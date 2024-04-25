# Comparing `tmp/cg-60.4.1.tar.gz` & `tmp/cg-60.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cg-60.4.1.tar", max compression
+gzip compressed data, was "cg-60.4.2.tar", max compression
```

## Comparing `cg-60.4.1.tar` & `cg-60.4.2.tar`

### file list

```diff
@@ -1,1361 +1,1318 @@
--rw-r--r--   0        0        0     2686 2024-04-25 12:07:50.743335 cg-60.4.1/README.md
--rw-r--r--   0        0        0       40 2024-04-25 12:07:50.743335 cg-60.4.1/cg/__init__.py
--rw-r--r--   0        0        0      315 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/__init__.py
--rw-r--r--   0        0        0       27 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/coverage/__init__.py
--rw-r--r--   0        0        0     2940 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/coverage/api.py
--rw-r--r--   0        0        0       56 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/crunchy/__init__.py
--rw-r--r--   0        0        0    12783 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/crunchy/crunchy.py
--rw-r--r--   0        0        0     4502 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/crunchy/files.py
--rw-r--r--   0        0        0      430 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/crunchy/models.py
--rw-r--r--   0        0        0      910 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/crunchy/sbatch.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/demultiplex/__init__.py
--rw-r--r--   0        0        0    11299 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/demultiplex/demultiplex_api.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/demultiplex/sample_sheet/__init__.py
--rw-r--r--   0        0        0    11227 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/demultiplex/sample_sheet/api.py
--rw-r--r--   0        0        0     2183 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/demultiplex/sample_sheet/index.py
--rw-r--r--   0        0        0     7341 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py
--rw-r--r--   0        0        0     3188 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py
--rw-r--r--   0        0        0     7071 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/demultiplex/sample_sheet/sample_models.py
--rw-r--r--   0        0        0     6076 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py
--rw-r--r--   0        0        0     1372 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py
--rw-r--r--   0        0        0     8092 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py
--rw-r--r--   0        0        0      824 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/demultiplex/sample_sheet/validators.py
--rw-r--r--   0        0        0      677 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/demultiplex/sbatch.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/downsample/__init__.py
--rw-r--r--   0        0        0     6160 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/downsample/downsample.py
--rw-r--r--   0        0        0     2125 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/downsample/utils.py
--rw-r--r--   0        0        0      298 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/environ.py
--rw-r--r--   0        0        0     1741 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/gens.py
--rw-r--r--   0        0        0     3419 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/gt.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/hermes/__init__.py
--rw-r--r--   0        0        0     2249 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/hermes/hermes_api.py
--rw-r--r--   0        0        0     1298 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/hermes/models.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/housekeeper/__init__.py
--rw-r--r--   0        0        0    30395 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/housekeeper/hk.py
--rw-r--r--   0        0        0      326 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/housekeeper/models.py
--rw-r--r--   0        0        0       32 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/invoice/__init__.py
--rw-r--r--   0        0        0     4804 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/invoice/render.py
--rw-r--r--   0        0        0   113467 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/invoice/templates/KI_pool_invoice.xlsx
--rw-r--r--   0        0        0    75562 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/invoice/templates/KI_sample_invoice.xlsx
--rw-r--r--   0        0        0   113512 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
--rw-r--r--   0        0        0    75459 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
--rw-r--r--   0        0        0       25 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/lims/__init__.py
--rw-r--r--   0        0        0    18873 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/lims/api.py
--rw-r--r--   0        0        0     2652 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/lims/batch.py
--rw-r--r--   0        0        0     8129 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/lims/order.py
--rw-r--r--   0        0        0     3118 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/lims/sample_sheet.py
--rw-r--r--   0        0        0     4866 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/loqus.py
--rw-r--r--   0        0        0       35 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/madeline/__init__.py
--rw-r--r--   0        0        0     3213 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/madeline/api.py
--rw-r--r--   0        0        0       23 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/mip/__init__.py
--rw-r--r--   0        0        0     3564 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/mip/confighandler.py
--rw-r--r--   0        0        0     2207 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/mutacc_auto.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/orderform/__init__.py
--rw-r--r--   0        0        0     9498 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/orderform/excel_orderform_parser.py
--rw-r--r--   0        0        0     3051 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/orderform/json_orderform_parser.py
--rw-r--r--   0        0        0     6419 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/orderform/orderform_parser.py
--rw-r--r--   0        0        0      252 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/orderform/utils.py
--rw-r--r--   0        0        0     2537 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/osticket.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/scout/__init__.py
--rw-r--r--   0        0        0     3177 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/scout/scout_export.py
--rw-r--r--   0        0        0    11108 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/scout/scoutapi.py
--rw-r--r--   0        0        0      444 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/scout/validators.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0        0        0     3457 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/sequencing_metrics_parser/api.py
--rw-r--r--   0        0        0      923 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/sequencing_metrics_parser/models.py
--rw-r--r--   0        0        0     6658 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/sequencing_metrics_parser/parser.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/slurm/__init__.py
--rw-r--r--   0        0        0     1277 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/slurm/sbatch.py
--rw-r--r--   0        0        0     3559 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/slurm/slurm_api.py
--rw-r--r--   0        0        0       32 2024-04-25 12:07:50.751335 cg-60.4.1/cg/apps/tb/__init__.py
--rw-r--r--   0        0        0     7995 2024-04-25 12:07:50.751335 cg-60.4.1/cg/apps/tb/api.py
--rw-r--r--   0        0        0      152 2024-04-25 12:07:50.751335 cg-60.4.1/cg/apps/tb/dto/create_job_request.py
--rw-r--r--   0        0        0      250 2024-04-25 12:07:50.751335 cg-60.4.1/cg/apps/tb/dto/summary_response.py
--rw-r--r--   0        0        0     1305 2024-04-25 12:07:50.751335 cg-60.4.1/cg/apps/tb/models.py
--rw-r--r--   0        0        0      305 2024-04-25 12:07:50.751335 cg-60.4.1/cg/apps/tb/validators.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/__init__.py
--rw-r--r--   0        0        0    11558 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/add.py
--rw-r--r--   0        0        0     2653 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/archive.py
--rw-r--r--   0        0        0    10118 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/backup.py
--rw-r--r--   0        0        0     3852 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/base.py
--rw-r--r--   0        0        0    10506 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/clean.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/compress/__init__.py
--rw-r--r--   0        0        0     2135 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/compress/base.py
--rw-r--r--   0        0        0     6706 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/compress/fastq.py
--rw-r--r--   0        0        0     8163 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/compress/helpers.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/delete/__init__.py
--rw-r--r--   0        0        0      564 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/delete/base.py
--rw-r--r--   0        0        0     4603 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/delete/case.py
--rw-r--r--   0        0        0     1884 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/delete/cases.py
--rw-r--r--   0        0        0     2633 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/delete/observations.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/deliver/__init__.py
--rw-r--r--   0        0        0     6030 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/deliver/base.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/demultiplex/__init__.py
--rw-r--r--   0        0        0      829 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/demultiplex/base.py
--rw-r--r--   0        0        0     4905 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py
--rw-r--r--   0        0        0     7726 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/demultiplex/demux.py
--rw-r--r--   0        0        0     1473 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/demultiplex/finish.py
--rw-r--r--   0        0        0     3119 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/demultiplex/sample_sheet.py
--rw-r--r--   0        0        0     2995 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/downsample.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/generate/__init__.py
--rw-r--r--   0        0        0      356 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/generate/base.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/generate/report/__init__.py
--rw-r--r--   0        0        0     4636 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/generate/report/base.py
--rw-r--r--   0        0        0      854 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/generate/report/options.py
--rw-r--r--   0        0        0     5340 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/generate/report/utils.py
--rw-r--r--   0        0        0     8327 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/get.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/set/__init__.py
--rw-r--r--   0        0        0     9856 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/set/base.py
--rw-r--r--   0        0        0     4384 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/set/case.py
--rw-r--r--   0        0        0     2595 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/set/cases.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/store/__init__.py
--rw-r--r--   0        0        0     1093 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/store/base.py
--rw-r--r--   0        0        0     6191 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/store/store.py
--rw-r--r--   0        0        0     1761 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/transfer.py
--rw-r--r--   0        0        0        1 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/__init__.py
--rw-r--r--   0        0        0     5706 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/base.py
--rw-r--r--   0        0        0     5503 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/clinical_delivery.py
--rw-r--r--   0        0        0     1175 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/coverage.py
--rw-r--r--   0        0        0     1528 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/delivery_report.py
--rw-r--r--   0        0        0     4022 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/fohm.py
--rw-r--r--   0        0        0     1463 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/genotype.py
--rw-r--r--   0        0        0     1885 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/gens.py
--rw-r--r--   0        0        0      584 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/gisaid.py
--rw-r--r--   0        0        0     2645 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/mutacc.py
--rw-r--r--   0        0        0       23 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/nipt/__init__.py
--rw-r--r--   0        0        0     3006 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/nipt/base.py
--rw-r--r--   0        0        0     2275 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/nipt/ftp.py
--rw-r--r--   0        0        0     1596 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/nipt/statina.py
--rw-r--r--   0        0        0      112 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/observations/__init__.py
--rw-r--r--   0        0        0     2672 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/observations/observations.py
--rw-r--r--   0        0        0     2904 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/observations/utils.py
--rw-r--r--   0        0        0     9970 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/scout.py
--rw-r--r--   0        0        0      650 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/utils.py
--rw-r--r--   0        0        0     1667 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/validate.py
--rw-r--r--   0        0        0      105 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/utils.py
--rw-r--r--   0        0        0       18 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/__init__.py
--rw-r--r--   0        0        0       22 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/balsamic/__init__.py
--rw-r--r--   0        0        0     8925 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/balsamic/base.py
--rw-r--r--   0        0        0     1980 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/balsamic/options.py
--rw-r--r--   0        0        0      881 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/balsamic/pon.py
--rw-r--r--   0        0        0     1162 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/balsamic/qc.py
--rw-r--r--   0        0        0     1177 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/balsamic/umi.py
--rw-r--r--   0        0        0     1342 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/base.py
--rw-r--r--   0        0        0    12379 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/commands.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/fastq/__init__.py
--rw-r--r--   0        0        0     1490 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/fastq/base.py
--rw-r--r--   0        0        0     1787 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/fastq/fastq_service.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/fluffy/__init__.py
--rw-r--r--   0        0        0     4177 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/fluffy/base.py
--rw-r--r--   0        0        0       22 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/jasen/__init__.py
--rw-r--r--   0        0        0      535 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/jasen/base.py
--rw-r--r--   0        0        0       22 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/microsalt/__init__.py
--rw-r--r--   0        0        0     7810 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/microsalt/base.py
--rw-r--r--   0        0        0       22 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/mip/__init__.py
--rw-r--r--   0        0        0     6596 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/mip/base.py
--rw-r--r--   0        0        0     1268 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/mip/options.py
--rw-r--r--   0        0        0       22 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/mip_dna/__init__.py
--rw-r--r--   0        0        0     1013 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/mip_dna/base.py
--rw-r--r--   0        0        0       22 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/mip_rna/__init__.py
--rw-r--r--   0        0        0      916 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/mip_rna/base.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/mutant/__init__.py
--rw-r--r--   0        0        0     3413 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/mutant/base.py
--rw-r--r--   0        0        0     9010 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/nf_analysis.py
--rw-r--r--   0        0        0       22 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/raredisease/__init__.py
--rw-r--r--   0        0        0     2210 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/raredisease/base.py
--rw-r--r--   0        0        0       22 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/rnafusion/__init__.py
--rw-r--r--   0        0        0     1179 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/rnafusion/base.py
--rw-r--r--   0        0        0       22 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/taxprofiler/__init__.py
--rw-r--r--   0        0        0     1211 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/taxprofiler/base.py
--rw-r--r--   0        0        0     1111 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/tomte/base.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.755335 cg-60.4.1/cg/clients/__init__.py
--rw-r--r--   0        0        0     1363 2024-04-25 12:07:50.755335 cg-60.4.1/cg/clients/arnold/api.py
--rw-r--r--   0        0        0      160 2024-04-25 12:07:50.755335 cg-60.4.1/cg/clients/arnold/dto/create_case_request.py
--rw-r--r--   0        0        0      384 2024-04-25 12:07:50.755335 cg-60.4.1/cg/clients/arnold/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.755335 cg-60.4.1/cg/clients/janus/__init__.py
--rw-r--r--   0        0        0     1246 2024-04-25 12:07:50.755335 cg-60.4.1/cg/clients/janus/api.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.755335 cg-60.4.1/cg/clients/janus/dto/__init__.py
--rw-r--r--   0        0        0      503 2024-04-25 12:07:50.755335 cg-60.4.1/cg/clients/janus/dto/create_qc_metrics_request.py
--rw-r--r--   0        0        0      420 2024-04-25 12:07:50.755335 cg-60.4.1/cg/clients/janus/exceptions.py
--rw-r--r--   0        0        0      937 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/__init__.py
--rw-r--r--   0        0        0      253 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/archiving.py
--rw-r--r--   0        0        0       35 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/backup.py
--rw-r--r--   0        0        0      769 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/bcl_convert_metrics.py
--rw-r--r--   0        0        0      469 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/compression.py
--rw-r--r--   0        0        0     6613 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/constants.py
--rw-r--r--   0        0        0     6033 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/delivery.py
--rw-r--r--   0        0        0     7387 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/demultiplexing.py
--rw-r--r--   0        0        0     1422 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/encryption.py
--rw-r--r--   0        0        0      372 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/extraction.py
--rw-r--r--   0        0        0     2157 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/gene_panel.py
--rw-r--r--   0        0        0     6704 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/housekeeper_tags.py
--rw-r--r--   0        0        0       95 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/invoice.py
--rw-r--r--   0        0        0     5815 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/lims.py
--rw-r--r--   0        0        0      743 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/metrics.py
--rw-r--r--   0        0        0      231 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/nanopore_files.py
--rw-r--r--   0        0        0      650 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/nextflow.py
--rw-r--r--   0        0        0     1529 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/nf_analysis.py
--rw-r--r--   0        0        0       19 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/nipt.py
--rw-r--r--   0        0        0     2257 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/observations.py
--rw-r--r--   0        0        0     1216 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/orderforms.py
--rw-r--r--   0        0        0       96 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/paths.py
--rw-r--r--   0        0        0      266 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/pdc.py
--rw-r--r--   0        0        0      160 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/pedigree.py
--rw-r--r--   0        0        0     1044 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/priority.py
--rw-r--r--   0        0        0       79 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/process.py
--rw-r--r--   0        0        0     5474 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/report.py
--rw-r--r--   0        0        0      569 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/sample_sources.py
--rw-r--r--   0        0        0     3111 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/scout.py
--rw-r--r--   0        0        0     1669 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/sequencing.py
--rw-r--r--   0        0        0      313 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/slurm.py
--rw-r--r--   0        0        0      529 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/subject.py
--rw-r--r--   0        0        0       55 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/symbols.py
--rw-r--r--   0        0        0      435 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/tb.py
--rw-r--r--   0        0        0      161 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/time.py
--rw-r--r--   0        0        0     6639 2024-04-25 12:07:50.755335 cg-60.4.1/cg/exc.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/__init__.py
--rw-r--r--   0        0        0     1037 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/api.py
--rw-r--r--   0        0        0      621 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/config.py
--rw-r--r--   0        0        0     2978 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/controller.py
--rw-r--r--   0        0        0     1763 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/csv.py
--rw-r--r--   0        0        0      210 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/gzip.py
--rw-r--r--   0        0        0      662 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/json.py
--rw-r--r--   0        0        0      525 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/png.py
--rw-r--r--   0        0        0     1094 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/txt.py
--rw-r--r--   0        0        0      552 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/validate_path.py
--rw-r--r--   0        0        0     1289 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/xml.py
--rw-r--r--   0        0        0     1153 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/yaml.py
--rw-r--r--   0        0        0      281 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/archive/__init__.py
--rw-r--r--   0        0        0    15193 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/archive/archive.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/archive/ddn/__init__.py
--rw-r--r--   0        0        0     1727 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/archive/ddn/constants.py
--rw-r--r--   0        0        0    10852 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/archive/ddn/ddn_data_flow_client.py
--rw-r--r--   0        0        0     3704 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/archive/ddn/models.py
--rw-r--r--   0        0        0     1250 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/archive/ddn/utils.py
--rw-r--r--   0        0        0     2024 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/archive/models.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/backup/__init__.py
--rw-r--r--   0        0        0    17426 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/backup/backup.py
--rw-r--r--   0        0        0     5397 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/backup/pdc.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/clean/__init__.py
--rw-r--r--   0        0        0     3901 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/clean/api.py
--rw-r--r--   0        0        0     7738 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/clean/clean_flow_cells.py
--rw-r--r--   0        0        0     1841 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/clean/clean_retrieved_spring_files.py
--rw-r--r--   0        0        0       34 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/compress/__init__.py
--rw-r--r--   0        0        0    14557 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/compress/compress.py
--rw-r--r--   0        0        0     4947 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/compress/files.py
--rw-r--r--   0        0        0       77 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/deliver/__init__.py
--rw-r--r--   0        0        0    14905 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/deliver/deliver.py
--rw-r--r--   0        0        0     4502 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/deliver/deliver_ticket.py
--rw-r--r--   0        0        0      904 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/deliver/fastq_path_generator.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/delivery/__init__.py
--rw-r--r--   0        0        0     8458 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/delivery/delivery.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/demultiplex/__init__.py
--rw-r--r--   0        0        0     2592 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/demultiplex/combine_sequencing_metrics.py
--rw-r--r--   0        0        0     5719 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/demultiplex/demux_post_processing.py
--rw-r--r--   0        0        0     4135 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/demultiplex/files.py
--rw-r--r--   0        0        0     7777 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/demultiplex/housekeeper_storage_functions.py
--rw-r--r--   0        0        0     6126 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/demultiplex/status_db_storage_functions.py
--rw-r--r--   0        0        0    10690 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/demultiplex/utils.py
--rw-r--r--   0        0        0     2855 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/demultiplex/validation.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/encryption/__init__.py
--rw-r--r--   0        0        0    20271 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/encryption/encryption.py
--rw-r--r--   0        0        0      537 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/encryption/sbatch.py
--rw-r--r--   0        0        0    10922 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/invoice.py
--rw-r--r--   0        0        0     2360 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/meta.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/observations/__init__.py
--rw-r--r--   0        0        0     6008 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/observations/balsamic_observations_api.py
--rw-r--r--   0        0        0     5277 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/observations/mip_dna_observations_api.py
--rw-r--r--   0        0        0     5364 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/observations/observations_api.py
--rw-r--r--   0        0        0       27 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/__init__.py
--rw-r--r--   0        0        0     3637 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/api.py
--rw-r--r--   0        0        0      121 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/balsamic_qc_submitter.py
--rw-r--r--   0        0        0      107 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/balsamic_submitter.py
--rw-r--r--   0        0        0      122 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/balsamic_umi_submitter.py
--rw-r--r--   0        0        0    15262 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/case_submitter.py
--rw-r--r--   0        0        0     6102 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/fastq_submitter.py
--rw-r--r--   0        0        0      105 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/fluffy_submitter.py
--rw-r--r--   0        0        0     1254 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/lims.py
--rw-r--r--   0        0        0     5782 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/metagenome_submitter.py
--rw-r--r--   0        0        0     6337 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/microbial_submitter.py
--rw-r--r--   0        0        0      123 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/microsalt_submitter.py
--rw-r--r--   0        0        0      105 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/mip_dna_submitter.py
--rw-r--r--   0        0        0      105 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/mip_rna_submitter.py
--rw-r--r--   0        0        0     7761 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/pool_submitter.py
--rw-r--r--   0        0        0      102 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/rml_submitter.py
--rw-r--r--   0        0        0      718 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/rnafusion_submitter.py
--rw-r--r--   0        0        0     1268 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/sars_cov_2_submitter.py
--rw-r--r--   0        0        0     1754 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/submitter.py
--rw-r--r--   0        0        0     7880 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/ticket_handler.py
--rw-r--r--   0        0        0     4105 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/qc_metrics/collect_qc_metrics.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/__init__.py
--rw-r--r--   0        0        0     8168 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/balsamic.py
--rw-r--r--   0        0        0      562 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/balsamic_qc.py
--rw-r--r--   0        0        0      717 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/balsamic_umi.py
--rw-r--r--   0        0        0     4171 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/field_validators.py
--rw-r--r--   0        0        0     6620 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/mip_dna.py
--rw-r--r--   0        0        0    18543 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/report_api.py
--rw-r--r--   0        0        0     5625 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/rnafusion.py
--rw-r--r--   0        0        0     1911 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/delivery-report.html
--rw-r--r--   0        0        0     4236 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/data_analysis/data_analysis.html
--rw-r--r--   0        0        0     1049 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/data_analysis/limitations.html
--rw-r--r--   0        0        0     3351 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html
--rw-r--r--   0        0        0     1364 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html
--rw-r--r--   0        0        0      753 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html
--rw-r--r--   0        0        0     3284 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html
--rw-r--r--   0        0        0     3670 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html
--rw-r--r--   0        0        0     2332 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/header.html
--rw-r--r--   0        0        0     2066 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/order.html
--rw-r--r--   0        0        0     2243 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/sample_prep.html
--rw-r--r--   0        0        0      472 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/ticket_system.html
--rw-r--r--   0        0        0     1165 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html
--rw-r--r--   0        0        0     1538 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html
--rw-r--r--   0        0        0      428 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/uploaded_files/rnafusion_uploaded_files.html
--rw-r--r--   0        0        0     4266 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html
--rw-r--r--   0        0        0       80 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/partials/footer.html
--rw-r--r--   0        0        0      172 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/partials/signature.html
--rw-r--r--   0        0        0   232803 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/report/templates/static/css/bootstrap.min.css
--rw-r--r--   0        0        0       33 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/report/templates/static/css/custom.css
--rw-r--r--   0        0        0    30068 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/report/templates/static/images/SWEDAC_logo.png
--rw-r--r--   0        0        0     3925 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/report/tomte.py
--rw-r--r--   0        0        0       32 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/rsync/__init__.py
--rw-r--r--   0        0        0    12291 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/rsync/rsync_api.py
--rw-r--r--   0        0        0      387 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/rsync/sbatch.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/tar/__init__.py
--rw-r--r--   0        0        0     1694 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/tar/tar.py
--rw-r--r--   0        0        0       71 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/transfer/__init__.py
--rw-r--r--   0        0        0    10016 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/transfer/external_data.py
--rw-r--r--   0        0        0     5814 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/transfer/lims.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/balsamic/__init__.py
--rw-r--r--   0        0        0     3107 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/balsamic/balsamic.py
--rw-r--r--   0        0        0     2224 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/coverage.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/fohm/__init__.py
--rw-r--r--   0        0        0    12102 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/fohm/fohm.py
--rw-r--r--   0        0        0       30 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/gisaid/__init__.py
--rw-r--r--   0        0        0      928 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/gisaid/constants.py
--rw-r--r--   0        0        0    13521 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/gisaid/gisaid.py
--rw-r--r--   0        0        0     3312 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/gisaid/models.py
--rw-r--r--   0        0        0     5310 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/gt.py
--rw-r--r--   0        0        0      898 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/microsalt/microsalt_upload_api.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/mip/__init__.py
--rw-r--r--   0        0        0     2546 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/mip/mip_dna.py
--rw-r--r--   0        0        0     1400 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/mip/mip_rna.py
--rw-r--r--   0        0        0     7294 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/mutacc.py
--rw-r--r--   0        0        0     1853 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/nf_analysis.py
--rw-r--r--   0        0        0       32 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/nipt/__init__.py
--rw-r--r--   0        0        0      696 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/nipt/models.py
--rw-r--r--   0        0        0     8106 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/nipt/nipt.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/scout/__init__.py
--rw-r--r--   0        0        0     4009 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/scout/balsamic_config_builder.py
--rw-r--r--   0        0        0     1491 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/scout/balsamic_umi_config_builder.py
--rw-r--r--   0        0        0     3322 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/scout/hk_tags.py
--rw-r--r--   0        0        0     9103 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/scout/mip_config_builder.py
--rw-r--r--   0        0        0     3495 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/scout/rnafusion_config_builder.py
--rw-r--r--   0        0        0     7231 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/scout/scout_config_builder.py
--rw-r--r--   0        0        0    23146 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/scout/uploadscoutapi.py
--rw-r--r--   0        0        0     3197 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/upload_api.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/__init__.py
--rw-r--r--   0        0        0    31068 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/analysis.py
--rw-r--r--   0        0        0    27751 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/balsamic.py
--rw-r--r--   0        0        0     2700 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/balsamic_pon.py
--rw-r--r--   0        0        0      553 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/balsamic_qc.py
--rw-r--r--   0        0        0      556 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/balsamic_umi.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/downsample/__init__.py
--rw-r--r--   0        0        0     3922 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/downsample/downsample.py
--rw-r--r--   0        0        0      711 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/downsample/sbatch.py
--rw-r--r--   0        0        0     8913 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/fastq.py
--rw-r--r--   0        0        0    10603 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/fluffy.py
--rw-r--r--   0        0        0      521 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/jasen.py
--rw-r--r--   0        0        0       70 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/microsalt/__init__.py
--rw-r--r--   0        0        0      116 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/microsalt/constants.py
--rw-r--r--   0        0        0      174 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/microsalt/metrics_parser/__init__.py
--rw-r--r--   0        0        0      366 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/microsalt/metrics_parser/metrics_parser.py
--rw-r--r--   0        0        0      903 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/microsalt/metrics_parser/models.py
--rw-r--r--   0        0        0    13173 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/microsalt/microsalt.py
--rw-r--r--   0        0        0      113 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/microsalt/quality_controller/__init__.py
--rw-r--r--   0        0        0      712 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/microsalt/quality_controller/models.py
--rw-r--r--   0        0        0     5697 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/microsalt/quality_controller/quality_controller.py
--rw-r--r--   0        0        0     1217 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/microsalt/quality_controller/report_generator.py
--rw-r--r--   0        0        0     2373 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/microsalt/quality_controller/result_logger.py
--rw-r--r--   0        0        0     5641 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/microsalt/quality_controller/utils.py
--rw-r--r--   0        0        0     1220 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/microsalt/utils.py
--rw-r--r--   0        0        0    12611 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/mip.py
--rw-r--r--   0        0        0     2948 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/mip_dna.py
--rw-r--r--   0        0        0     2124 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/mip_rna.py
--rw-r--r--   0        0        0    10974 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/mutant.py
--rw-r--r--   0        0        0    37948 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/nf_analysis.py
--rw-r--r--   0        0        0     6161 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/nf_handlers.py
--rw-r--r--   0        0        0     6357 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/prepare_fastq.py
--rw-r--r--   0        0        0     4965 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/raredisease.py
--rw-r--r--   0        0        0     5403 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/rnafusion.py
--rw-r--r--   0        0        0     4607 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/taxprofiler.py
--rw-r--r--   0        0        0     3576 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/tomte.py
--rw-r--r--   0        0        0      113 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/__init__.py
--rw-r--r--   0        0        0      367 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/analysis.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/balsamic/__init__.py
--rw-r--r--   0        0        0      459 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/balsamic/analysis.py
--rw-r--r--   0        0        0     4550 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/balsamic/config.py
--rw-r--r--   0        0        0     1986 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/balsamic/metrics.py
--rw-r--r--   0        0        0    17539 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/cg_config.py
--rw-r--r--   0        0        0     4302 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/compression_data.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/deliverables/__init__.py
--rw-r--r--   0        0        0     5213 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/deliverables/metric_deliverables.py
--rw-r--r--   0        0        0      243 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/delivery/delivery.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/demultiplex/__init__.py
--rw-r--r--   0        0        0    12040 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/demultiplex/run_parameters.py
--rw-r--r--   0        0        0      539 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/demultiplex/sbatch.py
--rw-r--r--   0        0        0     7006 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/downsample/downsample_data.py
--rw-r--r--   0        0        0      255 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/email.py
--rw-r--r--   0        0        0     1046 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/fastq.py
--rw-r--r--   0        0        0     2157 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/file_data.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/flow_cell/__init__.py
--rw-r--r--   0        0        0     9984 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/flow_cell/flow_cell.py
--rw-r--r--   0        0        0      317 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/flow_cell/utils.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/invoice/__init__.py
--rw-r--r--   0        0        0     1254 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/invoice/invoice.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/lims/__init__.py
--rw-r--r--   0        0        0     2019 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/lims/sample.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/mip/__init__.py
--rw-r--r--   0        0        0      337 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/mip/mip_analysis.py
--rw-r--r--   0        0        0     1564 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/mip/mip_config.py
--rw-r--r--   0        0        0     4696 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/mip/mip_metrics_deliverables.py
--rw-r--r--   0        0        0     2550 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/mip/mip_sample_info.py
--rw-r--r--   0        0        0     2472 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/nf_analysis.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/observations/__init__.py
--rw-r--r--   0        0        0      688 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/observations/input_files.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/__init__.py
--rw-r--r--   0        0        0     2659 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/constants.py
--rw-r--r--   0        0        0     5604 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/excel_sample.py
--rw-r--r--   0        0        0      898 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/json_sample.py
--rw-r--r--   0        0        0     1449 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/order.py
--rw-r--r--   0        0        0      811 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/orderform_schema.py
--rw-r--r--   0        0        0     4212 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/sample_base.py
--rw-r--r--   0        0        0     9668 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/samples.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/validators/__init__.py
--rw-r--r--   0        0        0     2300 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/validators/excel_sample_validators.py
--rw-r--r--   0        0        0      576 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/validators/json_sample_validators.py
--rw-r--r--   0        0        0       71 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/validators/sample_base_validators.py
--rw-r--r--   0        0        0      101 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/qc_metrics.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/raredisease/__init__.py
--rw-r--r--   0        0        0     1875 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/raredisease/raredisease.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/report/__init__.py
--rw-r--r--   0        0        0     7461 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/report/metadata.py
--rw-r--r--   0        0        0     6180 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/report/report.py
--rw-r--r--   0        0        0     5221 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/report/sample.py
--rw-r--r--   0        0        0     3004 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/report/validators.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/rnafusion/__init__.py
--rw-r--r--   0        0        0     1865 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/rnafusion/rnafusion.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/scout/__init__.py
--rw-r--r--   0        0        0     4783 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/scout/scout_load_config.py
--rw-r--r--   0        0        0      116 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/scout/validators.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/slurm/__init__.py
--rw-r--r--   0        0        0      617 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/slurm/sbatch.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/taxprofiler/__init__.py
--rw-r--r--   0        0        0     2443 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/taxprofiler/taxprofiler.py
--rw-r--r--   0        0        0     2588 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/tomte/tomte.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/workflow/__init__.py
--rw-r--r--   0        0        0      685 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/workflow/mutant.py
--rw-r--r--   0        0        0       70 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/workflow/validators.py
--rw-r--r--   0        0        0      842 2024-04-25 12:07:50.771335 cg-60.4.1/cg/resources/__init__.py
--rw-r--r--   0        0        0     3493 2024-04-25 12:07:50.771335 cg-60.4.1/cg/resources/rnafusion_bundle_filenames.yaml
--rw-r--r--   0        0        0     2434 2024-04-25 12:07:50.771335 cg-60.4.1/cg/resources/taxprofiler_bundle_filenames.yaml
--rw-r--r--   0        0        0     3732 2024-04-25 12:07:50.771335 cg-60.4.1/cg/resources/tomte_bundle_filenames.yaml
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/__init__.py
--rw-r--r--   0        0        0    20241 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/admin.py
--rw-r--r--   0        0        0    22743 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/api.py
--rw-r--r--   0        0        0     4887 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/app.py
--rw-r--r--   0        0        0       48 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/auto.py
--rw-r--r--   0        0        0     1184 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/config.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/dto/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/dto/delivery_message/__init__.py
--rw-r--r--   0        0        0      300 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/dto/delivery_message/delivery_message_request.py
--rw-r--r--   0        0        0      183 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/dto/delivery_message/delivery_message_response.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/dto/orders/__init__.py
--rw-r--r--   0        0        0      165 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/dto/orders/order_delivery_update_request.py
--rw-r--r--   0        0        0       91 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/dto/orders/order_patch_request.py
--rw-r--r--   0        0        0      662 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/dto/orders/orders_request.py
--rw-r--r--   0        0        0      413 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/dto/orders/orders_response.py
--rw-r--r--   0        0        0     2598 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/ext.py
--rw-r--r--   0        0        0       29 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/invoices/__init__.py
--rw-r--r--   0        0        0     4793 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/invoices/templates/invoices/index.html
--rw-r--r--   0        0        0     8171 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/invoices/templates/invoices/invoice.html
--rw-r--r--   0        0        0     2838 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/invoices/templates/invoices/layout.html
--rw-r--r--   0        0        0     4956 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/invoices/templates/invoices/new.html
--rw-r--r--   0        0        0     7708 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/invoices/views.py
--rw-r--r--   0        0        0      354 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/templates/admin/index.html
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/analysis_service/__init__.py
--rw-r--r--   0        0        0      482 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/analysis_service/analysis_service.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/__init__.py
--rw-r--r--   0        0        0     2531 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/delivery_message_service.py
--rw-r--r--   0        0        0      792 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/__init__.py
--rw-r--r--   0        0        0     1366 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/analysis_scout_message.py
--rw-r--r--   0        0        0      791 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/covid_message.py
--rw-r--r--   0        0        0      189 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/delivery_message.py
--rw-r--r--   0        0        0     1391 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/fastq_analysis_scout_message.py
--rw-r--r--   0        0        0      535 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/fastq_message.py
--rw-r--r--   0        0        0     1358 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/fastq_scout_message.py
--rw-r--r--   0        0        0      604 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/microsalt_mwr_message.py
--rw-r--r--   0        0        0      592 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/microsalt_mwx_message.py
--rw-r--r--   0        0        0      903 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/scout_message.py
--rw-r--r--   0        0        0      512 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/statina_message.py
--rw-r--r--   0        0        0      779 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/utils.py
--rw-r--r--   0        0        0     3300 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/utils.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/fastq_file_service/__init__.py
--rw-r--r--   0        0        0      101 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/fastq_file_service/exceptions.py
--rw-r--r--   0        0        0     1092 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/fastq_file_service/fastq_file_service.py
--rw-r--r--   0        0        0     2991 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/fastq_file_service/utils.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/orders/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/orders/order_service/__init__.py
--rw-r--r--   0        0        0     2684 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/orders/order_service/order_service.py
--rw-r--r--   0        0        0     1214 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/orders/order_service/utils.py
--rw-r--r--   0        0        0       94 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/orders/order_status_service/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/orders/order_status_service/dto/__init__.py
--rw-r--r--   0        0        0      192 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/orders/order_status_service/dto/case_summary.py
--rw-r--r--   0        0        0      289 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/orders/order_status_service/dto/order_summary.py
--rw-r--r--   0        0        0     1768 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/orders/order_status_service/order_summary_service.py
--rw-r--r--   0        0        0     1737 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/orders/order_status_service/utils.py
--rw-r--r--   0        0        0       95 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/quality_controller/__init__.py
--rw-r--r--   0        0        0     1819 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/quality_controller/quality_checks/checks.py
--rw-r--r--   0        0        0     4987 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/quality_controller/quality_checks/utils.py
--rw-r--r--   0        0        0     1040 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/quality_controller/quality_controller_service.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/slurm_service/__init__.py
--rw-r--r--   0        0        0      703 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/slurm_service/slurm_cli_service.py
--rw-r--r--   0        0        0      242 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/slurm_service/slurm_service.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/slurm_upload_service/__init__.py
--rw-r--r--   0        0        0      175 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/slurm_upload_service/slurm_upload_config.py
--rw-r--r--   0        0        0     2074 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/slurm_upload_service/slurm_upload_service.py
--rw-r--r--   0        0        0      203 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/slurm_upload_service/utils.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/__init__.py
--rw-r--r--   0        0        0     4650 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/base.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/crud/__init__.py
--rw-r--r--   0        0        0    13100 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/crud/create.py
--rw-r--r--   0        0        0     2144 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/crud/delete.py
--rw-r--r--   0        0        0    60036 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/crud/read.py
--rw-r--r--   0        0        0     1121 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/crud/update.py
--rw-r--r--   0        0        0     1662 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/database.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/filters/__init__.py
--rw-r--r--   0        0        0     5371 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/filters/status_analysis_filters.py
--rw-r--r--   0        0        0     1712 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/filters/status_application_filters.py
--rw-r--r--   0        0        0     1440 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/filters/status_application_limitations_filters.py
--rw-r--r--   0        0        0     2523 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/filters/status_application_version_filters.py
--rw-r--r--   0        0        0     1390 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/filters/status_bed_filters.py
--rw-r--r--   0        0        0     1317 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_bed_version_filters.py
--rw-r--r--   0        0        0    10787 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_case_filters.py
--rw-r--r--   0        0        0     3272 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_case_sample_filters.py
--rw-r--r--   0        0        0      903 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_collaboration_filters.py
--rw-r--r--   0        0        0     1412 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_customer_filters.py
--rw-r--r--   0        0        0     1880 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_flow_cell_filters.py
--rw-r--r--   0        0        0     1255 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_invoice_filters.py
--rw-r--r--   0        0        0     2792 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_metrics_filters.py
--rw-r--r--   0        0        0     3225 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_order_filters.py
--rw-r--r--   0        0        0      851 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_organism_filters.py
--rw-r--r--   0        0        0      783 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_panel_filters.py
--rw-r--r--   0        0        0     3923 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_pool_filters.py
--rw-r--r--   0        0        0     8660 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_sample_filters.py
--rw-r--r--   0        0        0      731 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_user_filters.py
--rw-r--r--   0        0        0    36081 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/models.py
--rw-r--r--   0        0        0      593 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/store.py
--rw-r--r--   0        0        0       30 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/__init__.py
--rw-r--r--   0        0        0      187 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/calculations.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/checksum/__init__.py
--rw-r--r--   0        0        0     1579 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/checksum/checksum.py
--rw-r--r--   0        0        0     1655 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/click/EnumChoice.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/click/__init__.py
--rw-r--r--   0        0        0     4910 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/commands.py
--rw-r--r--   0        0        0     1811 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/date.py
--rw-r--r--   0        0        0      635 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/dict.py
--rw-r--r--   0        0        0     2111 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/dispatcher.py
--rw-r--r--   0        0        0     1251 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/email.py
--rw-r--r--   0        0        0      134 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/enums.py
--rw-r--r--   0        0        0     3178 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/files.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/flask/__init__.py
--rw-r--r--   0        0        0     1052 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/flask/enum.py
--rw-r--r--   0        0        0      233 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/flow_cell.py
--rw-r--r--   0        0        0      834 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/time.py
--rw-r--r--   0        0        0     1410 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/utils.py
--rw-r--r--   0        0        0     1697 2024-04-25 12:07:50.775335 cg-60.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.775335 cg-60.4.1/tests/__init__.py
--rw-r--r--   0        0        0     1158 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/conftest.py
--rw-r--r--   0        0        0      231 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/coverage/conftest.py
--rw-r--r--   0        0        0     6188 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/coverage/test_coverage.py
--rw-r--r--   0        0        0     1693 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/crunchy/conftest.py
--rw-r--r--   0        0        0     5438 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/crunchy/test_compress_fastq.py
--rw-r--r--   0        0        0     2283 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/crunchy/test_config.py
--rw-r--r--   0        0        0    14032 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/crunchy/test_crunchy.py
--rw-r--r--   0        0        0     9109 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/crunchy/test_spring_decompression.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/__init__.py
--rw-r--r--   0        0        0     4994 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/conftest.py
--rw-r--r--   0        0        0     4010 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0        0        0     7986 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/test_demultiplex_api.py
--rw-r--r--   0        0        0     4782 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/test_index.py
--rw-r--r--   0        0        0     9468 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/test_override_cycles_validator.py
--rw-r--r--   0        0        0     4042 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/test_read_sample_sheet.py
--rw-r--r--   0        0        0    12389 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/test_sample_models.py
--rw-r--r--   0        0        0      951 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/test_sample_sheet_creator.py
--rw-r--r--   0        0        0     3175 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/test_sample_sheet_models.py
--rw-r--r--   0        0        0    10932 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/test_sample_sheet_validator.py
--rw-r--r--   0        0        0     4896 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/test_translate_sample_sheet.py
--rw-r--r--   0        0        0     1450 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/test_validate.py
--rw-r--r--   0        0        0     5094 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/downsample/test_downsample.py
--rw-r--r--   0        0        0     1419 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/downsample/test_downsample_utils.py
--rw-r--r--   0        0        0     1716 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/gens/test_gens_api.py
--rw-r--r--   0        0        0     1950 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/gt/conftest.py
--rw-r--r--   0        0        0     4276 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/gt/test_gt_api.py
--rw-r--r--   0        0        0     1453 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/hk/conftest.py
--rw-r--r--   0        0        0      684 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/hk/test__getattr__.py
--rw-r--r--   0        0        0     1593 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/hk/test_add_file.py
--rw-r--r--   0        0        0     3523 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/hk/test_bundles.py
--rw-r--r--   0        0        0      871 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/hk/test_core.py
--rw-r--r--   0        0        0    31172 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/hk/test_file.py
--rw-r--r--   0        0        0     5080 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/hk/test_version.py
--rw-r--r--   0        0        0     1840 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/lims/conftest.py
--rw-r--r--   0        0        0     3197 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/lims/test_api.py
--rw-r--r--   0        0        0     1451 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/lims/test_sample_sheet.py
--rw-r--r--   0        0        0     9223 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/loqus/conftest.py
--rw-r--r--   0        0        0     8994 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/loqus/test_loqusdb_api.py
--rw-r--r--   0        0        0     2439 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/madeline/conftest.py
--rw-r--r--   0        0        0     4653 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/madeline/test_madeline.py
--rw-r--r--   0        0        0     3328 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/mip/conftest.py
--rw-r--r--   0        0        0     2487 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/mip/test_config_mip.py
--rw-r--r--   0        0        0      883 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/mutacc_auto/conftest.py
--rw-r--r--   0        0        0     2473 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/mutacc_auto/test_mutacc_auto.py
--rw-r--r--   0        0        0    11930 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/orderform/conftest.py
--rw-r--r--   0        0        0     9484 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/orderform/test_excel_orderform_parser.py
--rw-r--r--   0        0        0     4351 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/orderform/test_excel_sample_schema.py
--rw-r--r--   0        0        0     1032 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/orderform/test_json_orderform_parser.py
--rw-r--r--   0        0        0     2474 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/orderform/test_orderform_parser.py
--rw-r--r--   0        0        0    16002 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/orderform/validators/test_excel_sample_validators.py
--rw-r--r--   0        0        0     3670 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/scout/conftest.py
--rw-r--r--   0        0        0     2269 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/scout/test_get_causative_variants.py
--rw-r--r--   0        0        0     1376 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/scout/test_get_scout_cases.py
--rw-r--r--   0        0        0     1840 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/scout/test_scout_load_config.py
--rw-r--r--   0        0        0     7047 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/scout/test_scout_models.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0        0        0     2639 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/sequencing_metrics_parser/conftest.py
--rw-r--r--   0        0        0     7069 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
--rw-r--r--   0        0        0     2958 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/sequencing_metrics_parser/parsers/test_sequencing_metrics_parser_api.py
--rw-r--r--   0        0        0     1131 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/slurm/conftest.py
--rw-r--r--   0        0        0     4412 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/slurm/test_slurm_api.py
--rw-r--r--   0        0        0      831 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/test_apps_environ.py
--rw-r--r--   0        0        0      957 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/test_osticket.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/add/__init__.py
--rw-r--r--   0        0        0     1174 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/add/test_cli_add.py
--rw-r--r--   0        0        0     2471 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/add/test_cli_add_customer.py
--rw-r--r--   0        0        0     6841 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/add/test_cli_add_family.py
--rw-r--r--   0        0        0     7588 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/add/test_cli_add_relationship.py
--rw-r--r--   0        0        0     8382 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/add/test_cli_add_sample.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/backup/__init__.py
--rw-r--r--   0        0        0      705 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/backup/conftest.py
--rw-r--r--   0        0        0    11101 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/backup/test_backup_command.py
--rw-r--r--   0        0        0     6865 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/clean/conftest.py
--rw-r--r--   0        0        0     5536 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/clean/test_balsamic_clean.py
--rw-r--r--   0        0        0     2557 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/clean/test_clean_flow_cell.py
--rw-r--r--   0        0        0     1830 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/clean/test_clean_hk_bundle_files.py
--rw-r--r--   0        0        0     2098 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/clean/test_hk_bundle_files.py
--rw-r--r--   0        0        0     4610 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/clean/test_hk_case_bundle_files.py
--rw-r--r--   0        0        0     3585 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/clean/test_microbial_clean.py
--rw-r--r--   0        0        0     1881 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/clean/test_rsync_past_run_dirs.py
--rw-r--r--   0        0        0     9707 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/compress/conftest.py
--rw-r--r--   0        0        0     7709 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/compress/test_cli_compress_fastq.py
--rw-r--r--   0        0        0     1416 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/compress/test_cli_decompress_spring.py
--rw-r--r--   0        0        0     5205 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/compress/test_compress_helpers.py
--rw-r--r--   0        0        0     1239 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/compress/test_store_fastq.py
--rw-r--r--   0        0        0     7558 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/conftest.py
--rw-r--r--   0        0        0    12747 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/delete/test_cli_delete_case.py
--rw-r--r--   0        0        0     1873 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/delete/test_cli_delete_cases.py
--rw-r--r--   0        0        0     3794 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/deliver/conftest.py
--rw-r--r--   0        0        0     4428 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/deliver/test_deliver_base.py
--rw-r--r--   0        0        0     1166 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/deliver/test_rsync_base.py
--rw-r--r--   0        0        0     8569 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/deliver/test_run_deliver_cmd.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/demultiplex/__init__.py
--rw-r--r--   0        0        0     5109 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0        0        0     4773 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/demultiplex/test_demultiplex_flowcell.py
--rw-r--r--   0        0        0     1607 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/demultiplex/test_finish_demux.py
--rw-r--r--   0        0        0     2989 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/demultiplex/test_validate_sample_sheet.py
--rw-r--r--   0        0        0     4423 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/demultiplex/test_verify_syncing.py
--rw-r--r--   0        0        0     1585 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/downsample/test_cli_downsample.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/generate/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/generate/report/__init__.py
--rw-r--r--   0        0        0     1622 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/generate/report/conftest.py
--rw-r--r--   0        0        0     2477 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/generate/report/test_cli_delivery_report.py
--rw-r--r--   0        0        0     2760 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/generate/report/test_utils.py
--rw-r--r--   0        0        0      563 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/generate/test_cli_base.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/get/__init__.py
--rw-r--r--   0        0        0      863 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/get/test_cli_get.py
--rw-r--r--   0        0        0     1526 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/get/test_cli_get_analysis.py
--rw-r--r--   0        0        0     1242 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/get/test_cli_get_case.py
--rw-r--r--   0        0        0     6208 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/get/test_cli_get_flow_cell.py
--rw-r--r--   0        0        0     8835 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/get/test_cli_get_sample.py
--rw-r--r--   0        0        0     1364 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/set/conftest.py
--rw-r--r--   0        0        0     7311 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/set/test_cli_set_case.py
--rw-r--r--   0        0        0     1460 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/set/test_cli_set_cases.py
--rw-r--r--   0        0        0     2016 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/set/test_cli_set_flowcell.py
--rw-r--r--   0        0        0     1685 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/set/test_cli_set_list_keys.py
--rw-r--r--   0        0        0    12450 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/set/test_cli_set_sample.py
--rw-r--r--   0        0        0     6124 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/set/test_cli_set_samples.py
--rw-r--r--   0        0        0     7015 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/store/test_store.py
--rw-r--r--   0        0        0     2332 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/test_base.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/__init__.py
--rw-r--r--   0        0        0    10057 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/conftest.py
--rw-r--r--   0        0        0     2295 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/test_cli_scout.py
--rw-r--r--   0        0        0     1789 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/test_cli_upload.py
--rw-r--r--   0        0        0      971 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/test_cli_upload_auto.py
--rw-r--r--   0        0        0     1669 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/test_cli_upload_delivery_report.py
--rw-r--r--   0        0        0      895 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/test_cli_upload_fastq.py
--rw-r--r--   0        0        0     1199 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/test_cli_upload_genotype.py
--rw-r--r--   0        0        0      694 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/test_cli_upload_gens.py
--rw-r--r--   0        0        0     9965 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/test_cli_upload_nipt.py
--rw-r--r--   0        0        0     4684 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/test_cli_upload_nipt_ftp.py
--rw-r--r--   0        0        0     1839 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/test_cli_upload_nipt_statina.py
--rw-r--r--   0        0        0     6177 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/test_cli_upload_observations.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/__init__.py
--rw-r--r--   0        0        0    31369 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/balsamic/conftest.py
--rw-r--r--   0        0        0    13938 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
--rw-r--r--   0        0        0     7984 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/balsamic/test_compound_commands.py
--rw-r--r--   0        0        0     2336 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/balsamic/test_link.py
--rw-r--r--   0        0        0     3554 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/balsamic/test_report_deliver.py
--rw-r--r--   0        0        0     6209 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/balsamic/test_run.py
--rw-r--r--   0        0        0     6934 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/balsamic/test_store_housekeeper.py
--rw-r--r--   0        0        0     8458 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/conftest.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/fastq/__init__.py
--rw-r--r--   0        0        0     2332 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/fastq/test_fastq_base.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/fluffy/__init__.py
--rw-r--r--   0        0        0     5237 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/fluffy/conftest.py
--rw-r--r--   0        0        0     5687 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
--rw-r--r--   0        0        0     3302 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/fluffy/test_cli_link.py
--rw-r--r--   0        0        0     1896 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/fluffy/test_cli_run.py
--rw-r--r--   0        0        0     2968 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/fluffy/test_cli_start.py
--rw-r--r--   0        0        0     7815 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/fluffy/test_cli_store.py
--rw-r--r--   0        0        0     2775 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/microsalt/conftest.py
--rw-r--r--   0        0        0     6926 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/microsalt/test_microsalt_case_config.py
--rw-r--r--   0        0        0     1000 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/microsalt/test_microsalt_run.py
--rw-r--r--   0        0        0     6544 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/conftest.py
--rw-r--r--   0        0        0     7011 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_base.py
--rw-r--r--   0        0        0     1542 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
--rw-r--r--   0        0        0      431 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_dna_link.py
--rw-r--r--   0        0        0     2108 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py
--rw-r--r--   0        0        0     1273 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
--rw-r--r--   0        0        0     3595 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_dna_run.py
--rw-r--r--   0        0        0     3884 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_dna_start.py
--rw-r--r--   0        0        0     1004 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
--rw-r--r--   0        0        0      527 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_rna_link.py
--rw-r--r--   0        0        0      716 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_rna_run.py
--rw-r--r--   0        0        0     8559 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_store.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/nf_analysis/__init__.py
--rw-r--r--   0        0        0     9318 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_config_case.py
--rw-r--r--   0        0        0     3831 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py
--rw-r--r--   0        0        0     5087 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py
--rw-r--r--   0        0        0     9211 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_run.py
--rw-r--r--   0        0        0     3267 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_start.py
--rw-r--r--   0        0        0     9877 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_store.py
--rw-r--r--   0        0        0    10373 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py
--rw-r--r--   0        0        0      978 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/raredisease/__init__.py
--rw-r--r--   0        0        0     3940 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py
--rw-r--r--   0        0        0      921 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/test_cli_workflow.py
--rw-r--r--   0        0        0     4310 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/test_cli_workflow_clean.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/clients/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/clients/arnold/__init__.py
--rw-r--r--   0        0        0     1080 2024-04-25 12:07:50.787335 cg-60.4.1/tests/clients/arnold/conftest.py
--rw-r--r--   0        0        0     1503 2024-04-25 12:07:50.787335 cg-60.4.1/tests/clients/arnold/test_arnold_api_client.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/clients/janus/__init__.py
--rw-r--r--   0        0        0     2381 2024-04-25 12:07:50.787335 cg-60.4.1/tests/clients/janus/conftest.py
--rw-r--r--   0        0        0     1716 2024-04-25 12:07:50.787335 cg-60.4.1/tests/clients/janus/test_janus_api_client.py
--rw-r--r--   0        0        0   133992 2024-04-25 12:07:50.787335 cg-60.4.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/delivery_fixtures/__init__.py
--rw-r--r--   0        0        0     2653 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py
--rw-r--r--   0        0        0     4972 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/delivery_fixtures/context_fixtures.py
--rw-r--r--   0        0        0     1494 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/delivery_fixtures/path_fixtures.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/__init__.py
--rw-r--r--   0        0        0     4625 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py
--rw-r--r--   0        0        0     3467 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py
--rw-r--r--   0        0        0    19179 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py
--rw-r--r--   0        0        0     3699 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py
--rw-r--r--   0        0        0     6000 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py
--rw-r--r--   0        0        0     8960 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py
--rw-r--r--   0        0        0     3174 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_check_scenario.py
--rw-r--r--   0        0        0     4801 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_fixtures.py
--rw-r--r--   0        0        0     1304 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/timestamp_fixtures.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
--rw-r--r--   0        0        0    14644 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
--rw-r--r--   0        0        0    15921 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/ADM2.cram
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/ADM3.cram
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/adm1.cram
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/adm1.mt.bam
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/multiqc.html
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/report.pdf
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/smn.vcf
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/snv.vcf
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/snv_research.vcf
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/str.vcf
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/sv.vcf
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/sv_research.vcf
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
--rw-r--r--   0        0        0       70 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/nf-analysis/pipeline_params.config
--rw-r--r--   0        0        0      195 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/nf-analysis/pipeline_resource_optimisation.config
--rw-r--r--   0        0        0      195 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/nf-analysis/platform.config
--rw-r--r--   0        0        0     8173 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/raredisease/multiqc_data.json
--rw-r--r--   0        0        0    20005 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml
--rw-r--r--   0        0        0     5497 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/rnafusion/multiqc_data.json
--rw-r--r--   0        0        0    12499 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml
--rw-r--r--   0        0        0     2873 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/sample_coverage.bed
--rw-r--r--   0        0        0     6506 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/taxprofiler/multiqc_data.json
--rw-r--r--   0        0        0    10513 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml
--rw-r--r--   0        0        0     5771 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/analysis/tomte/multiqc_data.json
--rw-r--r--   0        0        0    14859 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml
--rw-r--r--   0        0        0    10961 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/balsamic/case/config.json
--rw-r--r--   0        0        0     3465 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/balsamic/case/metadata.yml
--rw-r--r--   0        0        0       63 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/balsamic/case/metadata_directory.yml
--rw-r--r--   0        0        0      165 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
--rw-r--r--   0        0        0     2705 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
--rw-r--r--   0        0        0      692 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/crunchy/spring_metadata.json
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0      412 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      484 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      658 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/demuxcomplete.txt
--rw-r--r--   0        0        0     1757 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0        0        0        7 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0     6034 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0        0        0     1172 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0        0        0        7 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_1.fastq.gz
--rw-r--r--   0        0        0        7 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_2.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0      288 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      361 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      414 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/demuxcomplete.txt
--rw-r--r--   0        0        0      315 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      434 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0     8624 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml
--rw-r--r--   0        0        0      568 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0      220 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      463 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      622 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0      345 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      650 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      896 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0      619 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0      303 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      364 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      427 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/demuxcomplete.txt
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0     4439 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0        0        0     1172 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0     5127 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
--rw-r--r--   0        0        0       43 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz
--rw-r--r--   0        0        0       67 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz.md5
--rw-r--r--   0        0        0   338370 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz
--rw-r--r--   0        0        0       67 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz.md5
--rw-r--r--   0        0        0   338349 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/CopyComplete.txt
--rw-r--r--   0        0        0     2126 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json
--rw-r--r--   0        0        0     1827 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json
--rw-r--r--   0        0        0       90 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/README.txt
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAComplete.txt
--rw-r--r--   0        0        0     6895 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml
--rw-r--r--   0        0        0       37 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead1Complete.txt
--rw-r--r--   0        0        0       36 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead2Complete.txt
--rw-r--r--   0        0        0       36 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead3Complete.txt
--rw-r--r--   0        0        0    24755 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml
--rw-r--r--   0        0        0      692 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
--rw-r--r--   0        0        0      724 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0       61 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SequencingComplete.txt
--rw-r--r--   0        0        0     5775 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/CopyComplete.txt
--rw-r--r--   0        0        0     2282 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json
--rw-r--r--   0        0        0     1632 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json
--rw-r--r--   0        0        0       75 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/README.txt
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAComplete.txt
--rw-r--r--   0        0        0     6912 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml
--rw-r--r--   0        0        0       36 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead1Complete.txt
--rw-r--r--   0        0        0       36 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead2Complete.txt
--rw-r--r--   0        0        0       36 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead3Complete.txt
--rw-r--r--   0        0        0       36 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead4Complete.txt
--rw-r--r--   0        0        0    24814 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml
--rw-r--r--   0        0        0      814 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv
--rw-r--r--   0        0        0      660 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0       61 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SequencingComplete.txt
--rw-r--r--   0        0        0     5853 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/CopyComplete.txt
--rw-r--r--   0        0        0    21848 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json
--rw-r--r--   0        0        0    15512 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json
--rw-r--r--   0        0        0       79 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/README.txt
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RTAComplete.txt
--rw-r--r--   0        0        0      756 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml
--rw-r--r--   0        0        0     4118 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv
--rw-r--r--   0        0        0     1408 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0     5326 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/CopyComplete.txt
--rw-r--r--   0        0        0    15041 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json
--rw-r--r--   0        0        0    10649 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json
--rw-r--r--   0        0        0       80 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/README.txt
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RTAComplete.txt
--rw-r--r--   0        0        0      755 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml
--rw-r--r--   0        0        0     2878 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv
--rw-r--r--   0        0        0      928 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0     5359 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CopyComplete.txt
--rw-r--r--   0        0        0    27887 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv
--rw-r--r--   0        0        0   141870 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json
--rwxr-xr-x   0        0        0   122682 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json
--rw-r--r--   0        0        0      243 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/README.txt
--rw-r--r--   0        0        0    28230 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTAComplete.txt
--rw-r--r--   0        0        0    94426 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml
--rw-r--r--   0        0        0     5819 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/SequenceComplete.txt
--rw-r--r--   0        0        0     1757 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0        0        0     1757 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stdout
--rw-r--r--   0        0        0       12 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/README.txt
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RTAComplete.txt
--rw-r--r--   0        0        0     5945 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml
--rw-r--r--   0        0        0      260 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/copycomplete.txt
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/demuxstarted.txt
--rw-r--r--   0        0        0     1757 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0        0        0     1757 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout
--rw-r--r--   0        0        0    47522 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json
--rw-r--r--   0        0        0       12 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/README.txt
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0        0        0     6666 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0        0        0      254 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/copycomplete.txt
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/delivery.txt
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/demuxstarted.txt
--rwxr-xr-x   0        0        0    47434 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CopyComplete.txt
--rw-r--r--   0        0        0    10950 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv
--rw-r--r--   0        0        0      225 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/Manifest.tsv
--rw-r--r--   0        0        0       55 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/README.txt
--rwxr-xr-x   0        0        0     2493 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg
--rwxr-xr-x   0        0        0        1 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAComplete.txt
--rwxr-xr-x   0        0        0        2 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAExited.txt
--rwxr-xr-x   0        0        0      730 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml
--rwxr-xr-x   0        0        0    79277 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml
--rwxr-xr-x   0        0        0     2694 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
--rw-r--r--   0        0        0    10950 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
--rw-r--r--   0        0        0      619 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0        0        0       12 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/README.txt
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0        0        0      399 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CopyComplete.txt
--rw-r--r--   0        0        0     4941 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv
--rwxr-xr-x   0        0        0    20050 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stderr
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stdout
--rw-r--r--   0        0        0      244 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/README.txt
--rw-r--r--   0        0        0     6391 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTAComplete.txt
--rw-r--r--   0        0        0    16428 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml
--rw-r--r--   0        0        0     6728 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
--rw-r--r--   0        0        0     5127 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SequenceComplete.txt
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/demuxstarted.txt
--rw-r--r--   0        0        0      133 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/README.txt
--rw-r--r--   0        0        0      724 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
--rw-r--r--   0        0        0     5775 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
--rw-r--r--   0        0        0      124 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/180509_D00450_0598_BHGYFNBCX2/README.txt
--rw-r--r--   0        0        0      310 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/README.txt
--rw-r--r--   0        0        0     5819 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
--rw-r--r--   0        0        0      122 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/README.txt
--rwxr-xr-x   0        0        0     2694 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
--rw-r--r--   0        0        0      311 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/README.txt
--rw-r--r--   0        0        0     6728 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0        0        0      399 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
--rw-r--r--   0        0        0      399 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_0.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_1.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/final_summary_PAS86456_72d9fceb_8a4fd683.txt
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_0.pod5
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_1.pod5
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_0.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_1.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/final_summary_PAS97781_595b5663_efc7f02e.txt
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_0.pod5
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_1.pod5
--rw-r--r--   0        0        0   111989 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
--rw-r--r--   0        0        0     5319 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml
--rw-r--r--   0        0        0     5944 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
--rwxr-xr-x   0        0        0     2603 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
--rwxr-xr-x   0        0        0     2597 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml
--rw-r--r--   0        0        0     5899 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
--rw-r--r--   0        0        0     4941 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv
--rw-r--r--   0        0        0    10950 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/spring/dummy_run_001.spring
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/spring/dummy_run_002.spring
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/spring/dummy_spring_meta_data.json
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
--rw-r--r--   0        0        0     5554 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/fluffy/SampleSheet.csv
--rw-r--r--   0        0        0      901 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/fluffy/deliverables.yaml
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/fluffy/multiqc_report.html
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/fluffy/summary.csv
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/gt/yellowhog.bcf
--rw-r--r--   0        0        0     5114 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/madeline/madeline.xml
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/case_file.txt
--rw-r--r--   0        0        0     3241 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
--rw-r--r--   0        0        0    21811 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/dna/store/case_config.yaml
--rw-r--r--   0        0        0    23364 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
--rw-r--r--   0        0        0    37367 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
--rw-r--r--   0        0        0       16 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
--rw-r--r--   0        0        0       16 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
--rw-r--r--   0        0        0       16 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
--rw-r--r--   0        0        0      123 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
--rw-r--r--   0        0        0    62741 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
--rw-r--r--   0        0        0    11242 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/rna/case_config.yaml
--rw-r--r--   0        0        0    12164 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
--rw-r--r--   0        0        0     5231 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
--rw-r--r--   0        0        0     9774 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/rna/store/case_config.yaml
--rw-r--r--   0        0        0     4624 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
--rw-r--r--   0        0        0    13666 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/sample_file.txt
--rw-r--r--   0        0        0     1885 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/scout/643594.config.yaml
--rw-r--r--   0        0        0     6027 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/scout/case_export.json
--rw-r--r--   0        0        0     9349 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/scout/export_causatives.json
--rw-r--r--   0        0        0     1315 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/scout/none_case_export.json
--rw-r--r--   0        0        0     3518 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/scout/other_sex_case.json
--rw-r--r--   0        0        0     8874 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/scout/panel_export.bed
--rw-r--r--   0        0        0     4169 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/scout/panel_export.csv
--rw-r--r--   0        0        0      619 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/SampleSheet.csv
--rw-r--r--   0        0        0    63569 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0    42478 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0    69708 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0       42 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/apps/shipping/scout-deploy.yaml
--rw-r--r--   0        0        0     1036 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/cgweb_orders/balsamic.json
--rw-r--r--   0        0        0     1104 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/cgweb_orders/fastq.json
--rw-r--r--   0        0        0     1313 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/cgweb_orders/metagenome.json
--rw-r--r--   0        0        0     3038 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/cgweb_orders/microsalt.json
--rw-r--r--   0        0        0     3705 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/cgweb_orders/mip.json
--rw-r--r--   0        0        0     1364 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/cgweb_orders/mip_rna.json
--rw-r--r--   0        0        0     2125 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/cgweb_orders/rml.json
--rw-r--r--   0        0        0     1368 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/cgweb_orders/rnafusion.json
--rw-r--r--   0        0        0     4684 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/cgweb_orders/sarscov2.json
--rw-r--r--   0        0        0     5609 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/data/SampleSheet.csv
--rw-r--r--   0        0        0      511 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/data/bcl_convert_sample_sheet.csv
--rw-r--r--   0        0        0   258048 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/data/cgfixture.db
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/data/fastq.fastq.gz
--rw-r--r--   0        0        0    49152 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/data/hkstore.db
--rw-r--r--   0        0        0       73 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/data/yellowhog/pedigree.yaml
--rw-r--r--   0        0        0       76 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/io/casava_five_parts.fastq.gz
--rw-r--r--   0        0        0       90 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/io/casava_seven_parts.fastq.gz
--rw-r--r--   0        0        0       96 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/io/casava_ten_parts.fastq.gz
--rw-r--r--   0        0        0      153 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/io/example.csv
--rw-r--r--   0        0        0       46 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/io/example.gz
--rw-r--r--   0        0        0      147 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/io/example.tsv
--rw-r--r--   0        0        0       20 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/io/example.txt
--rw-r--r--   0        0        0       20 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/io/example2.txt
--rw-r--r--   0        0        0      582 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/io/example_json.json
--rw-r--r--   0        0        0      103 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/io/example_xml.xml
--rw-r--r--   0        0        0       20 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/meta/qc_metrics/file_with_right_tags.json
--rw-r--r--   0        0        0       20 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/meta/qc_metrics/file_without_right_tags.json
--rw-r--r--   0        0        0   156910 2024-04-25 12:07:50.811334 cg-60.4.1/tests/fixtures/orderforms/1508.30.balsamic.xlsx
--rw-r--r--   0        0        0   156770 2024-04-25 12:07:50.811334 cg-60.4.1/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx
--rw-r--r--   0        0        0   156737 2024-04-25 12:07:50.811334 cg-60.4.1/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx
--rw-r--r--   0        0        0   156582 2024-04-25 12:07:50.811334 cg-60.4.1/tests/fixtures/orderforms/1508.30.fastq.xlsx
--rw-r--r--   0        0        0   155627 2024-04-25 12:07:50.811334 cg-60.4.1/tests/fixtures/orderforms/1508.30.metagenome.xlsx
--rw-r--r--   0        0        0   156850 2024-04-25 12:07:50.811334 cg-60.4.1/tests/fixtures/orderforms/1508.30.mip.xlsx
--rw-r--r--   0        0        0   258580 2024-04-25 12:07:50.811334 cg-60.4.1/tests/fixtures/orderforms/1508.30.mip_rna.xlsx
--rw-r--r--   0        0        0   258342 2024-04-25 12:07:50.815335 cg-60.4.1/tests/fixtures/orderforms/1508.30.rnafusion.xlsx
--rw-r--r--   0        0        0    82677 2024-04-25 12:07:50.815335 cg-60.4.1/tests/fixtures/orderforms/1603.11.microbial.xlsx
--rw-r--r--   0        0        0   149394 2024-04-25 12:07:50.815335 cg-60.4.1/tests/fixtures/orderforms/1604.17.rml.xlsx
--rw-r--r--   0        0        0   223184 2024-04-25 12:07:50.815335 cg-60.4.1/tests/fixtures/orderforms/2184.9.sarscov2.xlsx
--rw-r--r--   0        0        0    18639 2024-04-25 12:07:50.815335 cg-60.4.1/tests/fixtures/orderforms/NIPT-json.json
--rw-r--r--   0        0        0     6052 2024-04-25 12:07:50.815335 cg-60.4.1/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
--rw-r--r--   0        0        0     6611 2024-04-25 12:07:50.815335 cg-60.4.1/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
--rw-r--r--   0        0        0     1417 2024-04-25 12:07:50.815335 cg-60.4.1/tests/fixtures/report/case_data.json
--rw-r--r--   0        0        0     1109 2024-04-25 12:07:50.815335 cg-60.4.1/tests/fixtures/report/lims_exported_samples.json
--rw-r--r--   0        0        0     1562 2024-04-25 12:07:50.815335 cg-60.4.1/tests/fixtures/report/lims_family.json
--rw-r--r--   0        0        0     3296 2024-04-25 12:07:50.815335 cg-60.4.1/tests/io/conftest.py
--rw-r--r--   0        0        0      431 2024-04-25 12:07:50.815335 cg-60.4.1/tests/io/test_io_config.py
--rw-r--r--   0        0        0     8639 2024-04-25 12:07:50.815335 cg-60.4.1/tests/io/test_io_controller.py
--rw-r--r--   0        0        0     3877 2024-04-25 12:07:50.815335 cg-60.4.1/tests/io/test_io_csv.py
--rw-r--r--   0        0        0      482 2024-04-25 12:07:50.815335 cg-60.4.1/tests/io/test_io_gzip.py
--rw-r--r--   0        0        0     1779 2024-04-25 12:07:50.815335 cg-60.4.1/tests/io/test_io_json.py
--rw-r--r--   0        0        0     2914 2024-04-25 12:07:50.815335 cg-60.4.1/tests/io/test_io_txt.py
--rw-r--r--   0        0        0     1027 2024-04-25 12:07:50.815335 cg-60.4.1/tests/io/test_io_xml.py
--rw-r--r--   0        0        0     2131 2024-04-25 12:07:50.815335 cg-60.4.1/tests/io/test_io_yaml.py
--rw-r--r--   0        0        0     1233 2024-04-25 12:07:50.815335 cg-60.4.1/tests/io/test_validate_path.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/archive/__init__.py
--rw-r--r--   0        0        0    13131 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/archive/conftest.py
--rw-r--r--   0        0        0    16858 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/archive/test_archive_api.py
--rw-r--r--   0        0        0    10246 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/archive/test_archive_cli.py
--rw-r--r--   0        0        0    15766 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/archive/test_archiving.py
--rw-r--r--   0        0        0     3807 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/backup/conftest.py
--rw-r--r--   0        0        0    26368 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/backup/test_meta_backup.py
--rw-r--r--   0        0        0    10055 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/backup/test_meta_pdc.py
--rw-r--r--   0        0        0    12546 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/clean/conftest.py
--rw-r--r--   0        0        0    16944 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/clean/test_clean_flow_cells_api.py
--rw-r--r--   0        0        0     2286 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/clean/test_clean_retrieved_spring_files.py
--rw-r--r--   0        0        0     7691 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/compress/conftest.py
--rw-r--r--   0        0        0     7961 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/compress/test_clean_fastq.py
--rw-r--r--   0        0        0     1778 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/compress/test_compress_files.py
--rw-r--r--   0        0        0     3644 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/compress/test_compress_meta_fastq.py
--rw-r--r--   0        0        0     1180 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/compress/test_decompress_spring_meta.py
--rw-r--r--   0        0        0     7013 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/compress/test_meta_compress_update_hk.py
--rw-r--r--   0        0        0     8269 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/conftest.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/deliver/__init__.py
--rw-r--r--   0        0        0     3471 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/deliver/conftest.py
--rw-r--r--   0        0        0     5533 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/deliver/test_deliver_ticket.py
--rw-r--r--   0        0        0    10277 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/deliver/test_delivery_api.py
--rw-r--r--   0        0        0     1057 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/deliver/test_fastq_path_generator.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/delivery/__init__.py
--rw-r--r--   0        0        0    16660 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/delivery/test_delivery_api.py
--rw-r--r--   0        0        0     8874 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/demultiplex/conftest.py
--rw-r--r--   0        0        0     5382 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/demultiplex/test_combine_sequencing_metrics.py
--rw-r--r--   0        0        0     8339 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/demultiplex/test_demux_post_processing.py
--rw-r--r--   0        0        0    12406 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/demultiplex/test_housekeeper_storage_functions.py
--rw-r--r--   0        0        0     4392 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/demultiplex/test_status_db_storage_functions.py
--rw-r--r--   0        0        0    22837 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/demultiplex/test_utils.py
--rw-r--r--   0        0        0     6193 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/demultiplex/test_validation.py
--rw-r--r--   0        0        0     4943 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/encryption/conftest.py
--rw-r--r--   0        0        0    18133 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/encryption/test_encryption.py
--rw-r--r--   0        0        0     3122 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/observations/conftest.py
--rw-r--r--   0        0        0    16164 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/observations/test_meta_upload_observations.py
--rw-r--r--   0        0        0     4974 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/orders/conftest.py
--rw-r--r--   0        0        0     1749 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/orders/test_PoolSubmitter_validate_order.py
--rw-r--r--   0        0        0     1470 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
--rw-r--r--   0        0        0     1768 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/orders/test_SarsCov2Submitter_store_order.py
--rw-r--r--   0        0        0     2032 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
--rw-r--r--   0        0        0    19783 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/orders/test_meta_orders_api.py
--rw-r--r--   0        0        0     7086 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/orders/test_meta_orders_lims.py
--rw-r--r--   0        0        0    29515 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/orders/test_meta_orders_status.py
--rw-r--r--   0        0        0     1677 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/orders/test_rnafusion_submitter.py
--rw-r--r--   0        0        0     1068 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/orders/test_ticket_handler.py
--rw-r--r--   0        0        0     4336 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/qc_metrics/conftest.py
--rw-r--r--   0        0        0     1972 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/qc_metrics/test_collect_qc_metrics.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/report/__init__.py
--rw-r--r--   0        0        0     6512 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/report/conftest.py
--rw-r--r--   0        0        0      434 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/report/helper.py
--rw-r--r--   0        0        0     2604 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/report/test_balsamic_api.py
--rw-r--r--   0        0        0     4056 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/report/test_field_validators.py
--rw-r--r--   0        0        0     2858 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/report/test_mip_dna_api.py
--rw-r--r--   0        0        0    16042 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/report/test_report_api.py
--rw-r--r--   0        0        0     1365 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/report/test_rnafusion_api.py
--rw-r--r--   0        0        0     1250 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/report/test_tomte_api.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/rsync/__init__.py
--rw-r--r--   0        0        0      916 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/rsync/conftest.py
--rw-r--r--   0        0        0     9442 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/rsync/test_rsync.py
--rw-r--r--   0        0        0     3147 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/test_invoice.py
--rw-r--r--   0        0        0     1220 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/transfer/conftest.py
--rw-r--r--   0        0        0     9892 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/transfer/test_external_data.py
--rw-r--r--   0        0        0     4395 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/transfer/test_meta_transfer_lims.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/__init__.py
--rw-r--r--   0        0        0     2210 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/balsamic/test_balsamic.py
--rw-r--r--   0        0        0     4002 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/conftest.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/gisaid/__init__.py
--rw-r--r--   0        0        0     2557 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/gisaid/fixtures/four_samples.csv
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
--rw-r--r--   0        0        0      211 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
--rw-r--r--   0        0        0      371 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/mutacc/__init__.py
--rw-r--r--   0        0        0     3684 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/mutacc/conftest.py
--rw-r--r--   0        0        0     4188 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
--rw-r--r--   0        0        0     1149 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/nipt/conftest.py
--rw-r--r--   0        0        0     1683 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/nipt/test_models.py
--rw-r--r--   0        0        0     1242 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/nipt/test_nipt_upload_api.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/scout/__init__.py
--rw-r--r--   0        0        0    23954 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/scout/conftest.py
--rw-r--r--   0        0        0     4734 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/scout/test_generate_load_config.py
--rw-r--r--   0        0        0     4182 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/scout/test_meta_upload_scoutapi.py
--rw-r--r--   0        0        0    33260 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
--rw-r--r--   0        0        0     7372 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/scout/test_scout_config_builder.py
--rw-r--r--   0        0        0     2511 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/test_meta_upload_coverage.py
--rw-r--r--   0        0        0     1473 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/test_upload_api.py
--rw-r--r--   0        0        0     2547 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/test_upload_genotypes_api.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/workflow/__init__.py
--rw-r--r--   0        0        0    10262 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/workflow/conftest.py
--rw-r--r--   0        0        0     3679 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/workflow/microsalt/conftest.py
--rw-r--r--   0        0        0      318 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/workflow/microsalt/test_parsing_metrics.py
--rw-r--r--   0        0        0     3759 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/workflow/microsalt/test_quality_controller.py
--rw-r--r--   0        0        0    14367 2024-04-25 12:07:50.823335 cg-60.4.1/tests/meta/workflow/microsalt/test_quality_controller_utils.py
--rw-r--r--   0        0        0      825 2024-04-25 12:07:50.823335 cg-60.4.1/tests/meta/workflow/microsalt/test_report_generation.py
--rw-r--r--   0        0        0    20860 2024-04-25 12:07:50.823335 cg-60.4.1/tests/meta/workflow/test_analysis.py
--rw-r--r--   0        0        0     7934 2024-04-25 12:07:50.823335 cg-60.4.1/tests/meta/workflow/test_balsamic.py
--rw-r--r--   0        0        0     3034 2024-04-25 12:07:50.823335 cg-60.4.1/tests/meta/workflow/test_fastq.py
--rw-r--r--   0        0        0     1532 2024-04-25 12:07:50.823335 cg-60.4.1/tests/meta/workflow/test_microsalt.py
--rw-r--r--   0        0        0     2721 2024-04-25 12:07:50.823335 cg-60.4.1/tests/meta/workflow/test_nf_analysis.py
--rw-r--r--   0        0        0     7741 2024-04-25 12:07:50.823335 cg-60.4.1/tests/meta/workflow/test_prepare_fastq_api.py
--rw-r--r--   0        0        0     1920 2024-04-25 12:07:50.823335 cg-60.4.1/tests/meta/workflow/test_raredisease.py
--rw-r--r--   0        0        0     1674 2024-04-25 12:07:50.823335 cg-60.4.1/tests/meta/workflow/test_rnafusion.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/__init__.py
--rw-r--r--   0        0        0     1168 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/balsamic_analysis_mock.py
--rw-r--r--   0        0        0     3500 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/crunchy.py
--rw-r--r--   0        0        0    21778 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/hk_mock.py
--rw-r--r--   0        0        0     4106 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/limsmock.py
--rw-r--r--   0        0        0      572 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/madeline.py
--rw-r--r--   0        0        0     1297 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/mip_analysis_mock.py
--rw-r--r--   0        0        0     1525 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/osticket.py
--rw-r--r--   0        0        0     3239 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/process_mock.py
--rw-r--r--   0        0        0     4713 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/report.py
--rw-r--r--   0        0        0     3915 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/scout.py
--rw-r--r--   0        0        0      750 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/store_model.py
--rw-r--r--   0        0        0     1620 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/tb_mock.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/balsamic/__init__.py
--rw-r--r--   0        0        0     1194 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/balsamic/conftest.py
--rw-r--r--   0        0        0     1030 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/balsamic/test_balsamic_analysis.py
--rw-r--r--   0        0        0     1050 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/conftest.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/demultiplexing/__init__.py
--rw-r--r--   0        0        0    11446 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/demultiplexing/test_run_parameters.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/downsample/__init__.py
--rw-r--r--   0        0        0     2096 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/downsample/test_down_sample_meta_data.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/flow_cell/__init__.py
--rw-r--r--   0        0        0     6659 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/flow_cell/test_flowcell_model.py
--rw-r--r--   0        0        0     6637 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/mip/conftest.py
--rw-r--r--   0        0        0     1239 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/mip/test_mip_analysis.py
--rw-r--r--   0        0        0     2348 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/mip/test_mip_config.py
--rw-r--r--   0        0        0     6392 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/mip/test_mip_metrics_deliverables.py
--rw-r--r--   0        0        0     3959 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/mip/test_mip_sample_info.py
--rw-r--r--   0        0        0     3314 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/nextflow/test_nextflow_deliver.py
--rw-r--r--   0        0        0     1602 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/observations/conftest.py
--rw-r--r--   0        0        0     2579 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/observations/test_observations_input_files.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/report/__init__.py
--rw-r--r--   0        0        0     7327 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/report/test_validators.py
--rw-r--r--   0        0        0     3855 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/rnafusion/test_rnafusion_sample.py
--rw-r--r--   0        0        0     1374 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/test_cg_models.py
--rw-r--r--   0        0        0      990 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/test_compression_data.py
--rw-r--r--   0        0        0      729 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/test_fastq.py
--rw-r--r--   0        0        0     2860 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/test_file_data.py
--rw-r--r--   0        0        0     4539 2024-04-25 12:07:50.823335 cg-60.4.1/tests/server/conftest.py
--rw-r--r--   0        0        0     3135 2024-04-25 12:07:50.823335 cg-60.4.1/tests/server/endpoints/test_delivery_message_endpoint.py
--rw-r--r--   0        0        0     3239 2024-04-25 12:07:50.823335 cg-60.4.1/tests/server/endpoints/test_orders_endpoint.py
--rw-r--r--   0        0        0      271 2024-04-25 12:07:50.823335 cg-60.4.1/tests/server/test_server_auto.py
--rw-r--r--   0        0        0     1047 2024-04-25 12:07:50.823335 cg-60.4.1/tests/services/fastq_file_service/conftest.py
--rw-r--r--   0        0        0     3634 2024-04-25 12:07:50.823335 cg-60.4.1/tests/services/fastq_file_service/test_fastq_file_service.py
--rw-r--r--   0        0        0     4861 2024-04-25 12:07:50.823335 cg-60.4.1/tests/services/orders/order_status_service/conftest.py
--rw-r--r--   0        0        0     2865 2024-04-25 12:07:50.823335 cg-60.4.1/tests/services/orders/order_status_service/test_order_summary_service.py
--rw-r--r--   0        0        0     9595 2024-04-25 12:07:50.823335 cg-60.4.1/tests/services/quality_controller/test_sequencing_quality_checks_utils.py
--rw-r--r--   0        0        0      318 2024-04-25 12:07:50.823335 cg-60.4.1/tests/small_helpers.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/api/__init__.py
--rw-r--r--   0        0        0     3032 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/api/conftest.py
--rw-r--r--   0        0        0     1557 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/api/test_base.py
--rw-r--r--   0        0        0    20096 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/conftest.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/crud/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/crud/add/__init__.py
--rw-r--r--   0        0        0     1497 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/crud/add/test_store_add_application_version.py
--rw-r--r--   0        0        0     3958 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/crud/add/test_store_add_base.py
--rw-r--r--   0        0        0     2502 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/crud/add/test_store_add_customer.py
--rw-r--r--   0        0        0     1704 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/crud/add/test_store_add_flow_celll.py
--rw-r--r--   0        0        0    12290 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/crud/conftest.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/crud/delete/__init__.py
--rw-r--r--   0        0        0     5611 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/crud/delete/test_delete.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/crud/read/__init__.py
--rw-r--r--   0        0        0    56077 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/crud/read/test_read.py
--rw-r--r--   0        0        0     5461 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/crud/read/test_read_analyses_to_clean.py
--rw-r--r--   0        0        0     3553 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/crud/read/test_read_analyses_to_delivery_report.py
--rw-r--r--   0        0        0    17328 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/crud/read/test_read_analysis.py
--rw-r--r--   0        0        0     2743 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/crud/read/test_read_application_version.py
--rw-r--r--   0        0        0     1105 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/crud/read/test_read_customer.py
--rw-r--r--   0        0        0     1530 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/crud/read/test_read_pool.py
--rw-r--r--   0        0        0    21503 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/crud/read/test_read_sample.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/crud/update/__init__.py
--rw-r--r--   0        0        0      737 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/crud/update/test_update.py
--rw-r--r--   0        0        0    11693 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_analyses_filters.py
--rw-r--r--   0        0        0     3397 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_application_filters.py
--rw-r--r--   0        0        0     2073 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_application_limitations_filters.py
--rw-r--r--   0        0        0    10452 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_application_version_filters.py
--rw-r--r--   0        0        0     2804 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_bed_filters.py
--rw-r--r--   0        0        0     2362 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_bed_version_filters.py
--rw-r--r--   0        0        0     3495 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_case_sample_filters.py
--rw-r--r--   0        0        0    39100 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_cases_filters.py
--rw-r--r--   0        0        0     1345 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_collaboration_filters.py
--rw-r--r--   0        0        0     2482 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_customer_filters.py
--rw-r--r--   0        0        0     5153 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_flow_cell_filters.py
--rw-r--r--   0        0        0     2226 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_invoice_filters.py
--rw-r--r--   0        0        0     5871 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_metrics_filters.py
--rw-r--r--   0        0        0     2404 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_organism_filters.py
--rw-r--r--   0        0        0     1804 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_panel_filters.py
--rw-r--r--   0        0        0     8720 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_pool_filters.py
--rw-r--r--   0        0        0    22875 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_samples_filters.py
--rw-r--r--   0        0        0     1576 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_user_filters.py
--rw-r--r--   0        0        0     2147 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/test_delivery.py
--rw-r--r--   0        0        0     4127 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/test_store_models.py
--rw-r--r--   0        0        0    37125 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store_helpers.py
--rw-r--r--   0        0        0     4930 2024-04-25 12:07:50.827335 cg-60.4.1/tests/test_copy_novaseqx_flow_cell.py
--rw-r--r--   0        0        0      911 2024-04-25 12:07:50.827335 cg-60.4.1/tests/test_store_helpers.py
--rw-r--r--   0        0        0        0 2024-04-25 12:07:50.827335 cg-60.4.1/tests/utils/__init__.py
--rw-r--r--   0        0        0     1754 2024-04-25 12:07:50.827335 cg-60.4.1/tests/utils/conftest.py
--rw-r--r--   0        0        0      371 2024-04-25 12:07:50.827335 cg-60.4.1/tests/utils/test_calculations.py
--rw-r--r--   0        0        0     2920 2024-04-25 12:07:50.827335 cg-60.4.1/tests/utils/test_commands.py
--rw-r--r--   0        0        0      953 2024-04-25 12:07:50.827335 cg-60.4.1/tests/utils/test_date.py
--rw-r--r--   0        0        0     1508 2024-04-25 12:07:50.827335 cg-60.4.1/tests/utils/test_dict.py
--rw-r--r--   0        0        0     7154 2024-04-25 12:07:50.827335 cg-60.4.1/tests/utils/test_dispatcher.py
--rw-r--r--   0        0        0     4100 2024-04-25 12:07:50.827335 cg-60.4.1/tests/utils/test_files.py
--rw-r--r--   0        0        0     1170 2024-04-25 12:07:50.827335 cg-60.4.1/tests/utils/test_time.py
--rw-r--r--   0        0        0     2366 2024-04-25 12:07:50.827335 cg-60.4.1/tests/utils/test_utils.py
--rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 cg-60.4.1/PKG-INFO
+-rw-r--r--   0        0        0     2686 2024-04-25 13:46:16.659785 cg-60.4.2/README.md
+-rw-r--r--   0        0        0       40 2024-04-25 13:46:16.663785 cg-60.4.2/cg/__init__.py
+-rw-r--r--   0        0        0      315 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/coverage/__init__.py
+-rw-r--r--   0        0        0     2940 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/coverage/api.py
+-rw-r--r--   0        0        0       56 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/crunchy/__init__.py
+-rw-r--r--   0        0        0    12783 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/crunchy/crunchy.py
+-rw-r--r--   0        0        0     4502 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/crunchy/files.py
+-rw-r--r--   0        0        0      430 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/crunchy/models.py
+-rw-r--r--   0        0        0      910 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/crunchy/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/demultiplex/__init__.py
+-rw-r--r--   0        0        0    11299 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/demultiplex/demultiplex_api.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/demultiplex/sample_sheet/__init__.py
+-rw-r--r--   0        0        0    11227 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/demultiplex/sample_sheet/api.py
+-rw-r--r--   0        0        0     2183 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/demultiplex/sample_sheet/index.py
+-rw-r--r--   0        0        0     7341 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py
+-rw-r--r--   0        0        0     3188 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py
+-rw-r--r--   0        0        0     7071 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/demultiplex/sample_sheet/sample_models.py
+-rw-r--r--   0        0        0     6076 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py
+-rw-r--r--   0        0        0     1372 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py
+-rw-r--r--   0        0        0     8092 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py
+-rw-r--r--   0        0        0      824 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/demultiplex/sample_sheet/validators.py
+-rw-r--r--   0        0        0      677 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/demultiplex/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/downsample/__init__.py
+-rw-r--r--   0        0        0     6160 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/downsample/downsample.py
+-rw-r--r--   0        0        0     2125 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/downsample/utils.py
+-rw-r--r--   0        0        0      298 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/environ.py
+-rw-r--r--   0        0        0     1741 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/gens.py
+-rw-r--r--   0        0        0     3419 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/gt.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/hermes/__init__.py
+-rw-r--r--   0        0        0     2249 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/hermes/hermes_api.py
+-rw-r--r--   0        0        0     1298 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/hermes/models.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/housekeeper/__init__.py
+-rw-r--r--   0        0        0    30395 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/housekeeper/hk.py
+-rw-r--r--   0        0        0      326 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/housekeeper/models.py
+-rw-r--r--   0        0        0       32 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/invoice/__init__.py
+-rw-r--r--   0        0        0     4804 2024-04-25 13:46:16.663785 cg-60.4.2/cg/apps/invoice/render.py
+-rw-r--r--   0        0        0   113467 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/invoice/templates/KI_pool_invoice.xlsx
+-rw-r--r--   0        0        0    75562 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/invoice/templates/KI_sample_invoice.xlsx
+-rw-r--r--   0        0        0   113512 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
+-rw-r--r--   0        0        0    75459 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
+-rw-r--r--   0        0        0       25 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/lims/__init__.py
+-rw-r--r--   0        0        0    18873 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/lims/api.py
+-rw-r--r--   0        0        0     2652 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/lims/batch.py
+-rw-r--r--   0        0        0     8129 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/lims/order.py
+-rw-r--r--   0        0        0     3118 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/lims/sample_sheet.py
+-rw-r--r--   0        0        0     4866 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/loqus.py
+-rw-r--r--   0        0        0       35 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/madeline/__init__.py
+-rw-r--r--   0        0        0     3213 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/madeline/api.py
+-rw-r--r--   0        0        0       23 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/mip/__init__.py
+-rw-r--r--   0        0        0     3564 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/mip/confighandler.py
+-rw-r--r--   0        0        0     2207 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/mutacc_auto.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/orderform/__init__.py
+-rw-r--r--   0        0        0     9498 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/orderform/excel_orderform_parser.py
+-rw-r--r--   0        0        0     3051 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/orderform/json_orderform_parser.py
+-rw-r--r--   0        0        0     6419 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/orderform/orderform_parser.py
+-rw-r--r--   0        0        0      252 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/orderform/utils.py
+-rw-r--r--   0        0        0     2537 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/osticket.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/scout/__init__.py
+-rw-r--r--   0        0        0     3177 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/scout/scout_export.py
+-rw-r--r--   0        0        0    11108 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/scout/scoutapi.py
+-rw-r--r--   0        0        0      444 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/scout/validators.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0        0        0     3457 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/sequencing_metrics_parser/api.py
+-rw-r--r--   0        0        0      923 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/sequencing_metrics_parser/models.py
+-rw-r--r--   0        0        0     6658 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/sequencing_metrics_parser/parser.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/slurm/__init__.py
+-rw-r--r--   0        0        0     1277 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/slurm/sbatch.py
+-rw-r--r--   0        0        0     3559 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/slurm/slurm_api.py
+-rw-r--r--   0        0        0       32 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/tb/__init__.py
+-rw-r--r--   0        0        0     7995 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/tb/api.py
+-rw-r--r--   0        0        0      152 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/tb/dto/create_job_request.py
+-rw-r--r--   0        0        0      250 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/tb/dto/summary_response.py
+-rw-r--r--   0        0        0     1305 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/tb/models.py
+-rw-r--r--   0        0        0      305 2024-04-25 13:46:16.667785 cg-60.4.2/cg/apps/tb/validators.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/__init__.py
+-rw-r--r--   0        0        0    11558 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/add.py
+-rw-r--r--   0        0        0     2653 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/archive.py
+-rw-r--r--   0        0        0    10118 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/backup.py
+-rw-r--r--   0        0        0     3852 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/base.py
+-rw-r--r--   0        0        0    10506 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/clean.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/compress/__init__.py
+-rw-r--r--   0        0        0     2135 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/compress/base.py
+-rw-r--r--   0        0        0     6706 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/compress/fastq.py
+-rw-r--r--   0        0        0     8163 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/compress/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/delete/__init__.py
+-rw-r--r--   0        0        0      564 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/delete/base.py
+-rw-r--r--   0        0        0     4603 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/delete/case.py
+-rw-r--r--   0        0        0     1884 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/delete/cases.py
+-rw-r--r--   0        0        0     2633 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/delete/observations.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/deliver/__init__.py
+-rw-r--r--   0        0        0     6030 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/deliver/base.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/demultiplex/__init__.py
+-rw-r--r--   0        0        0      829 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/demultiplex/base.py
+-rw-r--r--   0        0        0     4905 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py
+-rw-r--r--   0        0        0     7726 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/demultiplex/demux.py
+-rw-r--r--   0        0        0     1473 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/demultiplex/finish.py
+-rw-r--r--   0        0        0     3119 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/demultiplex/sample_sheet.py
+-rw-r--r--   0        0        0     2995 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/downsample.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/generate/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/generate/base.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/generate/report/__init__.py
+-rw-r--r--   0        0        0     4636 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/generate/report/base.py
+-rw-r--r--   0        0        0      854 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/generate/report/options.py
+-rw-r--r--   0        0        0     5340 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/generate/report/utils.py
+-rw-r--r--   0        0        0     8327 2024-04-25 13:46:16.667785 cg-60.4.2/cg/cli/get.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/set/__init__.py
+-rw-r--r--   0        0        0     9856 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/set/base.py
+-rw-r--r--   0        0        0     4384 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/set/case.py
+-rw-r--r--   0        0        0     2595 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/set/cases.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/store/__init__.py
+-rw-r--r--   0        0        0     1093 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/store/base.py
+-rw-r--r--   0        0        0     6191 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/store/store.py
+-rw-r--r--   0        0        0     1761 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/transfer.py
+-rw-r--r--   0        0        0        1 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/upload/__init__.py
+-rw-r--r--   0        0        0     5706 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/upload/base.py
+-rw-r--r--   0        0        0     5503 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/upload/clinical_delivery.py
+-rw-r--r--   0        0        0     1175 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/upload/coverage.py
+-rw-r--r--   0        0        0     1528 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/upload/delivery_report.py
+-rw-r--r--   0        0        0     4022 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/upload/fohm.py
+-rw-r--r--   0        0        0     1463 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/upload/genotype.py
+-rw-r--r--   0        0        0     1885 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/upload/gens.py
+-rw-r--r--   0        0        0      584 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/upload/gisaid.py
+-rw-r--r--   0        0        0     2645 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/upload/mutacc.py
+-rw-r--r--   0        0        0       23 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/upload/nipt/__init__.py
+-rw-r--r--   0        0        0     3006 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/upload/nipt/base.py
+-rw-r--r--   0        0        0     2275 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/upload/nipt/ftp.py
+-rw-r--r--   0        0        0     1596 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/upload/nipt/statina.py
+-rw-r--r--   0        0        0      112 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/upload/observations/__init__.py
+-rw-r--r--   0        0        0     2672 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/upload/observations/observations.py
+-rw-r--r--   0        0        0     2904 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/upload/observations/utils.py
+-rw-r--r--   0        0        0     9970 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/upload/scout.py
+-rw-r--r--   0        0        0      650 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/upload/utils.py
+-rw-r--r--   0        0        0     1667 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/upload/validate.py
+-rw-r--r--   0        0        0      105 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/utils.py
+-rw-r--r--   0        0        0       18 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/balsamic/__init__.py
+-rw-r--r--   0        0        0     8925 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/balsamic/base.py
+-rw-r--r--   0        0        0     1980 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/balsamic/options.py
+-rw-r--r--   0        0        0      881 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/balsamic/pon.py
+-rw-r--r--   0        0        0     1162 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/balsamic/qc.py
+-rw-r--r--   0        0        0     1177 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/balsamic/umi.py
+-rw-r--r--   0        0        0     1342 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/base.py
+-rw-r--r--   0        0        0    12379 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/commands.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/fastq/__init__.py
+-rw-r--r--   0        0        0     1490 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/fastq/base.py
+-rw-r--r--   0        0        0     1787 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/fastq/fastq_service.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0        0        0     4177 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/fluffy/base.py
+-rw-r--r--   0        0        0       22 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/jasen/__init__.py
+-rw-r--r--   0        0        0      535 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/jasen/base.py
+-rw-r--r--   0        0        0       22 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/microsalt/__init__.py
+-rw-r--r--   0        0        0     7810 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/microsalt/base.py
+-rw-r--r--   0        0        0       22 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/mip/__init__.py
+-rw-r--r--   0        0        0     6596 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/mip/base.py
+-rw-r--r--   0        0        0     1268 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/mip/options.py
+-rw-r--r--   0        0        0       22 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/mip_dna/__init__.py
+-rw-r--r--   0        0        0     1013 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/mip_dna/base.py
+-rw-r--r--   0        0        0       22 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/mip_rna/__init__.py
+-rw-r--r--   0        0        0      916 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/mip_rna/base.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/mutant/__init__.py
+-rw-r--r--   0        0        0     3413 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/mutant/base.py
+-rw-r--r--   0        0        0     9010 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/nf_analysis.py
+-rw-r--r--   0        0        0       22 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/raredisease/__init__.py
+-rw-r--r--   0        0        0     2210 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/raredisease/base.py
+-rw-r--r--   0        0        0       22 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/rnafusion/__init__.py
+-rw-r--r--   0        0        0     1179 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/rnafusion/base.py
+-rw-r--r--   0        0        0       22 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/taxprofiler/__init__.py
+-rw-r--r--   0        0        0     1211 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/taxprofiler/base.py
+-rw-r--r--   0        0        0     1111 2024-04-25 13:46:16.671785 cg-60.4.2/cg/cli/workflow/tomte/base.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.671785 cg-60.4.2/cg/clients/__init__.py
+-rw-r--r--   0        0        0     1363 2024-04-25 13:46:16.671785 cg-60.4.2/cg/clients/arnold/api.py
+-rw-r--r--   0        0        0      160 2024-04-25 13:46:16.671785 cg-60.4.2/cg/clients/arnold/dto/create_case_request.py
+-rw-r--r--   0        0        0      384 2024-04-25 13:46:16.671785 cg-60.4.2/cg/clients/arnold/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.671785 cg-60.4.2/cg/clients/janus/__init__.py
+-rw-r--r--   0        0        0     1246 2024-04-25 13:46:16.671785 cg-60.4.2/cg/clients/janus/api.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.671785 cg-60.4.2/cg/clients/janus/dto/__init__.py
+-rw-r--r--   0        0        0      503 2024-04-25 13:46:16.671785 cg-60.4.2/cg/clients/janus/dto/create_qc_metrics_request.py
+-rw-r--r--   0        0        0      420 2024-04-25 13:46:16.671785 cg-60.4.2/cg/clients/janus/exceptions.py
+-rw-r--r--   0        0        0      937 2024-04-25 13:46:16.671785 cg-60.4.2/cg/constants/__init__.py
+-rw-r--r--   0        0        0      253 2024-04-25 13:46:16.671785 cg-60.4.2/cg/constants/archiving.py
+-rw-r--r--   0        0        0       35 2024-04-25 13:46:16.671785 cg-60.4.2/cg/constants/backup.py
+-rw-r--r--   0        0        0      769 2024-04-25 13:46:16.671785 cg-60.4.2/cg/constants/bcl_convert_metrics.py
+-rw-r--r--   0        0        0      469 2024-04-25 13:46:16.671785 cg-60.4.2/cg/constants/compression.py
+-rw-r--r--   0        0        0     6613 2024-04-25 13:46:16.671785 cg-60.4.2/cg/constants/constants.py
+-rw-r--r--   0        0        0     6033 2024-04-25 13:46:16.671785 cg-60.4.2/cg/constants/delivery.py
+-rw-r--r--   0        0        0     7321 2024-04-25 13:46:16.671785 cg-60.4.2/cg/constants/demultiplexing.py
+-rw-r--r--   0        0        0     1422 2024-04-25 13:46:16.671785 cg-60.4.2/cg/constants/encryption.py
+-rw-r--r--   0        0        0      372 2024-04-25 13:46:16.671785 cg-60.4.2/cg/constants/extraction.py
+-rw-r--r--   0        0        0     2157 2024-04-25 13:46:16.671785 cg-60.4.2/cg/constants/gene_panel.py
+-rw-r--r--   0        0        0     6704 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/housekeeper_tags.py
+-rw-r--r--   0        0        0       95 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/invoice.py
+-rw-r--r--   0        0        0     5815 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/lims.py
+-rw-r--r--   0        0        0      743 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/metrics.py
+-rw-r--r--   0        0        0      231 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/nanopore_files.py
+-rw-r--r--   0        0        0      650 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/nextflow.py
+-rw-r--r--   0        0        0     1529 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/nf_analysis.py
+-rw-r--r--   0        0        0       19 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/nipt.py
+-rw-r--r--   0        0        0     2257 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/observations.py
+-rw-r--r--   0        0        0     1216 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/orderforms.py
+-rw-r--r--   0        0        0       96 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/paths.py
+-rw-r--r--   0        0        0      266 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/pdc.py
+-rw-r--r--   0        0        0      160 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/pedigree.py
+-rw-r--r--   0        0        0     1044 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/priority.py
+-rw-r--r--   0        0        0       79 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/process.py
+-rw-r--r--   0        0        0     5474 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/report.py
+-rw-r--r--   0        0        0      569 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/sample_sources.py
+-rw-r--r--   0        0        0     3111 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/scout.py
+-rw-r--r--   0        0        0     1669 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/sequencing.py
+-rw-r--r--   0        0        0      313 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/slurm.py
+-rw-r--r--   0        0        0      529 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/subject.py
+-rw-r--r--   0        0        0       55 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/symbols.py
+-rw-r--r--   0        0        0      435 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/tb.py
+-rw-r--r--   0        0        0      161 2024-04-25 13:46:16.675785 cg-60.4.2/cg/constants/time.py
+-rw-r--r--   0        0        0     6639 2024-04-25 13:46:16.675785 cg-60.4.2/cg/exc.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.675785 cg-60.4.2/cg/io/__init__.py
+-rw-r--r--   0        0        0     1037 2024-04-25 13:46:16.675785 cg-60.4.2/cg/io/api.py
+-rw-r--r--   0        0        0      621 2024-04-25 13:46:16.675785 cg-60.4.2/cg/io/config.py
+-rw-r--r--   0        0        0     2978 2024-04-25 13:46:16.675785 cg-60.4.2/cg/io/controller.py
+-rw-r--r--   0        0        0     1763 2024-04-25 13:46:16.675785 cg-60.4.2/cg/io/csv.py
+-rw-r--r--   0        0        0      210 2024-04-25 13:46:16.675785 cg-60.4.2/cg/io/gzip.py
+-rw-r--r--   0        0        0      662 2024-04-25 13:46:16.675785 cg-60.4.2/cg/io/json.py
+-rw-r--r--   0        0        0      525 2024-04-25 13:46:16.675785 cg-60.4.2/cg/io/png.py
+-rw-r--r--   0        0        0     1094 2024-04-25 13:46:16.675785 cg-60.4.2/cg/io/txt.py
+-rw-r--r--   0        0        0      552 2024-04-25 13:46:16.675785 cg-60.4.2/cg/io/validate_path.py
+-rw-r--r--   0        0        0     1289 2024-04-25 13:46:16.675785 cg-60.4.2/cg/io/xml.py
+-rw-r--r--   0        0        0     1153 2024-04-25 13:46:16.675785 cg-60.4.2/cg/io/yaml.py
+-rw-r--r--   0        0        0      281 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/archive/__init__.py
+-rw-r--r--   0        0        0    15193 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/archive/archive.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/archive/ddn/__init__.py
+-rw-r--r--   0        0        0     1727 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/archive/ddn/constants.py
+-rw-r--r--   0        0        0    10852 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/archive/ddn/ddn_data_flow_client.py
+-rw-r--r--   0        0        0     3704 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/archive/ddn/models.py
+-rw-r--r--   0        0        0     1250 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/archive/ddn/utils.py
+-rw-r--r--   0        0        0     2024 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/archive/models.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/backup/__init__.py
+-rw-r--r--   0        0        0    17426 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/backup/backup.py
+-rw-r--r--   0        0        0     5397 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/backup/pdc.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/clean/__init__.py
+-rw-r--r--   0        0        0     3901 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/clean/api.py
+-rw-r--r--   0        0        0     7738 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/clean/clean_flow_cells.py
+-rw-r--r--   0        0        0     1841 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/clean/clean_retrieved_spring_files.py
+-rw-r--r--   0        0        0       34 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/compress/__init__.py
+-rw-r--r--   0        0        0    14557 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/compress/compress.py
+-rw-r--r--   0        0        0     4947 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/compress/files.py
+-rw-r--r--   0        0        0       77 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/deliver/__init__.py
+-rw-r--r--   0        0        0    14905 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/deliver/deliver.py
+-rw-r--r--   0        0        0     4502 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/deliver/deliver_ticket.py
+-rw-r--r--   0        0        0      904 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/deliver/fastq_path_generator.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/delivery/__init__.py
+-rw-r--r--   0        0        0     8458 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/delivery/delivery.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/demultiplex/__init__.py
+-rw-r--r--   0        0        0     2592 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/demultiplex/combine_sequencing_metrics.py
+-rw-r--r--   0        0        0     5719 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/demultiplex/demux_post_processing.py
+-rw-r--r--   0        0        0     4135 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/demultiplex/files.py
+-rw-r--r--   0        0        0     7777 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/demultiplex/housekeeper_storage_functions.py
+-rw-r--r--   0        0        0     6126 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/demultiplex/status_db_storage_functions.py
+-rw-r--r--   0        0        0    10690 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/demultiplex/utils.py
+-rw-r--r--   0        0        0     2855 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/demultiplex/validation.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/encryption/__init__.py
+-rw-r--r--   0        0        0    20271 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/encryption/encryption.py
+-rw-r--r--   0        0        0      537 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/encryption/sbatch.py
+-rw-r--r--   0        0        0    10922 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/invoice.py
+-rw-r--r--   0        0        0     2360 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/meta.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/observations/__init__.py
+-rw-r--r--   0        0        0     6008 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/observations/balsamic_observations_api.py
+-rw-r--r--   0        0        0     5277 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/observations/mip_dna_observations_api.py
+-rw-r--r--   0        0        0     5364 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/observations/observations_api.py
+-rw-r--r--   0        0        0       27 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/orders/__init__.py
+-rw-r--r--   0        0        0     3637 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/orders/api.py
+-rw-r--r--   0        0        0      121 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/orders/balsamic_qc_submitter.py
+-rw-r--r--   0        0        0      107 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/orders/balsamic_submitter.py
+-rw-r--r--   0        0        0      122 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/orders/balsamic_umi_submitter.py
+-rw-r--r--   0        0        0    15262 2024-04-25 13:46:16.675785 cg-60.4.2/cg/meta/orders/case_submitter.py
+-rw-r--r--   0        0        0     6102 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/orders/fastq_submitter.py
+-rw-r--r--   0        0        0      105 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/orders/fluffy_submitter.py
+-rw-r--r--   0        0        0     1254 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/orders/lims.py
+-rw-r--r--   0        0        0     5782 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/orders/metagenome_submitter.py
+-rw-r--r--   0        0        0     6337 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/orders/microbial_submitter.py
+-rw-r--r--   0        0        0      123 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/orders/microsalt_submitter.py
+-rw-r--r--   0        0        0      105 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/orders/mip_dna_submitter.py
+-rw-r--r--   0        0        0      105 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/orders/mip_rna_submitter.py
+-rw-r--r--   0        0        0     7761 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/orders/pool_submitter.py
+-rw-r--r--   0        0        0      102 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/orders/rml_submitter.py
+-rw-r--r--   0        0        0      718 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/orders/rnafusion_submitter.py
+-rw-r--r--   0        0        0     1268 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/orders/sars_cov_2_submitter.py
+-rw-r--r--   0        0        0     1754 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/orders/submitter.py
+-rw-r--r--   0        0        0     7880 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/orders/ticket_handler.py
+-rw-r--r--   0        0        0     4105 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/qc_metrics/collect_qc_metrics.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/__init__.py
+-rw-r--r--   0        0        0     8168 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/balsamic.py
+-rw-r--r--   0        0        0      562 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/balsamic_qc.py
+-rw-r--r--   0        0        0      717 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/balsamic_umi.py
+-rw-r--r--   0        0        0     4171 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/field_validators.py
+-rw-r--r--   0        0        0     6620 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/mip_dna.py
+-rw-r--r--   0        0        0    18543 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/report_api.py
+-rw-r--r--   0        0        0     5625 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/rnafusion.py
+-rw-r--r--   0        0        0     1911 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/templates/delivery-report.html
+-rw-r--r--   0        0        0     4236 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/templates/macros/data_analysis/data_analysis.html
+-rw-r--r--   0        0        0     1049 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/templates/macros/data_analysis/limitations.html
+-rw-r--r--   0        0        0     3351 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html
+-rw-r--r--   0        0        0     1364 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html
+-rw-r--r--   0        0        0      753 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html
+-rw-r--r--   0        0        0     3284 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html
+-rw-r--r--   0        0        0     3670 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html
+-rw-r--r--   0        0        0     2332 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/templates/macros/header.html
+-rw-r--r--   0        0        0     2066 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/templates/macros/order.html
+-rw-r--r--   0        0        0     2243 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/templates/macros/sample_prep.html
+-rw-r--r--   0        0        0      472 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/templates/macros/ticket_system.html
+-rw-r--r--   0        0        0     1165 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html
+-rw-r--r--   0        0        0     1538 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html
+-rw-r--r--   0        0        0      428 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/templates/macros/uploaded_files/rnafusion_uploaded_files.html
+-rw-r--r--   0        0        0     4266 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html
+-rw-r--r--   0        0        0       80 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/templates/partials/footer.html
+-rw-r--r--   0        0        0      172 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/templates/partials/signature.html
+-rw-r--r--   0        0        0   232803 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/templates/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0       33 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/templates/static/css/custom.css
+-rw-r--r--   0        0        0    30068 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/templates/static/images/SWEDAC_logo.png
+-rw-r--r--   0        0        0     3925 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/report/tomte.py
+-rw-r--r--   0        0        0       32 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/rsync/__init__.py
+-rw-r--r--   0        0        0    12291 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/rsync/rsync_api.py
+-rw-r--r--   0        0        0      387 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/rsync/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/tar/__init__.py
+-rw-r--r--   0        0        0     1694 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/tar/tar.py
+-rw-r--r--   0        0        0       71 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/transfer/__init__.py
+-rw-r--r--   0        0        0    10016 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/transfer/external_data.py
+-rw-r--r--   0        0        0     5814 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/transfer/lims.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/upload/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/upload/balsamic/__init__.py
+-rw-r--r--   0        0        0     3107 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/upload/balsamic/balsamic.py
+-rw-r--r--   0        0        0     2224 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/upload/coverage.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/upload/fohm/__init__.py
+-rw-r--r--   0        0        0    12102 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/upload/fohm/fohm.py
+-rw-r--r--   0        0        0       30 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/upload/gisaid/__init__.py
+-rw-r--r--   0        0        0      928 2024-04-25 13:46:16.679785 cg-60.4.2/cg/meta/upload/gisaid/constants.py
+-rw-r--r--   0        0        0    13521 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/upload/gisaid/gisaid.py
+-rw-r--r--   0        0        0     3312 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/upload/gisaid/models.py
+-rw-r--r--   0        0        0     5310 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/upload/gt.py
+-rw-r--r--   0        0        0      898 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/upload/microsalt/microsalt_upload_api.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/upload/mip/__init__.py
+-rw-r--r--   0        0        0     2546 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/upload/mip/mip_dna.py
+-rw-r--r--   0        0        0     1400 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/upload/mip/mip_rna.py
+-rw-r--r--   0        0        0     7294 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/upload/mutacc.py
+-rw-r--r--   0        0        0     1853 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/upload/nf_analysis.py
+-rw-r--r--   0        0        0       32 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/upload/nipt/__init__.py
+-rw-r--r--   0        0        0      696 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/upload/nipt/models.py
+-rw-r--r--   0        0        0     8106 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/upload/nipt/nipt.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/upload/scout/__init__.py
+-rw-r--r--   0        0        0     4009 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/upload/scout/balsamic_config_builder.py
+-rw-r--r--   0        0        0     1491 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/upload/scout/balsamic_umi_config_builder.py
+-rw-r--r--   0        0        0     3322 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/upload/scout/hk_tags.py
+-rw-r--r--   0        0        0     9103 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/upload/scout/mip_config_builder.py
+-rw-r--r--   0        0        0     3495 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/upload/scout/rnafusion_config_builder.py
+-rw-r--r--   0        0        0     7231 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/upload/scout/scout_config_builder.py
+-rw-r--r--   0        0        0    23146 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/upload/scout/uploadscoutapi.py
+-rw-r--r--   0        0        0     3197 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/upload/upload_api.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/__init__.py
+-rw-r--r--   0        0        0    31068 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/analysis.py
+-rw-r--r--   0        0        0    27751 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/balsamic.py
+-rw-r--r--   0        0        0     2700 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/balsamic_pon.py
+-rw-r--r--   0        0        0      553 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/balsamic_qc.py
+-rw-r--r--   0        0        0      556 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/balsamic_umi.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/downsample/__init__.py
+-rw-r--r--   0        0        0     3922 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/downsample/downsample.py
+-rw-r--r--   0        0        0      711 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/downsample/sbatch.py
+-rw-r--r--   0        0        0     8913 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/fastq.py
+-rw-r--r--   0        0        0    10603 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/fluffy.py
+-rw-r--r--   0        0        0      521 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/jasen.py
+-rw-r--r--   0        0        0       70 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/microsalt/__init__.py
+-rw-r--r--   0        0        0      116 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/microsalt/constants.py
+-rw-r--r--   0        0        0      174 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/microsalt/metrics_parser/__init__.py
+-rw-r--r--   0        0        0      366 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/microsalt/metrics_parser/metrics_parser.py
+-rw-r--r--   0        0        0      903 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/microsalt/metrics_parser/models.py
+-rw-r--r--   0        0        0    13173 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/microsalt/microsalt.py
+-rw-r--r--   0        0        0      113 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/microsalt/quality_controller/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/microsalt/quality_controller/models.py
+-rw-r--r--   0        0        0     5697 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/microsalt/quality_controller/quality_controller.py
+-rw-r--r--   0        0        0     1217 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/microsalt/quality_controller/report_generator.py
+-rw-r--r--   0        0        0     2373 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/microsalt/quality_controller/result_logger.py
+-rw-r--r--   0        0        0     5641 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/microsalt/quality_controller/utils.py
+-rw-r--r--   0        0        0     1220 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/microsalt/utils.py
+-rw-r--r--   0        0        0    12611 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/mip.py
+-rw-r--r--   0        0        0     2948 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/mip_dna.py
+-rw-r--r--   0        0        0     2124 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/mip_rna.py
+-rw-r--r--   0        0        0    10974 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/mutant.py
+-rw-r--r--   0        0        0    37948 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/nf_analysis.py
+-rw-r--r--   0        0        0     6161 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/nf_handlers.py
+-rw-r--r--   0        0        0     6357 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/prepare_fastq.py
+-rw-r--r--   0        0        0     4965 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/raredisease.py
+-rw-r--r--   0        0        0     5403 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/rnafusion.py
+-rw-r--r--   0        0        0     4607 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/taxprofiler.py
+-rw-r--r--   0        0        0     3576 2024-04-25 13:46:16.683785 cg-60.4.2/cg/meta/workflow/tomte.py
+-rw-r--r--   0        0        0      113 2024-04-25 13:46:16.683785 cg-60.4.2/cg/models/__init__.py
+-rw-r--r--   0        0        0      367 2024-04-25 13:46:16.683785 cg-60.4.2/cg/models/analysis.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.683785 cg-60.4.2/cg/models/balsamic/__init__.py
+-rw-r--r--   0        0        0      459 2024-04-25 13:46:16.683785 cg-60.4.2/cg/models/balsamic/analysis.py
+-rw-r--r--   0        0        0     4550 2024-04-25 13:46:16.683785 cg-60.4.2/cg/models/balsamic/config.py
+-rw-r--r--   0        0        0     1986 2024-04-25 13:46:16.683785 cg-60.4.2/cg/models/balsamic/metrics.py
+-rw-r--r--   0        0        0    17539 2024-04-25 13:46:16.683785 cg-60.4.2/cg/models/cg_config.py
+-rw-r--r--   0        0        0     4302 2024-04-25 13:46:16.683785 cg-60.4.2/cg/models/compression_data.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.683785 cg-60.4.2/cg/models/deliverables/__init__.py
+-rw-r--r--   0        0        0     5213 2024-04-25 13:46:16.683785 cg-60.4.2/cg/models/deliverables/metric_deliverables.py
+-rw-r--r--   0        0        0      243 2024-04-25 13:46:16.683785 cg-60.4.2/cg/models/delivery/delivery.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.683785 cg-60.4.2/cg/models/demultiplex/__init__.py
+-rw-r--r--   0        0        0    12040 2024-04-25 13:46:16.683785 cg-60.4.2/cg/models/demultiplex/run_parameters.py
+-rw-r--r--   0        0        0      539 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/demultiplex/sbatch.py
+-rw-r--r--   0        0        0     7006 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/downsample/downsample_data.py
+-rw-r--r--   0        0        0      255 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/email.py
+-rw-r--r--   0        0        0     1046 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/fastq.py
+-rw-r--r--   0        0        0     2157 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/file_data.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/flow_cell/__init__.py
+-rw-r--r--   0        0        0     9984 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/flow_cell/flow_cell.py
+-rw-r--r--   0        0        0      317 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/flow_cell/utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/invoice/__init__.py
+-rw-r--r--   0        0        0     1254 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/invoice/invoice.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/lims/__init__.py
+-rw-r--r--   0        0        0     2019 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/lims/sample.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/mip/__init__.py
+-rw-r--r--   0        0        0      337 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/mip/mip_analysis.py
+-rw-r--r--   0        0        0     1564 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/mip/mip_config.py
+-rw-r--r--   0        0        0     4696 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/mip/mip_metrics_deliverables.py
+-rw-r--r--   0        0        0     2550 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/mip/mip_sample_info.py
+-rw-r--r--   0        0        0     2472 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/nf_analysis.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/observations/__init__.py
+-rw-r--r--   0        0        0      688 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/observations/input_files.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/orders/__init__.py
+-rw-r--r--   0        0        0     2659 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/orders/constants.py
+-rw-r--r--   0        0        0     5604 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/orders/excel_sample.py
+-rw-r--r--   0        0        0      898 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/orders/json_sample.py
+-rw-r--r--   0        0        0     1449 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/orders/order.py
+-rw-r--r--   0        0        0      811 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/orders/orderform_schema.py
+-rw-r--r--   0        0        0     4212 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/orders/sample_base.py
+-rw-r--r--   0        0        0     9668 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/orders/samples.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/orders/validators/__init__.py
+-rw-r--r--   0        0        0     2300 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/orders/validators/excel_sample_validators.py
+-rw-r--r--   0        0        0      576 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/orders/validators/json_sample_validators.py
+-rw-r--r--   0        0        0       71 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/orders/validators/sample_base_validators.py
+-rw-r--r--   0        0        0      101 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/qc_metrics.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/raredisease/__init__.py
+-rw-r--r--   0        0        0     1875 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/raredisease/raredisease.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/report/__init__.py
+-rw-r--r--   0        0        0     7461 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/report/metadata.py
+-rw-r--r--   0        0        0     6180 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/report/report.py
+-rw-r--r--   0        0        0     5221 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/report/sample.py
+-rw-r--r--   0        0        0     3004 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/report/validators.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/rnafusion/__init__.py
+-rw-r--r--   0        0        0     1865 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/rnafusion/rnafusion.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/scout/__init__.py
+-rw-r--r--   0        0        0     4783 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/scout/scout_load_config.py
+-rw-r--r--   0        0        0      116 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/scout/validators.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/slurm/__init__.py
+-rw-r--r--   0        0        0      617 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/slurm/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/taxprofiler/__init__.py
+-rw-r--r--   0        0        0     2443 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/taxprofiler/taxprofiler.py
+-rw-r--r--   0        0        0     2588 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/tomte/tomte.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/workflow/__init__.py
+-rw-r--r--   0        0        0      685 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/workflow/mutant.py
+-rw-r--r--   0        0        0       70 2024-04-25 13:46:16.687785 cg-60.4.2/cg/models/workflow/validators.py
+-rw-r--r--   0        0        0      842 2024-04-25 13:46:16.687785 cg-60.4.2/cg/resources/__init__.py
+-rw-r--r--   0        0        0     3493 2024-04-25 13:46:16.687785 cg-60.4.2/cg/resources/rnafusion_bundle_filenames.yaml
+-rw-r--r--   0        0        0     2434 2024-04-25 13:46:16.687785 cg-60.4.2/cg/resources/taxprofiler_bundle_filenames.yaml
+-rw-r--r--   0        0        0     3732 2024-04-25 13:46:16.687785 cg-60.4.2/cg/resources/tomte_bundle_filenames.yaml
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/__init__.py
+-rw-r--r--   0        0        0    20241 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/admin.py
+-rw-r--r--   0        0        0    22743 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/api.py
+-rw-r--r--   0        0        0     4887 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/app.py
+-rw-r--r--   0        0        0       48 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/auto.py
+-rw-r--r--   0        0        0     1184 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/config.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/dto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/dto/delivery_message/__init__.py
+-rw-r--r--   0        0        0      300 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/dto/delivery_message/delivery_message_request.py
+-rw-r--r--   0        0        0      183 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/dto/delivery_message/delivery_message_response.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/dto/orders/__init__.py
+-rw-r--r--   0        0        0      165 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/dto/orders/order_delivery_update_request.py
+-rw-r--r--   0        0        0       91 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/dto/orders/order_patch_request.py
+-rw-r--r--   0        0        0      662 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/dto/orders/orders_request.py
+-rw-r--r--   0        0        0      413 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/dto/orders/orders_response.py
+-rw-r--r--   0        0        0     2598 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/ext.py
+-rw-r--r--   0        0        0       29 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/invoices/__init__.py
+-rw-r--r--   0        0        0     4793 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/invoices/templates/invoices/index.html
+-rw-r--r--   0        0        0     8171 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/invoices/templates/invoices/invoice.html
+-rw-r--r--   0        0        0     2838 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/invoices/templates/invoices/layout.html
+-rw-r--r--   0        0        0     4956 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/invoices/templates/invoices/new.html
+-rw-r--r--   0        0        0     7708 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/invoices/views.py
+-rw-r--r--   0        0        0      354 2024-04-25 13:46:16.687785 cg-60.4.2/cg/server/templates/admin/index.html
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.687785 cg-60.4.2/cg/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.687785 cg-60.4.2/cg/services/analysis_service/__init__.py
+-rw-r--r--   0        0        0      482 2024-04-25 13:46:16.687785 cg-60.4.2/cg/services/analysis_service/analysis_service.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.687785 cg-60.4.2/cg/services/delivery_message/__init__.py
+-rw-r--r--   0        0        0     2531 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/delivery_message/delivery_message_service.py
+-rw-r--r--   0        0        0      792 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/delivery_message/messages/__init__.py
+-rw-r--r--   0        0        0     1366 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/delivery_message/messages/analysis_scout_message.py
+-rw-r--r--   0        0        0      791 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/delivery_message/messages/covid_message.py
+-rw-r--r--   0        0        0      189 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/delivery_message/messages/delivery_message.py
+-rw-r--r--   0        0        0     1391 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/delivery_message/messages/fastq_analysis_scout_message.py
+-rw-r--r--   0        0        0      535 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/delivery_message/messages/fastq_message.py
+-rw-r--r--   0        0        0     1358 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/delivery_message/messages/fastq_scout_message.py
+-rw-r--r--   0        0        0      604 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/delivery_message/messages/microsalt_mwr_message.py
+-rw-r--r--   0        0        0      592 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/delivery_message/messages/microsalt_mwx_message.py
+-rw-r--r--   0        0        0      903 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/delivery_message/messages/scout_message.py
+-rw-r--r--   0        0        0      512 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/delivery_message/messages/statina_message.py
+-rw-r--r--   0        0        0      779 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/delivery_message/messages/utils.py
+-rw-r--r--   0        0        0     3300 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/delivery_message/utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/fastq_file_service/__init__.py
+-rw-r--r--   0        0        0      101 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/fastq_file_service/exceptions.py
+-rw-r--r--   0        0        0     1092 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/fastq_file_service/fastq_file_service.py
+-rw-r--r--   0        0        0     2991 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/fastq_file_service/utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/orders/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/orders/order_service/__init__.py
+-rw-r--r--   0        0        0     2684 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/orders/order_service/order_service.py
+-rw-r--r--   0        0        0     1214 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/orders/order_service/utils.py
+-rw-r--r--   0        0        0       94 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/orders/order_status_service/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/orders/order_status_service/dto/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/orders/order_status_service/dto/case_summary.py
+-rw-r--r--   0        0        0      289 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/orders/order_status_service/dto/order_summary.py
+-rw-r--r--   0        0        0     1768 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/orders/order_status_service/order_summary_service.py
+-rw-r--r--   0        0        0     1737 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/orders/order_status_service/utils.py
+-rw-r--r--   0        0        0       95 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/quality_controller/__init__.py
+-rw-r--r--   0        0        0     1819 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/quality_controller/quality_checks/checks.py
+-rw-r--r--   0        0        0     4987 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/quality_controller/quality_checks/utils.py
+-rw-r--r--   0        0        0     1040 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/quality_controller/quality_controller_service.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/slurm_service/__init__.py
+-rw-r--r--   0        0        0      703 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/slurm_service/slurm_cli_service.py
+-rw-r--r--   0        0        0      242 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/slurm_service/slurm_service.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/slurm_upload_service/__init__.py
+-rw-r--r--   0        0        0      175 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/slurm_upload_service/slurm_upload_config.py
+-rw-r--r--   0        0        0     2074 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/slurm_upload_service/slurm_upload_service.py
+-rw-r--r--   0        0        0      203 2024-04-25 13:46:16.691785 cg-60.4.2/cg/services/slurm_upload_service/utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/__init__.py
+-rw-r--r--   0        0        0     4650 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/base.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/crud/__init__.py
+-rw-r--r--   0        0        0    13100 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/crud/create.py
+-rw-r--r--   0        0        0     2144 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/crud/delete.py
+-rw-r--r--   0        0        0    60036 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/crud/read.py
+-rw-r--r--   0        0        0     1121 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/crud/update.py
+-rw-r--r--   0        0        0     1662 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/database.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/filters/__init__.py
+-rw-r--r--   0        0        0     5371 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/filters/status_analysis_filters.py
+-rw-r--r--   0        0        0     1712 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/filters/status_application_filters.py
+-rw-r--r--   0        0        0     1440 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/filters/status_application_limitations_filters.py
+-rw-r--r--   0        0        0     2523 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/filters/status_application_version_filters.py
+-rw-r--r--   0        0        0     1390 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/filters/status_bed_filters.py
+-rw-r--r--   0        0        0     1317 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/filters/status_bed_version_filters.py
+-rw-r--r--   0        0        0    10787 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/filters/status_case_filters.py
+-rw-r--r--   0        0        0     3272 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/filters/status_case_sample_filters.py
+-rw-r--r--   0        0        0      903 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/filters/status_collaboration_filters.py
+-rw-r--r--   0        0        0     1412 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/filters/status_customer_filters.py
+-rw-r--r--   0        0        0     1880 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/filters/status_flow_cell_filters.py
+-rw-r--r--   0        0        0     1255 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/filters/status_invoice_filters.py
+-rw-r--r--   0        0        0     2792 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/filters/status_metrics_filters.py
+-rw-r--r--   0        0        0     3225 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/filters/status_order_filters.py
+-rw-r--r--   0        0        0      851 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/filters/status_organism_filters.py
+-rw-r--r--   0        0        0      783 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/filters/status_panel_filters.py
+-rw-r--r--   0        0        0     3923 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/filters/status_pool_filters.py
+-rw-r--r--   0        0        0     8660 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/filters/status_sample_filters.py
+-rw-r--r--   0        0        0      731 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/filters/status_user_filters.py
+-rw-r--r--   0        0        0    36081 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/models.py
+-rw-r--r--   0        0        0      593 2024-04-25 13:46:16.691785 cg-60.4.2/cg/store/store.py
+-rw-r--r--   0        0        0       30 2024-04-25 13:46:16.691785 cg-60.4.2/cg/utils/__init__.py
+-rw-r--r--   0        0        0      187 2024-04-25 13:46:16.691785 cg-60.4.2/cg/utils/calculations.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.691785 cg-60.4.2/cg/utils/checksum/__init__.py
+-rw-r--r--   0        0        0     1579 2024-04-25 13:46:16.691785 cg-60.4.2/cg/utils/checksum/checksum.py
+-rw-r--r--   0        0        0     1655 2024-04-25 13:46:16.691785 cg-60.4.2/cg/utils/click/EnumChoice.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.691785 cg-60.4.2/cg/utils/click/__init__.py
+-rw-r--r--   0        0        0     4910 2024-04-25 13:46:16.691785 cg-60.4.2/cg/utils/commands.py
+-rw-r--r--   0        0        0     1811 2024-04-25 13:46:16.691785 cg-60.4.2/cg/utils/date.py
+-rw-r--r--   0        0        0      635 2024-04-25 13:46:16.691785 cg-60.4.2/cg/utils/dict.py
+-rw-r--r--   0        0        0     2111 2024-04-25 13:46:16.691785 cg-60.4.2/cg/utils/dispatcher.py
+-rw-r--r--   0        0        0     1251 2024-04-25 13:46:16.691785 cg-60.4.2/cg/utils/email.py
+-rw-r--r--   0        0        0      134 2024-04-25 13:46:16.691785 cg-60.4.2/cg/utils/enums.py
+-rw-r--r--   0        0        0     3178 2024-04-25 13:46:16.691785 cg-60.4.2/cg/utils/files.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.691785 cg-60.4.2/cg/utils/flask/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-25 13:46:16.691785 cg-60.4.2/cg/utils/flask/enum.py
+-rw-r--r--   0        0        0      233 2024-04-25 13:46:16.691785 cg-60.4.2/cg/utils/flow_cell.py
+-rw-r--r--   0        0        0      834 2024-04-25 13:46:16.691785 cg-60.4.2/cg/utils/time.py
+-rw-r--r--   0        0        0     1410 2024-04-25 13:46:16.691785 cg-60.4.2/cg/utils/utils.py
+-rw-r--r--   0        0        0     1697 2024-04-25 13:46:16.695785 cg-60.4.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.695785 cg-60.4.2/tests/__init__.py
+-rw-r--r--   0        0        0     1158 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/conftest.py
+-rw-r--r--   0        0        0      231 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/coverage/conftest.py
+-rw-r--r--   0        0        0     6188 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/coverage/test_coverage.py
+-rw-r--r--   0        0        0     1693 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/crunchy/conftest.py
+-rw-r--r--   0        0        0     5438 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/crunchy/test_compress_fastq.py
+-rw-r--r--   0        0        0     2283 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/crunchy/test_config.py
+-rw-r--r--   0        0        0    14032 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/crunchy/test_crunchy.py
+-rw-r--r--   0        0        0     9109 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/crunchy/test_spring_decompression.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/demultiplex/__init__.py
+-rw-r--r--   0        0        0     4994 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/demultiplex/conftest.py
+-rw-r--r--   0        0        0     4010 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0        0        0     7986 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/demultiplex/test_demultiplex_api.py
+-rw-r--r--   0        0        0     4782 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/demultiplex/test_index.py
+-rw-r--r--   0        0        0     9468 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/demultiplex/test_override_cycles_validator.py
+-rw-r--r--   0        0        0     4042 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/demultiplex/test_read_sample_sheet.py
+-rw-r--r--   0        0        0    12389 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/demultiplex/test_sample_models.py
+-rw-r--r--   0        0        0      951 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/demultiplex/test_sample_sheet_creator.py
+-rw-r--r--   0        0        0     3175 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/demultiplex/test_sample_sheet_models.py
+-rw-r--r--   0        0        0    10932 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/demultiplex/test_sample_sheet_validator.py
+-rw-r--r--   0        0        0     4896 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/demultiplex/test_translate_sample_sheet.py
+-rw-r--r--   0        0        0     1450 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/demultiplex/test_validate.py
+-rw-r--r--   0        0        0     5094 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/downsample/test_downsample.py
+-rw-r--r--   0        0        0     1419 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/downsample/test_downsample_utils.py
+-rw-r--r--   0        0        0     1716 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/gens/test_gens_api.py
+-rw-r--r--   0        0        0     1950 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/gt/conftest.py
+-rw-r--r--   0        0        0     4276 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/gt/test_gt_api.py
+-rw-r--r--   0        0        0     1453 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/hk/conftest.py
+-rw-r--r--   0        0        0      684 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/hk/test__getattr__.py
+-rw-r--r--   0        0        0     1593 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/hk/test_add_file.py
+-rw-r--r--   0        0        0     3523 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/hk/test_bundles.py
+-rw-r--r--   0        0        0      871 2024-04-25 13:46:16.695785 cg-60.4.2/tests/apps/hk/test_core.py
+-rw-r--r--   0        0        0    31172 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/hk/test_file.py
+-rw-r--r--   0        0        0     5080 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/hk/test_version.py
+-rw-r--r--   0        0        0     1840 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/lims/conftest.py
+-rw-r--r--   0        0        0     3197 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/lims/test_api.py
+-rw-r--r--   0        0        0     1451 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/lims/test_sample_sheet.py
+-rw-r--r--   0        0        0     9223 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/loqus/conftest.py
+-rw-r--r--   0        0        0     8994 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/loqus/test_loqusdb_api.py
+-rw-r--r--   0        0        0     2439 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/madeline/conftest.py
+-rw-r--r--   0        0        0     4653 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/madeline/test_madeline.py
+-rw-r--r--   0        0        0     3328 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/mip/conftest.py
+-rw-r--r--   0        0        0     2487 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/mip/test_config_mip.py
+-rw-r--r--   0        0        0      883 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/mutacc_auto/conftest.py
+-rw-r--r--   0        0        0     2473 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/mutacc_auto/test_mutacc_auto.py
+-rw-r--r--   0        0        0    11930 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/orderform/conftest.py
+-rw-r--r--   0        0        0     9484 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/orderform/test_excel_orderform_parser.py
+-rw-r--r--   0        0        0     4351 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/orderform/test_excel_sample_schema.py
+-rw-r--r--   0        0        0     1032 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/orderform/test_json_orderform_parser.py
+-rw-r--r--   0        0        0     2474 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/orderform/test_orderform_parser.py
+-rw-r--r--   0        0        0    16002 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/orderform/validators/test_excel_sample_validators.py
+-rw-r--r--   0        0        0     3670 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/scout/conftest.py
+-rw-r--r--   0        0        0     2269 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/scout/test_get_causative_variants.py
+-rw-r--r--   0        0        0     1376 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/scout/test_get_scout_cases.py
+-rw-r--r--   0        0        0     1840 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/scout/test_scout_load_config.py
+-rw-r--r--   0        0        0     7047 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/scout/test_scout_models.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0        0        0     2639 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/sequencing_metrics_parser/conftest.py
+-rw-r--r--   0        0        0     7069 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
+-rw-r--r--   0        0        0     2958 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/sequencing_metrics_parser/parsers/test_sequencing_metrics_parser_api.py
+-rw-r--r--   0        0        0     1131 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/slurm/conftest.py
+-rw-r--r--   0        0        0     4412 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/slurm/test_slurm_api.py
+-rw-r--r--   0        0        0      831 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/test_apps_environ.py
+-rw-r--r--   0        0        0      957 2024-04-25 13:46:16.699785 cg-60.4.2/tests/apps/test_osticket.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/add/__init__.py
+-rw-r--r--   0        0        0     1174 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/add/test_cli_add.py
+-rw-r--r--   0        0        0     2471 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/add/test_cli_add_customer.py
+-rw-r--r--   0        0        0     6841 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/add/test_cli_add_family.py
+-rw-r--r--   0        0        0     7588 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/add/test_cli_add_relationship.py
+-rw-r--r--   0        0        0     8382 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/add/test_cli_add_sample.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/backup/__init__.py
+-rw-r--r--   0        0        0      705 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/backup/conftest.py
+-rw-r--r--   0        0        0    11101 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/backup/test_backup_command.py
+-rw-r--r--   0        0        0     6865 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/clean/conftest.py
+-rw-r--r--   0        0        0     5536 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/clean/test_balsamic_clean.py
+-rw-r--r--   0        0        0     2557 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/clean/test_clean_flow_cell.py
+-rw-r--r--   0        0        0     1830 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/clean/test_clean_hk_bundle_files.py
+-rw-r--r--   0        0        0     2098 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/clean/test_hk_bundle_files.py
+-rw-r--r--   0        0        0     4610 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/clean/test_hk_case_bundle_files.py
+-rw-r--r--   0        0        0     3585 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/clean/test_microbial_clean.py
+-rw-r--r--   0        0        0     1881 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/clean/test_rsync_past_run_dirs.py
+-rw-r--r--   0        0        0     9707 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/compress/conftest.py
+-rw-r--r--   0        0        0     7709 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/compress/test_cli_compress_fastq.py
+-rw-r--r--   0        0        0     1416 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/compress/test_cli_decompress_spring.py
+-rw-r--r--   0        0        0     5205 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/compress/test_compress_helpers.py
+-rw-r--r--   0        0        0     1239 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/compress/test_store_fastq.py
+-rw-r--r--   0        0        0     7558 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/conftest.py
+-rw-r--r--   0        0        0    12747 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/delete/test_cli_delete_case.py
+-rw-r--r--   0        0        0     1873 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/delete/test_cli_delete_cases.py
+-rw-r--r--   0        0        0     3794 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/deliver/conftest.py
+-rw-r--r--   0        0        0     4428 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/deliver/test_deliver_base.py
+-rw-r--r--   0        0        0     1166 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/deliver/test_rsync_base.py
+-rw-r--r--   0        0        0     8569 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/deliver/test_run_deliver_cmd.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/demultiplex/__init__.py
+-rw-r--r--   0        0        0     5109 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0        0        0     4799 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/demultiplex/test_demultiplex_flowcell.py
+-rw-r--r--   0        0        0     1639 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/demultiplex/test_finish_demux.py
+-rw-r--r--   0        0        0     3015 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/demultiplex/test_validate_sample_sheet.py
+-rw-r--r--   0        0        0     4291 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/demultiplex/test_verify_syncing.py
+-rw-r--r--   0        0        0     1585 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/downsample/test_cli_downsample.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/generate/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/generate/report/__init__.py
+-rw-r--r--   0        0        0     1622 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/generate/report/conftest.py
+-rw-r--r--   0        0        0     2477 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/generate/report/test_cli_delivery_report.py
+-rw-r--r--   0        0        0     2760 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/generate/report/test_utils.py
+-rw-r--r--   0        0        0      563 2024-04-25 13:46:16.699785 cg-60.4.2/tests/cli/generate/test_cli_base.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/get/__init__.py
+-rw-r--r--   0        0        0      863 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/get/test_cli_get.py
+-rw-r--r--   0        0        0     1526 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/get/test_cli_get_analysis.py
+-rw-r--r--   0        0        0     1242 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/get/test_cli_get_case.py
+-rw-r--r--   0        0        0     6208 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/get/test_cli_get_flow_cell.py
+-rw-r--r--   0        0        0     8835 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/get/test_cli_get_sample.py
+-rw-r--r--   0        0        0     1364 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/set/conftest.py
+-rw-r--r--   0        0        0     7311 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/set/test_cli_set_case.py
+-rw-r--r--   0        0        0     1460 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/set/test_cli_set_cases.py
+-rw-r--r--   0        0        0     2016 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/set/test_cli_set_flowcell.py
+-rw-r--r--   0        0        0     1685 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/set/test_cli_set_list_keys.py
+-rw-r--r--   0        0        0    12450 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/set/test_cli_set_sample.py
+-rw-r--r--   0        0        0     6124 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/set/test_cli_set_samples.py
+-rw-r--r--   0        0        0     7015 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/store/test_store.py
+-rw-r--r--   0        0        0     2332 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/test_base.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/upload/__init__.py
+-rw-r--r--   0        0        0    10057 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/upload/conftest.py
+-rw-r--r--   0        0        0     2295 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/upload/test_cli_scout.py
+-rw-r--r--   0        0        0     1789 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/upload/test_cli_upload.py
+-rw-r--r--   0        0        0      971 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/upload/test_cli_upload_auto.py
+-rw-r--r--   0        0        0     1669 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/upload/test_cli_upload_delivery_report.py
+-rw-r--r--   0        0        0      895 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/upload/test_cli_upload_fastq.py
+-rw-r--r--   0        0        0     1199 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/upload/test_cli_upload_genotype.py
+-rw-r--r--   0        0        0      694 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/upload/test_cli_upload_gens.py
+-rw-r--r--   0        0        0     9965 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/upload/test_cli_upload_nipt.py
+-rw-r--r--   0        0        0     4684 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/upload/test_cli_upload_nipt_ftp.py
+-rw-r--r--   0        0        0     1839 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/upload/test_cli_upload_nipt_statina.py
+-rw-r--r--   0        0        0     6177 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/upload/test_cli_upload_observations.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/__init__.py
+-rw-r--r--   0        0        0    31369 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/balsamic/conftest.py
+-rw-r--r--   0        0        0    13938 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
+-rw-r--r--   0        0        0     7984 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/balsamic/test_compound_commands.py
+-rw-r--r--   0        0        0     2336 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/balsamic/test_link.py
+-rw-r--r--   0        0        0     3554 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/balsamic/test_report_deliver.py
+-rw-r--r--   0        0        0     6209 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/balsamic/test_run.py
+-rw-r--r--   0        0        0     6934 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/balsamic/test_store_housekeeper.py
+-rw-r--r--   0        0        0     8458 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/fastq/__init__.py
+-rw-r--r--   0        0        0     2332 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/fastq/test_fastq_base.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0        0        0     5237 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/fluffy/conftest.py
+-rw-r--r--   0        0        0     5687 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
+-rw-r--r--   0        0        0     3302 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/fluffy/test_cli_link.py
+-rw-r--r--   0        0        0     1896 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/fluffy/test_cli_run.py
+-rw-r--r--   0        0        0     2968 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/fluffy/test_cli_start.py
+-rw-r--r--   0        0        0     7815 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/fluffy/test_cli_store.py
+-rw-r--r--   0        0        0     2775 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/microsalt/conftest.py
+-rw-r--r--   0        0        0     6926 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/microsalt/test_microsalt_case_config.py
+-rw-r--r--   0        0        0     1000 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/microsalt/test_microsalt_run.py
+-rw-r--r--   0        0        0     6544 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/mip/conftest.py
+-rw-r--r--   0        0        0     7011 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/mip/test_cli_mip_base.py
+-rw-r--r--   0        0        0     1542 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
+-rw-r--r--   0        0        0      431 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/mip/test_cli_mip_dna_link.py
+-rw-r--r--   0        0        0     2108 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py
+-rw-r--r--   0        0        0     1273 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
+-rw-r--r--   0        0        0     3595 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/mip/test_cli_mip_dna_run.py
+-rw-r--r--   0        0        0     3884 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/mip/test_cli_mip_dna_start.py
+-rw-r--r--   0        0        0     1004 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
+-rw-r--r--   0        0        0      527 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/mip/test_cli_mip_rna_link.py
+-rw-r--r--   0        0        0      716 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/mip/test_cli_mip_rna_run.py
+-rw-r--r--   0        0        0     8559 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/mip/test_cli_mip_store.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/nf_analysis/__init__.py
+-rw-r--r--   0        0        0     9318 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/nf_analysis/test_cli_config_case.py
+-rw-r--r--   0        0        0     3831 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py
+-rw-r--r--   0        0        0     5087 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py
+-rw-r--r--   0        0        0     9211 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/nf_analysis/test_cli_run.py
+-rw-r--r--   0        0        0     3267 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/nf_analysis/test_cli_start.py
+-rw-r--r--   0        0        0     9877 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/nf_analysis/test_cli_store.py
+-rw-r--r--   0        0        0    10373 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py
+-rw-r--r--   0        0        0      978 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/raredisease/__init__.py
+-rw-r--r--   0        0        0     3940 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py
+-rw-r--r--   0        0        0      921 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/test_cli_workflow.py
+-rw-r--r--   0        0        0     4310 2024-04-25 13:46:16.703785 cg-60.4.2/tests/cli/workflow/test_cli_workflow_clean.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.703785 cg-60.4.2/tests/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.703785 cg-60.4.2/tests/clients/arnold/__init__.py
+-rw-r--r--   0        0        0     1080 2024-04-25 13:46:16.703785 cg-60.4.2/tests/clients/arnold/conftest.py
+-rw-r--r--   0        0        0     1503 2024-04-25 13:46:16.703785 cg-60.4.2/tests/clients/arnold/test_arnold_api_client.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.703785 cg-60.4.2/tests/clients/janus/__init__.py
+-rw-r--r--   0        0        0     2381 2024-04-25 13:46:16.703785 cg-60.4.2/tests/clients/janus/conftest.py
+-rw-r--r--   0        0        0     1716 2024-04-25 13:46:16.703785 cg-60.4.2/tests/clients/janus/test_janus_api_client.py
+-rw-r--r--   0        0        0   129141 2024-04-25 13:46:16.707785 cg-60.4.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixture_plugins/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixture_plugins/delivery_fixtures/__init__.py
+-rw-r--r--   0        0        0     2653 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py
+-rw-r--r--   0        0        0     4972 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixture_plugins/delivery_fixtures/context_fixtures.py
+-rw-r--r--   0        0        0     1494 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixture_plugins/delivery_fixtures/path_fixtures.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixture_plugins/demultiplex_fixtures/__init__.py
+-rw-r--r--   0        0        0     4636 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py
+-rw-r--r--   0        0        0     3413 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py
+-rw-r--r--   0        0        0    20458 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py
+-rw-r--r--   0        0        0     3412 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py
+-rw-r--r--   0        0        0     5988 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py
+-rw-r--r--   0        0        0     8960 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py
+-rw-r--r--   0        0        0     3174 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_check_scenario.py
+-rw-r--r--   0        0        0     4801 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_fixtures.py
+-rw-r--r--   0        0        0     1304 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixture_plugins/timestamp_fixtures.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
+-rw-r--r--   0        0        0    14644 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
+-rw-r--r--   0        0        0    15921 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/mip/dna/ADM2.cram
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/mip/dna/ADM3.cram
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/mip/dna/adm1.cram
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/mip/dna/adm1.mt.bam
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/mip/dna/multiqc.html
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/mip/dna/report.pdf
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/mip/dna/smn.vcf
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/mip/dna/snv.vcf
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/mip/dna/snv_research.vcf
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/mip/dna/str.vcf
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/mip/dna/sv.vcf
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/mip/dna/sv_research.vcf
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
+-rw-r--r--   0        0        0       70 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/nf-analysis/pipeline_params.config
+-rw-r--r--   0        0        0      195 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/nf-analysis/pipeline_resource_optimisation.config
+-rw-r--r--   0        0        0      195 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/nf-analysis/platform.config
+-rw-r--r--   0        0        0     8173 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/raredisease/multiqc_data.json
+-rw-r--r--   0        0        0    20005 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml
+-rw-r--r--   0        0        0     5497 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/rnafusion/multiqc_data.json
+-rw-r--r--   0        0        0    12499 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml
+-rw-r--r--   0        0        0     2873 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/sample_coverage.bed
+-rw-r--r--   0        0        0     6506 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/taxprofiler/multiqc_data.json
+-rw-r--r--   0        0        0    10513 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0     5771 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/tomte/multiqc_data.json
+-rw-r--r--   0        0        0    14859 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml
+-rw-r--r--   0        0        0    10961 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/balsamic/case/config.json
+-rw-r--r--   0        0        0     3465 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/balsamic/case/metadata.yml
+-rw-r--r--   0        0        0       63 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/balsamic/case/metadata_directory.yml
+-rw-r--r--   0        0        0      165 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
+-rw-r--r--   0        0        0     2705 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
+-rw-r--r--   0        0        0      692 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/crunchy/spring_metadata.json
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0      412 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      484 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      658 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/demuxcomplete.txt
+-rw-r--r--   0        0        0     1757 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0        0        0        7 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0     6034 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0        0        0     1172 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0        0        0        7 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_1.fastq.gz
+-rw-r--r--   0        0        0        7 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_2.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0      288 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      361 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      414 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/demuxcomplete.txt
+-rw-r--r--   0        0        0      315 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      434 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0     8624 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0      303 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      364 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      427 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/demuxcomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0     4439 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0        0        0     1172 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0     5127 2024-04-25 13:46:16.707785 cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
+-rw-r--r--   0        0        0       43 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz
+-rw-r--r--   0        0        0       67 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz.md5
+-rw-r--r--   0        0        0   338370 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz
+-rw-r--r--   0        0        0       67 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz.md5
+-rw-r--r--   0        0        0   338349 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/CopyComplete.txt
+-rw-r--r--   0        0        0     2126 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json
+-rw-r--r--   0        0        0     1827 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json
+-rw-r--r--   0        0        0       78 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/README.txt
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAComplete.txt
+-rw-r--r--   0        0        0     6895 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml
+-rw-r--r--   0        0        0       37 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead1Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead2Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead3Complete.txt
+-rw-r--r--   0        0        0    24755 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml
+-rw-r--r--   0        0        0      692 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
+-rw-r--r--   0        0        0      724 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0       61 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SequencingComplete.txt
+-rw-r--r--   0        0        0     5775 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/CopyComplete.txt
+-rw-r--r--   0        0        0     2282 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json
+-rw-r--r--   0        0        0     1632 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json
+-rw-r--r--   0        0        0       76 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/README.txt
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAComplete.txt
+-rw-r--r--   0        0        0     6912 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml
+-rw-r--r--   0        0        0       36 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead1Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead2Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead3Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead4Complete.txt
+-rw-r--r--   0        0        0    24814 2024-04-25 13:46:16.711785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml
+-rw-r--r--   0        0        0      814 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv
+-rw-r--r--   0        0        0      660 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0       61 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SequencingComplete.txt
+-rw-r--r--   0        0        0     5853 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/CopyComplete.txt
+-rw-r--r--   0        0        0    21848 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json
+-rw-r--r--   0        0        0    15512 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json
+-rw-r--r--   0        0        0       79 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/README.txt
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RTAComplete.txt
+-rw-r--r--   0        0        0      756 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml
+-rw-r--r--   0        0        0     4118 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv
+-rw-r--r--   0        0        0     1408 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0     5326 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/CopyComplete.txt
+-rw-r--r--   0        0        0    15041 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json
+-rw-r--r--   0        0        0    10649 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json
+-rw-r--r--   0        0        0       81 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/README.txt
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RTAComplete.txt
+-rw-r--r--   0        0        0      755 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml
+-rw-r--r--   0        0        0     2878 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv
+-rw-r--r--   0        0        0      928 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0     5359 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CopyComplete.txt
+-rw-r--r--   0        0        0    27887 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv
+-rw-r--r--   0        0        0   141870 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json
+-rwxr-xr-x   0        0        0   122682 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json
+-rw-r--r--   0        0        0      243 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/README.txt
+-rw-r--r--   0        0        0    28230 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTAComplete.txt
+-rw-r--r--   0        0        0    94426 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml
+-rw-r--r--   0        0        0     5819 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/SequenceComplete.txt
+-rw-r--r--   0        0        0     1757 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0        0        0     1757 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout
+-rw-r--r--   0        0        0    47522 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json
+-rw-r--r--   0        0        0       12 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/README.txt
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0        0        0     6666 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0        0        0      254 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/copycomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/delivery.txt
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/demuxstarted.txt
+-rwxr-xr-x   0        0        0    47434 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CopyComplete.txt
+-rw-r--r--   0        0        0    10950 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv
+-rw-r--r--   0        0        0      225 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/Manifest.tsv
+-rw-r--r--   0        0        0       55 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/README.txt
+-rwxr-xr-x   0        0        0     2493 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg
+-rwxr-xr-x   0        0        0        1 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAComplete.txt
+-rwxr-xr-x   0        0        0        2 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAExited.txt
+-rwxr-xr-x   0        0        0      730 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml
+-rwxr-xr-x   0        0        0    79277 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml
+-rwxr-xr-x   0        0        0     2694 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
+-rw-r--r--   0        0        0    10950 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
+-rw-r--r--   0        0        0      619 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CopyComplete.txt
+-rw-r--r--   0        0        0     4941 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv
+-rwxr-xr-x   0        0        0    20050 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stderr
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stdout
+-rw-r--r--   0        0        0      244 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/README.txt
+-rw-r--r--   0        0        0     6391 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTAComplete.txt
+-rw-r--r--   0        0        0    16428 2024-04-25 13:46:16.715785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml
+-rw-r--r--   0        0        0     6728 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
+-rw-r--r--   0        0        0     5127 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SequenceComplete.txt
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/demuxstarted.txt
+-rw-r--r--   0        0        0      133 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/README.txt
+-rw-r--r--   0        0        0      724 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
+-rw-r--r--   0        0        0     5775 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
+-rw-r--r--   0        0        0      124 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/180509_D00450_0598_BHGYFNBCX2/README.txt
+-rw-r--r--   0        0        0      310 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/README.txt
+-rw-r--r--   0        0        0     5819 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
+-rw-r--r--   0        0        0      122 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/README.txt
+-rwxr-xr-x   0        0        0     2694 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
+-rw-r--r--   0        0        0      311 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/README.txt
+-rw-r--r--   0        0        0     6728 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0        0        0      399 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
+-rw-r--r--   0        0        0      399 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_0.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_1.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/final_summary_PAS86456_72d9fceb_8a4fd683.txt
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_0.pod5
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_1.pod5
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_0.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_1.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/final_summary_PAS97781_595b5663_efc7f02e.txt
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_0.pod5
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_1.pod5
+-rw-r--r--   0        0        0     5319 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml
+-rw-r--r--   0        0        0     5944 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
+-rwxr-xr-x   0        0        0     2603 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
+-rwxr-xr-x   0        0        0     2597 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml
+-rw-r--r--   0        0        0     5899 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
+-rw-r--r--   0        0        0     4941 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv
+-rw-r--r--   0        0        0    10950 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/spring/dummy_run_001.spring
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/spring/dummy_run_002.spring
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/demultiplexing/spring/dummy_spring_meta_data.json
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
+-rw-r--r--   0        0        0     5554 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/fluffy/SampleSheet.csv
+-rw-r--r--   0        0        0      901 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/fluffy/deliverables.yaml
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/fluffy/multiqc_report.html
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/fluffy/summary.csv
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/gt/yellowhog.bcf
+-rw-r--r--   0        0        0     5114 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/madeline/madeline.xml
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/mip/case_file.txt
+-rw-r--r--   0        0        0     3241 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0    21811 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/mip/dna/store/case_config.yaml
+-rw-r--r--   0        0        0    23364 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
+-rw-r--r--   0        0        0    37367 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
+-rw-r--r--   0        0        0       16 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
+-rw-r--r--   0        0        0       16 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0       16 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
+-rw-r--r--   0        0        0      123 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
+-rw-r--r--   0        0        0    62741 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
+-rw-r--r--   0        0        0    11242 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/mip/rna/case_config.yaml
+-rw-r--r--   0        0        0    12164 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
+-rw-r--r--   0        0        0     5231 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
+-rw-r--r--   0        0        0     9774 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/mip/rna/store/case_config.yaml
+-rw-r--r--   0        0        0     4624 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
+-rw-r--r--   0        0        0    13666 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/mip/sample_file.txt
+-rw-r--r--   0        0        0     1885 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/scout/643594.config.yaml
+-rw-r--r--   0        0        0     6027 2024-04-25 13:46:16.719785 cg-60.4.2/tests/fixtures/apps/scout/case_export.json
+-rw-r--r--   0        0        0     9349 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/apps/scout/export_causatives.json
+-rw-r--r--   0        0        0     1315 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/apps/scout/none_case_export.json
+-rw-r--r--   0        0        0     3518 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/apps/scout/other_sex_case.json
+-rw-r--r--   0        0        0     8874 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/apps/scout/panel_export.bed
+-rw-r--r--   0        0        0     4169 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/apps/scout/panel_export.csv
+-rw-r--r--   0        0        0      619 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/SampleSheet.csv
+-rw-r--r--   0        0        0    63569 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0    42478 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0    69708 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0       42 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/apps/shipping/scout-deploy.yaml
+-rw-r--r--   0        0        0     1036 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/cgweb_orders/balsamic.json
+-rw-r--r--   0        0        0     1104 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/cgweb_orders/fastq.json
+-rw-r--r--   0        0        0     1313 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/cgweb_orders/metagenome.json
+-rw-r--r--   0        0        0     3038 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/cgweb_orders/microsalt.json
+-rw-r--r--   0        0        0     3705 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/cgweb_orders/mip.json
+-rw-r--r--   0        0        0     1364 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/cgweb_orders/mip_rna.json
+-rw-r--r--   0        0        0     2125 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/cgweb_orders/rml.json
+-rw-r--r--   0        0        0     1368 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/cgweb_orders/rnafusion.json
+-rw-r--r--   0        0        0     4684 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/cgweb_orders/sarscov2.json
+-rw-r--r--   0        0        0     5609 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/data/SampleSheet.csv
+-rw-r--r--   0        0        0      511 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/data/bcl_convert_sample_sheet.csv
+-rw-r--r--   0        0        0   258048 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/data/cgfixture.db
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/data/fastq.fastq.gz
+-rw-r--r--   0        0        0    49152 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/data/hkstore.db
+-rw-r--r--   0        0        0       73 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/data/yellowhog/pedigree.yaml
+-rw-r--r--   0        0        0       76 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/io/casava_five_parts.fastq.gz
+-rw-r--r--   0        0        0       90 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/io/casava_seven_parts.fastq.gz
+-rw-r--r--   0        0        0       96 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/io/casava_ten_parts.fastq.gz
+-rw-r--r--   0        0        0      153 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/io/example.csv
+-rw-r--r--   0        0        0       46 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/io/example.gz
+-rw-r--r--   0        0        0      147 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/io/example.tsv
+-rw-r--r--   0        0        0       20 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/io/example.txt
+-rw-r--r--   0        0        0       20 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/io/example2.txt
+-rw-r--r--   0        0        0      582 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/io/example_json.json
+-rw-r--r--   0        0        0      103 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/io/example_xml.xml
+-rw-r--r--   0        0        0       20 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/meta/qc_metrics/file_with_right_tags.json
+-rw-r--r--   0        0        0       20 2024-04-25 13:46:16.723785 cg-60.4.2/tests/fixtures/meta/qc_metrics/file_without_right_tags.json
+-rw-r--r--   0        0        0   156910 2024-04-25 13:46:16.727785 cg-60.4.2/tests/fixtures/orderforms/1508.30.balsamic.xlsx
+-rw-r--r--   0        0        0   156770 2024-04-25 13:46:16.727785 cg-60.4.2/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx
+-rw-r--r--   0        0        0   156737 2024-04-25 13:46:16.727785 cg-60.4.2/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx
+-rw-r--r--   0        0        0   156582 2024-04-25 13:46:16.727785 cg-60.4.2/tests/fixtures/orderforms/1508.30.fastq.xlsx
+-rw-r--r--   0        0        0   155627 2024-04-25 13:46:16.727785 cg-60.4.2/tests/fixtures/orderforms/1508.30.metagenome.xlsx
+-rw-r--r--   0        0        0   156850 2024-04-25 13:46:16.727785 cg-60.4.2/tests/fixtures/orderforms/1508.30.mip.xlsx
+-rw-r--r--   0        0        0   258580 2024-04-25 13:46:16.731785 cg-60.4.2/tests/fixtures/orderforms/1508.30.mip_rna.xlsx
+-rw-r--r--   0        0        0   258342 2024-04-25 13:46:16.731785 cg-60.4.2/tests/fixtures/orderforms/1508.30.rnafusion.xlsx
+-rw-r--r--   0        0        0    82677 2024-04-25 13:46:16.731785 cg-60.4.2/tests/fixtures/orderforms/1603.11.microbial.xlsx
+-rw-r--r--   0        0        0   149394 2024-04-25 13:46:16.731785 cg-60.4.2/tests/fixtures/orderforms/1604.17.rml.xlsx
+-rw-r--r--   0        0        0   223184 2024-04-25 13:46:16.731785 cg-60.4.2/tests/fixtures/orderforms/2184.9.sarscov2.xlsx
+-rw-r--r--   0        0        0    18639 2024-04-25 13:46:16.731785 cg-60.4.2/tests/fixtures/orderforms/NIPT-json.json
+-rw-r--r--   0        0        0     6052 2024-04-25 13:46:16.731785 cg-60.4.2/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
+-rw-r--r--   0        0        0     6611 2024-04-25 13:46:16.731785 cg-60.4.2/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
+-rw-r--r--   0        0        0     1417 2024-04-25 13:46:16.731785 cg-60.4.2/tests/fixtures/report/case_data.json
+-rw-r--r--   0        0        0     1109 2024-04-25 13:46:16.731785 cg-60.4.2/tests/fixtures/report/lims_exported_samples.json
+-rw-r--r--   0        0        0     1562 2024-04-25 13:46:16.731785 cg-60.4.2/tests/fixtures/report/lims_family.json
+-rw-r--r--   0        0        0     3296 2024-04-25 13:46:16.731785 cg-60.4.2/tests/io/conftest.py
+-rw-r--r--   0        0        0      431 2024-04-25 13:46:16.731785 cg-60.4.2/tests/io/test_io_config.py
+-rw-r--r--   0        0        0     8639 2024-04-25 13:46:16.731785 cg-60.4.2/tests/io/test_io_controller.py
+-rw-r--r--   0        0        0     3877 2024-04-25 13:46:16.731785 cg-60.4.2/tests/io/test_io_csv.py
+-rw-r--r--   0        0        0      482 2024-04-25 13:46:16.731785 cg-60.4.2/tests/io/test_io_gzip.py
+-rw-r--r--   0        0        0     1779 2024-04-25 13:46:16.731785 cg-60.4.2/tests/io/test_io_json.py
+-rw-r--r--   0        0        0     2914 2024-04-25 13:46:16.731785 cg-60.4.2/tests/io/test_io_txt.py
+-rw-r--r--   0        0        0     1027 2024-04-25 13:46:16.731785 cg-60.4.2/tests/io/test_io_xml.py
+-rw-r--r--   0        0        0     2131 2024-04-25 13:46:16.731785 cg-60.4.2/tests/io/test_io_yaml.py
+-rw-r--r--   0        0        0     1233 2024-04-25 13:46:16.731785 cg-60.4.2/tests/io/test_validate_path.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.731785 cg-60.4.2/tests/meta/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.731785 cg-60.4.2/tests/meta/archive/__init__.py
+-rw-r--r--   0        0        0    13131 2024-04-25 13:46:16.731785 cg-60.4.2/tests/meta/archive/conftest.py
+-rw-r--r--   0        0        0    16858 2024-04-25 13:46:16.731785 cg-60.4.2/tests/meta/archive/test_archive_api.py
+-rw-r--r--   0        0        0    10246 2024-04-25 13:46:16.731785 cg-60.4.2/tests/meta/archive/test_archive_cli.py
+-rw-r--r--   0        0        0    15766 2024-04-25 13:46:16.731785 cg-60.4.2/tests/meta/archive/test_archiving.py
+-rw-r--r--   0        0        0     3807 2024-04-25 13:46:16.731785 cg-60.4.2/tests/meta/backup/conftest.py
+-rw-r--r--   0        0        0    26368 2024-04-25 13:46:16.731785 cg-60.4.2/tests/meta/backup/test_meta_backup.py
+-rw-r--r--   0        0        0    10055 2024-04-25 13:46:16.731785 cg-60.4.2/tests/meta/backup/test_meta_pdc.py
+-rw-r--r--   0        0        0    12570 2024-04-25 13:46:16.731785 cg-60.4.2/tests/meta/clean/conftest.py
+-rw-r--r--   0        0        0    16944 2024-04-25 13:46:16.731785 cg-60.4.2/tests/meta/clean/test_clean_flow_cells_api.py
+-rw-r--r--   0        0        0     2286 2024-04-25 13:46:16.731785 cg-60.4.2/tests/meta/clean/test_clean_retrieved_spring_files.py
+-rw-r--r--   0        0        0     7691 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/compress/conftest.py
+-rw-r--r--   0        0        0     7961 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/compress/test_clean_fastq.py
+-rw-r--r--   0        0        0     1778 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/compress/test_compress_files.py
+-rw-r--r--   0        0        0     3644 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/compress/test_compress_meta_fastq.py
+-rw-r--r--   0        0        0     1180 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/compress/test_decompress_spring_meta.py
+-rw-r--r--   0        0        0     7045 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/compress/test_meta_compress_update_hk.py
+-rw-r--r--   0        0        0     8269 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/deliver/__init__.py
+-rw-r--r--   0        0        0     3471 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/deliver/conftest.py
+-rw-r--r--   0        0        0     5533 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/deliver/test_deliver_ticket.py
+-rw-r--r--   0        0        0    10277 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/deliver/test_delivery_api.py
+-rw-r--r--   0        0        0     1057 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/deliver/test_fastq_path_generator.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/delivery/__init__.py
+-rw-r--r--   0        0        0    16660 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/delivery/test_delivery_api.py
+-rw-r--r--   0        0        0     8066 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/demultiplex/conftest.py
+-rw-r--r--   0        0        0     5382 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/demultiplex/test_combine_sequencing_metrics.py
+-rw-r--r--   0        0        0     8445 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/demultiplex/test_demux_post_processing.py
+-rw-r--r--   0        0        0    12406 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/demultiplex/test_housekeeper_storage_functions.py
+-rw-r--r--   0        0        0     4392 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/demultiplex/test_status_db_storage_functions.py
+-rw-r--r--   0        0        0    22787 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/demultiplex/test_utils.py
+-rw-r--r--   0        0        0     6258 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/demultiplex/test_validation.py
+-rw-r--r--   0        0        0     4943 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/encryption/conftest.py
+-rw-r--r--   0        0        0    18133 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/encryption/test_encryption.py
+-rw-r--r--   0        0        0     3122 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/observations/conftest.py
+-rw-r--r--   0        0        0    16164 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/observations/test_meta_upload_observations.py
+-rw-r--r--   0        0        0     4974 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/orders/conftest.py
+-rw-r--r--   0        0        0     1749 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/orders/test_PoolSubmitter_validate_order.py
+-rw-r--r--   0        0        0     1470 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
+-rw-r--r--   0        0        0     1768 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/orders/test_SarsCov2Submitter_store_order.py
+-rw-r--r--   0        0        0     2032 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
+-rw-r--r--   0        0        0    19783 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/orders/test_meta_orders_api.py
+-rw-r--r--   0        0        0     7086 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/orders/test_meta_orders_lims.py
+-rw-r--r--   0        0        0    29515 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/orders/test_meta_orders_status.py
+-rw-r--r--   0        0        0     1677 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/orders/test_rnafusion_submitter.py
+-rw-r--r--   0        0        0     1068 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/orders/test_ticket_handler.py
+-rw-r--r--   0        0        0     4336 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/qc_metrics/conftest.py
+-rw-r--r--   0        0        0     1972 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/qc_metrics/test_collect_qc_metrics.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/report/__init__.py
+-rw-r--r--   0        0        0     6512 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/report/conftest.py
+-rw-r--r--   0        0        0      434 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/report/helper.py
+-rw-r--r--   0        0        0     2604 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/report/test_balsamic_api.py
+-rw-r--r--   0        0        0     4056 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/report/test_field_validators.py
+-rw-r--r--   0        0        0     2858 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/report/test_mip_dna_api.py
+-rw-r--r--   0        0        0    16042 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/report/test_report_api.py
+-rw-r--r--   0        0        0     1365 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/report/test_rnafusion_api.py
+-rw-r--r--   0        0        0     1250 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/report/test_tomte_api.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/rsync/__init__.py
+-rw-r--r--   0        0        0      916 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/rsync/conftest.py
+-rw-r--r--   0        0        0     9442 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/rsync/test_rsync.py
+-rw-r--r--   0        0        0     3147 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/test_invoice.py
+-rw-r--r--   0        0        0     1220 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/transfer/conftest.py
+-rw-r--r--   0        0        0     9892 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/transfer/test_external_data.py
+-rw-r--r--   0        0        0     4395 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/transfer/test_meta_transfer_lims.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/upload/__init__.py
+-rw-r--r--   0        0        0     2210 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/upload/balsamic/test_balsamic.py
+-rw-r--r--   0        0        0     4002 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/upload/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/upload/gisaid/__init__.py
+-rw-r--r--   0        0        0     2557 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/upload/gisaid/fixtures/four_samples.csv
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
+-rw-r--r--   0        0        0      211 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
+-rw-r--r--   0        0        0      371 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/upload/mutacc/__init__.py
+-rw-r--r--   0        0        0     3684 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/upload/mutacc/conftest.py
+-rw-r--r--   0        0        0     4188 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
+-rw-r--r--   0        0        0     1149 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/upload/nipt/conftest.py
+-rw-r--r--   0        0        0     1683 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/upload/nipt/test_models.py
+-rw-r--r--   0        0        0     1242 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/upload/nipt/test_nipt_upload_api.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/upload/scout/__init__.py
+-rw-r--r--   0        0        0    23954 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/upload/scout/conftest.py
+-rw-r--r--   0        0        0     4734 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/upload/scout/test_generate_load_config.py
+-rw-r--r--   0        0        0     4182 2024-04-25 13:46:16.735785 cg-60.4.2/tests/meta/upload/scout/test_meta_upload_scoutapi.py
+-rw-r--r--   0        0        0    33260 2024-04-25 13:46:16.739785 cg-60.4.2/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
+-rw-r--r--   0        0        0     7372 2024-04-25 13:46:16.739785 cg-60.4.2/tests/meta/upload/scout/test_scout_config_builder.py
+-rw-r--r--   0        0        0     2511 2024-04-25 13:46:16.739785 cg-60.4.2/tests/meta/upload/test_meta_upload_coverage.py
+-rw-r--r--   0        0        0     1473 2024-04-25 13:46:16.739785 cg-60.4.2/tests/meta/upload/test_upload_api.py
+-rw-r--r--   0        0        0     2547 2024-04-25 13:46:16.739785 cg-60.4.2/tests/meta/upload/test_upload_genotypes_api.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.739785 cg-60.4.2/tests/meta/workflow/__init__.py
+-rw-r--r--   0        0        0    10262 2024-04-25 13:46:16.739785 cg-60.4.2/tests/meta/workflow/conftest.py
+-rw-r--r--   0        0        0     3679 2024-04-25 13:46:16.739785 cg-60.4.2/tests/meta/workflow/microsalt/conftest.py
+-rw-r--r--   0        0        0      318 2024-04-25 13:46:16.739785 cg-60.4.2/tests/meta/workflow/microsalt/test_parsing_metrics.py
+-rw-r--r--   0        0        0     3759 2024-04-25 13:46:16.739785 cg-60.4.2/tests/meta/workflow/microsalt/test_quality_controller.py
+-rw-r--r--   0        0        0    14367 2024-04-25 13:46:16.739785 cg-60.4.2/tests/meta/workflow/microsalt/test_quality_controller_utils.py
+-rw-r--r--   0        0        0      825 2024-04-25 13:46:16.739785 cg-60.4.2/tests/meta/workflow/microsalt/test_report_generation.py
+-rw-r--r--   0        0        0    20860 2024-04-25 13:46:16.739785 cg-60.4.2/tests/meta/workflow/test_analysis.py
+-rw-r--r--   0        0        0     7934 2024-04-25 13:46:16.739785 cg-60.4.2/tests/meta/workflow/test_balsamic.py
+-rw-r--r--   0        0        0     3034 2024-04-25 13:46:16.739785 cg-60.4.2/tests/meta/workflow/test_fastq.py
+-rw-r--r--   0        0        0     1532 2024-04-25 13:46:16.739785 cg-60.4.2/tests/meta/workflow/test_microsalt.py
+-rw-r--r--   0        0        0     2721 2024-04-25 13:46:16.739785 cg-60.4.2/tests/meta/workflow/test_nf_analysis.py
+-rw-r--r--   0        0        0     7741 2024-04-25 13:46:16.739785 cg-60.4.2/tests/meta/workflow/test_prepare_fastq_api.py
+-rw-r--r--   0        0        0     1920 2024-04-25 13:46:16.739785 cg-60.4.2/tests/meta/workflow/test_raredisease.py
+-rw-r--r--   0        0        0     1674 2024-04-25 13:46:16.739785 cg-60.4.2/tests/meta/workflow/test_rnafusion.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.739785 cg-60.4.2/tests/mocks/__init__.py
+-rw-r--r--   0        0        0     1168 2024-04-25 13:46:16.739785 cg-60.4.2/tests/mocks/balsamic_analysis_mock.py
+-rw-r--r--   0        0        0     3500 2024-04-25 13:46:16.739785 cg-60.4.2/tests/mocks/crunchy.py
+-rw-r--r--   0        0        0    21778 2024-04-25 13:46:16.739785 cg-60.4.2/tests/mocks/hk_mock.py
+-rw-r--r--   0        0        0     4106 2024-04-25 13:46:16.739785 cg-60.4.2/tests/mocks/limsmock.py
+-rw-r--r--   0        0        0      572 2024-04-25 13:46:16.739785 cg-60.4.2/tests/mocks/madeline.py
+-rw-r--r--   0        0        0     1297 2024-04-25 13:46:16.739785 cg-60.4.2/tests/mocks/mip_analysis_mock.py
+-rw-r--r--   0        0        0     1525 2024-04-25 13:46:16.739785 cg-60.4.2/tests/mocks/osticket.py
+-rw-r--r--   0        0        0     3239 2024-04-25 13:46:16.739785 cg-60.4.2/tests/mocks/process_mock.py
+-rw-r--r--   0        0        0     4713 2024-04-25 13:46:16.739785 cg-60.4.2/tests/mocks/report.py
+-rw-r--r--   0        0        0     3915 2024-04-25 13:46:16.739785 cg-60.4.2/tests/mocks/scout.py
+-rw-r--r--   0        0        0      750 2024-04-25 13:46:16.739785 cg-60.4.2/tests/mocks/store_model.py
+-rw-r--r--   0        0        0     1620 2024-04-25 13:46:16.739785 cg-60.4.2/tests/mocks/tb_mock.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/balsamic/__init__.py
+-rw-r--r--   0        0        0     1194 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/balsamic/conftest.py
+-rw-r--r--   0        0        0     1030 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/balsamic/test_balsamic_analysis.py
+-rw-r--r--   0        0        0     1050 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/demultiplexing/__init__.py
+-rw-r--r--   0        0        0    11723 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/demultiplexing/test_run_parameters.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/downsample/__init__.py
+-rw-r--r--   0        0        0     2096 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/downsample/test_down_sample_meta_data.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/flow_cell/__init__.py
+-rw-r--r--   0        0        0     6723 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/flow_cell/test_flowcell_model.py
+-rw-r--r--   0        0        0     6637 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/mip/conftest.py
+-rw-r--r--   0        0        0     1239 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/mip/test_mip_analysis.py
+-rw-r--r--   0        0        0     2348 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/mip/test_mip_config.py
+-rw-r--r--   0        0        0     6392 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/mip/test_mip_metrics_deliverables.py
+-rw-r--r--   0        0        0     3959 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/mip/test_mip_sample_info.py
+-rw-r--r--   0        0        0     3314 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/nextflow/test_nextflow_deliver.py
+-rw-r--r--   0        0        0     1602 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/observations/conftest.py
+-rw-r--r--   0        0        0     2579 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/observations/test_observations_input_files.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/report/__init__.py
+-rw-r--r--   0        0        0     7327 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/report/test_validators.py
+-rw-r--r--   0        0        0     3855 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/rnafusion/test_rnafusion_sample.py
+-rw-r--r--   0        0        0     1374 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/test_cg_models.py
+-rw-r--r--   0        0        0      990 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/test_compression_data.py
+-rw-r--r--   0        0        0      729 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/test_fastq.py
+-rw-r--r--   0        0        0     2860 2024-04-25 13:46:16.739785 cg-60.4.2/tests/models/test_file_data.py
+-rw-r--r--   0        0        0     4539 2024-04-25 13:46:16.739785 cg-60.4.2/tests/server/conftest.py
+-rw-r--r--   0        0        0     3135 2024-04-25 13:46:16.739785 cg-60.4.2/tests/server/endpoints/test_delivery_message_endpoint.py
+-rw-r--r--   0        0        0     3239 2024-04-25 13:46:16.739785 cg-60.4.2/tests/server/endpoints/test_orders_endpoint.py
+-rw-r--r--   0        0        0      271 2024-04-25 13:46:16.739785 cg-60.4.2/tests/server/test_server_auto.py
+-rw-r--r--   0        0        0     1047 2024-04-25 13:46:16.739785 cg-60.4.2/tests/services/fastq_file_service/conftest.py
+-rw-r--r--   0        0        0     3634 2024-04-25 13:46:16.739785 cg-60.4.2/tests/services/fastq_file_service/test_fastq_file_service.py
+-rw-r--r--   0        0        0     4861 2024-04-25 13:46:16.739785 cg-60.4.2/tests/services/orders/order_status_service/conftest.py
+-rw-r--r--   0        0        0     2865 2024-04-25 13:46:16.739785 cg-60.4.2/tests/services/orders/order_status_service/test_order_summary_service.py
+-rw-r--r--   0        0        0     9595 2024-04-25 13:46:16.739785 cg-60.4.2/tests/services/quality_controller/test_sequencing_quality_checks_utils.py
+-rw-r--r--   0        0        0      318 2024-04-25 13:46:16.739785 cg-60.4.2/tests/small_helpers.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.739785 cg-60.4.2/tests/store/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.739785 cg-60.4.2/tests/store/api/__init__.py
+-rw-r--r--   0        0        0     3032 2024-04-25 13:46:16.739785 cg-60.4.2/tests/store/api/conftest.py
+-rw-r--r--   0        0        0     1557 2024-04-25 13:46:16.739785 cg-60.4.2/tests/store/api/test_base.py
+-rw-r--r--   0        0        0    20096 2024-04-25 13:46:16.739785 cg-60.4.2/tests/store/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.739785 cg-60.4.2/tests/store/crud/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.739785 cg-60.4.2/tests/store/crud/add/__init__.py
+-rw-r--r--   0        0        0     1497 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/crud/add/test_store_add_application_version.py
+-rw-r--r--   0        0        0     3958 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/crud/add/test_store_add_base.py
+-rw-r--r--   0        0        0     2502 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/crud/add/test_store_add_customer.py
+-rw-r--r--   0        0        0     1704 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/crud/add/test_store_add_flow_celll.py
+-rw-r--r--   0        0        0    12290 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/crud/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/crud/delete/__init__.py
+-rw-r--r--   0        0        0     5611 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/crud/delete/test_delete.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/crud/read/__init__.py
+-rw-r--r--   0        0        0    56073 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/crud/read/test_read.py
+-rw-r--r--   0        0        0     5461 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/crud/read/test_read_analyses_to_clean.py
+-rw-r--r--   0        0        0     3553 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/crud/read/test_read_analyses_to_delivery_report.py
+-rw-r--r--   0        0        0    17328 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/crud/read/test_read_analysis.py
+-rw-r--r--   0        0        0     2743 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/crud/read/test_read_application_version.py
+-rw-r--r--   0        0        0     1105 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/crud/read/test_read_customer.py
+-rw-r--r--   0        0        0     1530 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/crud/read/test_read_pool.py
+-rw-r--r--   0        0        0    21503 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/crud/read/test_read_sample.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/crud/update/__init__.py
+-rw-r--r--   0        0        0      737 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/crud/update/test_update.py
+-rw-r--r--   0        0        0    11693 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/filters/test_status_analyses_filters.py
+-rw-r--r--   0        0        0     3397 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/filters/test_status_application_filters.py
+-rw-r--r--   0        0        0     2073 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/filters/test_status_application_limitations_filters.py
+-rw-r--r--   0        0        0    10452 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/filters/test_status_application_version_filters.py
+-rw-r--r--   0        0        0     2804 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/filters/test_status_bed_filters.py
+-rw-r--r--   0        0        0     2362 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/filters/test_status_bed_version_filters.py
+-rw-r--r--   0        0        0     3495 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/filters/test_status_case_sample_filters.py
+-rw-r--r--   0        0        0    39100 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/filters/test_status_cases_filters.py
+-rw-r--r--   0        0        0     1345 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/filters/test_status_collaboration_filters.py
+-rw-r--r--   0        0        0     2482 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/filters/test_status_customer_filters.py
+-rw-r--r--   0        0        0     5153 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/filters/test_status_flow_cell_filters.py
+-rw-r--r--   0        0        0     2226 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/filters/test_status_invoice_filters.py
+-rw-r--r--   0        0        0     5871 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/filters/test_status_metrics_filters.py
+-rw-r--r--   0        0        0     2404 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/filters/test_status_organism_filters.py
+-rw-r--r--   0        0        0     1804 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/filters/test_status_panel_filters.py
+-rw-r--r--   0        0        0     8720 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/filters/test_status_pool_filters.py
+-rw-r--r--   0        0        0    22875 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/filters/test_status_samples_filters.py
+-rw-r--r--   0        0        0     1576 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/filters/test_status_user_filters.py
+-rw-r--r--   0        0        0     2147 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/test_delivery.py
+-rw-r--r--   0        0        0     4127 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store/test_store_models.py
+-rw-r--r--   0        0        0    37125 2024-04-25 13:46:16.743785 cg-60.4.2/tests/store_helpers.py
+-rw-r--r--   0        0        0     4988 2024-04-25 13:46:16.743785 cg-60.4.2/tests/test_copy_novaseqx_flow_cell.py
+-rw-r--r--   0        0        0      911 2024-04-25 13:46:16.743785 cg-60.4.2/tests/test_store_helpers.py
+-rw-r--r--   0        0        0        0 2024-04-25 13:46:16.743785 cg-60.4.2/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1754 2024-04-25 13:46:16.743785 cg-60.4.2/tests/utils/conftest.py
+-rw-r--r--   0        0        0      371 2024-04-25 13:46:16.743785 cg-60.4.2/tests/utils/test_calculations.py
+-rw-r--r--   0        0        0     2920 2024-04-25 13:46:16.743785 cg-60.4.2/tests/utils/test_commands.py
+-rw-r--r--   0        0        0      953 2024-04-25 13:46:16.743785 cg-60.4.2/tests/utils/test_date.py
+-rw-r--r--   0        0        0     1508 2024-04-25 13:46:16.743785 cg-60.4.2/tests/utils/test_dict.py
+-rw-r--r--   0        0        0     7154 2024-04-25 13:46:16.743785 cg-60.4.2/tests/utils/test_dispatcher.py
+-rw-r--r--   0        0        0     4100 2024-04-25 13:46:16.743785 cg-60.4.2/tests/utils/test_files.py
+-rw-r--r--   0        0        0     1170 2024-04-25 13:46:16.743785 cg-60.4.2/tests/utils/test_time.py
+-rw-r--r--   0        0        0     2366 2024-04-25 13:46:16.743785 cg-60.4.2/tests/utils/test_utils.py
+-rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 cg-60.4.2/PKG-INFO
```

### Comparing `cg-60.4.1/README.md` & `cg-60.4.2/README.md`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/coverage/api.py` & `cg-60.4.2/cg/apps/coverage/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/crunchy/crunchy.py` & `cg-60.4.2/cg/apps/crunchy/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/crunchy/files.py` & `cg-60.4.2/cg/apps/crunchy/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/crunchy/sbatch.py` & `cg-60.4.2/cg/apps/crunchy/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/demultiplex/demultiplex_api.py` & `cg-60.4.2/cg/apps/demultiplex/demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/demultiplex/sample_sheet/api.py` & `cg-60.4.2/cg/apps/demultiplex/sample_sheet/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/demultiplex/sample_sheet/index.py` & `cg-60.4.2/cg/apps/demultiplex/sample_sheet/index.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py` & `cg-60.4.2/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py` & `cg-60.4.2/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/demultiplex/sample_sheet/sample_models.py` & `cg-60.4.2/cg/apps/demultiplex/sample_sheet/sample_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py` & `cg-60.4.2/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py` & `cg-60.4.2/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py` & `cg-60.4.2/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/demultiplex/sample_sheet/validators.py` & `cg-60.4.2/cg/apps/demultiplex/sample_sheet/validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/demultiplex/sbatch.py` & `cg-60.4.2/cg/apps/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/downsample/downsample.py` & `cg-60.4.2/cg/apps/downsample/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/downsample/utils.py` & `cg-60.4.2/cg/apps/downsample/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/gens.py` & `cg-60.4.2/cg/apps/gens.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/gt.py` & `cg-60.4.2/cg/apps/gt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/hermes/hermes_api.py` & `cg-60.4.2/cg/apps/hermes/hermes_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/hermes/models.py` & `cg-60.4.2/cg/apps/hermes/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/housekeeper/hk.py` & `cg-60.4.2/cg/apps/housekeeper/hk.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/invoice/render.py` & `cg-60.4.2/cg/apps/invoice/render.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/invoice/templates/KI_pool_invoice.xlsx` & `cg-60.4.2/cg/apps/invoice/templates/KI_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/invoice/templates/KI_sample_invoice.xlsx` & `cg-60.4.2/cg/apps/invoice/templates/KI_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/invoice/templates/KTH_pool_invoice.xlsx` & `cg-60.4.2/cg/apps/invoice/templates/KTH_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/invoice/templates/KTH_sample_invoice.xlsx` & `cg-60.4.2/cg/apps/invoice/templates/KTH_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/lims/api.py` & `cg-60.4.2/cg/apps/lims/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/lims/batch.py` & `cg-60.4.2/cg/apps/lims/batch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/lims/order.py` & `cg-60.4.2/cg/apps/lims/order.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/lims/sample_sheet.py` & `cg-60.4.2/cg/apps/lims/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/loqus.py` & `cg-60.4.2/cg/apps/loqus.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/madeline/api.py` & `cg-60.4.2/cg/apps/madeline/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/mip/confighandler.py` & `cg-60.4.2/cg/apps/mip/confighandler.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/mutacc_auto.py` & `cg-60.4.2/cg/apps/mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/orderform/excel_orderform_parser.py` & `cg-60.4.2/cg/apps/orderform/excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/orderform/json_orderform_parser.py` & `cg-60.4.2/cg/apps/orderform/json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/orderform/orderform_parser.py` & `cg-60.4.2/cg/apps/orderform/orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/osticket.py` & `cg-60.4.2/cg/apps/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/scout/scout_export.py` & `cg-60.4.2/cg/apps/scout/scout_export.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/scout/scoutapi.py` & `cg-60.4.2/cg/apps/scout/scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/sequencing_metrics_parser/api.py` & `cg-60.4.2/cg/apps/sequencing_metrics_parser/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/sequencing_metrics_parser/models.py` & `cg-60.4.2/cg/apps/sequencing_metrics_parser/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/sequencing_metrics_parser/parser.py` & `cg-60.4.2/cg/apps/sequencing_metrics_parser/parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/slurm/sbatch.py` & `cg-60.4.2/cg/apps/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/slurm/slurm_api.py` & `cg-60.4.2/cg/apps/slurm/slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/tb/api.py` & `cg-60.4.2/cg/apps/tb/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/apps/tb/models.py` & `cg-60.4.2/cg/apps/tb/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/add.py` & `cg-60.4.2/cg/cli/add.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/archive.py` & `cg-60.4.2/cg/cli/archive.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/backup.py` & `cg-60.4.2/cg/cli/backup.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/base.py` & `cg-60.4.2/cg/cli/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/clean.py` & `cg-60.4.2/cg/cli/clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/compress/base.py` & `cg-60.4.2/cg/cli/compress/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/compress/fastq.py` & `cg-60.4.2/cg/cli/compress/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/compress/helpers.py` & `cg-60.4.2/cg/cli/compress/helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/delete/base.py` & `cg-60.4.2/cg/cli/delete/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/delete/case.py` & `cg-60.4.2/cg/cli/delete/case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/delete/cases.py` & `cg-60.4.2/cg/cli/delete/cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/delete/observations.py` & `cg-60.4.2/cg/cli/delete/observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/deliver/base.py` & `cg-60.4.2/cg/cli/deliver/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/demultiplex/base.py` & `cg-60.4.2/cg/cli/demultiplex/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py` & `cg-60.4.2/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/demultiplex/demux.py` & `cg-60.4.2/cg/cli/demultiplex/demux.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 def demultiplex_flow_cell(
     context: CGConfig,
     dry_run: bool,
     flow_cell_name: str,
 ):
     """Demultiplex a flow cell using BCLConvert.
 
-    flow cell name is the flow cell run directory name, e.g. '201203_D00483_0200_AHVKJCDRXX'
+    flow cell name is the flow cell run directory name, e.g. '230912_A00187_1009_AHK33MDRX3'
     """
 
     LOG.info(f"Starting demultiplexing of flow cell {flow_cell_name}")
     sample_sheet_api: SampleSheetAPI = context.sample_sheet_api
     demultiplex_api: DemultiplexingAPI = context.demultiplex_api
     flow_cell_directory: Path = Path(context.demultiplex_api.flow_cells_dir, flow_cell_name)
     demultiplex_api.set_dry_run(dry_run=dry_run)
```

### Comparing `cg-60.4.1/cg/cli/demultiplex/finish.py` & `cg-60.4.2/cg/cli/demultiplex/finish.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 @click.argument("flow-cell-directory-name")
 @click.option("--force", is_flag=True)
 @DRY_RUN
 @click.pass_obj
 def finish_flow_cell(context: CGConfig, flow_cell_directory_name: str, force: bool, dry_run: bool):
     """Command to finish up a flow cell after demultiplexing.
 
-    flow-cell-name is full flow cell name, e.g. '201203_D00483_0200_AHVKJCDRXX'.
+    flow-cell-name is full flow cell name, e.g. '230912_A00187_1009_AHK33MDRX3'.
     """
     demux_post_processing_api = DemuxPostProcessingAPI(config=context)
     demux_post_processing_api.set_dry_run(dry_run=dry_run)
     demux_post_processing_api.finish_flow_cell(
         flow_cell_directory_name=flow_cell_directory_name,
         force=force,
     )
```

### Comparing `cg-60.4.1/cg/cli/demultiplex/sample_sheet.py` & `cg-60.4.2/cg/cli/demultiplex/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/downsample.py` & `cg-60.4.2/cg/cli/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/generate/report/base.py` & `cg-60.4.2/cg/cli/generate/report/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/generate/report/options.py` & `cg-60.4.2/cg/cli/generate/report/options.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/generate/report/utils.py` & `cg-60.4.2/cg/cli/generate/report/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/get.py` & `cg-60.4.2/cg/cli/get.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/set/base.py` & `cg-60.4.2/cg/cli/set/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/set/case.py` & `cg-60.4.2/cg/cli/set/case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/set/cases.py` & `cg-60.4.2/cg/cli/set/cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/store/base.py` & `cg-60.4.2/cg/cli/store/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/store/store.py` & `cg-60.4.2/cg/cli/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/transfer.py` & `cg-60.4.2/cg/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/upload/base.py` & `cg-60.4.2/cg/cli/upload/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/upload/clinical_delivery.py` & `cg-60.4.2/cg/cli/upload/clinical_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/upload/coverage.py` & `cg-60.4.2/cg/cli/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/upload/delivery_report.py` & `cg-60.4.2/cg/cli/upload/delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/upload/fohm.py` & `cg-60.4.2/cg/cli/upload/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/upload/genotype.py` & `cg-60.4.2/cg/cli/upload/genotype.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/upload/gens.py` & `cg-60.4.2/cg/cli/upload/gens.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/upload/gisaid.py` & `cg-60.4.2/cg/cli/upload/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/upload/mutacc.py` & `cg-60.4.2/cg/cli/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/upload/nipt/base.py` & `cg-60.4.2/cg/cli/upload/nipt/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/upload/nipt/ftp.py` & `cg-60.4.2/cg/cli/upload/nipt/ftp.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/upload/nipt/statina.py` & `cg-60.4.2/cg/cli/upload/nipt/statina.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/upload/observations/observations.py` & `cg-60.4.2/cg/cli/upload/observations/observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/upload/observations/utils.py` & `cg-60.4.2/cg/cli/upload/observations/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/upload/scout.py` & `cg-60.4.2/cg/cli/upload/scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/upload/utils.py` & `cg-60.4.2/cg/cli/upload/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/upload/validate.py` & `cg-60.4.2/cg/cli/upload/validate.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/workflow/balsamic/base.py` & `cg-60.4.2/cg/cli/workflow/balsamic/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/workflow/balsamic/options.py` & `cg-60.4.2/cg/cli/workflow/balsamic/options.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/workflow/balsamic/pon.py` & `cg-60.4.2/cg/cli/workflow/balsamic/pon.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/workflow/balsamic/qc.py` & `cg-60.4.2/cg/cli/workflow/balsamic/qc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/workflow/balsamic/umi.py` & `cg-60.4.2/cg/cli/workflow/balsamic/umi.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/workflow/base.py` & `cg-60.4.2/cg/cli/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/workflow/commands.py` & `cg-60.4.2/cg/cli/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/workflow/fastq/base.py` & `cg-60.4.2/cg/cli/workflow/fastq/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/workflow/fastq/fastq_service.py` & `cg-60.4.2/cg/cli/workflow/fastq/fastq_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/workflow/fluffy/base.py` & `cg-60.4.2/cg/cli/workflow/fluffy/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/workflow/jasen/base.py` & `cg-60.4.2/cg/cli/workflow/jasen/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/workflow/microsalt/base.py` & `cg-60.4.2/cg/cli/workflow/microsalt/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/workflow/mip/base.py` & `cg-60.4.2/cg/cli/workflow/mip/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/workflow/mip/options.py` & `cg-60.4.2/cg/cli/workflow/mip/options.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/workflow/mip_dna/base.py` & `cg-60.4.2/cg/cli/workflow/mip_dna/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/workflow/mip_rna/base.py` & `cg-60.4.2/cg/cli/workflow/mip_rna/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/workflow/mutant/base.py` & `cg-60.4.2/cg/cli/workflow/mutant/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/workflow/nf_analysis.py` & `cg-60.4.2/cg/cli/workflow/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/workflow/raredisease/base.py` & `cg-60.4.2/cg/cli/workflow/raredisease/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/workflow/rnafusion/base.py` & `cg-60.4.2/cg/cli/workflow/rnafusion/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/workflow/taxprofiler/base.py` & `cg-60.4.2/cg/cli/workflow/taxprofiler/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/cli/workflow/tomte/base.py` & `cg-60.4.2/cg/cli/workflow/tomte/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/clients/arnold/api.py` & `cg-60.4.2/cg/clients/arnold/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/clients/janus/api.py` & `cg-60.4.2/cg/clients/janus/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/constants/__init__.py` & `cg-60.4.2/cg/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/constants/bcl_convert_metrics.py` & `cg-60.4.2/cg/constants/bcl_convert_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/constants/constants.py` & `cg-60.4.2/cg/constants/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/constants/delivery.py` & `cg-60.4.2/cg/constants/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/constants/demultiplexing.py` & `cg-60.4.2/cg/constants/demultiplexing.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     UNALIGNED_DIR_NAME: str = "Unaligned"
     QUEUED_FOR_POST_PROCESSING: str = "post_processing_queued.txt"
     ANALYSIS_COMPLETED: str = "Secondary_Analysis_Complete.txt"
     ANALYSIS: str = "Analysis"
     DATA: str = "Data"
     BCL_CONVERT: str = "BCLConvert"
     FLOW_CELLS_DIRECTORY_NAME: str = "flow_cells"
-    DEMULTIPLEXED_RUNS_DIRECTORY_NAME: str = "demultiplexed_runs"
     ILLUMINA_FILE_MANIFEST: str = "Manifest.tsv"
     CG_FILE_MANIFEST: str = "file_manifest.tsv"
     INTER_OP: str = "InterOp"
 
 
 class RunParametersXMLNodes(StrEnum):
     """Define names of the used XML nodes in run parameters files."""
```

### Comparing `cg-60.4.1/cg/constants/encryption.py` & `cg-60.4.2/cg/constants/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/constants/gene_panel.py` & `cg-60.4.2/cg/constants/gene_panel.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/constants/housekeeper_tags.py` & `cg-60.4.2/cg/constants/housekeeper_tags.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/constants/lims.py` & `cg-60.4.2/cg/constants/lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/constants/metrics.py` & `cg-60.4.2/cg/constants/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/constants/nextflow.py` & `cg-60.4.2/cg/constants/nextflow.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/constants/nf_analysis.py` & `cg-60.4.2/cg/constants/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/constants/observations.py` & `cg-60.4.2/cg/constants/observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/constants/orderforms.py` & `cg-60.4.2/cg/constants/orderforms.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/constants/priority.py` & `cg-60.4.2/cg/constants/priority.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/constants/report.py` & `cg-60.4.2/cg/constants/report.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/constants/sample_sources.py` & `cg-60.4.2/cg/constants/sample_sources.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/constants/scout.py` & `cg-60.4.2/cg/constants/scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/constants/sequencing.py` & `cg-60.4.2/cg/constants/sequencing.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/constants/subject.py` & `cg-60.4.2/cg/constants/subject.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/exc.py` & `cg-60.4.2/cg/exc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/io/api.py` & `cg-60.4.2/cg/io/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/io/config.py` & `cg-60.4.2/cg/io/config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/io/controller.py` & `cg-60.4.2/cg/io/controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/io/csv.py` & `cg-60.4.2/cg/io/csv.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/io/json.py` & `cg-60.4.2/cg/io/json.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/io/png.py` & `cg-60.4.2/cg/io/png.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/io/txt.py` & `cg-60.4.2/cg/io/txt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/io/validate_path.py` & `cg-60.4.2/cg/io/validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/io/xml.py` & `cg-60.4.2/cg/io/xml.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/io/yaml.py` & `cg-60.4.2/cg/io/yaml.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/archive/archive.py` & `cg-60.4.2/cg/meta/archive/archive.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/archive/ddn/constants.py` & `cg-60.4.2/cg/meta/archive/ddn/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/archive/ddn/ddn_data_flow_client.py` & `cg-60.4.2/cg/meta/archive/ddn/ddn_data_flow_client.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/archive/ddn/models.py` & `cg-60.4.2/cg/meta/archive/ddn/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/archive/ddn/utils.py` & `cg-60.4.2/cg/meta/archive/ddn/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/archive/models.py` & `cg-60.4.2/cg/meta/archive/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/backup/backup.py` & `cg-60.4.2/cg/meta/backup/backup.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/backup/pdc.py` & `cg-60.4.2/cg/meta/backup/pdc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/clean/api.py` & `cg-60.4.2/cg/meta/clean/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/clean/clean_flow_cells.py` & `cg-60.4.2/cg/meta/clean/clean_flow_cells.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/clean/clean_retrieved_spring_files.py` & `cg-60.4.2/cg/meta/clean/clean_retrieved_spring_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/compress/compress.py` & `cg-60.4.2/cg/meta/compress/compress.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/compress/files.py` & `cg-60.4.2/cg/meta/compress/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/deliver/deliver.py` & `cg-60.4.2/cg/meta/deliver/deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/deliver/deliver_ticket.py` & `cg-60.4.2/cg/meta/deliver/deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/deliver/fastq_path_generator.py` & `cg-60.4.2/cg/meta/deliver/fastq_path_generator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/delivery/delivery.py` & `cg-60.4.2/cg/meta/delivery/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/demultiplex/combine_sequencing_metrics.py` & `cg-60.4.2/cg/meta/demultiplex/combine_sequencing_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/demultiplex/demux_post_processing.py` & `cg-60.4.2/cg/meta/demultiplex/demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/demultiplex/files.py` & `cg-60.4.2/cg/meta/demultiplex/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/demultiplex/housekeeper_storage_functions.py` & `cg-60.4.2/cg/meta/demultiplex/housekeeper_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/demultiplex/status_db_storage_functions.py` & `cg-60.4.2/cg/meta/demultiplex/status_db_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/demultiplex/utils.py` & `cg-60.4.2/cg/meta/demultiplex/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/demultiplex/validation.py` & `cg-60.4.2/cg/meta/demultiplex/validation.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/encryption/encryption.py` & `cg-60.4.2/cg/meta/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/encryption/sbatch.py` & `cg-60.4.2/cg/meta/encryption/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/invoice.py` & `cg-60.4.2/cg/meta/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/meta.py` & `cg-60.4.2/cg/meta/meta.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/observations/balsamic_observations_api.py` & `cg-60.4.2/cg/meta/observations/balsamic_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/observations/mip_dna_observations_api.py` & `cg-60.4.2/cg/meta/observations/mip_dna_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/observations/observations_api.py` & `cg-60.4.2/cg/meta/observations/observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/orders/api.py` & `cg-60.4.2/cg/meta/orders/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/orders/case_submitter.py` & `cg-60.4.2/cg/meta/orders/case_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/orders/fastq_submitter.py` & `cg-60.4.2/cg/meta/orders/fastq_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/orders/lims.py` & `cg-60.4.2/cg/meta/orders/lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/orders/metagenome_submitter.py` & `cg-60.4.2/cg/meta/orders/metagenome_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/orders/microbial_submitter.py` & `cg-60.4.2/cg/meta/orders/microbial_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/orders/pool_submitter.py` & `cg-60.4.2/cg/meta/orders/pool_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/orders/rnafusion_submitter.py` & `cg-60.4.2/cg/meta/orders/rnafusion_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/orders/sars_cov_2_submitter.py` & `cg-60.4.2/cg/meta/orders/sars_cov_2_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/orders/submitter.py` & `cg-60.4.2/cg/meta/orders/submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/orders/ticket_handler.py` & `cg-60.4.2/cg/meta/orders/ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/qc_metrics/collect_qc_metrics.py` & `cg-60.4.2/cg/meta/qc_metrics/collect_qc_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/balsamic.py` & `cg-60.4.2/cg/meta/report/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/balsamic_qc.py` & `cg-60.4.2/cg/meta/report/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/balsamic_umi.py` & `cg-60.4.2/cg/meta/report/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/field_validators.py` & `cg-60.4.2/cg/meta/report/field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/mip_dna.py` & `cg-60.4.2/cg/meta/report/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/report_api.py` & `cg-60.4.2/cg/meta/report/report_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/rnafusion.py` & `cg-60.4.2/cg/meta/report/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/templates/delivery-report.html` & `cg-60.4.2/cg/meta/report/templates/delivery-report.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/templates/macros/data_analysis/data_analysis.html` & `cg-60.4.2/cg/meta/report/templates/macros/data_analysis/data_analysis.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/templates/macros/data_analysis/limitations.html` & `cg-60.4.2/cg/meta/report/templates/macros/data_analysis/limitations.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html` & `cg-60.4.2/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html` & `cg-60.4.2/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html` & `cg-60.4.2/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html` & `cg-60.4.2/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html` & `cg-60.4.2/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/templates/macros/header.html` & `cg-60.4.2/cg/meta/report/templates/macros/header.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/templates/macros/order.html` & `cg-60.4.2/cg/meta/report/templates/macros/order.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/templates/macros/sample_prep.html` & `cg-60.4.2/cg/meta/report/templates/macros/sample_prep.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html` & `cg-60.4.2/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html` & `cg-60.4.2/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html` & `cg-60.4.2/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/templates/static/css/bootstrap.min.css` & `cg-60.4.2/cg/meta/report/templates/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/templates/static/images/SWEDAC_logo.png` & `cg-60.4.2/cg/meta/report/templates/static/images/SWEDAC_logo.png`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/report/tomte.py` & `cg-60.4.2/cg/meta/report/tomte.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/rsync/rsync_api.py` & `cg-60.4.2/cg/meta/rsync/rsync_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/tar/tar.py` & `cg-60.4.2/cg/meta/tar/tar.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/transfer/external_data.py` & `cg-60.4.2/cg/meta/transfer/external_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/transfer/lims.py` & `cg-60.4.2/cg/meta/transfer/lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/upload/balsamic/balsamic.py` & `cg-60.4.2/cg/meta/upload/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/upload/coverage.py` & `cg-60.4.2/cg/meta/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/upload/fohm/fohm.py` & `cg-60.4.2/cg/meta/upload/fohm/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/upload/gisaid/constants.py` & `cg-60.4.2/cg/meta/upload/gisaid/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/upload/gisaid/gisaid.py` & `cg-60.4.2/cg/meta/upload/gisaid/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/upload/gisaid/models.py` & `cg-60.4.2/cg/meta/upload/gisaid/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/upload/gt.py` & `cg-60.4.2/cg/meta/upload/gt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/upload/microsalt/microsalt_upload_api.py` & `cg-60.4.2/cg/meta/upload/microsalt/microsalt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/upload/mip/mip_dna.py` & `cg-60.4.2/cg/meta/upload/mip/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/upload/mip/mip_rna.py` & `cg-60.4.2/cg/meta/upload/mip/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/upload/mutacc.py` & `cg-60.4.2/cg/meta/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/upload/nf_analysis.py` & `cg-60.4.2/cg/meta/upload/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/upload/nipt/models.py` & `cg-60.4.2/cg/meta/upload/nipt/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/upload/nipt/nipt.py` & `cg-60.4.2/cg/meta/upload/nipt/nipt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/upload/scout/balsamic_config_builder.py` & `cg-60.4.2/cg/meta/upload/scout/balsamic_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/upload/scout/balsamic_umi_config_builder.py` & `cg-60.4.2/cg/meta/upload/scout/balsamic_umi_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/upload/scout/hk_tags.py` & `cg-60.4.2/cg/meta/upload/scout/hk_tags.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/upload/scout/mip_config_builder.py` & `cg-60.4.2/cg/meta/upload/scout/mip_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/upload/scout/rnafusion_config_builder.py` & `cg-60.4.2/cg/meta/upload/scout/rnafusion_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/upload/scout/scout_config_builder.py` & `cg-60.4.2/cg/meta/upload/scout/scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/upload/scout/uploadscoutapi.py` & `cg-60.4.2/cg/meta/upload/scout/uploadscoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/upload/upload_api.py` & `cg-60.4.2/cg/meta/upload/upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/analysis.py` & `cg-60.4.2/cg/meta/workflow/analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/balsamic.py` & `cg-60.4.2/cg/meta/workflow/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/balsamic_pon.py` & `cg-60.4.2/cg/meta/workflow/balsamic_pon.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/balsamic_qc.py` & `cg-60.4.2/cg/meta/workflow/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/balsamic_umi.py` & `cg-60.4.2/cg/meta/workflow/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/downsample/downsample.py` & `cg-60.4.2/cg/meta/workflow/downsample/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/downsample/sbatch.py` & `cg-60.4.2/cg/meta/workflow/downsample/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/fastq.py` & `cg-60.4.2/cg/meta/workflow/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/fluffy.py` & `cg-60.4.2/cg/meta/workflow/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/jasen.py` & `cg-60.4.2/cg/meta/workflow/jasen.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/microsalt/metrics_parser/models.py` & `cg-60.4.2/cg/meta/workflow/microsalt/metrics_parser/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/microsalt/microsalt.py` & `cg-60.4.2/cg/meta/workflow/microsalt/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/microsalt/quality_controller/models.py` & `cg-60.4.2/cg/meta/workflow/microsalt/quality_controller/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/microsalt/quality_controller/quality_controller.py` & `cg-60.4.2/cg/meta/workflow/microsalt/quality_controller/quality_controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/microsalt/quality_controller/report_generator.py` & `cg-60.4.2/cg/meta/workflow/microsalt/quality_controller/report_generator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/microsalt/quality_controller/result_logger.py` & `cg-60.4.2/cg/meta/workflow/microsalt/quality_controller/result_logger.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/microsalt/quality_controller/utils.py` & `cg-60.4.2/cg/meta/workflow/microsalt/quality_controller/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/microsalt/utils.py` & `cg-60.4.2/cg/meta/workflow/microsalt/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/mip.py` & `cg-60.4.2/cg/meta/workflow/mip.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/mip_dna.py` & `cg-60.4.2/cg/meta/workflow/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/mip_rna.py` & `cg-60.4.2/cg/meta/workflow/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/mutant.py` & `cg-60.4.2/cg/meta/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/nf_analysis.py` & `cg-60.4.2/cg/meta/workflow/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/nf_handlers.py` & `cg-60.4.2/cg/meta/workflow/nf_handlers.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/prepare_fastq.py` & `cg-60.4.2/cg/meta/workflow/prepare_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/raredisease.py` & `cg-60.4.2/cg/meta/workflow/raredisease.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/rnafusion.py` & `cg-60.4.2/cg/meta/workflow/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/taxprofiler.py` & `cg-60.4.2/cg/meta/workflow/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/meta/workflow/tomte.py` & `cg-60.4.2/cg/meta/workflow/tomte.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/balsamic/config.py` & `cg-60.4.2/cg/models/balsamic/config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/balsamic/metrics.py` & `cg-60.4.2/cg/models/balsamic/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/cg_config.py` & `cg-60.4.2/cg/models/cg_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/compression_data.py` & `cg-60.4.2/cg/models/compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/deliverables/metric_deliverables.py` & `cg-60.4.2/cg/models/deliverables/metric_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/demultiplex/run_parameters.py` & `cg-60.4.2/cg/models/demultiplex/run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/demultiplex/sbatch.py` & `cg-60.4.2/cg/models/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/downsample/downsample_data.py` & `cg-60.4.2/cg/models/downsample/downsample_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/fastq.py` & `cg-60.4.2/cg/models/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/file_data.py` & `cg-60.4.2/cg/models/file_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/flow_cell/flow_cell.py` & `cg-60.4.2/cg/models/flow_cell/flow_cell.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         self._sample_sheet_path_hk: Path | None = None
         self.sample_sheet_validator = SampleSheetValidator()
 
     def parse_flow_cell_dir_name(self):
         """Parse relevant information from flow cell name.
         This will assume that the flow cell naming convention is used. If not we skip the flow cell.
         Convention is: <date>_<machine>_<run_numbers>_<A|B><flow_cell_id>
-        Example: '201203_D00483_0200_AHVKJCDRXX'.
+        Example: '230912_A00187_1009_AHK33MDRX3'.
         """
 
         self.validate_flow_cell_dir_name()
         self.run_date = self._parse_date()
         self.machine_name = self.split_flow_cell_name[1]
         self.machine_number = int(self.split_flow_cell_name[2])
         base_name: str = self.split_flow_cell_name[-1]
@@ -158,15 +158,15 @@
             return datetime.datetime.strptime(self.split_flow_cell_name[0], "%Y%m%d")
         return datetime.datetime.strptime(self.split_flow_cell_name[0], "%y%m%d")
 
     def validate_flow_cell_dir_name(self) -> None:
         """
         Validate on the following criteria:
         Convention is: <date>_<machine>_<run_numbers>_<A|B><flow_cell_id>
-        Example: '201203_D00483_0200_AHVKJCDRXX'.
+        Example: '230912_A00187_1009_AHK33MDRX3'.
         """
         if len(self.split_flow_cell_name) != 4:
             message = f"Flowcell {self.full_name} does not follow the flow cell naming convention"
             LOG.warning(message)
             raise FlowCellError(message)
 
     def has_demultiplexing_started_locally(self) -> bool:
```

### Comparing `cg-60.4.1/cg/models/invoice/invoice.py` & `cg-60.4.2/cg/models/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/lims/sample.py` & `cg-60.4.2/cg/models/lims/sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/mip/mip_config.py` & `cg-60.4.2/cg/models/mip/mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/mip/mip_metrics_deliverables.py` & `cg-60.4.2/cg/models/mip/mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/mip/mip_sample_info.py` & `cg-60.4.2/cg/models/mip/mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/nf_analysis.py` & `cg-60.4.2/cg/models/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/observations/input_files.py` & `cg-60.4.2/cg/models/observations/input_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/orders/constants.py` & `cg-60.4.2/cg/models/orders/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/orders/excel_sample.py` & `cg-60.4.2/cg/models/orders/excel_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/orders/json_sample.py` & `cg-60.4.2/cg/models/orders/json_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/orders/order.py` & `cg-60.4.2/cg/models/orders/order.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/orders/orderform_schema.py` & `cg-60.4.2/cg/models/orders/orderform_schema.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/orders/sample_base.py` & `cg-60.4.2/cg/models/orders/sample_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/orders/samples.py` & `cg-60.4.2/cg/models/orders/samples.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/orders/validators/excel_sample_validators.py` & `cg-60.4.2/cg/models/orders/validators/excel_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/orders/validators/json_sample_validators.py` & `cg-60.4.2/cg/models/orders/validators/json_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/raredisease/raredisease.py` & `cg-60.4.2/cg/models/raredisease/raredisease.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/report/metadata.py` & `cg-60.4.2/cg/models/report/metadata.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/report/report.py` & `cg-60.4.2/cg/models/report/report.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/report/sample.py` & `cg-60.4.2/cg/models/report/sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/report/validators.py` & `cg-60.4.2/cg/models/report/validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/rnafusion/rnafusion.py` & `cg-60.4.2/cg/models/rnafusion/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/scout/scout_load_config.py` & `cg-60.4.2/cg/models/scout/scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/slurm/sbatch.py` & `cg-60.4.2/cg/models/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/taxprofiler/taxprofiler.py` & `cg-60.4.2/cg/models/taxprofiler/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/tomte/tomte.py` & `cg-60.4.2/cg/models/tomte/tomte.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/models/workflow/mutant.py` & `cg-60.4.2/cg/models/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/resources/__init__.py` & `cg-60.4.2/cg/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/resources/rnafusion_bundle_filenames.yaml` & `cg-60.4.2/cg/resources/rnafusion_bundle_filenames.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/resources/taxprofiler_bundle_filenames.yaml` & `cg-60.4.2/cg/resources/taxprofiler_bundle_filenames.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/resources/tomte_bundle_filenames.yaml` & `cg-60.4.2/cg/resources/tomte_bundle_filenames.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/server/admin.py` & `cg-60.4.2/cg/server/admin.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/server/api.py` & `cg-60.4.2/cg/server/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/server/app.py` & `cg-60.4.2/cg/server/app.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/server/config.py` & `cg-60.4.2/cg/server/config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/server/dto/orders/orders_request.py` & `cg-60.4.2/cg/server/dto/orders/orders_request.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/server/ext.py` & `cg-60.4.2/cg/server/ext.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/server/invoices/templates/invoices/index.html` & `cg-60.4.2/cg/server/invoices/templates/invoices/index.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/server/invoices/templates/invoices/invoice.html` & `cg-60.4.2/cg/server/invoices/templates/invoices/invoice.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/server/invoices/templates/invoices/layout.html` & `cg-60.4.2/cg/server/invoices/templates/invoices/layout.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/server/invoices/templates/invoices/new.html` & `cg-60.4.2/cg/server/invoices/templates/invoices/new.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/server/invoices/views.py` & `cg-60.4.2/cg/server/invoices/views.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/delivery_message/delivery_message_service.py` & `cg-60.4.2/cg/services/delivery_message/delivery_message_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/delivery_message/messages/__init__.py` & `cg-60.4.2/cg/services/delivery_message/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/delivery_message/messages/analysis_scout_message.py` & `cg-60.4.2/cg/services/delivery_message/messages/analysis_scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/delivery_message/messages/covid_message.py` & `cg-60.4.2/cg/services/delivery_message/messages/covid_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/delivery_message/messages/fastq_analysis_scout_message.py` & `cg-60.4.2/cg/services/delivery_message/messages/fastq_analysis_scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/delivery_message/messages/fastq_message.py` & `cg-60.4.2/cg/services/delivery_message/messages/fastq_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/delivery_message/messages/fastq_scout_message.py` & `cg-60.4.2/cg/services/delivery_message/messages/fastq_scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/delivery_message/messages/microsalt_mwr_message.py` & `cg-60.4.2/cg/services/delivery_message/messages/microsalt_mwr_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/delivery_message/messages/microsalt_mwx_message.py` & `cg-60.4.2/cg/services/delivery_message/messages/microsalt_mwx_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/delivery_message/messages/scout_message.py` & `cg-60.4.2/cg/services/delivery_message/messages/scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/delivery_message/messages/statina_message.py` & `cg-60.4.2/cg/services/delivery_message/messages/statina_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/delivery_message/messages/utils.py` & `cg-60.4.2/cg/services/delivery_message/messages/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/delivery_message/utils.py` & `cg-60.4.2/cg/services/delivery_message/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/fastq_file_service/fastq_file_service.py` & `cg-60.4.2/cg/services/fastq_file_service/fastq_file_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/fastq_file_service/utils.py` & `cg-60.4.2/cg/services/fastq_file_service/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/orders/order_service/order_service.py` & `cg-60.4.2/cg/services/orders/order_service/order_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/orders/order_service/utils.py` & `cg-60.4.2/cg/services/orders/order_service/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/orders/order_status_service/order_summary_service.py` & `cg-60.4.2/cg/services/orders/order_status_service/order_summary_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/orders/order_status_service/utils.py` & `cg-60.4.2/cg/services/orders/order_status_service/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/quality_controller/quality_checks/checks.py` & `cg-60.4.2/cg/services/quality_controller/quality_checks/checks.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/quality_controller/quality_checks/utils.py` & `cg-60.4.2/cg/services/quality_controller/quality_checks/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/quality_controller/quality_controller_service.py` & `cg-60.4.2/cg/services/quality_controller/quality_controller_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/slurm_service/slurm_cli_service.py` & `cg-60.4.2/cg/services/slurm_service/slurm_cli_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/services/slurm_upload_service/slurm_upload_service.py` & `cg-60.4.2/cg/services/slurm_upload_service/slurm_upload_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/base.py` & `cg-60.4.2/cg/store/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/crud/create.py` & `cg-60.4.2/cg/store/crud/create.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/crud/delete.py` & `cg-60.4.2/cg/store/crud/delete.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/crud/read.py` & `cg-60.4.2/cg/store/crud/read.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/crud/update.py` & `cg-60.4.2/cg/store/crud/update.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/database.py` & `cg-60.4.2/cg/store/database.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/filters/status_analysis_filters.py` & `cg-60.4.2/cg/store/filters/status_analysis_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/filters/status_application_filters.py` & `cg-60.4.2/cg/store/filters/status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/filters/status_application_limitations_filters.py` & `cg-60.4.2/cg/store/filters/status_application_limitations_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/filters/status_application_version_filters.py` & `cg-60.4.2/cg/store/filters/status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/filters/status_bed_filters.py` & `cg-60.4.2/cg/store/filters/status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/filters/status_bed_version_filters.py` & `cg-60.4.2/cg/store/filters/status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/filters/status_case_filters.py` & `cg-60.4.2/cg/store/filters/status_case_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/filters/status_case_sample_filters.py` & `cg-60.4.2/cg/store/filters/status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/filters/status_collaboration_filters.py` & `cg-60.4.2/cg/store/filters/status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/filters/status_customer_filters.py` & `cg-60.4.2/cg/store/filters/status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/filters/status_flow_cell_filters.py` & `cg-60.4.2/cg/store/filters/status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/filters/status_invoice_filters.py` & `cg-60.4.2/cg/store/filters/status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/filters/status_metrics_filters.py` & `cg-60.4.2/cg/store/filters/status_metrics_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/filters/status_order_filters.py` & `cg-60.4.2/cg/store/filters/status_order_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/filters/status_organism_filters.py` & `cg-60.4.2/cg/store/filters/status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/filters/status_panel_filters.py` & `cg-60.4.2/cg/store/filters/status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/filters/status_pool_filters.py` & `cg-60.4.2/cg/store/filters/status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/filters/status_sample_filters.py` & `cg-60.4.2/cg/store/filters/status_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/filters/status_user_filters.py` & `cg-60.4.2/cg/store/filters/status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/models.py` & `cg-60.4.2/cg/store/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/store/store.py` & `cg-60.4.2/cg/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/utils/checksum/checksum.py` & `cg-60.4.2/cg/utils/checksum/checksum.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/utils/click/EnumChoice.py` & `cg-60.4.2/cg/utils/click/EnumChoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/utils/commands.py` & `cg-60.4.2/cg/utils/commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/utils/date.py` & `cg-60.4.2/cg/utils/date.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/utils/dict.py` & `cg-60.4.2/cg/utils/dict.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/utils/dispatcher.py` & `cg-60.4.2/cg/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/utils/email.py` & `cg-60.4.2/cg/utils/email.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/utils/files.py` & `cg-60.4.2/cg/utils/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/utils/flask/enum.py` & `cg-60.4.2/cg/utils/flask/enum.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/utils/time.py` & `cg-60.4.2/cg/utils/time.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/cg/utils/utils.py` & `cg-60.4.2/cg/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/pyproject.toml` & `cg-60.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cg"
-version = "60.4.1"
+version = "60.4.2"
 description = "Clinical Genomics command center"
 authors = ["Clinical Genomics <support@clinicalgenomics.se>"]
 readme = "README.md"
 homepage = "https://github.com/Clinical-Genomics/cg"
 repository = "https://github.com/Clinical-Genomics/cg"
 classifiers = [
   "Programming Language :: Python",
```

### Comparing `cg-60.4.1/tests/apps/conftest.py` & `cg-60.4.2/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/coverage/test_coverage.py` & `cg-60.4.2/tests/apps/coverage/test_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/crunchy/conftest.py` & `cg-60.4.2/tests/apps/crunchy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/crunchy/test_compress_fastq.py` & `cg-60.4.2/tests/apps/crunchy/test_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/crunchy/test_config.py` & `cg-60.4.2/tests/apps/crunchy/test_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/crunchy/test_crunchy.py` & `cg-60.4.2/tests/apps/crunchy/test_crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/crunchy/test_spring_decompression.py` & `cg-60.4.2/tests/apps/crunchy/test_spring_decompression.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/demultiplex/conftest.py` & `cg-60.4.2/tests/apps/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/demultiplex/test_create_sample_sheet.py` & `cg-60.4.2/tests/apps/demultiplex/test_create_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/demultiplex/test_demultiplex_api.py` & `cg-60.4.2/tests/apps/demultiplex/test_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/demultiplex/test_index.py` & `cg-60.4.2/tests/apps/demultiplex/test_index.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/demultiplex/test_override_cycles_validator.py` & `cg-60.4.2/tests/apps/demultiplex/test_override_cycles_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/demultiplex/test_read_sample_sheet.py` & `cg-60.4.2/tests/apps/demultiplex/test_read_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/demultiplex/test_sample_models.py` & `cg-60.4.2/tests/apps/demultiplex/test_sample_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/demultiplex/test_sample_sheet_creator.py` & `cg-60.4.2/tests/apps/demultiplex/test_sample_sheet_creator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/demultiplex/test_sample_sheet_models.py` & `cg-60.4.2/tests/apps/demultiplex/test_sample_sheet_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/demultiplex/test_sample_sheet_validator.py` & `cg-60.4.2/tests/apps/demultiplex/test_sample_sheet_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/demultiplex/test_translate_sample_sheet.py` & `cg-60.4.2/tests/apps/demultiplex/test_translate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/demultiplex/test_validate.py` & `cg-60.4.2/tests/apps/demultiplex/test_validate.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/downsample/test_downsample.py` & `cg-60.4.2/tests/apps/downsample/test_downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/downsample/test_downsample_utils.py` & `cg-60.4.2/tests/apps/downsample/test_downsample_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/gens/test_gens_api.py` & `cg-60.4.2/tests/apps/gens/test_gens_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/gt/conftest.py` & `cg-60.4.2/tests/apps/gt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/gt/test_gt_api.py` & `cg-60.4.2/tests/apps/gt/test_gt_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/hk/conftest.py` & `cg-60.4.2/tests/apps/hk/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/hk/test__getattr__.py` & `cg-60.4.2/tests/apps/hk/test__getattr__.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/hk/test_add_file.py` & `cg-60.4.2/tests/apps/hk/test_add_file.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/hk/test_bundles.py` & `cg-60.4.2/tests/apps/hk/test_bundles.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/hk/test_core.py` & `cg-60.4.2/tests/apps/hk/test_core.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/hk/test_file.py` & `cg-60.4.2/tests/apps/hk/test_file.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/hk/test_version.py` & `cg-60.4.2/tests/apps/hk/test_version.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/lims/conftest.py` & `cg-60.4.2/tests/apps/lims/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/lims/test_api.py` & `cg-60.4.2/tests/apps/lims/test_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/lims/test_sample_sheet.py` & `cg-60.4.2/tests/apps/lims/test_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/loqus/conftest.py` & `cg-60.4.2/tests/apps/loqus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/loqus/test_loqusdb_api.py` & `cg-60.4.2/tests/apps/loqus/test_loqusdb_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/madeline/conftest.py` & `cg-60.4.2/tests/apps/madeline/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/madeline/test_madeline.py` & `cg-60.4.2/tests/apps/madeline/test_madeline.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/mip/conftest.py` & `cg-60.4.2/tests/apps/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/mip/test_config_mip.py` & `cg-60.4.2/tests/apps/mip/test_config_mip.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/mutacc_auto/conftest.py` & `cg-60.4.2/tests/apps/mutacc_auto/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/mutacc_auto/test_mutacc_auto.py` & `cg-60.4.2/tests/apps/mutacc_auto/test_mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/orderform/conftest.py` & `cg-60.4.2/tests/apps/orderform/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/orderform/test_excel_orderform_parser.py` & `cg-60.4.2/tests/apps/orderform/test_excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/orderform/test_excel_sample_schema.py` & `cg-60.4.2/tests/apps/orderform/test_excel_sample_schema.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/orderform/test_json_orderform_parser.py` & `cg-60.4.2/tests/apps/orderform/test_json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/orderform/test_orderform_parser.py` & `cg-60.4.2/tests/apps/orderform/test_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/orderform/validators/test_excel_sample_validators.py` & `cg-60.4.2/tests/apps/orderform/validators/test_excel_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/scout/conftest.py` & `cg-60.4.2/tests/apps/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/scout/test_get_causative_variants.py` & `cg-60.4.2/tests/apps/scout/test_get_causative_variants.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/scout/test_get_scout_cases.py` & `cg-60.4.2/tests/apps/scout/test_get_scout_cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/scout/test_scout_load_config.py` & `cg-60.4.2/tests/apps/scout/test_scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/scout/test_scout_models.py` & `cg-60.4.2/tests/apps/scout/test_scout_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/sequencing_metrics_parser/conftest.py` & `cg-60.4.2/tests/apps/sequencing_metrics_parser/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py` & `cg-60.4.2/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/sequencing_metrics_parser/parsers/test_sequencing_metrics_parser_api.py` & `cg-60.4.2/tests/apps/sequencing_metrics_parser/parsers/test_sequencing_metrics_parser_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/slurm/conftest.py` & `cg-60.4.2/tests/apps/slurm/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/slurm/test_slurm_api.py` & `cg-60.4.2/tests/apps/slurm/test_slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/test_apps_environ.py` & `cg-60.4.2/tests/apps/test_apps_environ.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/apps/test_osticket.py` & `cg-60.4.2/tests/apps/test_osticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/add/test_cli_add.py` & `cg-60.4.2/tests/cli/add/test_cli_add.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/add/test_cli_add_customer.py` & `cg-60.4.2/tests/cli/add/test_cli_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/add/test_cli_add_family.py` & `cg-60.4.2/tests/cli/add/test_cli_add_family.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/add/test_cli_add_relationship.py` & `cg-60.4.2/tests/cli/add/test_cli_add_relationship.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/add/test_cli_add_sample.py` & `cg-60.4.2/tests/cli/add/test_cli_add_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/backup/conftest.py` & `cg-60.4.2/tests/cli/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/backup/test_backup_command.py` & `cg-60.4.2/tests/cli/backup/test_backup_command.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/clean/conftest.py` & `cg-60.4.2/tests/cli/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/clean/test_balsamic_clean.py` & `cg-60.4.2/tests/cli/clean/test_balsamic_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/clean/test_clean_flow_cell.py` & `cg-60.4.2/tests/cli/clean/test_clean_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/clean/test_clean_hk_bundle_files.py` & `cg-60.4.2/tests/cli/clean/test_clean_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/clean/test_hk_bundle_files.py` & `cg-60.4.2/tests/cli/clean/test_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/clean/test_hk_case_bundle_files.py` & `cg-60.4.2/tests/cli/clean/test_hk_case_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/clean/test_microbial_clean.py` & `cg-60.4.2/tests/cli/clean/test_microbial_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/clean/test_rsync_past_run_dirs.py` & `cg-60.4.2/tests/cli/clean/test_rsync_past_run_dirs.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/compress/conftest.py` & `cg-60.4.2/tests/cli/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/compress/test_cli_compress_fastq.py` & `cg-60.4.2/tests/cli/compress/test_cli_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/compress/test_cli_decompress_spring.py` & `cg-60.4.2/tests/cli/compress/test_cli_decompress_spring.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/compress/test_compress_helpers.py` & `cg-60.4.2/tests/cli/compress/test_compress_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/compress/test_store_fastq.py` & `cg-60.4.2/tests/cli/compress/test_store_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/conftest.py` & `cg-60.4.2/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/delete/test_cli_delete_case.py` & `cg-60.4.2/tests/cli/delete/test_cli_delete_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/delete/test_cli_delete_cases.py` & `cg-60.4.2/tests/cli/delete/test_cli_delete_cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/deliver/conftest.py` & `cg-60.4.2/tests/cli/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/deliver/test_deliver_base.py` & `cg-60.4.2/tests/cli/deliver/test_deliver_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/deliver/test_rsync_base.py` & `cg-60.4.2/tests/cli/deliver/test_rsync_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/deliver/test_run_deliver_cmd.py` & `cg-60.4.2/tests/cli/deliver/test_run_deliver_cmd.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/demultiplex/test_create_sample_sheet.py` & `cg-60.4.2/tests/cli/demultiplex/test_create_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/demultiplex/test_demultiplex_flowcell.py` & `cg-60.4.2/tests/cli/demultiplex/test_demultiplex_flowcell.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 )
 from cg.models.cg_config import CGConfig
 from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
 
 
 def test_demultiplex_dragen_flowcell(
     cli_runner: testing.CliRunner,
-    tmp_flow_cell_directory_bclconvert: Path,
+    tmp_flow_cell_directory_bcl_convert: Path,
     demultiplexing_context_for_demux: CGConfig,
     caplog,
     mocker,
 ):
     caplog.set_level(logging.INFO)
 
     # GIVEN that all files are present for Dragen demultiplexing
 
-    flow_cell = FlowCellDirectoryData(tmp_flow_cell_directory_bclconvert)
+    flow_cell = FlowCellDirectoryData(tmp_flow_cell_directory_bcl_convert)
     add_and_include_sample_sheet_path_to_housekeeper(
-        flow_cell_directory=tmp_flow_cell_directory_bclconvert,
+        flow_cell_directory=tmp_flow_cell_directory_bcl_convert,
         flow_cell_name=flow_cell.id,
         hk_api=demultiplexing_context_for_demux.housekeeper_api,
     )
 
     # GIVEN a flow cell that is ready for demultiplexing
     demux_api: DemultiplexingAPI = demultiplexing_context_for_demux.demultiplex_api
     demux_dir: Path = demux_api.flow_cell_out_dir_path(flow_cell)
@@ -44,15 +44,15 @@
     marker_file = Path(demux_dir, "dummy_file_present_in_old_dir")
     marker_file.touch()
     assert marker_file.exists()
 
     # WHEN starting demultiplexing from the CLI
     result: testing.Result = cli_runner.invoke(
         demultiplex_flow_cell,
-        [str(tmp_flow_cell_directory_bclconvert)],
+        [str(tmp_flow_cell_directory_bcl_convert)],
         obj=demultiplexing_context_for_demux,
     )
 
     # THEN assert the command exits without problems
     assert result.exit_code == 0
 
     # THEN assert the results folder was created
@@ -101,20 +101,20 @@
     # THEN assert it found the directory
     assert "Found directory" in caplog.text
 
     # THEN assert it found a flow cell that is ready for demultiplexing
     assert f"Flow cell {flow_cell.id} is ready for downstream processing" in caplog.text
 
 
-def test_is_demultiplexing_complete(tmp_flow_cell_directory_bcl2fastq: Path):
+def test_is_demultiplexing_complete(tmp_novaseq_6000_pre_1_5_kits_flow_cell_path: Path):
     """Tests the is_demultiplexing_complete property of FlowCellDirectoryData."""
 
     # GIVEN a demultiplexing directory with no demuxcomplete.txt file
     flow_cell: FlowCellDirectoryData = FlowCellDirectoryData(
-        flow_cell_path=tmp_flow_cell_directory_bcl2fastq
+        flow_cell_path=tmp_novaseq_6000_pre_1_5_kits_flow_cell_path
     )
     assert not flow_cell.is_demultiplexing_complete
 
     # WHEN creating the demuxcomplete.txt file
     Path(flow_cell.path, DemultiplexingDirsAndFiles.DEMUX_COMPLETE).touch()
 
     # THEN the property should return true
```

### Comparing `cg-60.4.1/tests/cli/demultiplex/test_finish_demux.py` & `cg-60.4.2/tests/cli/demultiplex/test_finish_demux.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,26 +33,26 @@
 
 
 def test_finish_flow_cell_dry_run(
     caplog,
     cli_runner: testing.CliRunner,
     demultiplex_context: CGConfig,
     tmp_illumina_demultiplexed_flow_cells_directory,
-    bcl2fastq_flow_cell_full_name: str,
+    novaseq_6000_pre_1_5_kits_flow_cell_full_name: str,
 ):
     caplog.set_level(logging.INFO)
 
     # GIVEN a demultiplex flow cell finished output directory that exist
 
     # GIVEN a demultiplex context
 
     # GIVEN a flow cell id
 
     # WHEN starting post-processing for new demultiplexing from the CLI with dry run flag
     result: testing.Result = cli_runner.invoke(
         finish_flow_cell,
-        ["--dry-run", bcl2fastq_flow_cell_full_name],
+        ["--dry-run", novaseq_6000_pre_1_5_kits_flow_cell_full_name],
         obj=demultiplex_context,
     )
 
     # THEN assert the command exits successfully
     assert result.exit_code == EXIT_SUCCESS
```

### Comparing `cg-60.4.1/tests/cli/demultiplex/test_validate_sample_sheet.py` & `cg-60.4.2/tests/cli/demultiplex/test_validate_sample_sheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,21 +30,21 @@
     assert result.exit_code != EXIT_SUCCESS
     # THEN assert the correct information was communicated
     assert f"File '{sample_sheet.name}' does not exist" in result.output
 
 
 def test_validate_sample_sheet_wrong_file_type(
     cli_runner: CliRunner,
-    novaseq_6000_run_parameters_path: Path,
+    novaseq_6000_run_parameters_pre_1_5_kits_path: Path,
     sample_sheet_context: CGConfig,
     caplog,
 ):
     """Test validate sample sheet when sample sheet is in wrong format."""
     # GIVEN an existing file in the wrong file format
-    sample_sheet: Path = novaseq_6000_run_parameters_path
+    sample_sheet: Path = novaseq_6000_run_parameters_pre_1_5_kits_path
     assert sample_sheet.exists()
     assert sample_sheet.suffix != FileExtensions.CSV
 
     # WHEN validating the sample sheet
     result: Result = cli_runner.invoke(
         validate_sample_sheet,
         [str(sample_sheet)],
```

### Comparing `cg-60.4.1/tests/cli/demultiplex/test_verify_syncing.py` & `cg-60.4.2/tests/cli/demultiplex/test_verify_syncing.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,23 @@
 from cg.cli.demultiplex.demux import create_manifest_files
 from cg.constants.demultiplexing import DemultiplexingDirsAndFiles
 from cg.io.csv import read_csv
 from tests.meta.demultiplex.conftest import get_all_files_in_directory_tree
 
 
 def test_create_manifest_files_true(
-    cli_runner, tmp_flow_cells_directory_ready_for_demultiplexing_bcl_convert: Path
+    cli_runner, tmp_flow_cells_directory_ready_for_demultiplexing: Path
 ):
     """Test that manifest files are created for flow cells where the sequencing is complete."""
     # GIVEN two flowcell directories
-    first_flowcell_directory: Path = tmp_flow_cells_directory_ready_for_demultiplexing_bcl_convert
+    first_flowcell_directory: Path = tmp_flow_cells_directory_ready_for_demultiplexing
     second_flowcell_directory = Path(
         shutil.copytree(
             first_flowcell_directory,
-            Path(
-                tmp_flow_cells_directory_ready_for_demultiplexing_bcl_convert.parent, "flowcell_2"
-            ),
+            Path(tmp_flow_cells_directory_ready_for_demultiplexing.parent, "flowcell_2"),
         )
     )
 
     # WHEN creating manifest files
     cli_runner.invoke(
         cli=create_manifest_files,
         args=["--source-directory", first_flowcell_directory.parent.as_posix()],
@@ -37,26 +35,24 @@
         # THEN the manifest file should contain all files in the flowcell directory
         assert_manifest_file_contains_all_files(
             manifest_file=manifest_file, directory_of_interest=flow_cell
         )
 
 
 def test_create_manifest_files_false(
-    cli_runner, tmp_flow_cells_directory_ready_for_demultiplexing_bcl_convert: Path
+    cli_runner, tmp_flow_cells_directory_ready_for_demultiplexing: Path
 ):
     """Test that manifest files are not created for flow cells where the sequencing is not complete."""
     # GIVEN two flowcell directories with missing CopyComplete.txt
-    first_flowcell_directory = tmp_flow_cells_directory_ready_for_demultiplexing_bcl_convert
+    first_flowcell_directory = tmp_flow_cells_directory_ready_for_demultiplexing
     Path(first_flowcell_directory, DemultiplexingDirsAndFiles.COPY_COMPLETE).unlink()
     second_flowcell_directory = Path(
         shutil.copytree(
             first_flowcell_directory,
-            Path(
-                tmp_flow_cells_directory_ready_for_demultiplexing_bcl_convert.parent, "flowcell_2"
-            ),
+            Path(tmp_flow_cells_directory_ready_for_demultiplexing.parent, "flowcell_2"),
         )
     )
 
     # WHEN creating manifest files
     cli_runner.invoke(
         cli=create_manifest_files,
         args=["--source-directory", first_flowcell_directory.parent.as_posix()],
```

### Comparing `cg-60.4.1/tests/cli/downsample/test_cli_downsample.py` & `cg-60.4.2/tests/cli/downsample/test_cli_downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/generate/report/conftest.py` & `cg-60.4.2/tests/cli/generate/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/generate/report/test_cli_delivery_report.py` & `cg-60.4.2/tests/cli/generate/report/test_cli_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/generate/report/test_utils.py` & `cg-60.4.2/tests/cli/generate/report/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/generate/test_cli_base.py` & `cg-60.4.2/tests/cli/generate/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/get/test_cli_get.py` & `cg-60.4.2/tests/cli/get/test_cli_get.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/get/test_cli_get_analysis.py` & `cg-60.4.2/tests/cli/get/test_cli_get_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/get/test_cli_get_case.py` & `cg-60.4.2/tests/cli/get/test_cli_get_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/get/test_cli_get_flow_cell.py` & `cg-60.4.2/tests/cli/get/test_cli_get_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/get/test_cli_get_sample.py` & `cg-60.4.2/tests/cli/get/test_cli_get_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/set/conftest.py` & `cg-60.4.2/tests/cli/set/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/set/test_cli_set_case.py` & `cg-60.4.2/tests/cli/set/test_cli_set_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/set/test_cli_set_cases.py` & `cg-60.4.2/tests/cli/set/test_cli_set_cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/set/test_cli_set_flowcell.py` & `cg-60.4.2/tests/cli/set/test_cli_set_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/set/test_cli_set_list_keys.py` & `cg-60.4.2/tests/cli/set/test_cli_set_list_keys.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/set/test_cli_set_sample.py` & `cg-60.4.2/tests/cli/set/test_cli_set_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/set/test_cli_set_samples.py` & `cg-60.4.2/tests/cli/set/test_cli_set_samples.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/store/test_store.py` & `cg-60.4.2/tests/cli/store/test_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/test_base.py` & `cg-60.4.2/tests/cli/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/upload/conftest.py` & `cg-60.4.2/tests/cli/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/upload/test_cli_scout.py` & `cg-60.4.2/tests/cli/upload/test_cli_scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/upload/test_cli_upload.py` & `cg-60.4.2/tests/cli/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/upload/test_cli_upload_auto.py` & `cg-60.4.2/tests/cli/upload/test_cli_upload_auto.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/upload/test_cli_upload_delivery_report.py` & `cg-60.4.2/tests/cli/upload/test_cli_upload_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/upload/test_cli_upload_fastq.py` & `cg-60.4.2/tests/cli/upload/test_cli_upload_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/upload/test_cli_upload_genotype.py` & `cg-60.4.2/tests/cli/upload/test_cli_upload_genotype.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/upload/test_cli_upload_gens.py` & `cg-60.4.2/tests/cli/upload/test_cli_upload_gens.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/upload/test_cli_upload_nipt.py` & `cg-60.4.2/tests/cli/upload/test_cli_upload_nipt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/upload/test_cli_upload_nipt_ftp.py` & `cg-60.4.2/tests/cli/upload/test_cli_upload_nipt_ftp.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/upload/test_cli_upload_nipt_statina.py` & `cg-60.4.2/tests/cli/upload/test_cli_upload_nipt_statina.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/upload/test_cli_upload_observations.py` & `cg-60.4.2/tests/cli/upload/test_cli_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/balsamic/conftest.py` & `cg-60.4.2/tests/cli/workflow/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py` & `cg-60.4.2/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/balsamic/test_compound_commands.py` & `cg-60.4.2/tests/cli/workflow/balsamic/test_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/balsamic/test_link.py` & `cg-60.4.2/tests/cli/workflow/balsamic/test_link.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/balsamic/test_report_deliver.py` & `cg-60.4.2/tests/cli/workflow/balsamic/test_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/balsamic/test_run.py` & `cg-60.4.2/tests/cli/workflow/balsamic/test_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/balsamic/test_store_housekeeper.py` & `cg-60.4.2/tests/cli/workflow/balsamic/test_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/conftest.py` & `cg-60.4.2/tests/cli/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/fastq/test_fastq_base.py` & `cg-60.4.2/tests/cli/workflow/fastq/test_fastq_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/fluffy/conftest.py` & `cg-60.4.2/tests/cli/workflow/fluffy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py` & `cg-60.4.2/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/fluffy/test_cli_link.py` & `cg-60.4.2/tests/cli/workflow/fluffy/test_cli_link.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/fluffy/test_cli_run.py` & `cg-60.4.2/tests/cli/workflow/fluffy/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/fluffy/test_cli_start.py` & `cg-60.4.2/tests/cli/workflow/fluffy/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/fluffy/test_cli_store.py` & `cg-60.4.2/tests/cli/workflow/fluffy/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/microsalt/conftest.py` & `cg-60.4.2/tests/cli/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/microsalt/test_microsalt_case_config.py` & `cg-60.4.2/tests/cli/workflow/microsalt/test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/microsalt/test_microsalt_run.py` & `cg-60.4.2/tests/cli/workflow/microsalt/test_microsalt_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/mip/conftest.py` & `cg-60.4.2/tests/cli/workflow/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_base.py` & `cg-60.4.2/tests/cli/workflow/mip/test_cli_mip_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py` & `cg-60.4.2/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py` & `cg-60.4.2/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_dna_panel.py` & `cg-60.4.2/tests/cli/workflow/mip/test_cli_mip_dna_panel.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_dna_run.py` & `cg-60.4.2/tests/cli/workflow/mip/test_cli_mip_dna_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_dna_start.py` & `cg-60.4.2/tests/cli/workflow/mip/test_cli_mip_dna_start.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py` & `cg-60.4.2/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_rna_link.py` & `cg-60.4.2/tests/cli/workflow/mip/test_cli_mip_rna_link.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_rna_run.py` & `cg-60.4.2/tests/cli/workflow/mip/test_cli_mip_rna_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_store.py` & `cg-60.4.2/tests/cli/workflow/mip/test_cli_mip_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_config_case.py` & `cg-60.4.2/tests/cli/workflow/nf_analysis/test_cli_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py` & `cg-60.4.2/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py` & `cg-60.4.2/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_run.py` & `cg-60.4.2/tests/cli/workflow/nf_analysis/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_start.py` & `cg-60.4.2/tests/cli/workflow/nf_analysis/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_store.py` & `cg-60.4.2/tests/cli/workflow/nf_analysis/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py` & `cg-60.4.2/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py` & `cg-60.4.2/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py` & `cg-60.4.2/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/test_cli_workflow.py` & `cg-60.4.2/tests/cli/workflow/test_cli_workflow.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/cli/workflow/test_cli_workflow_clean.py` & `cg-60.4.2/tests/cli/workflow/test_cli_workflow_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/clients/arnold/conftest.py` & `cg-60.4.2/tests/clients/arnold/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/clients/arnold/test_arnold_api_client.py` & `cg-60.4.2/tests/clients/arnold/test_arnold_api_client.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/clients/janus/conftest.py` & `cg-60.4.2/tests/clients/janus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/clients/janus/test_janus_api_client.py` & `cg-60.4.2/tests/clients/janus/test_janus_api_client.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/conftest.py` & `cg-60.4.2/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -686,26 +686,14 @@
 @pytest.fixture(scope="session")
 def data_dir(fixtures_dir: Path) -> Path:
     """Return the path to the data dir."""
     return Path(fixtures_dir, "data")
 
 
 @pytest.fixture
-def fastq_dir(demultiplex_fixtures: Path) -> Path:
-    """Return the path to the fastq files dir."""
-    return Path(demultiplex_fixtures, "fastq")
-
-
-@pytest.fixture
-def spring_dir(demultiplex_fixtures: Path) -> Path:
-    """Return the path to the fastq files dir."""
-    return Path(demultiplex_fixtures, "spring")
-
-
-@pytest.fixture
 def project_dir(tmpdir_factory) -> Generator[Path, None, None]:
     """Path to a temporary directory where intermediate files can be stored."""
     yield Path(tmpdir_factory.mktemp("data"))
 
 
 @pytest.fixture
 def tmp_file(project_dir) -> Path:
@@ -860,44 +848,14 @@
 
 @pytest.fixture(name="vcf_file")
 def vcf_file(mip_dna_store_files: Path) -> Path:
     """Return the path to a VCF file."""
     return Path(mip_dna_store_files, "yellowhog_clinical_selected.vcf")
 
 
-@pytest.fixture(name="fastq_file")
-def fastq_file(fastq_dir: Path) -> Path:
-    """Return the path to a FASTQ file."""
-    return Path(fastq_dir, "dummy_run_R1_001.fastq.gz")
-
-
-@pytest.fixture(name="fastq_file_father")
-def fastq_file_father(fastq_dir: Path) -> Path:
-    """Return the path to a FASTQ file."""
-    return Path(fastq_dir, "fastq_run_R1_001.fastq.gz")
-
-
-@pytest.fixture(name="spring_file")
-def spring_file(spring_dir: Path) -> Path:
-    """Return the path to an existing spring file."""
-    return Path(spring_dir, "dummy_run_001.spring")
-
-
-@pytest.fixture(name="spring_meta_data_file")
-def spring_meta_data_file(spring_dir: Path) -> Path:
-    """Return the path to an existing spring file."""
-    return Path(spring_dir, "dummy_spring_meta_data.json")
-
-
-@pytest.fixture(name="spring_file_father")
-def spring_file_father(spring_dir: Path) -> Path:
-    """Return the path to a second existing spring file."""
-    return Path(spring_dir, "dummy_run_002.spring")
-
-
 @pytest.fixture(name="madeline_output")
 def madeline_output(apps_dir: Path) -> Path:
     """Return str of path for file with Madeline output."""
     return Path(apps_dir, "madeline", "madeline.xml")
 
 
 @pytest.fixture(name="file_does_not_exist")
@@ -1253,15 +1211,15 @@
     store: Store,
     helpers: StoreHelpers,
     selected_novaseq_6000_post_1_5_kits_sample_ids: list[str],
     selected_hiseq_x_dual_index_sample_ids: list[str],
     hiseq_x_dual_index_flow_cell_id: str,
     novaseq_6000_post_1_5_kits_flow_cell_id: str,
 ) -> Store:
-    """Return a store with samples that have been demultiplexed with BCL Convert and BCL2Fastq."""
+    """Return a store with samples that have been demultiplexed."""
     helpers.add_flow_cell(store, novaseq_6000_post_1_5_kits_flow_cell_id, sequencer_type="novaseq")
     helpers.add_flow_cell(store, hiseq_x_dual_index_flow_cell_id, sequencer_type="hiseqx")
     for i, sample_internal_id in enumerate(selected_novaseq_6000_post_1_5_kits_sample_ids):
         helpers.add_sample(store, internal_id=sample_internal_id, name=f"sample_bcl_convert_{i}")
         helpers.ensure_sample_lane_sequencing_metrics(
             store,
             sample_internal_id=sample_internal_id,
@@ -3762,32 +3720,26 @@
 
 @pytest.fixture(scope="session")
 def expected_total_reads() -> int:
     return 1_000_000
 
 
 @pytest.fixture
-def flow_cell_full_name(flow_cell_name: str) -> str:
-    """Return flow cell full name."""
-    return f"201203_D00483_0200_A{flow_cell_name}"
-
-
-@pytest.fixture(name="expected_average_q30_for_sample")
 def expected_average_q30_for_sample() -> float:
     """Return expected average Q30 for a sample."""
     return (85.5 + 80.5) / 2
 
 
-@pytest.fixture(name="expected_average_q30_for_flow_cell")
+@pytest.fixture
 def expected_average_q30_for_flow_cell() -> float:
     return (((85.5 + 80.5) / 2) + ((83.5 + 81.5) / 2)) / 2
 
 
-@pytest.fixture(name="expected_total_reads_flow_cell_bcl2fastq")
-def expected_total_reads_flow_cell_2() -> int:
+@pytest.fixture
+def expected_total_reads_hiseq_x_flow_cell() -> int:
     """Return an expected read count"""
     return 8_000_000
 
 
 @pytest.fixture
 def store_with_sequencing_metrics(
     store: Store,
@@ -3817,98 +3769,14 @@
     )
     helpers.add_multiple_sample_lane_sequencing_metrics_entries(
         metrics_data=sample_sequencing_metrics_details, store=store
     )
     return store
 
 
-@pytest.fixture(scope="function")
-def novaseqx_latest_analysis_version() -> str:
-    """Return the latest analysis version for NovaseqX analysis data directory."""
-    return "2"
-
-
-@pytest.fixture(scope="function")
-def novaseqx_flow_cell_directory(tmp_path: Path, novaseq_x_flow_cell_full_name: str) -> Path:
-    """Return the path to a NovaseqX flow cell directory."""
-    return Path(tmp_path, novaseq_x_flow_cell_full_name)
-
-
-@pytest.fixture(scope="function")
-def demultiplexed_runs_flow_cell_directory(tmp_path: Path) -> Path:
-    """Return the path to a demultiplexed flow cell run directory."""
-    demultiplexed_runs = Path(
-        tmp_path, DemultiplexingDirsAndFiles.DEMULTIPLEXED_RUNS_DIRECTORY_NAME
-    )
-    demultiplexed_runs.mkdir()
-    return demultiplexed_runs
-
-
-def add_novaseqx_analysis_data(novaseqx_flow_cell_directory: Path, analysis_version: str):
-    """Add NovaseqX analysis data to a flow cell directory."""
-    analysis_path: Path = Path(
-        novaseqx_flow_cell_directory, DemultiplexingDirsAndFiles.ANALYSIS, analysis_version
-    )
-    analysis_path.mkdir(parents=True)
-    analysis_path.joinpath(DemultiplexingDirsAndFiles.COPY_COMPLETE).touch()
-    data = analysis_path.joinpath(DemultiplexingDirsAndFiles.DATA)
-    data.mkdir()
-    data.joinpath(DemultiplexingDirsAndFiles.ANALYSIS_COMPLETED).touch()
-    return analysis_path
-
-
-@pytest.fixture(scope="function")
-def novaseqx_flow_cell_dir_with_analysis_data(
-    novaseqx_flow_cell_directory: Path, novaseqx_latest_analysis_version: str
-) -> Path:
-    """Return the path to a NovaseqX flow cell directory with multiple analysis data directories."""
-    add_novaseqx_analysis_data(novaseqx_flow_cell_directory, "0")
-    add_novaseqx_analysis_data(novaseqx_flow_cell_directory, "1")
-    add_novaseqx_analysis_data(novaseqx_flow_cell_directory, novaseqx_latest_analysis_version)
-    return novaseqx_flow_cell_directory
-
-
-@pytest.fixture(scope="function")
-def post_processed_novaseqx_flow_cell(novaseqx_flow_cell_dir_with_analysis_data: Path) -> Path:
-    """Return the path to a NovaseqX flow cell that is post processed."""
-    Path(
-        novaseqx_flow_cell_dir_with_analysis_data,
-        DemultiplexingDirsAndFiles.QUEUED_FOR_POST_PROCESSING,
-    ).touch()
-    return novaseqx_flow_cell_dir_with_analysis_data
-
-
-@pytest.fixture(scope="function")
-def novaseqx_flow_cell_analysis_incomplete(
-    novaseqx_flow_cell_directory: Path, novaseqx_latest_analysis_version: str
-) -> Path:
-    """
-    Return the path to a flow cell for which the analysis is not complete.
-    It misses the ANALYSIS_COMPLETED file.
-    """
-    Path(
-        novaseqx_flow_cell_directory,
-        DemultiplexingDirsAndFiles.ANALYSIS,
-        novaseqx_latest_analysis_version,
-    ).mkdir(parents=True)
-    Path(
-        novaseqx_flow_cell_directory,
-        DemultiplexingDirsAndFiles.ANALYSIS,
-        novaseqx_latest_analysis_version,
-        DemultiplexingDirsAndFiles.COPY_COMPLETE,
-    ).touch()
-    return novaseqx_flow_cell_directory
-
-
-@pytest.fixture(scope="function")
-def demultiplex_not_complete_novaseqx_flow_cell(tmp_file: Path) -> Path:
-    """Return the path to a NovaseqX flow cell for which demultiplexing is not complete."""
-    return tmp_file
-
-
 @pytest.fixture
 def flow_cell_encryption_api(
     cg_context: CGConfig, flow_cell_full_name: str
 ) -> FlowCellEncryptionAPI:
     flow_cell_encryption_api = FlowCellEncryptionAPI(
         binary_path=cg_context.encryption.binary_path,
         encryption_dir=Path(cg_context.backup.pdc_archiving_directory.current),
```

### Comparing `cg-60.4.1/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py` & `cg-60.4.2/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixture_plugins/delivery_fixtures/context_fixtures.py` & `cg-60.4.2/tests/fixture_plugins/delivery_fixtures/context_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixture_plugins/delivery_fixtures/path_fixtures.py` & `cg-60.4.2/tests/fixture_plugins/delivery_fixtures/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py` & `cg-60.4.2/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Fixtures for flow cell objects."""
+"""Fixtures for Illumina flow cell objects."""
 
 from pathlib import Path
 
 import pytest
 
 from cg.constants.demultiplexing import DemultiplexingDirsAndFiles
 from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
@@ -105,18 +105,18 @@
     sample_sheet_path = Path(flow_cell.path, DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME)
     flow_cell._sample_sheet_path_hk = sample_sheet_path
     return flow_cell
 
 
 @pytest.fixture
 def tmp_bcl_convert_flow_cell(
-    tmp_flow_cell_directory_bclconvert: Path,
+    tmp_flow_cell_directory_bcl_convert: Path,
 ) -> FlowCellDirectoryData:
     """Create a flow cell object with flow cell that is demultiplexed."""
-    return FlowCellDirectoryData(tmp_flow_cell_directory_bclconvert)
+    return FlowCellDirectoryData(tmp_flow_cell_directory_bcl_convert)
 
 
 @pytest.fixture
 def hiseq_x_single_index_demultiplexed_flow_cell_with_sample_sheet(
     illumina_demultiplexed_runs_directory: Path,
     hiseq_x_single_index_flow_cell_name: str,
     hiseq_x_single_index_sample_sheet_path: Path,
```

### Comparing `cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py` & `cg-60.4.2/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,45 @@
+"""Module for demultiplex fixtures returning strings."""
+
 import pytest
 
 
 @pytest.fixture
 def flow_cell_name() -> str:
     """Return flow cell name."""
     return "HVKJCDRXX"
 
 
-@pytest.fixture(scope="session")
-def bcl2fastq_flow_cell_full_name() -> str:
-    """Return full flow cell name."""
+@pytest.fixture
+def flow_cell_full_name(flow_cell_name: str) -> str:
+    """Return flow cell full name."""
     return "201203_D00483_0200_AHVKJCDRXX"
 
 
 @pytest.fixture(scope="session")
-def bcl_convert_flow_cell_full_name() -> str:
-    """Return the full name of a bcl_convert flow cell."""
-    return "211101_A00187_0615_AHLG5GDRZZ"
-
-
-@pytest.fixture(scope="session")
 def hiseq_x_single_index_flow_cell_id() -> str:
-    """Return the id of a HiSeqX single-index flow cell."""
+    """Return the id of a HiSeqX flow cell with only one index."""
     return "HJCFFALXX"
 
 
 @pytest.fixture(scope="session")
 def hiseq_x_single_index_flow_cell_name(hiseq_x_single_index_flow_cell_id) -> str:
     """Return the full name of a HiSeqX flow cell with only one index."""
     return f"170517_ST-E00266_0210_B{hiseq_x_single_index_flow_cell_id}"
 
 
 @pytest.fixture(scope="session")
 def hiseq_x_dual_index_flow_cell_id() -> str:
-    """Return the id of a HiSeqX flow cell with two indexes."""
+    """Return the id of a HiSeqX flow cell with double indexes."""
     return "HL32LCCXY"
 
 
 @pytest.fixture(scope="session")
 def hiseq_x_dual_index_flow_cell_name(hiseq_x_dual_index_flow_cell_id: str) -> str:
-    """Return the full name of a HiSeqX flow cell with two indexes."""
+    """Return the full name of a HiSeqX flow cell with double indexes."""
     return f"180508_ST-E00269_0269_A{hiseq_x_dual_index_flow_cell_id}"
 
 
 @pytest.fixture(scope="session")
 def hiseq_2500_dual_index_flow_cell_id() -> str:
     """Return the id of a HiSeq2500 flow cell with double indexes."""
     return "HM2LNBCX2"
@@ -53,49 +49,49 @@
 def hiseq_2500_dual_index_flow_cell_name(hiseq_2500_dual_index_flow_cell_id: str) -> str:
     """Return the full name of a HiSeq2500 flow cell with double indexes."""
     return f"181005_D00410_0735_B{hiseq_2500_dual_index_flow_cell_id}"
 
 
 @pytest.fixture(scope="session")
 def hiseq_2500_custom_index_flow_cell_id() -> str:
-    """Return the id of a HiSeq2500 flow cell with double indexes."""
+    """Return the id of a HiSeq2500 flow cell with custom indexes."""
     return "HGYFNBCX2"
 
 
 @pytest.fixture(scope="session")
 def hiseq_2500_custom_index_flow_cell_name(hiseq_2500_custom_index_flow_cell_id) -> str:
-    """Return the full name of a HiSeq2500 flow cell with double indexes."""
+    """Return the full name of a HiSeq2500 flow cell with custom indexes."""
     return f"180509_D00450_0598_B{hiseq_2500_custom_index_flow_cell_id}"
 
 
 @pytest.fixture(scope="session")
 def novaseq_6000_pre_1_5_kits_flow_cell_id() -> str:
-    """Return the id of a NovaSeqX flow cell."""
+    """Return the id of a pre-1.5 kits NovaSeq6000 flow cell."""
     return "HLYWYDSXX"
 
 
 @pytest.fixture(scope="session")
 def novaseq_6000_pre_1_5_kits_flow_cell_full_name(
     novaseq_6000_pre_1_5_kits_flow_cell_id: str,
 ) -> str:
-    """Return the full name of a NovaSeqX flow cell."""
+    """Return the full name of a pre-1.5 kits NovaSeq6000 flow cell."""
     return f"190927_A00689_0069_B{novaseq_6000_pre_1_5_kits_flow_cell_id}"
 
 
 @pytest.fixture(scope="session")
 def novaseq_6000_post_1_5_kits_flow_cell_id() -> str:
-    """Return the id of a NovaSeqX flow cell."""
+    """Return the id of a post-1.5 kits NovaSeq6000 flow cell."""
     return "HK33MDRX3"
 
 
 @pytest.fixture(scope="session")
 def novaseq_6000_post_1_5_kits_flow_cell_full_name(
     novaseq_6000_post_1_5_kits_flow_cell_id: str,
 ) -> str:
-    """Return the full name of a NovaSeqX flow cell."""
+    """Return the full name of a post-1.5 kits NovaSeq6000 flow cell."""
     return f"230912_A00187_1009_A{novaseq_6000_post_1_5_kits_flow_cell_id}"
 
 
 @pytest.fixture(scope="session")
 def novaseq_x_flow_cell_id() -> str:
     """Return the id of a NovaSeqX flow cell."""
     return "22F52TLT3"
```

### Comparing `cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py` & `cg-60.4.2/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,396 +1,383 @@
-"""Path fixtures for demultiplex tests."""
+"""Module for demultiplex fixtures returning Path objects."""
 
 import shutil
 from pathlib import Path
 
 import pytest
 
 from cg.constants.demultiplexing import DemultiplexingDirsAndFiles
 from cg.constants.nanopore_files import NanoporeDirsAndFiles
 
 CORRECT_SAMPLE_SHEET: str = "CorrectSampleSheet.csv"
 
 
-@pytest.fixture
-def tmp_illumina_flow_cells_directory(tmp_path: Path, illumina_flow_cells_directory: Path) -> Path:
-    """
-    Return the path to a temporary flow cells directory with flow cells ready for demultiplexing.
-    Generates a copy of the original flow cells directory
-    """
-    original_dir = illumina_flow_cells_directory
-    tmp_dir = Path(tmp_path, "flow_cells")
-
-    return Path(shutil.copytree(original_dir, tmp_dir))
+# Directory fixtures
 
 
-@pytest.fixture
-def tmp_broken_flow_cells_directory(tmp_path: Path, broken_flow_cells_dir: Path) -> Path:
-    """
-    Return the path to a temporary flow cells directory with incomplete or broken flow cells.
-    Generates a copy of the original flow cells directory
-    """
-    original_dir = broken_flow_cells_dir
-    tmp_dir = Path(tmp_path, "broken_flow_cells")
+@pytest.fixture(scope="session")
+def demultiplex_fixtures(apps_dir: Path) -> Path:
+    """Return the path to the demultiplex fixture directory."""
+    return Path(apps_dir, "demultiplexing")
 
-    return Path(shutil.copytree(original_dir, tmp_dir))
 
+@pytest.fixture(scope="session")
+def illumina_flow_cells_directory(demultiplex_fixtures: Path) -> Path:
+    """Return the path to the sequenced flow cells fixture directory."""
+    return Path(demultiplex_fixtures, DemultiplexingDirsAndFiles.FLOW_CELLS_DIRECTORY_NAME)
 
-@pytest.fixture
-def tmp_illumina_flow_cells_demux_all_directory(
-    tmp_path: Path, illumina_demux_all_directory: Path
-) -> Path:
-    """
-    Return the path to a temporary flow cells directory with flow cells ready for demultiplexing.
-    Generates a copy of the original flow cells directory.
-    This fixture is used for testing of the cg demutliplex all cmd.
-    """
-    original_dir = illumina_demux_all_directory
-    tmp_dir = Path(tmp_path, "flow_cells_demux_all")
 
-    return Path(shutil.copytree(original_dir, tmp_dir))
+@pytest.fixture(scope="session")
+def illumina_demultiplexed_runs_directory(demultiplex_fixtures: Path) -> Path:
+    """Return the path to the demultiplexed flow cells fixture directory."""
+    return Path(demultiplex_fixtures, "demultiplexed-runs")
 
 
-@pytest.fixture
-def tmp_illumina_flow_cells_demux_results_not_finished_directory(
-    tmp_path: Path, illumina_demux_results_not_finished_dir: Path
-) -> Path:
-    """Return the path to a temporary flow cells directory with unfinished demultiplexing results."""
-    original_dir = illumina_demux_results_not_finished_dir
-    tmp_dir = Path(tmp_path, "demultiplexed-runs-unfinished")
+@pytest.fixture(scope="session")
+def illumina_demux_all_directory(demultiplex_fixtures: Path) -> Path:
+    """Return the path to the sequenced flow cells fixture directory."""
+    return Path(demultiplex_fixtures, "flow_cells_demux_all")
 
-    return Path(shutil.copytree(original_dir, tmp_dir))
 
+@pytest.fixture(scope="session")
+def nanopore_flow_cells_dir(demultiplex_fixtures: Path) -> Path:
+    """Return the path to the sequenced flow cells fixture directory."""
+    return Path(demultiplex_fixtures, NanoporeDirsAndFiles.DATA_DIRECTORY)
 
-@pytest.fixture(name="tmp_flow_cell_directory_bcl2fastq")
-def flow_cell_working_directory_bcl2fastq(
-    bcl2fastq_flow_cell_dir: Path, tmp_illumina_flow_cells_directory
-) -> Path:
-    """Return the path to a working directory that will be deleted after test is run.
 
-    This is a path to a flow cell directory with the run parameters present.
-    """
-    return Path(tmp_illumina_flow_cells_directory, bcl2fastq_flow_cell_dir.name)
+@pytest.fixture(scope="session")
+def run_parameters_dir(demultiplex_fixtures: Path) -> Path:
+    """Return the path to the run parameters fixture directory."""
+    return Path(demultiplex_fixtures, "run_parameters")
 
 
-@pytest.fixture(name="tmp_flow_cell_directory_bclconvert")
-def flow_cell_working_directory_bclconvert(
-    bcl_convert_flow_cell_dir: Path, tmp_illumina_flow_cells_directory
-) -> Path:
-    """Return the path to a working directory that will be deleted after test is run.
-    This is a path to a flow cell directory with the run parameters present.
-    """
-    return Path(tmp_illumina_flow_cells_directory, bcl_convert_flow_cell_dir.name)
+@pytest.fixture(scope="session")
+def sample_sheet_dir(demultiplex_fixtures: Path) -> Path:
+    """Return the path to the sample sheet fixture directory."""
+    return Path(demultiplex_fixtures, "sample_sheets")
 
 
 @pytest.fixture
-def tmp_flow_cell_with_bcl2fastq_sample_sheet(
-    tmp_broken_flow_cells_directory: Path, hiseq_x_single_index_flow_cell_name: str
-) -> Path:
-    """This is a path to a flow cell directory with a bcl2fastq sample sheet."""
-    return Path(tmp_broken_flow_cells_directory, hiseq_x_single_index_flow_cell_name)
+def fastq_dir(demultiplex_fixtures: Path) -> Path:
+    """Return the path to the fastq files dir."""
+    return Path(demultiplex_fixtures, "fastq")
 
 
 @pytest.fixture
-def tmp_flow_cell_without_run_parameters_path(
-    tmp_broken_flow_cells_directory: Path, hiseq_2500_custom_index_flow_cell_name: str
-) -> Path:
-    """This is a path to a flow cell directory with the run parameters missing."""
-    return Path(tmp_broken_flow_cells_directory, hiseq_2500_custom_index_flow_cell_name)
+def spring_dir(demultiplex_fixtures: Path) -> Path:
+    """Return the path to the fastq files dir."""
+    return Path(demultiplex_fixtures, "spring")
 
 
-@pytest.fixture
-def tmp_novaseq_6000_pre_1_5_kits_flow_cell_without_sample_sheet_path(
-    tmp_broken_flow_cells_directory: Path,
-) -> Path:
-    """This is a path to a flow cell directory with the sample sheet missing."""
-    return Path(tmp_broken_flow_cells_directory, "190927_A00689_0069_BHLYWYDSXX")
+@pytest.fixture(scope="session")
+def broken_flow_cells_dir(demultiplex_fixtures: Path) -> Path:
+    """Return the path to the broken or incomplete flow cells fixture directory."""
+    return Path(demultiplex_fixtures, "flow_cells_broken")
 
 
-@pytest.fixture
-def tmp_novaseq_6000_post_1_5_kits_flow_cell_without_sample_sheet_path(
-    tmp_broken_flow_cells_directory: Path,
-) -> Path:
-    """This is a path to a flow cell directory with the sample sheet missing."""
-    return Path(tmp_broken_flow_cells_directory, "230912_A00187_1009_AHK33MDRX3")
+@pytest.fixture(scope="session")
+def illumina_demux_results_not_finished_dir(demultiplex_fixtures: Path) -> Path:
+    """Return the path to a dir with demultiplexing results where nothing has been cleaned."""
+    return Path(demultiplex_fixtures, "demultiplexed-runs-unfinished")
+
+
+# Temporary directory fixtures
 
 
 @pytest.fixture
-def tmp_novaseq_x_without_sample_sheet_flow_cell_path(
-    tmp_broken_flow_cells_directory: Path,
-) -> Path:
-    """This is a path to a flow cell directory with the sample sheet missing."""
-    return Path(tmp_broken_flow_cells_directory, "20231108_LH00188_0028_B22F52TLT3")
+def tmp_illumina_flow_cells_directory(tmp_path: Path, illumina_flow_cells_directory: Path) -> Path:
+    """
+    Return the path to a temporary flow cells directory with flow cells ready for demultiplexing.
+    Generates a copy of the original flow cells directory
+    """
+    original_dir = illumina_flow_cells_directory
+    tmp_dir = Path(tmp_path, "flow_cells")
+
+    return Path(shutil.copytree(original_dir, tmp_dir))
 
 
 @pytest.fixture
-def tmp_flow_cells_directory_ready_for_demultiplexing_bcl_convert(
-    bcl_convert_flow_cell_full_name: str, tmp_illumina_flow_cells_directory
-) -> Path:
-    """This is a path to a flow cell directory with the run parameters missing."""
-    return Path(tmp_illumina_flow_cells_directory, bcl_convert_flow_cell_full_name)
+def tmp_demultiplexed_runs_flow_cell_directory(tmp_path: Path) -> Path:
+    """Return the path to a demultiplexed flow cell run directory."""
+    demultiplexed_runs = Path(tmp_path, "demultiplexed-runs")
+    demultiplexed_runs.mkdir()
+    return demultiplexed_runs
 
 
-# Temporary demultiplexed runs fixtures
 @pytest.fixture
 def tmp_illumina_demultiplexed_flow_cells_directory(
     tmp_path: Path, illumina_demultiplexed_runs_directory
 ) -> Path:
     """Return the path to a temporary demultiplex-runs directory.
     Generates a copy of the original demultiplexed-runs
     """
     original_dir = illumina_demultiplexed_runs_directory
     tmp_dir = Path(tmp_path, "demultiplexed-runs")
     return Path(shutil.copytree(original_dir, tmp_dir))
 
 
 @pytest.fixture
-def tmp_demultiplexed_runs_bcl2fastq_directory(
-    tmp_illumina_demultiplexed_flow_cells_directory, bcl2fastq_flow_cell_dir: Path
-) -> Path:
-    """Return the path to a temporary demultiplex-runs bcl2fastq flow cell directory."""
-    return Path(tmp_illumina_demultiplexed_flow_cells_directory, bcl2fastq_flow_cell_dir.name)
-
-
-@pytest.fixture
-def tmp_demultiplexed_runs_not_finished_flow_cells_directory(
-    tmp_path: Path, illumina_novaseq_demux_results_not_finished_dir
+def tmp_illumina_flow_cells_demux_all_directory(
+    tmp_path: Path, illumina_demux_all_directory: Path
 ) -> Path:
     """
-    Return a temporary demultiplex-runs-unfinished path with an unfinished flow cell directory.
-    Generates a copy of the original demultiplexed-runs-unfinished directory.
+    Return the path to a temporary flow cells directory with flow cells ready for demultiplexing.
+    Generates a copy of the original flow cells directory.
+    This fixture is used for testing of the cg demutliplex all cmd.
     """
-    original_dir = illumina_novaseq_demux_results_not_finished_dir
-    tmp_dir = Path(tmp_path, "demultiplexed-runs-unfinished")
-    return Path(shutil.copytree(original_dir, tmp_dir))
-
+    original_dir = illumina_demux_all_directory
+    tmp_dir = Path(tmp_path, "flow_cells_demux_all")
 
-@pytest.fixture
-def tmp_demultiplexed_flow_cell_no_fastq_files(
-    tmp_illumina_flow_cells_demux_results_not_finished_directory: Path,
-    novaseq_6000_post_1_5_kits_flow_cell_full_name: str,
-) -> Path:
-    """Return the path to a demultiplexed flow cell directory without fastq files."""
-    return Path(
-        tmp_illumina_flow_cells_demux_results_not_finished_directory,
-        novaseq_6000_post_1_5_kits_flow_cell_full_name,
-    )
+    return Path(shutil.copytree(original_dir, tmp_dir))
 
 
 @pytest.fixture
-def demultiplexed_runs_unfinished_bcl2fastq_flow_cell_directory(
-    tmp_demultiplexed_runs_not_finished_directory: Path,
-    bcl2fastq_flow_cell_full_name: str,
-) -> Path:
-    """Copy the content of a demultiplexed but not finished directory to a temporary location."""
-    return Path(tmp_demultiplexed_runs_not_finished_directory, bcl2fastq_flow_cell_full_name)
-
-
-# Directory fixtures
-
-
-@pytest.fixture(scope="session")
-def demultiplex_fixtures(apps_dir: Path) -> Path:
-    """Return the path to the demultiplex fixture directory."""
-    return Path(apps_dir, "demultiplexing")
-
-
-@pytest.fixture(scope="session")
-def raw_lims_sample_dir(demultiplex_fixtures: Path) -> Path:
-    """Return the path to the raw samples fixture directory."""
-    return Path(demultiplex_fixtures, "raw_lims_samples")
-
-
-@pytest.fixture(scope="session")
-def run_parameters_dir(demultiplex_fixtures: Path) -> Path:
-    """Return the path to the run parameters fixture directory."""
-    return Path(demultiplex_fixtures, "run_parameters")
-
-
-@pytest.fixture(scope="session")
-def sample_sheet_dir(demultiplex_fixtures: Path) -> Path:
-    """Return the path to the sample sheet fixture directory."""
-    return Path(demultiplex_fixtures, "sample_sheets")
-
+def tmp_broken_flow_cells_directory(tmp_path: Path, broken_flow_cells_dir: Path) -> Path:
+    """
+    Return the path to a temporary flow cells directory with incomplete or broken flow cells.
+    Generates a copy of the original flow cells directory
+    """
+    original_dir = broken_flow_cells_dir
+    tmp_dir = Path(tmp_path, "broken_flow_cells")
 
-@pytest.fixture(scope="session")
-def illumina_demultiplexed_runs_directory(demultiplex_fixtures: Path) -> Path:
-    """Return the path to the demultiplexed flow cells fixture directory."""
-    return Path(demultiplex_fixtures, "demultiplexed-runs")
+    return Path(shutil.copytree(original_dir, tmp_dir))
 
 
-@pytest.fixture(scope="session")
-def illumina_flow_cells_directory(demultiplex_fixtures: Path) -> Path:
-    """Return the path to the sequenced flow cells fixture directory."""
-    return Path(demultiplex_fixtures, DemultiplexingDirsAndFiles.FLOW_CELLS_DIRECTORY_NAME)
+# Canonical flow cell paths
 
 
 @pytest.fixture(scope="session")
-def broken_flow_cells_dir(demultiplex_fixtures: Path) -> Path:
-    """Return the path to the broken or incomplete flow cells fixture directory."""
-    return Path(demultiplex_fixtures, "flow_cells_broken")
+def hiseq_x_single_index_flow_cell_dir(
+    illumina_flow_cells_directory, hiseq_x_single_index_flow_cell_name: str
+) -> Path:
+    """Return the path to a HiSeqX flow cell."""
+    return Path(illumina_flow_cells_directory, hiseq_x_single_index_flow_cell_name)
 
 
 @pytest.fixture(scope="session")
-def nanopore_flow_cells_dir(demultiplex_fixtures: Path) -> Path:
-    """Return the path to the sequenced flow cells fixture directory."""
-    return Path(demultiplex_fixtures, NanoporeDirsAndFiles.DATA_DIRECTORY)
+def hiseq_x_dual_index_flow_cell_dir(
+    illumina_flow_cells_directory, hiseq_x_dual_index_flow_cell_name: str
+) -> Path:
+    """Return the path to a dual-index HiSeqX flow cell."""
+    return Path(illumina_flow_cells_directory, hiseq_x_dual_index_flow_cell_name)
 
 
 @pytest.fixture(scope="session")
-def illumina_demux_all_directory(demultiplex_fixtures: Path) -> Path:
-    """Return the path to the sequenced flow cells fixture directory."""
-    return Path(demultiplex_fixtures, "flow_cells_demux_all")
+def hiseq_2500_dual_index_flow_cell_dir(
+    illumina_flow_cells_directory, hiseq_2500_dual_index_flow_cell_name: str
+) -> Path:
+    """Return the path to a HiSeq2500 flow cell."""
+    return Path(illumina_flow_cells_directory, hiseq_2500_dual_index_flow_cell_name)
 
 
 @pytest.fixture(scope="session")
-def illumina_demux_results_not_finished_dir(demultiplex_fixtures: Path) -> Path:
-    """Return the path to a dir with demultiplexing results where nothing has been cleaned."""
-    return Path(demultiplex_fixtures, "demultiplexed-runs-unfinished")
+def hiseq_2500_custom_index_flow_cell_dir(
+    illumina_flow_cells_directory, hiseq_2500_custom_index_flow_cell_name: str
+) -> Path:
+    """Return the path to a HiSeq2500 flow cell."""
+    return Path(illumina_flow_cells_directory, hiseq_2500_custom_index_flow_cell_name)
 
 
-###
+@pytest.fixture
+def novaseq_6000_pre_1_5_kits_flow_cell_path(
+    tmp_illumina_flow_cells_directory: Path, novaseq_6000_pre_1_5_kits_flow_cell_full_name: str
+) -> Path:
+    return Path(tmp_illumina_flow_cells_directory, novaseq_6000_pre_1_5_kits_flow_cell_full_name)
 
 
 @pytest.fixture
 def novaseq_6000_post_1_5_kits_flow_cell_path(
     tmp_illumina_flow_cells_directory: Path, novaseq_6000_post_1_5_kits_flow_cell_full_name: str
 ) -> Path:
     return Path(tmp_illumina_flow_cells_directory, novaseq_6000_post_1_5_kits_flow_cell_full_name)
 
 
 @pytest.fixture
-def novaseq_6000_post_1_5_kits_correct_sample_sheet_path(
-    novaseq_6000_post_1_5_kits_flow_cell_path: Path,
+def novaseq_x_flow_cell_dir(
+    illumina_flow_cells_directory: Path, novaseq_x_flow_cell_full_name: str
 ) -> Path:
-    return Path(novaseq_6000_post_1_5_kits_flow_cell_path, CORRECT_SAMPLE_SHEET)
+    """Return the path to a NovaSeqX flow cell."""
+    return Path(illumina_flow_cells_directory, novaseq_x_flow_cell_full_name)
 
 
-@pytest.fixture
-def novaseq_6000_pre_1_5_kits_flow_cell_path(tmp_illumina_flow_cells_directory: Path) -> Path:
-    return Path(tmp_illumina_flow_cells_directory, "190927_A00689_0069_BHLYWYDSXX")
+# Tmp flow cell paths
 
 
 @pytest.fixture
-def novaseq_6000_pre_1_5_kits_correct_sample_sheet_path(
-    novaseq_6000_pre_1_5_kits_flow_cell_path: Path,
+def tmp_novaseq_6000_pre_1_5_kits_flow_cell_path(
+    tmp_illumina_flow_cells_directory: Path, novaseq_6000_pre_1_5_kits_flow_cell_full_name: str
 ) -> Path:
-    return Path(novaseq_6000_pre_1_5_kits_flow_cell_path, CORRECT_SAMPLE_SHEET)
+    return Path(tmp_illumina_flow_cells_directory, novaseq_6000_pre_1_5_kits_flow_cell_full_name)
 
 
 @pytest.fixture
-def novaseq_x_flow_cell_directory(tmp_illumina_flow_cells_directory) -> Path:
-    return Path(tmp_illumina_flow_cells_directory, "20231108_LH00188_0028_B22F52TLT3")
-
+def tmp_illumina_flow_cells_demux_results_not_finished_directory(
+    tmp_path: Path, illumina_demux_results_not_finished_dir: Path
+) -> Path:
+    """Return the path to a temporary flow cells directory with unfinished demultiplexing results."""
+    original_dir: Path = illumina_demux_results_not_finished_dir
+    tmp_dir = Path(tmp_path, "demultiplexed-runs-unfinished")
 
-@pytest.fixture
-def novaseq_x_correct_sample_sheet(novaseq_x_flow_cell_directory: Path) -> Path:
-    return Path(novaseq_x_flow_cell_directory, CORRECT_SAMPLE_SHEET)
+    return Path(shutil.copytree(original_dir, tmp_dir))
 
 
 @pytest.fixture
-def novaseq_x_manifest_file(novaseq_x_flow_cell_dir: Path) -> Path:
-    """Return the path to a NovaSeqX manifest file."""
-    return Path(novaseq_x_flow_cell_dir, "Manifest.tsv")
+def tmp_flow_cell_directory_bcl_convert(tmp_illumina_flow_cells_directory: Path) -> Path:
+    """Return a path to a flow cell directory with the run parameters present."""
+    return Path(tmp_illumina_flow_cells_directory, "211101_A00187_0615_AHLG5GDRZZ")
 
 
-@pytest.fixture(scope="session")
-def hiseq_x_single_index_flow_cell_dir(
-    illumina_flow_cells_directory, hiseq_x_single_index_flow_cell_name: str
+@pytest.fixture
+def tmp_flow_cell_with_bcl2fastq_sample_sheet(
+    tmp_broken_flow_cells_directory: Path, hiseq_x_single_index_flow_cell_name: str
 ) -> Path:
-    """Return the path to a HiSeqX flow cell."""
-    return Path(illumina_flow_cells_directory, hiseq_x_single_index_flow_cell_name)
+    """Return a path to a flow cell directory with a BCL2FASTQ sample sheet for translation."""
+    return Path(tmp_broken_flow_cells_directory, hiseq_x_single_index_flow_cell_name)
 
 
 @pytest.fixture
-def hiseq_x_single_index_sample_sheet_path(hiseq_x_single_index_flow_cell_dir: Path) -> Path:
-    """Return the path to a single-index HiSeqX sample sheet."""
-    return Path(
-        hiseq_x_single_index_flow_cell_dir, DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME
-    )
+def tmp_flow_cell_without_run_parameters_path(
+    tmp_broken_flow_cells_directory: Path, hiseq_2500_custom_index_flow_cell_name: str
+) -> Path:
+    """Return a path to a flow cell directory with the run parameters missing."""
+    return Path(tmp_broken_flow_cells_directory, hiseq_2500_custom_index_flow_cell_name)
 
 
-@pytest.fixture(scope="session")
-def hiseq_x_dual_index_flow_cell_dir(
-    illumina_flow_cells_directory, hiseq_x_dual_index_flow_cell_name: str
+@pytest.fixture
+def tmp_novaseq_6000_pre_1_5_kits_flow_cell_without_sample_sheet_path(
+    tmp_broken_flow_cells_directory: Path,
+    novaseq_6000_pre_1_5_kits_flow_cell_full_name: str,
 ) -> Path:
-    """Return the path to a dual-index HiSeqX flow cell."""
-    return Path(illumina_flow_cells_directory, hiseq_x_dual_index_flow_cell_name)
+    """Return a path to a flow cell directory with the sample sheet missing."""
+    return Path(tmp_broken_flow_cells_directory, novaseq_6000_pre_1_5_kits_flow_cell_full_name)
 
 
 @pytest.fixture
-def hiseq_x_dual_index_sample_sheet_path(hiseq_x_dual_index_flow_cell_dir: Path) -> Path:
-    """Return the path to a dual-index HiSeqX sample sheet."""
-    return Path(hiseq_x_dual_index_flow_cell_dir, DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME)
+def tmp_novaseq_6000_post_1_5_kits_flow_cell_without_sample_sheet_path(
+    tmp_broken_flow_cells_directory: Path,
+    novaseq_6000_post_1_5_kits_flow_cell_full_name: str,
+) -> Path:
+    """Return a path to a flow cell directory with the sample sheet missing."""
+    return Path(tmp_broken_flow_cells_directory, novaseq_6000_post_1_5_kits_flow_cell_full_name)
 
 
-@pytest.fixture(scope="session")
-def hiseq_2500_dual_index_flow_cell_dir(
-    illumina_flow_cells_directory, hiseq_2500_dual_index_flow_cell_name: str
+@pytest.fixture
+def tmp_novaseq_x_without_sample_sheet_flow_cell_path(
+    tmp_broken_flow_cells_directory: Path,
+    novaseq_x_flow_cell_full_name: str,
 ) -> Path:
-    """Return the path to a HiSeq2500 flow cell."""
-    return Path(illumina_flow_cells_directory, hiseq_2500_dual_index_flow_cell_name)
+    """Return a path to a flow cell directory with the sample sheet missing."""
+    return Path(tmp_broken_flow_cells_directory, novaseq_x_flow_cell_full_name)
 
 
 @pytest.fixture
-def hiseq_2500_dual_index_sample_sheet_path(hiseq_2500_dual_index_flow_cell_dir: Path) -> Path:
-    """Return the path to a dual-index HiSeq2500 sample sheet."""
-    return Path(
-        hiseq_2500_dual_index_flow_cell_dir, DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME
-    )
+def tmp_novaseqx_flow_cell_directory(tmp_path: Path, novaseq_x_flow_cell_full_name: str) -> Path:
+    """Return the path to a NovaseqX flow cell directory."""
+    return Path(tmp_path, novaseq_x_flow_cell_full_name)
 
 
-@pytest.fixture(scope="session")
-def hiseq_2500_custom_index_flow_cell_dir(
-    illumina_flow_cells_directory, hiseq_2500_custom_index_flow_cell_name: str
+@pytest.fixture
+def tmp_flow_cells_directory_ready_for_demultiplexing(
+    hiseq_2500_dual_index_flow_cell_name: str, tmp_illumina_flow_cells_directory
 ) -> Path:
-    """Return the path to a HiSeq2500 flow cell."""
-    return Path(illumina_flow_cells_directory, hiseq_2500_custom_index_flow_cell_name)
+    """Return a path to a flow cell directory with the run parameters missing."""
+    return Path(tmp_illumina_flow_cells_directory, hiseq_2500_dual_index_flow_cell_name)
+
+
+# Temporary demultiplexed runs fixtures
 
 
 @pytest.fixture
-def hiseq_2500_custom_index_sample_sheet_path(hiseq_2500_custom_index_flow_cell_dir: Path) -> Path:
-    """Return the path to a custom-index HiSeq2500 sample sheet."""
+def tmp_demultiplexed_flow_cell_no_fastq_files(
+    tmp_illumina_flow_cells_demux_results_not_finished_directory: Path,
+    novaseq_6000_post_1_5_kits_flow_cell_full_name: str,
+) -> Path:
+    """Return the path to a demultiplexed flow cell directory without fastq files."""
     return Path(
-        hiseq_2500_custom_index_flow_cell_dir, DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME
+        tmp_illumina_flow_cells_demux_results_not_finished_directory,
+        novaseq_6000_post_1_5_kits_flow_cell_full_name,
     )
 
 
+# Fixtures for test demultiplex flow cell
 @pytest.fixture
-def novaseq_x_flow_cell_dir(illumina_flow_cells_directory: Path) -> Path:
-    """Return the path to a NovaSeqX flow cell."""
-    return Path(illumina_flow_cells_directory, "20231108_LH00188_0028_B22F52TLT3")
-
-
-@pytest.fixture(scope="session")
-def bcl2fastq_flow_cell_dir(
-    illumina_flow_cells_directory, bcl2fastq_flow_cell_full_name: str
+def tmp_empty_demultiplexed_runs_directory(
+    tmp_illumina_demultiplexed_flow_cells_directory,
 ) -> Path:
-    """Return the path to the bcl2fastq flow cell demultiplex fixture directory."""
-    return Path(illumina_flow_cells_directory, bcl2fastq_flow_cell_full_name)
+    return Path(tmp_illumina_demultiplexed_flow_cells_directory, "empty")
 
 
-@pytest.fixture(scope="session")
-def bcl_convert_flow_cell_dir(
-    illumina_flow_cells_directory, bcl_convert_flow_cell_full_name: str
-) -> Path:
-    """Return the path to the bcl_convert flow cell demultiplex fixture directory."""
-    return Path(illumina_flow_cells_directory, bcl_convert_flow_cell_full_name)
+@pytest.fixture(scope="function")
+def novaseqx_latest_analysis_version() -> str:
+    """Return the latest analysis version for NovaseqX analysis data directory."""
+    return "2"
 
 
-@pytest.fixture
-def novaseq_6000_sample_sheet_with_reversed_cycles(sample_sheet_dir: Path) -> Path:
-    """Return the path to a NovaSeq6000 sample sheet with reversed index2 cycles."""
-    return Path(sample_sheet_dir, "novaseq_6000_sample_sheet_with_reversed_cycles.csv")
+def add_novaseqx_analysis_data(novaseqx_flow_cell_directory: Path, analysis_version: str):
+    """Add NovaSeqX analysis data to a flow cell directory."""
+    analysis_path: Path = Path(
+        novaseqx_flow_cell_directory, DemultiplexingDirsAndFiles.ANALYSIS, analysis_version
+    )
+    analysis_path.mkdir(parents=True)
+    analysis_path.joinpath(DemultiplexingDirsAndFiles.COPY_COMPLETE).touch()
+    data = analysis_path.joinpath(DemultiplexingDirsAndFiles.DATA)
+    data.mkdir()
+    data.joinpath(DemultiplexingDirsAndFiles.ANALYSIS_COMPLETED).touch()
+
+
+@pytest.fixture(scope="function")
+def novaseqx_flow_cell_dir_with_analysis_data(
+    tmp_novaseqx_flow_cell_directory: Path, novaseqx_latest_analysis_version: str
+) -> Path:
+    """Return the path to a NovaseqX flow cell directory with multiple analysis data directories."""
+    add_novaseqx_analysis_data(tmp_novaseqx_flow_cell_directory, "0")
+    add_novaseqx_analysis_data(tmp_novaseqx_flow_cell_directory, "1")
+    add_novaseqx_analysis_data(tmp_novaseqx_flow_cell_directory, novaseqx_latest_analysis_version)
+    return tmp_novaseqx_flow_cell_directory
+
+
+@pytest.fixture(scope="function")
+def post_processed_novaseqx_flow_cell(novaseqx_flow_cell_dir_with_analysis_data: Path) -> Path:
+    """Return the path to a NovaseqX flow cell that is post processed."""
+    Path(
+        novaseqx_flow_cell_dir_with_analysis_data,
+        DemultiplexingDirsAndFiles.QUEUED_FOR_POST_PROCESSING,
+    ).touch()
+    return novaseqx_flow_cell_dir_with_analysis_data
+
+
+@pytest.fixture(scope="function")
+def novaseqx_flow_cell_analysis_incomplete(
+    tmp_novaseqx_flow_cell_directory: Path, novaseqx_latest_analysis_version: str
+) -> Path:
+    """
+    Return the path to a flow cell for which the analysis is not complete.
+    It misses the ANALYSIS_COMPLETED file.
+    """
+    Path(
+        tmp_novaseqx_flow_cell_directory,
+        DemultiplexingDirsAndFiles.ANALYSIS,
+        novaseqx_latest_analysis_version,
+    ).mkdir(parents=True)
+    Path(
+        tmp_novaseqx_flow_cell_directory,
+        DemultiplexingDirsAndFiles.ANALYSIS,
+        novaseqx_latest_analysis_version,
+        DemultiplexingDirsAndFiles.COPY_COMPLETE,
+    ).touch()
+    return tmp_novaseqx_flow_cell_directory
+
+
+@pytest.fixture(scope="function")
+def demultiplex_not_complete_novaseqx_flow_cell(tmp_file: Path) -> Path:
+    """Return the path to a NovaseqX flow cell for which demultiplexing is not complete."""
+    return tmp_file
 
 
-@pytest.fixture
-def novaseq_x_sample_sheet_with_forward_cycles(sample_sheet_dir: Path) -> Path:
-    """Return the path to a NovaSeqX sample sheet with forward index2 cycles."""
-    return Path(sample_sheet_dir, "novaseq_x_sample_sheet_with_forward_cycles.csv")
+# Path to run parameter files
 
 
 @pytest.fixture(scope="session")
 def run_parameters_wrong_instrument(run_parameters_dir: Path) -> Path:
     """Return a NovaSeqX run parameters file path with a wrong instrument value."""
     return Path(run_parameters_dir, "RunParameters_novaseq_X_wrong_instrument.xml")
 
@@ -431,18 +418,21 @@
 ) -> Path:
     """Return the path to a HiSeq2500 run parameters file with custom index."""
     return Path(
         hiseq_2500_custom_index_flow_cell_dir, DemultiplexingDirsAndFiles.RUN_PARAMETERS_CAMEL_CASE
     )
 
 
-@pytest.fixture(scope="session")
-def novaseq_6000_run_parameters_path(bcl2fastq_flow_cell_dir: Path) -> Path:
+@pytest.fixture
+def novaseq_6000_run_parameters_path(novaseq_6000_pre_1_5_kits_flow_cell_path: Path) -> Path:
     """Return the path to a NovaSeq6000 run parameters file."""
-    return Path(bcl2fastq_flow_cell_dir, DemultiplexingDirsAndFiles.RUN_PARAMETERS_PASCAL_CASE)
+    return Path(
+        novaseq_6000_pre_1_5_kits_flow_cell_path,
+        DemultiplexingDirsAndFiles.RUN_PARAMETERS_PASCAL_CASE,
+    )
 
 
 @pytest.fixture
 def novaseq_6000_run_parameters_pre_1_5_kits_path(
     novaseq_6000_pre_1_5_kits_flow_cell_path: Path,
 ) -> Path:
     """Return the path to a NovaSeq6000 pre 1.5 kit run parameters file."""
@@ -473,41 +463,108 @@
 def run_parameters_missing_versions_path(
     run_parameters_dir: Path,
 ) -> Path:
     """Return a NovaSeq6000 run parameters path without software and reagent kit versions."""
     return Path(run_parameters_dir, "RunParameters_novaseq_no_software_nor_reagent_version.xml")
 
 
-@pytest.fixture(name="lims_novaseq_samples_file")
-def lims_novaseq_samples_file(raw_lims_sample_dir: Path) -> Path:
-    """Return the path to a file with sample info in lims format."""
-    return Path(raw_lims_sample_dir, "raw_samplesheet_novaseq.json")
+# Path to sample sheets
+
+
+@pytest.fixture
+def hiseq_x_single_index_sample_sheet_path(hiseq_x_single_index_flow_cell_dir: Path) -> Path:
+    """Return the path to a single-index HiSeqX sample sheet."""
+    return Path(
+        hiseq_x_single_index_flow_cell_dir, DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME
+    )
+
+
+@pytest.fixture
+def hiseq_x_dual_index_sample_sheet_path(hiseq_x_dual_index_flow_cell_dir: Path) -> Path:
+    """Return the path to a dual-index HiSeqX sample sheet."""
+    return Path(hiseq_x_dual_index_flow_cell_dir, DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME)
 
 
 @pytest.fixture
-def lims_novaseq_6000_samples_file(bcl2fastq_flow_cell_dir: Path) -> Path:
-    """Return the path to the file with the raw samples of HVKJCDRXX flow cell in lims format."""
-    return Path(bcl2fastq_flow_cell_dir, "HVKJCDRXX_raw.json")
+def hiseq_2500_dual_index_sample_sheet_path(hiseq_2500_dual_index_flow_cell_dir: Path) -> Path:
+    """Return the path to a dual-index HiSeq2500 sample sheet."""
+    return Path(
+        hiseq_2500_dual_index_flow_cell_dir, DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME
+    )
 
 
 @pytest.fixture
-def demultiplexed_flow_cell(
-    illumina_demultiplexed_runs_directory, bcl2fastq_flow_cell_full_name: str
+def hiseq_2500_custom_index_sample_sheet_path(hiseq_2500_custom_index_flow_cell_dir: Path) -> Path:
+    """Return the path to a custom-index HiSeq2500 sample sheet."""
+    return Path(
+        hiseq_2500_custom_index_flow_cell_dir, DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME
+    )
+
+
+@pytest.fixture
+def novaseq_6000_pre_1_5_kits_correct_sample_sheet_path(
+    novaseq_6000_pre_1_5_kits_flow_cell_path: Path,
 ) -> Path:
-    """Return the path to a demultiplexed flow cell with bcl2fastq."""
-    return Path(illumina_demultiplexed_runs_directory, bcl2fastq_flow_cell_full_name)
+    return Path(novaseq_6000_pre_1_5_kits_flow_cell_path, CORRECT_SAMPLE_SHEET)
 
 
-# Fixtures for test demultiplex flow cell
 @pytest.fixture
-def tmp_empty_demultiplexed_runs_directory(
-    tmp_illumina_demultiplexed_flow_cells_directory,
+def novaseq_6000_post_1_5_kits_correct_sample_sheet_path(
+    novaseq_6000_post_1_5_kits_flow_cell_path: Path,
 ) -> Path:
-    return Path(tmp_illumina_demultiplexed_flow_cells_directory, "empty")
+    return Path(novaseq_6000_post_1_5_kits_flow_cell_path, CORRECT_SAMPLE_SHEET)
+
+
+@pytest.fixture
+def novaseq_x_correct_sample_sheet(novaseq_x_flow_cell_dir: Path) -> Path:
+    return Path(novaseq_x_flow_cell_dir, CORRECT_SAMPLE_SHEET)
+
+
+@pytest.fixture
+def novaseq_6000_sample_sheet_with_reversed_cycles(sample_sheet_dir: Path) -> Path:
+    """Return the path to a NovaSeq6000 sample sheet with reversed index2 cycles."""
+    return Path(sample_sheet_dir, "novaseq_6000_sample_sheet_with_reversed_cycles.csv")
+
+
+@pytest.fixture
+def novaseq_x_sample_sheet_with_forward_cycles(sample_sheet_dir: Path) -> Path:
+    """Return the path to a NovaSeqX sample sheet with forward index2 cycles."""
+    return Path(sample_sheet_dir, "novaseq_x_sample_sheet_with_forward_cycles.csv")
+
+
+# Path to other flow cell attributes
 
 
 @pytest.fixture
-def novaseqx_demultiplexed_flow_cell(
-    illumina_demultiplexed_runs_directory: Path, novaseq_x_flow_cell_full_name: str
-):
-    """Return the path to a demultiplexed NovaSeqX flow cell."""
-    return Path(illumina_demultiplexed_runs_directory, novaseq_x_flow_cell_full_name)
+def novaseq_x_manifest_file(novaseq_x_flow_cell_dir: Path) -> Path:
+    """Return the path to a NovaSeqX manifest file."""
+    return Path(novaseq_x_flow_cell_dir, "Manifest.tsv")
+
+
+@pytest.fixture(name="fastq_file")
+def fastq_file(fastq_dir: Path) -> Path:
+    """Return the path to a FASTQ file."""
+    return Path(fastq_dir, "dummy_run_R1_001.fastq.gz")
+
+
+@pytest.fixture(name="fastq_file_father")
+def fastq_file_father(fastq_dir: Path) -> Path:
+    """Return the path to a FASTQ file."""
+    return Path(fastq_dir, "fastq_run_R1_001.fastq.gz")
+
+
+@pytest.fixture(name="spring_file")
+def spring_file(spring_dir: Path) -> Path:
+    """Return the path to an existing spring file."""
+    return Path(spring_dir, "dummy_run_001.spring")
+
+
+@pytest.fixture(name="spring_meta_data_file")
+def spring_meta_data_file(spring_dir: Path) -> Path:
+    """Return the path to an existing spring file."""
+    return Path(spring_dir, "dummy_spring_meta_data.json")
+
+
+@pytest.fixture(name="spring_file_father")
+def spring_file_father(spring_dir: Path) -> Path:
+    """Return the path to a second existing spring file."""
+    return Path(spring_dir, "dummy_run_002.spring")
```

### Comparing `cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py` & `cg-60.4.2/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,22 +60,14 @@
 def hiseq_2500_custom_index_run_parameters(
     hiseq_2500_custom_index_run_parameters_path: Path,
 ) -> RunParametersHiSeq:
     """Return a HiSeq2500 run parameters object with custom index."""
     return RunParametersHiSeq(run_parameters_path=hiseq_2500_custom_index_run_parameters_path)
 
 
-@pytest.fixture(scope="session")
-def novaseq_6000_run_parameters(
-    novaseq_6000_run_parameters_path: Path,
-) -> RunParametersNovaSeq6000:
-    """Return a NovaSeq6000 run parameters object."""
-    return RunParametersNovaSeq6000(run_parameters_path=novaseq_6000_run_parameters_path)
-
-
 @pytest.fixture
 def novaseq_6000_run_parameters_pre_1_5_kits(
     novaseq_6000_run_parameters_pre_1_5_kits_path: Path,
 ) -> RunParametersNovaSeq6000:
     """Return a NovaSeq6000 run parameters pre 1.5 kit object."""
     return RunParametersNovaSeq6000(
         run_parameters_path=novaseq_6000_run_parameters_pre_1_5_kits_path
```

### Comparing `cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py` & `cg-60.4.2/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,17 +100,17 @@
 @pytest.fixture
 def selected_novaseq_6000_post_1_5_kits_sample_ids() -> list[str]:
     """Return a list of sample ids for a HiSeqX single index flow cell."""
     return ["ACC12642A4", "ACC12642A7"]
 
 
 @pytest.fixture
-def novaseq_x_lims_samples(novaseq_x_flow_cell_directory: Path) -> list[FlowCellSample]:
+def novaseq_x_lims_samples(novaseq_x_flow_cell_dir: Path) -> list[FlowCellSample]:
     """Return a list of BCLConvert samples parsed from LIMS for a NovaSeqX flow cell."""
-    path = Path(novaseq_x_flow_cell_directory, "22F52TLT3_raw.json")
+    path = Path(novaseq_x_flow_cell_dir, "22F52TLT3_raw.json")
     return [FlowCellSample.model_validate(sample) for sample in read_json(path)]
 
 
 @pytest.fixture
 def selected_novaseq_x_sample_ids() -> list[str]:
     """Return a list of sample ids for a HiSeqX single index flow cell."""
     return ["ACC13169A1", "ACC13170A6"]
```

### Comparing `cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py` & `cg-60.4.2/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_check_scenario.py` & `cg-60.4.2/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_check_scenario.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_fixtures.py` & `cg-60.4.2/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixture_plugins/timestamp_fixtures.py` & `cg-60.4.2/tests/fixture_plugins/timestamp_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json` & `cg-60.4.2/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json` & `cg-60.4.2/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/analysis/raredisease/multiqc_data.json` & `cg-60.4.2/tests/fixtures/analysis/raredisease/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml` & `cg-60.4.2/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/analysis/rnafusion/multiqc_data.json` & `cg-60.4.2/tests/fixtures/analysis/rnafusion/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml` & `cg-60.4.2/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/analysis/sample_coverage.bed` & `cg-60.4.2/tests/fixtures/analysis/sample_coverage.bed`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/analysis/taxprofiler/multiqc_data.json` & `cg-60.4.2/tests/fixtures/analysis/taxprofiler/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml` & `cg-60.4.2/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/analysis/tomte/multiqc_data.json` & `cg-60.4.2/tests/fixtures/analysis/tomte/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml` & `cg-60.4.2/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/balsamic/case/config.json` & `cg-60.4.2/tests/fixtures/apps/balsamic/case/config.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/balsamic/case/metadata.yml` & `cg-60.4.2/tests/fixtures/apps/balsamic/case/metadata.yml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml` & `cg-60.4.2/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/crunchy/spring_metadata.json` & `cg-60.4.2/tests/fixtures/apps/crunchy/spring_metadata.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv` & `cg-60.4.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/SampleSheet.csv`

 * *Files 14% similar despite different names*

```diff
@@ -11,9 +11,10 @@
 Index2Cycles,8
 [BCLConvert_Settings]
 SoftwareVersion,4.1.7
 FastqCompressionFormat,gzip
 [BCLConvert_Data]
 Lane,Sample_ID,Index,Index2,OverrideCycles,AdapterRead1,AdapterRead2,BarcodeMismatchesIndex1,BarcodeMismatchesIndex2
 1,ACC11927A2,TTGAATAG,GTTATGGA,Y51;I8;I8;Y51,,,1,1
+1,ACC11927A5,TCTGGCGA,GTTGAATT,Y51;I8;I8;Y51,,,1,1
 2,ACC11927A2,TTGAATAG,GTTATGGA,Y51;I8;I8;Y51,,,1,1
 2,ACC11927A5,TCTGGCGA,GTTGAATT,Y51;I8;I8;Y51,,,1,1
```

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stderr` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stdout` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml`

 * *Files 0% similar despite different names*

#### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml`

```diff
@@ -2,15 +2,15 @@
 <RunParameters xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
   <Surface>Both</Surface>
   <ReadType>PairedEnd</ReadType>
   <Side>A</Side>
   <Read1NumberOfCycles>151</Read1NumberOfCycles>
   <Read2NumberOfCycles>151</Read2NumberOfCycles>
   <IndexRead1NumberOfCycles>10</IndexRead1NumberOfCycles>
-  <IndexRead2NumberOfCycles>10</IndexRead2NumberOfCycles>
+  <IndexRead2NumberOfCycles>8</IndexRead2NumberOfCycles>
   <PlannedRead1Cycles>151</PlannedRead1Cycles>
   <PlannedRead2Cycles>151</PlannedRead2Cycles>
   <PlannedIndex1ReadCycles>10</PlannedIndex1ReadCycles>
   <PlannedIndex2ReadCycles>10</PlannedIndex2ReadCycles>
   <RunNumber>226</RunNumber>
   <RtaVersion>v3.4.4</RtaVersion>
   <RecipeVersion>1.7.0</RecipeVersion>
```

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RunParameters.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml`

 * *Files 22% similar despite different names*

#### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml`

```diff
@@ -7,93 +7,82 @@
   <Read2NumberOfCycles>51</Read2NumberOfCycles>
   <IndexRead1NumberOfCycles>8</IndexRead1NumberOfCycles>
   <IndexRead2NumberOfCycles>8</IndexRead2NumberOfCycles>
   <PlannedRead1Cycles>51</PlannedRead1Cycles>
   <PlannedRead2Cycles>51</PlannedRead2Cycles>
   <PlannedIndex1ReadCycles>8</PlannedIndex1ReadCycles>
   <PlannedIndex2ReadCycles>8</PlannedIndex2ReadCycles>
-  <RunNumber>615</RunNumber>
+  <RunNumber>636</RunNumber>
   <RtaVersion>v3.4.4</RtaVersion>
   <RecipeVersion>1.7.5</RecipeVersion>
-  <ExperimentName>HLG5GDRXY</ExperimentName>
+  <ExperimentName>H7CJFDRX2_NIPT</ExperimentName>
   <RfidsInfo>
-    <FlowCellSerialBarcode>HLG5GDRXY</FlowCellSerialBarcode>
+    <FlowCellSerialBarcode>H7CJFDRX2</FlowCellSerialBarcode>
     <FlowCellPartNumber>20026406</FlowCellPartNumber>
-    <FlowCellLotNumber>20574340</FlowCellLotNumber>
-    <FlowCellExpirationdate>08/19/2022 00:00:00</FlowCellExpirationdate>
-    <FlowCellStartDate>11/01/2021 11:50:00</FlowCellStartDate>
+    <FlowCellLotNumber>20630580</FlowCellLotNumber>
+    <FlowCellExpirationdate>03/06/2023 00:00:00</FlowCellExpirationdate>
+    <FlowCellStartDate>09/06/2022 10:10:00</FlowCellStartDate>
     <FlowCellNumberOfReuseRemaining>1</FlowCellNumberOfReuseRemaining>
     <FlowCellSupportedModes>LTWashOnly;SP</FlowCellSupportedModes>
     <FlowCellMode>SP</FlowCellMode>
     <FlowCellConsumableVersion>1</FlowCellConsumableVersion>
-    <FlowCellRssi>2</FlowCellRssi>
-    <LibraryTubeSerialBarcode>NV0394639-LIB</LibraryTubeSerialBarcode>
+    <FlowCellRssi>3</FlowCellRssi>
+    <LibraryTubeSerialBarcode>NV0552761-LIB</LibraryTubeSerialBarcode>
     <LibraryTubeSupportedModes>Universal</LibraryTubeSupportedModes>
     <LibraryTubePartNumber>20005221</LibraryTubePartNumber>
-    <LibraryTubeLotNumber>1000010192</LibraryTubeLotNumber>
+    <LibraryTubeLotNumber>1000012287</LibraryTubeLotNumber>
     <LibraryTubeExpirationdate>12/31/2169 00:00:00</LibraryTubeExpirationdate>
-    <LibraryTubeStartDate>11/01/2021 11:50:00</LibraryTubeStartDate>
+    <LibraryTubeStartDate>09/06/2022 10:10:00</LibraryTubeStartDate>
     <LibraryTubeRssi>3</LibraryTubeRssi>
-    <SbsSerialBarcode>NV3512584-RGSBS</SbsSerialBarcode>
+    <SbsSerialBarcode>NV4070602-RGSBS</SbsSerialBarcode>
     <SbsSupportedModes>S2;S1;SP</SbsSupportedModes>
     <SbsPartNumber>20031052</SbsPartNumber>
-    <SbsLotNumber>20559158</SbsLotNumber>
-    <SbsExpirationdate>07/20/2022 00:00:00</SbsExpirationdate>
-    <SbsStartDate>11/01/2021 11:50:00</SbsStartDate>
+    <SbsLotNumber>20638353</SbsLotNumber>
+    <SbsExpirationdate>03/30/2023 00:00:00</SbsExpirationdate>
+    <SbsStartDate>09/06/2022 10:10:00</SbsStartDate>
     <SbsCycleKit>138</SbsCycleKit>
     <SbsNumberOfCyclesRemaining>20</SbsNumberOfCyclesRemaining>
     <SbsNumberOfCyclesSupported>138</SbsNumberOfCyclesSupported>
-    <SbsConsumableVersion>3</SbsConsumableVersion>
     <SbsRssi>4</SbsRssi>
-    <ClusterSerialBarcode>NV3552837-RGCPE</ClusterSerialBarcode>
+    <ClusterSerialBarcode>NV4087232-RGCPE</ClusterSerialBarcode>
     <ClusterSupportedModes>SP</ClusterSupportedModes>
     <ClusterPartNumber>20031059</ClusterPartNumber>
-    <ClusterLotNumber>20566881</ClusterLotNumber>
-    <ClusterExpirationdate>08/06/2022 00:00:00</ClusterExpirationdate>
-    <ClusterStartDate>11/01/2021 11:50:00</ClusterStartDate>
+    <ClusterLotNumber>20640436</ClusterLotNumber>
+    <ClusterExpirationdate>04/04/2023 00:00:00</ClusterExpirationdate>
+    <ClusterStartDate>09/06/2022 10:10:00</ClusterStartDate>
     <ClusterCycleKit>545</ClusterCycleKit>
     <ClusterNumberOfCyclesRemaining>427</ClusterNumberOfCyclesRemaining>
     <ClusterRssi>5</ClusterRssi>
-    <BufferSerialBarcode>NV5203688-BUFFR</BufferSerialBarcode>
+    <BufferSerialBarcode>NV5388324-BUFFR</BufferSerialBarcode>
     <BufferSupportedModes>S2;S1;SP</BufferSupportedModes>
     <BufferPartNumber>20013524</BufferPartNumber>
-    <BufferLotNumber>50000217</BufferLotNumber>
-    <BufferExpirationdate>04/16/2022 00:00:00</BufferExpirationdate>
+    <BufferLotNumber>50000370</BufferLotNumber>
+    <BufferExpirationdate>03/02/2023 00:00:00</BufferExpirationdate>
     <BufferNumberOfCyclesRemaining>212</BufferNumberOfCyclesRemaining>
-    <BufferStartDate>11/01/2021 11:50:00</BufferStartDate>
-    <BufferRssi>3</BufferRssi>
+    <BufferStartDate>09/06/2022 10:10:00</BufferStartDate>
+    <BufferRssi>4</BufferRssi>
   </RfidsInfo>
-  <RecipeFilePath>C:\Program Files\Illumina\NovaSeq Control Software\Recipe</RecipeFilePath>
   <SamplesheetFile/>
-  <UsedLimsSetup>false</UsedLimsSetup>
-  <CeLinuxRunFolder>/ilmn/outputfolder/211101_A00187_0615_AHLG5GDRXY/</CeLinuxRunFolder>
-  <RtaRawRunFolder>/ilmn/outputfolder</RtaRawRunFolder>
-  <CeMountRunFolder>Z:\outputfolder\211101_A00187_0615_AHLG5GDRXY\</CeMountRunFolder>
-  <OutputRunFolder>\\172.16.1.6\clinicaldata\Runs\211101_A00187_0615_AHLG5GDRXY\</OutputRunFolder>
-  <OutputRootFolder>\\172.16.1.6\clinicaldata\Runs</OutputRootFolder>
-  <SbcRunFolder>C:\ProgramData\Illumina\NovaSeq\NovaSeqTemp\211101_A00187_0615_AHLG5GDRXY\</SbcRunFolder>
-  <PreRunFolder>C:\ProgramData\Illumina\NovaSeq\NovaSeqTemp\RunSetupLogs\A00187_2021-11-01__11_35_59_SideA</PreRunFolder>
-  <RunStartDate>211101</RunStartDate>
-  <RunId>211101_A00187_0615_AHLG5GDRXY</RunId>
+  <RunStartDate>220906</RunStartDate>
+  <RunId>220906_A00689_0636_AH7CJFDRX2</RunId>
   <UseBaseSpace>true</UseBaseSpace>
   <UseBaseSpaceMonitoringAndStorage>false</UseBaseSpaceMonitoringAndStorage>
-  <BaseSpaceRunId>7618619</BaseSpaceRunId>
+  <BaseSpaceRunId>10109099</BaseSpaceRunId>
   <BaseSpaceEnvironment>euc1-prod</BaseSpaceEnvironment>
   <BaseSpaceDomain/>
   <Autocenter>true</Autocenter>
   <BiDirectionalScanning>true</BiDirectionalScanning>
   <UseCustomRecipe>false</UseCustomRecipe>
   <UseCustomRead1Primer>false</UseCustomRead1Primer>
   <UseCustomRead2Primer>false</UseCustomRead2Primer>
   <UseCustomIndexRead1Primer>false</UseCustomIndexRead1Primer>
   <IsRehyb>false</IsRehyb>
-  <InstrumentName>A00187</InstrumentName>
+  <InstrumentName>A00689</InstrumentName>
   <PlatformType>HighThroughput</PlatformType>
   <Application>NovaSeq Control Software</Application>
-  <ApplicationVersion>1.7.5</ApplicationVersion>
   <Build>27</Build>
   <FirmwareVersions>
     <FirmwareVersion>
       <Board>Fluidics Board</Board>
       <Version>novaseq_flu@NovaSeq_1.26.1</Version>
     </FirmwareVersion>
     <FirmwareVersion>
@@ -130,12 +119,11 @@
     </FirmwareVersion>
     <FirmwareVersion>
       <Board>Right Reagent Chiller Board</Board>
       <Version>novaseq_rca@NovaSeq_1.26.1</Version>
     </FirmwareVersion>
   </FirmwareVersions>
   <SendIlluminaHealthData>true</SendIlluminaHealthData>
-  <UcsRunId>187B23D04A498564</UcsRunId>
   <UcsVersion>1.6.3.1575</UcsVersion>
   <RunSetupMode>Manual</RunSetupMode>
   <WorkflowType>NovaSeqStandard</WorkflowType>
 </RunParameters>
```

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv` & `cg-60.4.2/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/fluffy/SampleSheet.csv` & `cg-60.4.2/tests/fixtures/apps/fluffy/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/fluffy/deliverables.yaml` & `cg-60.4.2/tests/fixtures/apps/fluffy/deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/madeline/madeline.xml` & `cg-60.4.2/tests/fixtures/apps/madeline/madeline.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/mip/case_metrics_deliverables.yaml` & `cg-60.4.2/tests/fixtures/apps/mip/case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/mip/dna/store/case_config.yaml` & `cg-60.4.2/tests/fixtures/apps/mip/dna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml` & `cg-60.4.2/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml` & `cg-60.4.2/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf` & `cg-60.4.2/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/mip/rna/case_config.yaml` & `cg-60.4.2/tests/fixtures/apps/mip/rna/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml` & `cg-60.4.2/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/mip/rna/store/bundle_data.yaml` & `cg-60.4.2/tests/fixtures/apps/mip/rna/store/bundle_data.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/mip/rna/store/case_config.yaml` & `cg-60.4.2/tests/fixtures/apps/mip/rna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml` & `cg-60.4.2/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml` & `cg-60.4.2/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/scout/643594.config.yaml` & `cg-60.4.2/tests/fixtures/apps/scout/643594.config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/scout/case_export.json` & `cg-60.4.2/tests/fixtures/apps/scout/case_export.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/scout/export_causatives.json` & `cg-60.4.2/tests/fixtures/apps/scout/export_causatives.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/scout/none_case_export.json` & `cg-60.4.2/tests/fixtures/apps/scout/none_case_export.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/scout/other_sex_case.json` & `cg-60.4.2/tests/fixtures/apps/scout/other_sex_case.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/scout/panel_export.bed` & `cg-60.4.2/tests/fixtures/apps/scout/panel_export.bed`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/scout/panel_export.csv` & `cg-60.4.2/tests/fixtures/apps/scout/panel_export.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv` & `cg-60.4.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv` & `cg-60.4.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv` & `cg-60.4.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/cgweb_orders/balsamic.json` & `cg-60.4.2/tests/fixtures/cgweb_orders/balsamic.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/cgweb_orders/fastq.json` & `cg-60.4.2/tests/fixtures/cgweb_orders/fastq.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/cgweb_orders/metagenome.json` & `cg-60.4.2/tests/fixtures/cgweb_orders/metagenome.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/cgweb_orders/microsalt.json` & `cg-60.4.2/tests/fixtures/cgweb_orders/microsalt.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/cgweb_orders/mip.json` & `cg-60.4.2/tests/fixtures/cgweb_orders/mip.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/cgweb_orders/mip_rna.json` & `cg-60.4.2/tests/fixtures/cgweb_orders/mip_rna.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/cgweb_orders/rml.json` & `cg-60.4.2/tests/fixtures/cgweb_orders/rml.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/cgweb_orders/rnafusion.json` & `cg-60.4.2/tests/fixtures/cgweb_orders/rnafusion.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/cgweb_orders/sarscov2.json` & `cg-60.4.2/tests/fixtures/cgweb_orders/sarscov2.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/data/SampleSheet.csv` & `cg-60.4.2/tests/fixtures/data/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/data/cgfixture.db` & `cg-60.4.2/tests/fixtures/data/cgfixture.db`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/data/hkstore.db` & `cg-60.4.2/tests/fixtures/data/hkstore.db`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/io/example_json.json` & `cg-60.4.2/tests/fixtures/io/example_json.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/orderforms/1508.30.balsamic.xlsx` & `cg-60.4.2/tests/fixtures/orderforms/1508.30.balsamic.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx` & `cg-60.4.2/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx` & `cg-60.4.2/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/orderforms/1508.30.fastq.xlsx` & `cg-60.4.2/tests/fixtures/orderforms/1508.30.fastq.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/orderforms/1508.30.metagenome.xlsx` & `cg-60.4.2/tests/fixtures/orderforms/1508.30.metagenome.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/orderforms/1508.30.mip.xlsx` & `cg-60.4.2/tests/fixtures/orderforms/1508.30.mip.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/orderforms/1508.30.mip_rna.xlsx` & `cg-60.4.2/tests/fixtures/orderforms/1508.30.mip_rna.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/orderforms/1508.30.rnafusion.xlsx` & `cg-60.4.2/tests/fixtures/orderforms/1508.30.rnafusion.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/orderforms/1603.11.microbial.xlsx` & `cg-60.4.2/tests/fixtures/orderforms/1603.11.microbial.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/orderforms/1604.17.rml.xlsx` & `cg-60.4.2/tests/fixtures/orderforms/1604.17.rml.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/orderforms/2184.9.sarscov2.xlsx` & `cg-60.4.2/tests/fixtures/orderforms/2184.9.sarscov2.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/orderforms/NIPT-json.json` & `cg-60.4.2/tests/fixtures/orderforms/NIPT-json.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json` & `cg-60.4.2/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/orderforms/mip_uploaded_json_orderform.json` & `cg-60.4.2/tests/fixtures/orderforms/mip_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/report/case_data.json` & `cg-60.4.2/tests/fixtures/report/case_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/report/lims_exported_samples.json` & `cg-60.4.2/tests/fixtures/report/lims_exported_samples.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/fixtures/report/lims_family.json` & `cg-60.4.2/tests/fixtures/report/lims_family.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/io/conftest.py` & `cg-60.4.2/tests/io/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/io/test_io_controller.py` & `cg-60.4.2/tests/io/test_io_controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/io/test_io_csv.py` & `cg-60.4.2/tests/io/test_io_csv.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/io/test_io_json.py` & `cg-60.4.2/tests/io/test_io_json.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/io/test_io_txt.py` & `cg-60.4.2/tests/io/test_io_txt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/io/test_io_xml.py` & `cg-60.4.2/tests/io/test_io_xml.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/io/test_io_yaml.py` & `cg-60.4.2/tests/io/test_io_yaml.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/io/test_validate_path.py` & `cg-60.4.2/tests/io/test_validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/archive/conftest.py` & `cg-60.4.2/tests/meta/archive/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/archive/test_archive_api.py` & `cg-60.4.2/tests/meta/archive/test_archive_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/archive/test_archive_cli.py` & `cg-60.4.2/tests/meta/archive/test_archive_cli.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/archive/test_archiving.py` & `cg-60.4.2/tests/meta/archive/test_archiving.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/backup/conftest.py` & `cg-60.4.2/tests/meta/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/backup/test_meta_backup.py` & `cg-60.4.2/tests/meta/backup/test_meta_backup.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/backup/test_meta_pdc.py` & `cg-60.4.2/tests/meta/backup/test_meta_pdc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/clean/conftest.py` & `cg-60.4.2/tests/meta/clean/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,29 +46,29 @@
         status_db=store_with_flow_cell_not_to_clean,
         housekeeper_api=real_housekeeper_api,
         dry_run=False,
     )
 
 
 @pytest.fixture(scope="function")
-def tmp_flow_cell_to_clean_path(tmp_flow_cell_directory_bclconvert: Path):
+def tmp_flow_cell_to_clean_path(tmp_flow_cell_directory_bcl_convert: Path):
     """Returns the path to a flow cell fulfilling all cleaning criteria."""
-    return tmp_flow_cell_directory_bclconvert
+    return tmp_flow_cell_directory_bcl_convert
 
 
 @pytest.fixture(scope="function")
 def tmp_flow_cell_to_clean(tmp_flow_cell_to_clean_path: Path) -> FlowCellDirectoryData:
     """Returns a flow cell directory object for a flow cell that fulfills all cleaning criteria."""
     return FlowCellDirectoryData(tmp_flow_cell_to_clean_path)
 
 
 @pytest.fixture(scope="function")
-def tmp_flow_cell_not_to_clean_path(tmp_flow_cell_directory_bcl2fastq: Path):
+def tmp_flow_cell_not_to_clean_path(tmp_novaseq_6000_pre_1_5_kits_flow_cell_path: Path):
     """Return the path to a flow cell not fulfilling all cleaning criteria."""
-    return tmp_flow_cell_directory_bcl2fastq
+    return tmp_novaseq_6000_pre_1_5_kits_flow_cell_path
 
 
 @pytest.fixture(scope="function")
 def tmp_flow_cell_not_to_clean(tmp_flow_cell_not_to_clean_path: Path) -> FlowCellDirectoryData:
     """Returns a flow cell directory object for a flow cell that does not fulfill all cleaning criteria."""
     return FlowCellDirectoryData(tmp_flow_cell_not_to_clean_path)
```

### Comparing `cg-60.4.1/tests/meta/clean/test_clean_flow_cells_api.py` & `cg-60.4.2/tests/meta/clean/test_clean_flow_cells_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/clean/test_clean_retrieved_spring_files.py` & `cg-60.4.2/tests/meta/clean/test_clean_retrieved_spring_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/compress/conftest.py` & `cg-60.4.2/tests/meta/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/compress/test_clean_fastq.py` & `cg-60.4.2/tests/meta/compress/test_clean_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/compress/test_compress_files.py` & `cg-60.4.2/tests/meta/compress/test_compress_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/compress/test_compress_meta_fastq.py` & `cg-60.4.2/tests/meta/compress/test_compress_meta_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/compress/test_decompress_spring_meta.py` & `cg-60.4.2/tests/meta/compress/test_decompress_spring_meta.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/compress/test_meta_compress_update_hk.py` & `cg-60.4.2/tests/meta/compress/test_meta_compress_update_hk.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,22 +36,22 @@
     # THEN the flow cell id retrieved should be identical to the flow cell id used
     assert returned_flow_cell_name == hiseq_x_single_index_flow_cell_id
 
 
 def test_get_flow_cell_id_when_novaseq(
     compress_api: CompressAPI,
     novaseq_6000_pre_1_5_kits_flow_cell_id: str,
-    bcl2fastq_flow_cell_full_name: str,
+    novaseq_6000_pre_1_5_kits_flow_cell_full_name: str,
 ):
     """Test extracting the flow cell id from a fastq file path."""
 
     # GIVEN a CompressAPI and a flow cell id within a fastq file path
     fastq_path: Path = compress_api.demux_root.joinpath(
         Path(
-            bcl2fastq_flow_cell_full_name,
+            novaseq_6000_pre_1_5_kits_flow_cell_full_name,
             f"{novaseq_6000_pre_1_5_kits_flow_cell_id}_ACC10950A36_S36_L001_R1_001.fastq.gz",
         )
     )
 
     # WHEN retrieving the flow cell id
     returned_flow_cell_name: str = compress_api.get_flow_cell_id(fastq_path=fastq_path)
```

### Comparing `cg-60.4.1/tests/meta/conftest.py` & `cg-60.4.2/tests/meta/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/deliver/conftest.py` & `cg-60.4.2/tests/meta/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/deliver/test_deliver_ticket.py` & `cg-60.4.2/tests/meta/deliver/test_deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/deliver/test_delivery_api.py` & `cg-60.4.2/tests/meta/deliver/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/deliver/test_fastq_path_generator.py` & `cg-60.4.2/tests/meta/deliver/test_fastq_path_generator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/delivery/test_delivery_api.py` & `cg-60.4.2/tests/meta/delivery/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/demultiplex/conftest.py` & `cg-60.4.2/tests/meta/demultiplex/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 from tests.store_helpers import StoreHelpers
 
 FlowCellInfo = namedtuple("FlowCellInfo", "directory name sample_internal_ids")
 
 
 @pytest.fixture(name="tmp_demulitplexing_dir")
 def tmp_illumina_novaseq_demulitplexing_dir(
-    illumina_demultiplexed_runs_directory: Path, bcl2fastq_flow_cell_full_name: str
+    illumina_demultiplexed_runs_directory: Path, novaseq_6000_pre_1_5_kits_flow_cell_full_name: str
 ) -> Path:
     """Return a tmp directory in demultiplexed-runs."""
     tmp_demulitplexing_dir: Path = Path(
-        illumina_demultiplexed_runs_directory, bcl2fastq_flow_cell_full_name
+        illumina_demultiplexed_runs_directory, novaseq_6000_pre_1_5_kits_flow_cell_full_name
     )
     tmp_demulitplexing_dir.mkdir(exist_ok=True, parents=True)
     return tmp_demulitplexing_dir
 
 
 @pytest.fixture(name="tmp_fastq_paths")
 def temp_fastq_paths(tmp_demulitplexing_dir: Path) -> list[Path]:
@@ -42,43 +42,23 @@
 
 @pytest.fixture
 def demultiplex_fastq_file_path() -> Path:
     """Return a path to non-existent a fastq file."""
     return Path("path/to/sample_internal_id_S1_L001_R1_001.fastq.gz")
 
 
-@pytest.fixture(name="tmp_sample_sheet_path")
-def tmp_samplesheet_path(tmp_demulitplexing_dir: Path) -> Path:
+@pytest.fixture
+def tmp_sample_sheet_path(tmp_demulitplexing_dir: Path) -> Path:
     """Return SampleSheet in temporary demuliplexing folder."""
     tmp_sample_sheet_path = Path(tmp_demulitplexing_dir, "SampleSheet.csv")
     with tmp_sample_sheet_path.open("w+") as fh:
         fh.write("content")
     return tmp_sample_sheet_path
 
 
-@pytest.fixture(name="tmp_flow_cell_run_base_path")
-def tmp_flow_cell_run_base_path(project_dir: Path, bcl2fastq_flow_cell_full_name: str) -> Path:
-    """Flow cell run directory in temporary folder."""
-
-    tmp_flow_cell_run_path: Path = Path(project_dir, "flow_cells")
-    tmp_flow_cell_run_path.mkdir(exist_ok=True, parents=True)
-
-    return tmp_flow_cell_run_path
-
-
-@pytest.fixture(name="tmp_flow_cell_demux_base_path")
-def tmp_flow_cell_demux_base_path(project_dir: Path, bcl2fastq_flow_cell_full_name: str) -> Path:
-    """Flow cell demux directory in temporary folder."""
-
-    tmp_flow_cell_demux_path: Path = Path(project_dir, "demultiplexed-runs")
-    tmp_flow_cell_demux_path.mkdir(exist_ok=True, parents=True)
-
-    return tmp_flow_cell_demux_path
-
-
 @pytest.fixture(name="populated_flow_cell_store")
 def populated_flow_cell_store(
     family_name: str,
     novaseq_6000_pre_1_5_kits_flow_cell_id: str,
     sample_id: str,
     store: Store,
     helpers: StoreHelpers,
@@ -98,15 +78,15 @@
         flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id,
         sequencer_type="novaseq",
         samples=[sample],
     )
     return populated_flow_cell_store
 
 
-@pytest.fixture(name="active_flow_cell_store")
+@pytest.fixture
 def active_flow_cell_store(
     family_name: str,
     novaseq_6000_pre_1_5_kits_flow_cell_id: str,
     sample_id: str,
     base_store: Store,
     helpers: StoreHelpers,
 ) -> Store:
```

### Comparing `cg-60.4.1/tests/meta/demultiplex/test_combine_sequencing_metrics.py` & `cg-60.4.2/tests/meta/demultiplex/test_combine_sequencing_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/demultiplex/test_demux_post_processing.py` & `cg-60.4.2/tests/meta/demultiplex/test_demux_post_processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,28 +122,31 @@
 
     assert delivery_path.exists()
 
 
 def test_get_all_demultiplexed_flow_cell_out_dirs(
     demultiplex_context: CGConfig,
     tmp_illumina_demultiplexed_flow_cells_directory,
-    tmp_demultiplexed_runs_bcl2fastq_directory: Path,
+    hiseq_x_single_index_flow_cell_name: str,
 ):
     """Test returning all flow cell directories from the demultiplexing run directory."""
     # GIVEN a demultiplex flow cell finished output directory that exist
 
     # GIVEN a demultiplex context
     demux_api: DemuxPostProcessingAPI = DemuxPostProcessingAPI(config=demultiplex_context)
     demux_api.demultiplexed_runs_dir = tmp_illumina_demultiplexed_flow_cells_directory
 
     # WHEN calling get_all_demultiplexed_flow_cell_dirs
     demultiplexed_flow_cell_dirs: list[Path] = demux_api.get_all_demultiplexed_flow_cell_dirs()
 
     # THEN the demultiplexed flow cells run directories should be returned
-    assert tmp_demultiplexed_runs_bcl2fastq_directory in demultiplexed_flow_cell_dirs
+    demuxed_flow_cell_path = Path(
+        tmp_illumina_demultiplexed_flow_cells_directory, hiseq_x_single_index_flow_cell_name
+    )
+    assert demuxed_flow_cell_path in demultiplexed_flow_cell_dirs
 
 
 def test_post_processing_tracks_undetermined_fastq_files(
     updated_demux_post_processing_api: DemuxPostProcessingAPI,
     hiseq_x_single_index_flow_cell: FlowCellDirectoryData,
     selected_hiseq_x_single_index_sample_ids: list[str],
 ):
```

### Comparing `cg-60.4.1/tests/meta/demultiplex/test_housekeeper_storage_functions.py` & `cg-60.4.2/tests/meta/demultiplex/test_housekeeper_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/demultiplex/test_status_db_storage_functions.py` & `cg-60.4.2/tests/meta/demultiplex/test_status_db_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/demultiplex/test_utils.py` & `cg-60.4.2/tests/meta/demultiplex/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -482,23 +482,21 @@
     # WHEN checking if the flow cell sync has been confirmed
     is_synced = is_flow_cell_sync_confirmed(tmp_path)
 
     # THEN the result should match what we expect
     assert is_synced == expected_result
 
 
-def test_create_manifest_file(tmp_flow_cells_directory_ready_for_demultiplexing_bcl_convert: Path):
+def test_create_manifest_file(tmp_flow_cells_directory_ready_for_demultiplexing: Path):
     # GIVEN a flow cell directory with files
     all_files: list[Path] = get_all_files_in_directory_tree(
-        tmp_flow_cells_directory_ready_for_demultiplexing_bcl_convert
+        tmp_flow_cells_directory_ready_for_demultiplexing
     )
     # WHEN creating a manifest file
-    manifest_file: Path = create_manifest_file(
-        tmp_flow_cells_directory_ready_for_demultiplexing_bcl_convert
-    )
+    manifest_file: Path = create_manifest_file(tmp_flow_cells_directory_ready_for_demultiplexing)
 
     # THEN a manifest file should be created
     assert manifest_file.exists()
 
     # Then all files should be included in the manifest_file
     assert_file_contains_all_file_paths(manifest_file=manifest_file, files_in_file=all_files)
```

### Comparing `cg-60.4.1/tests/meta/demultiplex/test_validation.py` & `cg-60.4.2/tests/meta/demultiplex/test_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,33 +51,33 @@
 def test_is_flow_cell_ready_for_delivery_false(tmp_path: Path):
     # GIVEN a path without DELIVERY file
 
     # WHEN checking if the flow cell is ready for delivery
     result = is_flow_cell_ready_for_delivery(tmp_path)
 
     # THEN the result should be False
-    assert result == False
+    assert not result
 
 
-def test_validate_sample_sheet_exists_raises_error(bcl2fastq_flow_cell_dir: Path):
+def test_validate_sample_sheet_exists_raises_error(hiseq_2500_custom_index_flow_cell_dir: Path):
     # GIVEN a flow cell without a sample sheet in housekeeper
-    flow_cell = FlowCellDirectoryData(flow_cell_path=bcl2fastq_flow_cell_dir)
+    flow_cell = FlowCellDirectoryData(flow_cell_path=hiseq_2500_custom_index_flow_cell_dir)
     flow_cell._sample_sheet_path_hk = None
     # WHEN validating the existence of the sample sheet
     # THEN it should raise a FlowCellError
     with pytest.raises(FlowCellError):
         validate_sample_sheet_exists(flow_cell=flow_cell)
 
 
-def test_validate_sample_sheet_exists(bcl2fastq_flow_cell_dir: Path):
+def test_validate_sample_sheet_exists(hiseq_2500_custom_index_flow_cell_dir: Path):
     # GIVEN a path with a sample sheet
     # GIVEN a flow cell without a sample sheet in housekeeper
-    flow_cell = FlowCellDirectoryData(flow_cell_path=bcl2fastq_flow_cell_dir)
+    flow_cell = FlowCellDirectoryData(flow_cell_path=hiseq_2500_custom_index_flow_cell_dir)
     sample_sheet_path = Path(
-        bcl2fastq_flow_cell_dir, DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME
+        hiseq_2500_custom_index_flow_cell_dir, DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME
     )
     sample_sheet_path.touch()
     flow_cell._sample_sheet_path_hk = sample_sheet_path
 
     # WHEN validating the existence of the sample sheet
     # THEN it should not raise an error
     assert validate_sample_sheet_exists(flow_cell=flow_cell) is None
```

### Comparing `cg-60.4.1/tests/meta/encryption/conftest.py` & `cg-60.4.2/tests/meta/encryption/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/encryption/test_encryption.py` & `cg-60.4.2/tests/meta/encryption/test_encryption.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/observations/conftest.py` & `cg-60.4.2/tests/meta/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/observations/test_meta_upload_observations.py` & `cg-60.4.2/tests/meta/observations/test_meta_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/orders/conftest.py` & `cg-60.4.2/tests/meta/orders/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/orders/test_PoolSubmitter_validate_order.py` & `cg-60.4.2/tests/meta/orders/test_PoolSubmitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py` & `cg-60.4.2/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/orders/test_SarsCov2Submitter_store_order.py` & `cg-60.4.2/tests/meta/orders/test_SarsCov2Submitter_store_order.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/orders/test_SarsCov2Submitter_validate_order.py` & `cg-60.4.2/tests/meta/orders/test_SarsCov2Submitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/orders/test_meta_orders_api.py` & `cg-60.4.2/tests/meta/orders/test_meta_orders_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/orders/test_meta_orders_lims.py` & `cg-60.4.2/tests/meta/orders/test_meta_orders_lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/orders/test_meta_orders_status.py` & `cg-60.4.2/tests/meta/orders/test_meta_orders_status.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/orders/test_rnafusion_submitter.py` & `cg-60.4.2/tests/meta/orders/test_rnafusion_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/orders/test_ticket_handler.py` & `cg-60.4.2/tests/meta/orders/test_ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/qc_metrics/conftest.py` & `cg-60.4.2/tests/meta/qc_metrics/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/qc_metrics/test_collect_qc_metrics.py` & `cg-60.4.2/tests/meta/qc_metrics/test_collect_qc_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/report/conftest.py` & `cg-60.4.2/tests/meta/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/report/test_balsamic_api.py` & `cg-60.4.2/tests/meta/report/test_balsamic_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/report/test_field_validators.py` & `cg-60.4.2/tests/meta/report/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/report/test_mip_dna_api.py` & `cg-60.4.2/tests/meta/report/test_mip_dna_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/report/test_report_api.py` & `cg-60.4.2/tests/meta/report/test_report_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/report/test_rnafusion_api.py` & `cg-60.4.2/tests/meta/report/test_rnafusion_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/report/test_tomte_api.py` & `cg-60.4.2/tests/meta/report/test_tomte_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/rsync/conftest.py` & `cg-60.4.2/tests/meta/rsync/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/rsync/test_rsync.py` & `cg-60.4.2/tests/meta/rsync/test_rsync.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/test_invoice.py` & `cg-60.4.2/tests/meta/test_invoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/transfer/conftest.py` & `cg-60.4.2/tests/meta/transfer/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/transfer/test_external_data.py` & `cg-60.4.2/tests/meta/transfer/test_external_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/transfer/test_meta_transfer_lims.py` & `cg-60.4.2/tests/meta/transfer/test_meta_transfer_lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/upload/balsamic/test_balsamic.py` & `cg-60.4.2/tests/meta/upload/balsamic/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/upload/conftest.py` & `cg-60.4.2/tests/meta/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/upload/gisaid/fixtures/four_samples.csv` & `cg-60.4.2/tests/meta/upload/gisaid/fixtures/four_samples.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/upload/mutacc/conftest.py` & `cg-60.4.2/tests/meta/upload/mutacc/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/upload/mutacc/test_meta_upload_mutacc.py` & `cg-60.4.2/tests/meta/upload/mutacc/test_meta_upload_mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/upload/nipt/conftest.py` & `cg-60.4.2/tests/meta/upload/nipt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/upload/nipt/test_models.py` & `cg-60.4.2/tests/meta/upload/nipt/test_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/upload/nipt/test_nipt_upload_api.py` & `cg-60.4.2/tests/meta/upload/nipt/test_nipt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/upload/scout/conftest.py` & `cg-60.4.2/tests/meta/upload/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/upload/scout/test_generate_load_config.py` & `cg-60.4.2/tests/meta/upload/scout/test_generate_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/upload/scout/test_meta_upload_scoutapi.py` & `cg-60.4.2/tests/meta/upload/scout/test_meta_upload_scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py` & `cg-60.4.2/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/upload/scout/test_scout_config_builder.py` & `cg-60.4.2/tests/meta/upload/scout/test_scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/upload/test_meta_upload_coverage.py` & `cg-60.4.2/tests/meta/upload/test_meta_upload_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/upload/test_upload_api.py` & `cg-60.4.2/tests/meta/upload/test_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/upload/test_upload_genotypes_api.py` & `cg-60.4.2/tests/meta/upload/test_upload_genotypes_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/workflow/conftest.py` & `cg-60.4.2/tests/meta/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/workflow/microsalt/conftest.py` & `cg-60.4.2/tests/meta/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/workflow/microsalt/test_quality_controller.py` & `cg-60.4.2/tests/meta/workflow/microsalt/test_quality_controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/workflow/microsalt/test_quality_controller_utils.py` & `cg-60.4.2/tests/meta/workflow/microsalt/test_quality_controller_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/workflow/microsalt/test_report_generation.py` & `cg-60.4.2/tests/meta/workflow/microsalt/test_report_generation.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/workflow/test_analysis.py` & `cg-60.4.2/tests/meta/workflow/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/workflow/test_balsamic.py` & `cg-60.4.2/tests/meta/workflow/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/workflow/test_fastq.py` & `cg-60.4.2/tests/meta/workflow/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/workflow/test_microsalt.py` & `cg-60.4.2/tests/meta/workflow/test_microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/workflow/test_nf_analysis.py` & `cg-60.4.2/tests/meta/workflow/test_nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/workflow/test_prepare_fastq_api.py` & `cg-60.4.2/tests/meta/workflow/test_prepare_fastq_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/workflow/test_raredisease.py` & `cg-60.4.2/tests/meta/workflow/test_raredisease.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/meta/workflow/test_rnafusion.py` & `cg-60.4.2/tests/meta/workflow/test_rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/mocks/balsamic_analysis_mock.py` & `cg-60.4.2/tests/mocks/balsamic_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/mocks/crunchy.py` & `cg-60.4.2/tests/mocks/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/mocks/hk_mock.py` & `cg-60.4.2/tests/mocks/hk_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/mocks/limsmock.py` & `cg-60.4.2/tests/mocks/limsmock.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/mocks/madeline.py` & `cg-60.4.2/tests/mocks/madeline.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/mocks/mip_analysis_mock.py` & `cg-60.4.2/tests/mocks/mip_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/mocks/osticket.py` & `cg-60.4.2/tests/mocks/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/mocks/process_mock.py` & `cg-60.4.2/tests/mocks/process_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/mocks/report.py` & `cg-60.4.2/tests/mocks/report.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/mocks/scout.py` & `cg-60.4.2/tests/mocks/scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/mocks/store_model.py` & `cg-60.4.2/tests/mocks/store_model.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/mocks/tb_mock.py` & `cg-60.4.2/tests/mocks/tb_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/models/balsamic/conftest.py` & `cg-60.4.2/tests/models/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/models/balsamic/test_balsamic_analysis.py` & `cg-60.4.2/tests/models/balsamic/test_balsamic_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/models/conftest.py` & `cg-60.4.2/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/models/demultiplexing/test_run_parameters.py` & `cg-60.4.2/tests/models/demultiplexing/test_run_parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 @pytest.mark.parametrize(
     "run_parameters_path_fixture",
     [
         "hiseq_x_single_index_run_parameters_path",
         "hiseq_2500_dual_index_run_parameters_path",
-        "novaseq_6000_run_parameters_path",
+        "novaseq_6000_run_parameters_pre_1_5_kits_path",
         "novaseq_x_run_parameters_path",
     ],
 )
 def test_run_parameters_parent_class_fails(
     run_parameters_path_fixture: str, request: FixtureRequest
 ):
     """Test that trying to instantiate the parent RunParameters class raises an error."""
@@ -48,15 +48,19 @@
 
 
 @pytest.mark.parametrize(
     "run_parameters_path, constructor, sequencer",
     [
         ("hiseq_x_single_index_run_parameters_path", RunParametersHiSeq, Sequencers.HISEQX),
         ("hiseq_2500_dual_index_run_parameters_path", RunParametersHiSeq, Sequencers.HISEQGA),
-        ("novaseq_6000_run_parameters_path", RunParametersNovaSeq6000, Sequencers.NOVASEQ),
+        (
+            "novaseq_6000_run_parameters_pre_1_5_kits_path",
+            RunParametersNovaSeq6000,
+            Sequencers.NOVASEQ,
+        ),
         ("novaseq_x_run_parameters_path", RunParametersNovaSeqX, Sequencers.NOVASEQX),
     ],
 )
 def test_run_parameters_init(
     run_parameters_path: str,
     constructor: Type[RunParameters],
     sequencer: str,
@@ -81,15 +85,15 @@
     error_msg: str
 
 
 @pytest.mark.parametrize(
     "scenario",
     [
         RunParametersScenario(
-            wrong_run_parameters_path_fixture="novaseq_6000_run_parameters_path",
+            wrong_run_parameters_path_fixture="novaseq_6000_run_parameters_pre_1_5_kits_path",
             constructor=RunParametersHiSeq,
             error_msg=f"Could not find node {RunParametersXMLNodes.APPLICATION_NAME} in the run parameters file.",
         ),
         RunParametersScenario(
             wrong_run_parameters_path_fixture="novaseq_x_run_parameters_path",
             constructor=RunParametersHiSeq,
             error_msg=f"Could not find node {RunParametersXMLNodes.APPLICATION_NAME} in the run parameters file.",
@@ -106,15 +110,15 @@
         ),
         RunParametersScenario(
             wrong_run_parameters_path_fixture="hiseq_x_single_index_run_parameters_path",
             constructor=RunParametersNovaSeqX,
             error_msg=f"Could not find node {RunParametersXMLNodes.INSTRUMENT_TYPE} in the run parameters file.",
         ),
         RunParametersScenario(
-            wrong_run_parameters_path_fixture="novaseq_6000_run_parameters_path",
+            wrong_run_parameters_path_fixture="novaseq_6000_run_parameters_pre_1_5_kits_path",
             constructor=RunParametersNovaSeqX,
             error_msg=f"Could not find node {RunParametersXMLNodes.INSTRUMENT_TYPE} in the run parameters file.",
         ),
     ],
     ids=[
         "NovaSeq 6000 file, HiSeq constructor",
         "NovaSeq X file, HiSeq constructor",
@@ -156,20 +160,24 @@
 
     # WHEN fetching the reagent kit version
 
     # THEN the reagent kit version is None
     assert not run_parameters.reagent_kit_version
 
 
-def test_reagent_kit_version_novaseq_6000(novaseq_6000_run_parameters: RunParametersNovaSeq6000):
-    """Test that getting reagent kit version from a correct file returns an expected value."""
+def test_reagent_kit_version_novaseq_6000_post_1_5_kits(
+    novaseq_6000_run_parameters_post_1_5_kits: RunParametersNovaSeq6000,
+):
+    """
+    Test that getting reagent kit version from a NovaSeq6000 post 1.5 kits does not return unknown.
+    """
     # GIVEN a valid RunParameters object for NovaSeq6000
 
     # WHEN fetching the reagent kit version
-    reagent_kit_version: str = novaseq_6000_run_parameters.reagent_kit_version
+    reagent_kit_version: str = novaseq_6000_run_parameters_post_1_5_kits.reagent_kit_version
 
     # THEN the reagent kit version exists and is not "unknown"
     assert reagent_kit_version
     assert reagent_kit_version != RunParametersXMLNodes.UNKNOWN_REAGENT_KIT_VERSION
 
 
 @pytest.mark.parametrize(
@@ -190,21 +198,23 @@
     # WHEN fetching the control software version
 
     # THEN the control software version is None
     assert not run_parameters.control_software_version
 
 
 def test_control_software_version_novaseq_6000(
-    novaseq_6000_run_parameters: RunParametersNovaSeq6000,
+    novaseq_6000_run_parameters_pre_1_5_kits: RunParametersNovaSeq6000,
 ):
     """Test that getting control software version from a correct file returns an expected value."""
     # GIVEN a valid RunParameters object for NovaSeq6000
 
     # WHEN fetching the control software version
-    control_software_version: str = novaseq_6000_run_parameters.control_software_version
+    control_software_version: str = (
+        novaseq_6000_run_parameters_pre_1_5_kits.control_software_version
+    )
 
     # THEN the control software version is a non-empty string
     assert isinstance(control_software_version, str)
     assert control_software_version != ""
 
 
 def test_novaseq_6000_no_version(run_parameters_missing_versions_path: Path, caplog):
@@ -222,17 +232,18 @@
         in caplog.text
     )
 
 
 @pytest.mark.parametrize(
     "run_parameters_fixture",
     [
-        "hiseq_2500_dual_index_run_parameters",
         "hiseq_x_single_index_run_parameters",
-        "novaseq_6000_run_parameters",
+        "hiseq_2500_dual_index_run_parameters",
+        "novaseq_6000_run_parameters_pre_1_5_kits",
+        "novaseq_6000_run_parameters_post_1_5_kits",
         "novaseq_x_run_parameters",
     ],
 )
 def test_get_cycles(run_parameters_fixture: str, request: FixtureRequest):
     """Test that the read and index cycles are read correctly for any RunParameters object."""
     # GIVEN a RunParameters object
     run_parameters: RunParameters = request.getfixturevalue(run_parameters_fixture)
```

### Comparing `cg-60.4.1/tests/models/downsample/test_down_sample_meta_data.py` & `cg-60.4.2/tests/models/downsample/test_down_sample_meta_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/models/flow_cell/test_flowcell_model.py` & `cg-60.4.2/tests/models/flow_cell/test_flowcell_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 from cg.constants.sequencing import Sequencers
 from cg.exc import FlowCellError
 from cg.models.demultiplex.run_parameters import RunParameters
 from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
 from cg.utils.flow_cell import get_flow_cell_id
 
 
-def test_flow_cell_id(bcl2fastq_flow_cell_dir: Path):
+def test_flow_cell_id(hiseq_2500_dual_index_flow_cell_dir: Path):
     """Test parsing of flow cell id."""
     # GIVEN the path to a finished flow cell run
     # GIVEN the flow cell id
-    flowcell_id: str = get_flow_cell_id(bcl2fastq_flow_cell_dir.name)
+    flowcell_id: str = get_flow_cell_id(hiseq_2500_dual_index_flow_cell_dir.name)
 
     # WHEN instantiating a flow cell object
-    flowcell_obj = FlowCellDirectoryData(flow_cell_path=bcl2fastq_flow_cell_dir)
+    flowcell_obj = FlowCellDirectoryData(flow_cell_path=hiseq_2500_dual_index_flow_cell_dir)
 
     # THEN assert that the flow cell id is parsed
     assert flowcell_obj.id == flowcell_id
 
 
-def test_flow_cell_position(bcl2fastq_flow_cell_dir: Path):
+def test_flow_cell_position(hiseq_2500_dual_index_flow_cell_dir: Path):
     """Test getting flow cell position."""
     # GIVEN the path to a finished flow cell
     # GIVEN a flow cell object
-    flow_cell = FlowCellDirectoryData(flow_cell_path=bcl2fastq_flow_cell_dir)
+    flow_cell = FlowCellDirectoryData(flow_cell_path=hiseq_2500_dual_index_flow_cell_dir)
 
     # WHEN fetching the flow cell position
     position = flow_cell.position
 
     # THEN assert it is A or B
     assert position in ["A", "B"]
 
@@ -107,31 +107,31 @@
     # WHEN creating the run parameters of the flow cell
     run_parameters: RunParameters = flow_cell.run_parameters
 
     # THEN the run parameters sequencer is the same as of the flow cell
     assert run_parameters.sequencer == expected_sequencer
 
 
-def test_has_demultiplexing_started_locally_false(tmp_flow_cell_directory_bclconvert: Path):
+def test_has_demultiplexing_started_locally_false(tmp_flow_cell_directory_bcl_convert: Path):
     # GIVEN a flow cell without a demuxstarted.txt file
-    flow_cell = FlowCellDirectoryData(tmp_flow_cell_directory_bclconvert)
+    flow_cell = FlowCellDirectoryData(tmp_flow_cell_directory_bcl_convert)
     assert not Path(flow_cell.path, DemultiplexingDirsAndFiles.DEMUX_STARTED).exists()
 
     # WHEN checking if the flow cell has started demultiplexing
     has_demux_started: bool = flow_cell.has_demultiplexing_started_locally()
 
     # THEN the response should be False
     assert not has_demux_started
 
 
 def test_has_demultiplexing_started_locally_true(
-    tmp_flow_cell_directory_bclconvert: Path,
+    tmp_flow_cell_directory_bcl_convert: Path,
 ):
     # GIVEN a flow cell with a demuxstarted.txt file
-    flow_cell = FlowCellDirectoryData(tmp_flow_cell_directory_bclconvert)
+    flow_cell = FlowCellDirectoryData(tmp_flow_cell_directory_bcl_convert)
     Path(flow_cell.path, DemultiplexingDirsAndFiles.DEMUX_STARTED).touch()
 
     # WHEN checking if the flow cell has started demultiplexing
     has_demux_started: bool = flow_cell.has_demultiplexing_started_locally()
 
     # THEN the response should be True
     assert has_demux_started
```

### Comparing `cg-60.4.1/tests/models/mip/conftest.py` & `cg-60.4.2/tests/models/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/models/mip/test_mip_analysis.py` & `cg-60.4.2/tests/models/mip/test_mip_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/models/mip/test_mip_config.py` & `cg-60.4.2/tests/models/mip/test_mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/models/mip/test_mip_metrics_deliverables.py` & `cg-60.4.2/tests/models/mip/test_mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/models/mip/test_mip_sample_info.py` & `cg-60.4.2/tests/models/mip/test_mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/models/nextflow/test_nextflow_deliver.py` & `cg-60.4.2/tests/models/nextflow/test_nextflow_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/models/observations/conftest.py` & `cg-60.4.2/tests/models/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/models/observations/test_observations_input_files.py` & `cg-60.4.2/tests/models/observations/test_observations_input_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/models/report/test_validators.py` & `cg-60.4.2/tests/models/report/test_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/models/rnafusion/test_rnafusion_sample.py` & `cg-60.4.2/tests/models/rnafusion/test_rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/models/test_cg_models.py` & `cg-60.4.2/tests/models/test_cg_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/models/test_compression_data.py` & `cg-60.4.2/tests/models/test_compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/models/test_fastq.py` & `cg-60.4.2/tests/models/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/models/test_file_data.py` & `cg-60.4.2/tests/models/test_file_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/server/conftest.py` & `cg-60.4.2/tests/server/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/server/endpoints/test_delivery_message_endpoint.py` & `cg-60.4.2/tests/server/endpoints/test_delivery_message_endpoint.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/server/endpoints/test_orders_endpoint.py` & `cg-60.4.2/tests/server/endpoints/test_orders_endpoint.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/services/fastq_file_service/conftest.py` & `cg-60.4.2/tests/services/fastq_file_service/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/services/fastq_file_service/test_fastq_file_service.py` & `cg-60.4.2/tests/services/fastq_file_service/test_fastq_file_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/services/orders/order_status_service/conftest.py` & `cg-60.4.2/tests/services/orders/order_status_service/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/services/orders/order_status_service/test_order_summary_service.py` & `cg-60.4.2/tests/services/orders/order_status_service/test_order_summary_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/services/quality_controller/test_sequencing_quality_checks_utils.py` & `cg-60.4.2/tests/services/quality_controller/test_sequencing_quality_checks_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/api/conftest.py` & `cg-60.4.2/tests/store/api/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/api/test_base.py` & `cg-60.4.2/tests/store/api/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/conftest.py` & `cg-60.4.2/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/crud/add/test_store_add_application_version.py` & `cg-60.4.2/tests/store/crud/add/test_store_add_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/crud/add/test_store_add_base.py` & `cg-60.4.2/tests/store/crud/add/test_store_add_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/crud/add/test_store_add_customer.py` & `cg-60.4.2/tests/store/crud/add/test_store_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/crud/add/test_store_add_flow_celll.py` & `cg-60.4.2/tests/store/crud/add/test_store_add_flow_celll.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/crud/conftest.py` & `cg-60.4.2/tests/store/crud/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/crud/delete/test_delete.py` & `cg-60.4.2/tests/store/crud/delete/test_delete.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/crud/read/test_read.py` & `cg-60.4.2/tests/store/crud/read/test_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1314,23 +1314,23 @@
     assert metrics_entry.flow_cell_lane_number == lane
     assert metrics_entry.sample_internal_id == sample_id
 
 
 def test_get_number_of_reads_for_flow_cell_from_sample_lane_metrics(
     store_with_sequencing_metrics: Store,
     hiseq_x_dual_index_flow_cell_id: str,
-    expected_total_reads_flow_cell_bcl2fastq: int,
+    expected_total_reads_hiseq_x_flow_cell: int,
 ):
     # GIVEN a store with sequencing metrics
     # WHEN getting total read counts for a flow cell
     reads = store_with_sequencing_metrics.get_number_of_reads_for_flow_cell(
         flow_cell_name=hiseq_x_dual_index_flow_cell_id
     )
     # THEN assert that the total read count is correct
-    assert reads == expected_total_reads_flow_cell_bcl2fastq
+    assert reads == expected_total_reads_hiseq_x_flow_cell
 
 
 def test_get_average_bases_above_q30_for_sample_from_metrics(
     store_with_sequencing_metrics: Store,
     expected_average_q30_for_sample: float,
     mother_sample_id: str,
     hiseq_x_dual_index_flow_cell_id: str,
```

### Comparing `cg-60.4.1/tests/store/crud/read/test_read_analyses_to_clean.py` & `cg-60.4.2/tests/store/crud/read/test_read_analyses_to_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/crud/read/test_read_analyses_to_delivery_report.py` & `cg-60.4.2/tests/store/crud/read/test_read_analyses_to_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/crud/read/test_read_analysis.py` & `cg-60.4.2/tests/store/crud/read/test_read_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/crud/read/test_read_application_version.py` & `cg-60.4.2/tests/store/crud/read/test_read_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/crud/read/test_read_customer.py` & `cg-60.4.2/tests/store/crud/read/test_read_customer.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/crud/read/test_read_pool.py` & `cg-60.4.2/tests/store/crud/read/test_read_pool.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/crud/read/test_read_sample.py` & `cg-60.4.2/tests/store/crud/read/test_read_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/crud/update/test_update.py` & `cg-60.4.2/tests/store/crud/update/test_update.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/filters/test_status_analyses_filters.py` & `cg-60.4.2/tests/store/filters/test_status_analyses_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/filters/test_status_application_filters.py` & `cg-60.4.2/tests/store/filters/test_status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/filters/test_status_application_limitations_filters.py` & `cg-60.4.2/tests/store/filters/test_status_application_limitations_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/filters/test_status_application_version_filters.py` & `cg-60.4.2/tests/store/filters/test_status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/filters/test_status_bed_filters.py` & `cg-60.4.2/tests/store/filters/test_status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/filters/test_status_bed_version_filters.py` & `cg-60.4.2/tests/store/filters/test_status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/filters/test_status_case_sample_filters.py` & `cg-60.4.2/tests/store/filters/test_status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/filters/test_status_cases_filters.py` & `cg-60.4.2/tests/store/filters/test_status_cases_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/filters/test_status_collaboration_filters.py` & `cg-60.4.2/tests/store/filters/test_status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/filters/test_status_customer_filters.py` & `cg-60.4.2/tests/store/filters/test_status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/filters/test_status_flow_cell_filters.py` & `cg-60.4.2/tests/store/filters/test_status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/filters/test_status_invoice_filters.py` & `cg-60.4.2/tests/store/filters/test_status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/filters/test_status_metrics_filters.py` & `cg-60.4.2/tests/store/filters/test_status_metrics_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/filters/test_status_organism_filters.py` & `cg-60.4.2/tests/store/filters/test_status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/filters/test_status_panel_filters.py` & `cg-60.4.2/tests/store/filters/test_status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/filters/test_status_pool_filters.py` & `cg-60.4.2/tests/store/filters/test_status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/filters/test_status_samples_filters.py` & `cg-60.4.2/tests/store/filters/test_status_samples_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/filters/test_status_user_filters.py` & `cg-60.4.2/tests/store/filters/test_status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/test_delivery.py` & `cg-60.4.2/tests/store/test_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store/test_store_models.py` & `cg-60.4.2/tests/store/test_store_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/store_helpers.py` & `cg-60.4.2/tests/store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/test_copy_novaseqx_flow_cell.py` & `cg-60.4.2/tests/test_copy_novaseqx_flow_cell.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,85 +1,85 @@
 from pathlib import Path
 
 from cg.cli.demultiplex.copy_novaseqx_demultiplex_data import get_latest_analysis_path
-from cg.cli.demultiplex.demux import (
-    hardlink_flow_cell_analysis_data,
-    is_ready_for_post_processing,
-)
+from cg.cli.demultiplex.demux import hardlink_flow_cell_analysis_data, is_ready_for_post_processing
 from cg.constants.demultiplexing import DemultiplexingDirsAndFiles
 from cg.utils.files import get_all_files_in_dir
 
 
 def test_flow_cell_is_ready_for_post_processing(
-    novaseqx_flow_cell_dir_with_analysis_data: Path, demultiplexed_runs_flow_cell_directory: Path
+    novaseqx_flow_cell_dir_with_analysis_data: Path,
+    tmp_demultiplexed_runs_flow_cell_directory: Path,
 ):
     # GIVEN a flow cell which is ready for post processing
 
     # WHEN checking if the flow cell is ready for post processing
     is_flow_cell_ready: bool = is_ready_for_post_processing(
-        novaseqx_flow_cell_dir_with_analysis_data, demultiplexed_runs_flow_cell_directory
+        novaseqx_flow_cell_dir_with_analysis_data, tmp_demultiplexed_runs_flow_cell_directory
     )
 
     # THEN the flow cell is ready for post processing
     assert is_flow_cell_ready
 
 
 def test_flow_cell_is_not_ready_for_post_processing_without_analysis(
-    novaseqx_flow_cell_analysis_incomplete: Path, demultiplexed_runs_flow_cell_directory: Path
+    novaseqx_flow_cell_analysis_incomplete: Path, tmp_demultiplexed_runs_flow_cell_directory: Path
 ):
     # GIVEN a flow cell for which analysis is not completed
 
     # WHEN checking if the flow cell is ready for post processing
     is_flow_cell_ready: bool = is_ready_for_post_processing(
-        novaseqx_flow_cell_analysis_incomplete, demultiplexed_runs_flow_cell_directory
+        novaseqx_flow_cell_analysis_incomplete, tmp_demultiplexed_runs_flow_cell_directory
     )
 
     # THEN the flow cell is not ready for post processing
     assert not is_flow_cell_ready
 
 
 def test_flow_cell_is_not_ready_for_post_processing_when_not_demultiplexed(
-    demultiplex_not_complete_novaseqx_flow_cell: Path, demultiplexed_runs_flow_cell_directory: Path
+    demultiplex_not_complete_novaseqx_flow_cell: Path,
+    tmp_demultiplexed_runs_flow_cell_directory: Path,
 ):
     # GIVEN a flow cell for which demultiplexing is not completed
 
     # WHEN checking if the flow cell is ready for post processing
     is_flow_cell_ready: bool = is_ready_for_post_processing(
-        demultiplex_not_complete_novaseqx_flow_cell, demultiplexed_runs_flow_cell_directory
+        demultiplex_not_complete_novaseqx_flow_cell, tmp_demultiplexed_runs_flow_cell_directory
     )
 
     # THEN the flow cell is not ready for post processing
     assert not is_flow_cell_ready
 
 
 def test_flow_cell_is_not_ready_when_already_post_processed(
-    post_processed_novaseqx_flow_cell: Path, demultiplexed_runs_flow_cell_directory: Path
+    post_processed_novaseqx_flow_cell: Path, tmp_demultiplexed_runs_flow_cell_directory: Path
 ):
     # GIVEN a flow cell for which post processing is done
 
     # WHEN checking if the flow cell is ready for post processing
     is_flow_cell_ready: bool = is_ready_for_post_processing(
-        post_processed_novaseqx_flow_cell, demultiplexed_runs_flow_cell_directory
+        post_processed_novaseqx_flow_cell, tmp_demultiplexed_runs_flow_cell_directory
     )
 
     # THEN the flow cell is not ready for post processing as the the flow cell has already been post processed
     assert not is_flow_cell_ready
 
 
 def test_previously_copied_flow_cell_is_not_ready(
-    novaseqx_flow_cell_dir_with_analysis_data: Path, demultiplexed_runs_flow_cell_directory: Path
+    novaseqx_flow_cell_dir_with_analysis_data: Path,
+    tmp_demultiplexed_runs_flow_cell_directory: Path,
 ):
     # GIVEN a flow cell which already exists in demultiplexed runs
     Path(
-        demultiplexed_runs_flow_cell_directory, novaseqx_flow_cell_dir_with_analysis_data.name
+        tmp_demultiplexed_runs_flow_cell_directory, novaseqx_flow_cell_dir_with_analysis_data.name
     ).mkdir()
 
     # WHEN checking if the flow cell is ready for post processing
     is_flow_cell_ready: bool = is_ready_for_post_processing(
-        novaseqx_flow_cell_dir_with_analysis_data, demultiplexed_runs_flow_cell_directory
+        novaseqx_flow_cell_dir_with_analysis_data, tmp_demultiplexed_runs_flow_cell_directory
     )
 
     # THEN the flow cell is not ready for post processing
     assert not is_flow_cell_ready
 
 
 def test_get_latest_analysis_version_path(
@@ -97,25 +97,25 @@
         DemultiplexingDirsAndFiles.ANALYSIS,
         novaseqx_latest_analysis_version,
     )
     assert analysis_path == latest_analysis_path
 
 
 def test_copy_novaseqx_flow_cell(
-    demultiplexed_runs_flow_cell_directory: Path,
+    tmp_demultiplexed_runs_flow_cell_directory: Path,
     novaseqx_flow_cell_dir_with_analysis_data: Path,
     novaseq_x_flow_cell_full_name: str,
 ):
     # GIVEN a demultiplexed runs directory for a NovaseqX flow cell
     demultiplexed_runs_novaseqx_dir: Path = Path(
-        demultiplexed_runs_flow_cell_directory, novaseq_x_flow_cell_full_name
+        tmp_demultiplexed_runs_flow_cell_directory, novaseq_x_flow_cell_full_name
     )
     # WHEN copying the flow cell analysis data to demultiplexed runs NovaseqX directory
     hardlink_flow_cell_analysis_data(
-        novaseqx_flow_cell_dir_with_analysis_data, demultiplexed_runs_flow_cell_directory
+        novaseqx_flow_cell_dir_with_analysis_data, tmp_demultiplexed_runs_flow_cell_directory
     )
 
     # THEN the data contains everything from the analysis folder
     analysis: Path = get_latest_analysis_path(novaseqx_flow_cell_dir_with_analysis_data)
     analysis_data_path: Path = Path(analysis / DemultiplexingDirsAndFiles.DATA)
 
     original_files = get_all_files_in_dir(analysis_data_path)
```

### Comparing `cg-60.4.1/tests/test_store_helpers.py` & `cg-60.4.2/tests/test_store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/utils/conftest.py` & `cg-60.4.2/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/utils/test_commands.py` & `cg-60.4.2/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/utils/test_date.py` & `cg-60.4.2/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/utils/test_dict.py` & `cg-60.4.2/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/utils/test_dispatcher.py` & `cg-60.4.2/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/utils/test_files.py` & `cg-60.4.2/tests/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/utils/test_time.py` & `cg-60.4.2/tests/utils/test_time.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/tests/utils/test_utils.py` & `cg-60.4.2/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.1/PKG-INFO` & `cg-60.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 60.4.1
+Version: 60.4.2
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

