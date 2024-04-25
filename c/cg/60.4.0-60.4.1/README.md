# Comparing `tmp/cg-60.4.0.tar.gz` & `tmp/cg-60.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cg-60.4.0.tar", max compression
+gzip compressed data, was "cg-60.4.1.tar", max compression
```

## Comparing `cg-60.4.0.tar` & `cg-60.4.1.tar`

### file list

```diff
@@ -1,1361 +1,1361 @@
--rw-r--r--   0        0        0     2686 2024-04-25 07:25:49.687614 cg-60.4.0/README.md
--rw-r--r--   0        0        0       40 2024-04-25 07:25:49.691614 cg-60.4.0/cg/__init__.py
--rw-r--r--   0        0        0      315 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/__init__.py
--rw-r--r--   0        0        0       27 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/coverage/__init__.py
--rw-r--r--   0        0        0     2940 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/coverage/api.py
--rw-r--r--   0        0        0       56 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/crunchy/__init__.py
--rw-r--r--   0        0        0    12783 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/crunchy/crunchy.py
--rw-r--r--   0        0        0     4502 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/crunchy/files.py
--rw-r--r--   0        0        0      430 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/crunchy/models.py
--rw-r--r--   0        0        0      910 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/crunchy/sbatch.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/demultiplex/__init__.py
--rw-r--r--   0        0        0    11299 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/demultiplex/demultiplex_api.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/demultiplex/sample_sheet/__init__.py
--rw-r--r--   0        0        0    11227 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/demultiplex/sample_sheet/api.py
--rw-r--r--   0        0        0     2183 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/demultiplex/sample_sheet/index.py
--rw-r--r--   0        0        0     7341 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py
--rw-r--r--   0        0        0     3188 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py
--rw-r--r--   0        0        0     7071 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/demultiplex/sample_sheet/sample_models.py
--rw-r--r--   0        0        0     6076 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py
--rw-r--r--   0        0        0     1372 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py
--rw-r--r--   0        0        0     8092 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py
--rw-r--r--   0        0        0      824 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/demultiplex/sample_sheet/validators.py
--rw-r--r--   0        0        0      677 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/demultiplex/sbatch.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/downsample/__init__.py
--rw-r--r--   0        0        0     6160 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/downsample/downsample.py
--rw-r--r--   0        0        0     2125 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/downsample/utils.py
--rw-r--r--   0        0        0      298 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/environ.py
--rw-r--r--   0        0        0     1741 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/gens.py
--rw-r--r--   0        0        0     3419 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/gt.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/hermes/__init__.py
--rw-r--r--   0        0        0     2249 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/hermes/hermes_api.py
--rw-r--r--   0        0        0     1298 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/hermes/models.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/housekeeper/__init__.py
--rw-r--r--   0        0        0    30395 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/housekeeper/hk.py
--rw-r--r--   0        0        0      326 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/housekeeper/models.py
--rw-r--r--   0        0        0       32 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/invoice/__init__.py
--rw-r--r--   0        0        0     4804 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/invoice/render.py
--rw-r--r--   0        0        0   113467 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/invoice/templates/KI_pool_invoice.xlsx
--rw-r--r--   0        0        0    75562 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/invoice/templates/KI_sample_invoice.xlsx
--rw-r--r--   0        0        0   113512 2024-04-25 07:25:49.691614 cg-60.4.0/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
--rw-r--r--   0        0        0    75459 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
--rw-r--r--   0        0        0       25 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/lims/__init__.py
--rw-r--r--   0        0        0    18546 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/lims/api.py
--rw-r--r--   0        0        0     2652 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/lims/batch.py
--rw-r--r--   0        0        0     8129 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/lims/order.py
--rw-r--r--   0        0        0     3118 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/lims/sample_sheet.py
--rw-r--r--   0        0        0     4866 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/loqus.py
--rw-r--r--   0        0        0       35 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/madeline/__init__.py
--rw-r--r--   0        0        0     3213 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/madeline/api.py
--rw-r--r--   0        0        0       23 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/mip/__init__.py
--rw-r--r--   0        0        0     3564 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/mip/confighandler.py
--rw-r--r--   0        0        0     2207 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/mutacc_auto.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/orderform/__init__.py
--rw-r--r--   0        0        0     9498 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/orderform/excel_orderform_parser.py
--rw-r--r--   0        0        0     3051 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/orderform/json_orderform_parser.py
--rw-r--r--   0        0        0     6419 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/orderform/orderform_parser.py
--rw-r--r--   0        0        0      252 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/orderform/utils.py
--rw-r--r--   0        0        0     2537 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/osticket.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/scout/__init__.py
--rw-r--r--   0        0        0     3177 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/scout/scout_export.py
--rw-r--r--   0        0        0    11054 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/scout/scoutapi.py
--rw-r--r--   0        0        0      444 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/scout/validators.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0        0        0     3457 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/sequencing_metrics_parser/api.py
--rw-r--r--   0        0        0      923 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/sequencing_metrics_parser/models.py
--rw-r--r--   0        0        0     6658 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/sequencing_metrics_parser/parser.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/slurm/__init__.py
--rw-r--r--   0        0        0     1277 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/slurm/sbatch.py
--rw-r--r--   0        0        0     3559 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/slurm/slurm_api.py
--rw-r--r--   0        0        0       32 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/tb/__init__.py
--rw-r--r--   0        0        0     7995 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/tb/api.py
--rw-r--r--   0        0        0      152 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/tb/dto/create_job_request.py
--rw-r--r--   0        0        0      250 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/tb/dto/summary_response.py
--rw-r--r--   0        0        0     1305 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/tb/models.py
--rw-r--r--   0        0        0      305 2024-04-25 07:25:49.695614 cg-60.4.0/cg/apps/tb/validators.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/__init__.py
--rw-r--r--   0        0        0    11558 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/add.py
--rw-r--r--   0        0        0     2653 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/archive.py
--rw-r--r--   0        0        0    10118 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/backup.py
--rw-r--r--   0        0        0     3852 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/base.py
--rw-r--r--   0        0        0    10506 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/clean.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/compress/__init__.py
--rw-r--r--   0        0        0     2135 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/compress/base.py
--rw-r--r--   0        0        0     6706 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/compress/fastq.py
--rw-r--r--   0        0        0     8163 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/compress/helpers.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/delete/__init__.py
--rw-r--r--   0        0        0      564 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/delete/base.py
--rw-r--r--   0        0        0     4603 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/delete/case.py
--rw-r--r--   0        0        0     1884 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/delete/cases.py
--rw-r--r--   0        0        0     2633 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/delete/observations.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/deliver/__init__.py
--rw-r--r--   0        0        0     6030 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/deliver/base.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/demultiplex/__init__.py
--rw-r--r--   0        0        0      829 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/demultiplex/base.py
--rw-r--r--   0        0        0     4905 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py
--rw-r--r--   0        0        0     7726 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/demultiplex/demux.py
--rw-r--r--   0        0        0     1473 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/demultiplex/finish.py
--rw-r--r--   0        0        0     3119 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/demultiplex/sample_sheet.py
--rw-r--r--   0        0        0     2995 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/downsample.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/generate/__init__.py
--rw-r--r--   0        0        0      356 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/generate/base.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/generate/report/__init__.py
--rw-r--r--   0        0        0     4636 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/generate/report/base.py
--rw-r--r--   0        0        0      854 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/generate/report/options.py
--rw-r--r--   0        0        0     5340 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/generate/report/utils.py
--rw-r--r--   0        0        0     8327 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/get.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/set/__init__.py
--rw-r--r--   0        0        0     9856 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/set/base.py
--rw-r--r--   0        0        0     4384 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/set/case.py
--rw-r--r--   0        0        0     2595 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/set/cases.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/store/__init__.py
--rw-r--r--   0        0        0     1093 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/store/base.py
--rw-r--r--   0        0        0     6191 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/store/store.py
--rw-r--r--   0        0        0     1761 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/transfer.py
--rw-r--r--   0        0        0        1 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/upload/__init__.py
--rw-r--r--   0        0        0     5706 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/upload/base.py
--rw-r--r--   0        0        0     5503 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/upload/clinical_delivery.py
--rw-r--r--   0        0        0     1175 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/upload/coverage.py
--rw-r--r--   0        0        0     1528 2024-04-25 07:25:49.695614 cg-60.4.0/cg/cli/upload/delivery_report.py
--rw-r--r--   0        0        0     4022 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/upload/fohm.py
--rw-r--r--   0        0        0     1463 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/upload/genotype.py
--rw-r--r--   0        0        0     1885 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/upload/gens.py
--rw-r--r--   0        0        0      584 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/upload/gisaid.py
--rw-r--r--   0        0        0     2645 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/upload/mutacc.py
--rw-r--r--   0        0        0       23 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/upload/nipt/__init__.py
--rw-r--r--   0        0        0     3006 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/upload/nipt/base.py
--rw-r--r--   0        0        0     2275 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/upload/nipt/ftp.py
--rw-r--r--   0        0        0     1596 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/upload/nipt/statina.py
--rw-r--r--   0        0        0      112 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/upload/observations/__init__.py
--rw-r--r--   0        0        0     2672 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/upload/observations/observations.py
--rw-r--r--   0        0        0     2904 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/upload/observations/utils.py
--rw-r--r--   0        0        0     9970 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/upload/scout.py
--rw-r--r--   0        0        0      650 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/upload/utils.py
--rw-r--r--   0        0        0     1667 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/upload/validate.py
--rw-r--r--   0        0        0      105 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/utils.py
--rw-r--r--   0        0        0       18 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/__init__.py
--rw-r--r--   0        0        0       22 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/balsamic/__init__.py
--rw-r--r--   0        0        0     8925 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/balsamic/base.py
--rw-r--r--   0        0        0     1980 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/balsamic/options.py
--rw-r--r--   0        0        0      881 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/balsamic/pon.py
--rw-r--r--   0        0        0     1162 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/balsamic/qc.py
--rw-r--r--   0        0        0     1177 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/balsamic/umi.py
--rw-r--r--   0        0        0     1342 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/base.py
--rw-r--r--   0        0        0    12379 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/commands.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/fastq/__init__.py
--rw-r--r--   0        0        0     1490 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/fastq/base.py
--rw-r--r--   0        0        0     1787 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/fastq/fastq_service.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/fluffy/__init__.py
--rw-r--r--   0        0        0     4177 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/fluffy/base.py
--rw-r--r--   0        0        0       22 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/jasen/__init__.py
--rw-r--r--   0        0        0      535 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/jasen/base.py
--rw-r--r--   0        0        0       22 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/microsalt/__init__.py
--rw-r--r--   0        0        0     7810 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/microsalt/base.py
--rw-r--r--   0        0        0       22 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/mip/__init__.py
--rw-r--r--   0        0        0     6596 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/mip/base.py
--rw-r--r--   0        0        0     1268 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/mip/options.py
--rw-r--r--   0        0        0       22 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/mip_dna/__init__.py
--rw-r--r--   0        0        0     1013 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/mip_dna/base.py
--rw-r--r--   0        0        0       22 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/mip_rna/__init__.py
--rw-r--r--   0        0        0      916 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/mip_rna/base.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/mutant/__init__.py
--rw-r--r--   0        0        0     3413 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/mutant/base.py
--rw-r--r--   0        0        0     9010 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/nf_analysis.py
--rw-r--r--   0        0        0       22 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/raredisease/__init__.py
--rw-r--r--   0        0        0     2210 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/raredisease/base.py
--rw-r--r--   0        0        0       22 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/rnafusion/__init__.py
--rw-r--r--   0        0        0     1179 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/rnafusion/base.py
--rw-r--r--   0        0        0       22 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/taxprofiler/__init__.py
--rw-r--r--   0        0        0     1211 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/taxprofiler/base.py
--rw-r--r--   0        0        0     1111 2024-04-25 07:25:49.699614 cg-60.4.0/cg/cli/workflow/tomte/base.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.699614 cg-60.4.0/cg/clients/__init__.py
--rw-r--r--   0        0        0     1363 2024-04-25 07:25:49.699614 cg-60.4.0/cg/clients/arnold/api.py
--rw-r--r--   0        0        0      160 2024-04-25 07:25:49.699614 cg-60.4.0/cg/clients/arnold/dto/create_case_request.py
--rw-r--r--   0        0        0      384 2024-04-25 07:25:49.699614 cg-60.4.0/cg/clients/arnold/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.699614 cg-60.4.0/cg/clients/janus/__init__.py
--rw-r--r--   0        0        0     1246 2024-04-25 07:25:49.699614 cg-60.4.0/cg/clients/janus/api.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.699614 cg-60.4.0/cg/clients/janus/dto/__init__.py
--rw-r--r--   0        0        0      503 2024-04-25 07:25:49.699614 cg-60.4.0/cg/clients/janus/dto/create_qc_metrics_request.py
--rw-r--r--   0        0        0      420 2024-04-25 07:25:49.699614 cg-60.4.0/cg/clients/janus/exceptions.py
--rw-r--r--   0        0        0      937 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/__init__.py
--rw-r--r--   0        0        0      253 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/archiving.py
--rw-r--r--   0        0        0       35 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/backup.py
--rw-r--r--   0        0        0      769 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/bcl_convert_metrics.py
--rw-r--r--   0        0        0      469 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/compression.py
--rw-r--r--   0        0        0     6613 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/constants.py
--rw-r--r--   0        0        0     6033 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/delivery.py
--rw-r--r--   0        0        0     7387 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/demultiplexing.py
--rw-r--r--   0        0        0     1422 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/encryption.py
--rw-r--r--   0        0        0      372 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/extraction.py
--rw-r--r--   0        0        0     2054 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/gene_panel.py
--rw-r--r--   0        0        0     6704 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/housekeeper_tags.py
--rw-r--r--   0        0        0       95 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/invoice.py
--rw-r--r--   0        0        0     5815 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/lims.py
--rw-r--r--   0        0        0      743 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/metrics.py
--rw-r--r--   0        0        0      231 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/nanopore_files.py
--rw-r--r--   0        0        0      650 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/nextflow.py
--rw-r--r--   0        0        0     1529 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/nf_analysis.py
--rw-r--r--   0        0        0       19 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/nipt.py
--rw-r--r--   0        0        0     2257 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/observations.py
--rw-r--r--   0        0        0     1216 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/orderforms.py
--rw-r--r--   0        0        0       96 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/paths.py
--rw-r--r--   0        0        0      266 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/pdc.py
--rw-r--r--   0        0        0      160 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/pedigree.py
--rw-r--r--   0        0        0     1044 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/priority.py
--rw-r--r--   0        0        0       79 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/process.py
--rw-r--r--   0        0        0     5474 2024-04-25 07:25:49.699614 cg-60.4.0/cg/constants/report.py
--rw-r--r--   0        0        0      485 2024-04-25 07:25:49.703614 cg-60.4.0/cg/constants/sample_sources.py
--rw-r--r--   0        0        0     3111 2024-04-25 07:25:49.703614 cg-60.4.0/cg/constants/scout.py
--rw-r--r--   0        0        0     1669 2024-04-25 07:25:49.703614 cg-60.4.0/cg/constants/sequencing.py
--rw-r--r--   0        0        0      313 2024-04-25 07:25:49.703614 cg-60.4.0/cg/constants/slurm.py
--rw-r--r--   0        0        0      529 2024-04-25 07:25:49.703614 cg-60.4.0/cg/constants/subject.py
--rw-r--r--   0        0        0       55 2024-04-25 07:25:49.703614 cg-60.4.0/cg/constants/symbols.py
--rw-r--r--   0        0        0      435 2024-04-25 07:25:49.703614 cg-60.4.0/cg/constants/tb.py
--rw-r--r--   0        0        0      161 2024-04-25 07:25:49.703614 cg-60.4.0/cg/constants/time.py
--rw-r--r--   0        0        0     6639 2024-04-25 07:25:49.703614 cg-60.4.0/cg/exc.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.703614 cg-60.4.0/cg/io/__init__.py
--rw-r--r--   0        0        0     1037 2024-04-25 07:25:49.703614 cg-60.4.0/cg/io/api.py
--rw-r--r--   0        0        0      621 2024-04-25 07:25:49.703614 cg-60.4.0/cg/io/config.py
--rw-r--r--   0        0        0     2978 2024-04-25 07:25:49.703614 cg-60.4.0/cg/io/controller.py
--rw-r--r--   0        0        0     1763 2024-04-25 07:25:49.703614 cg-60.4.0/cg/io/csv.py
--rw-r--r--   0        0        0      210 2024-04-25 07:25:49.703614 cg-60.4.0/cg/io/gzip.py
--rw-r--r--   0        0        0      662 2024-04-25 07:25:49.703614 cg-60.4.0/cg/io/json.py
--rw-r--r--   0        0        0      525 2024-04-25 07:25:49.703614 cg-60.4.0/cg/io/png.py
--rw-r--r--   0        0        0     1094 2024-04-25 07:25:49.703614 cg-60.4.0/cg/io/txt.py
--rw-r--r--   0        0        0      552 2024-04-25 07:25:49.703614 cg-60.4.0/cg/io/validate_path.py
--rw-r--r--   0        0        0     1289 2024-04-25 07:25:49.703614 cg-60.4.0/cg/io/xml.py
--rw-r--r--   0        0        0     1153 2024-04-25 07:25:49.703614 cg-60.4.0/cg/io/yaml.py
--rw-r--r--   0        0        0      281 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/archive/__init__.py
--rw-r--r--   0        0        0    15193 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/archive/archive.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/archive/ddn/__init__.py
--rw-r--r--   0        0        0     1727 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/archive/ddn/constants.py
--rw-r--r--   0        0        0    10852 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/archive/ddn/ddn_data_flow_client.py
--rw-r--r--   0        0        0     3704 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/archive/ddn/models.py
--rw-r--r--   0        0        0     1250 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/archive/ddn/utils.py
--rw-r--r--   0        0        0     2024 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/archive/models.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/backup/__init__.py
--rw-r--r--   0        0        0    17426 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/backup/backup.py
--rw-r--r--   0        0        0     5397 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/backup/pdc.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/clean/__init__.py
--rw-r--r--   0        0        0     3901 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/clean/api.py
--rw-r--r--   0        0        0     7738 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/clean/clean_flow_cells.py
--rw-r--r--   0        0        0     1841 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/clean/clean_retrieved_spring_files.py
--rw-r--r--   0        0        0       34 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/compress/__init__.py
--rw-r--r--   0        0        0    14557 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/compress/compress.py
--rw-r--r--   0        0        0     4947 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/compress/files.py
--rw-r--r--   0        0        0       77 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/deliver/__init__.py
--rw-r--r--   0        0        0    14905 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/deliver/deliver.py
--rw-r--r--   0        0        0     4502 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/deliver/deliver_ticket.py
--rw-r--r--   0        0        0      904 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/deliver/fastq_path_generator.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/delivery/__init__.py
--rw-r--r--   0        0        0     8458 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/delivery/delivery.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/demultiplex/__init__.py
--rw-r--r--   0        0        0     2592 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/demultiplex/combine_sequencing_metrics.py
--rw-r--r--   0        0        0     5719 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/demultiplex/demux_post_processing.py
--rw-r--r--   0        0        0     4135 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/demultiplex/files.py
--rw-r--r--   0        0        0     7777 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/demultiplex/housekeeper_storage_functions.py
--rw-r--r--   0        0        0     6126 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/demultiplex/status_db_storage_functions.py
--rw-r--r--   0        0        0    10690 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/demultiplex/utils.py
--rw-r--r--   0        0        0     2855 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/demultiplex/validation.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/encryption/__init__.py
--rw-r--r--   0        0        0    20271 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/encryption/encryption.py
--rw-r--r--   0        0        0      537 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/encryption/sbatch.py
--rw-r--r--   0        0        0    10922 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/invoice.py
--rw-r--r--   0        0        0     2360 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/meta.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/observations/__init__.py
--rw-r--r--   0        0        0     6008 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/observations/balsamic_observations_api.py
--rw-r--r--   0        0        0     5277 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/observations/mip_dna_observations_api.py
--rw-r--r--   0        0        0     5364 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/observations/observations_api.py
--rw-r--r--   0        0        0       27 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/orders/__init__.py
--rw-r--r--   0        0        0     3637 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/orders/api.py
--rw-r--r--   0        0        0      121 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/orders/balsamic_qc_submitter.py
--rw-r--r--   0        0        0      107 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/orders/balsamic_submitter.py
--rw-r--r--   0        0        0      122 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/orders/balsamic_umi_submitter.py
--rw-r--r--   0        0        0    15262 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/orders/case_submitter.py
--rw-r--r--   0        0        0     6102 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/orders/fastq_submitter.py
--rw-r--r--   0        0        0      105 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/orders/fluffy_submitter.py
--rw-r--r--   0        0        0     1254 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/orders/lims.py
--rw-r--r--   0        0        0     5782 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/orders/metagenome_submitter.py
--rw-r--r--   0        0        0     6337 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/orders/microbial_submitter.py
--rw-r--r--   0        0        0      123 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/orders/microsalt_submitter.py
--rw-r--r--   0        0        0      105 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/orders/mip_dna_submitter.py
--rw-r--r--   0        0        0      105 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/orders/mip_rna_submitter.py
--rw-r--r--   0        0        0     7761 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/orders/pool_submitter.py
--rw-r--r--   0        0        0      102 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/orders/rml_submitter.py
--rw-r--r--   0        0        0      718 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/orders/rnafusion_submitter.py
--rw-r--r--   0        0        0     1268 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/orders/sars_cov_2_submitter.py
--rw-r--r--   0        0        0     1754 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/orders/submitter.py
--rw-r--r--   0        0        0     7880 2024-04-25 07:25:49.703614 cg-60.4.0/cg/meta/orders/ticket_handler.py
--rw-r--r--   0        0        0     4105 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/qc_metrics/collect_qc_metrics.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/__init__.py
--rw-r--r--   0        0        0     8168 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/balsamic.py
--rw-r--r--   0        0        0      562 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/balsamic_qc.py
--rw-r--r--   0        0        0      717 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/balsamic_umi.py
--rw-r--r--   0        0        0     4171 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/field_validators.py
--rw-r--r--   0        0        0     6620 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/mip_dna.py
--rw-r--r--   0        0        0    18606 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/report_api.py
--rw-r--r--   0        0        0     5625 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/rnafusion.py
--rw-r--r--   0        0        0     1911 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/templates/delivery-report.html
--rw-r--r--   0        0        0     4236 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/templates/macros/data_analysis/data_analysis.html
--rw-r--r--   0        0        0     1049 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/templates/macros/data_analysis/limitations.html
--rw-r--r--   0        0        0     3351 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html
--rw-r--r--   0        0        0     1364 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html
--rw-r--r--   0        0        0      753 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html
--rw-r--r--   0        0        0     3284 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html
--rw-r--r--   0        0        0     3670 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html
--rw-r--r--   0        0        0     2332 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/templates/macros/header.html
--rw-r--r--   0        0        0     2066 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/templates/macros/order.html
--rw-r--r--   0        0        0     2243 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/templates/macros/sample_prep.html
--rw-r--r--   0        0        0      472 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/templates/macros/ticket_system.html
--rw-r--r--   0        0        0     1165 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html
--rw-r--r--   0        0        0     1538 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html
--rw-r--r--   0        0        0      428 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/templates/macros/uploaded_files/rnafusion_uploaded_files.html
--rw-r--r--   0        0        0     4266 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html
--rw-r--r--   0        0        0       80 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/templates/partials/footer.html
--rw-r--r--   0        0        0      172 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/templates/partials/signature.html
--rw-r--r--   0        0        0   232803 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/templates/static/css/bootstrap.min.css
--rw-r--r--   0        0        0       33 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/templates/static/css/custom.css
--rw-r--r--   0        0        0    30068 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/templates/static/images/SWEDAC_logo.png
--rw-r--r--   0        0        0     3925 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/report/tomte.py
--rw-r--r--   0        0        0       32 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/rsync/__init__.py
--rw-r--r--   0        0        0    12291 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/rsync/rsync_api.py
--rw-r--r--   0        0        0      387 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/rsync/sbatch.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/tar/__init__.py
--rw-r--r--   0        0        0     1694 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/tar/tar.py
--rw-r--r--   0        0        0       71 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/transfer/__init__.py
--rw-r--r--   0        0        0    10016 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/transfer/external_data.py
--rw-r--r--   0        0        0     5814 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/transfer/lims.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/upload/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/upload/balsamic/__init__.py
--rw-r--r--   0        0        0     3107 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/upload/balsamic/balsamic.py
--rw-r--r--   0        0        0     2224 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/upload/coverage.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/upload/fohm/__init__.py
--rw-r--r--   0        0        0    12102 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/upload/fohm/fohm.py
--rw-r--r--   0        0        0       30 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/upload/gisaid/__init__.py
--rw-r--r--   0        0        0      928 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/upload/gisaid/constants.py
--rw-r--r--   0        0        0    13521 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/upload/gisaid/gisaid.py
--rw-r--r--   0        0        0     3312 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/upload/gisaid/models.py
--rw-r--r--   0        0        0     5310 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/upload/gt.py
--rw-r--r--   0        0        0      898 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/upload/microsalt/microsalt_upload_api.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/upload/mip/__init__.py
--rw-r--r--   0        0        0     2546 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/upload/mip/mip_dna.py
--rw-r--r--   0        0        0     1400 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/upload/mip/mip_rna.py
--rw-r--r--   0        0        0     7294 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/upload/mutacc.py
--rw-r--r--   0        0        0     1853 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/upload/nf_analysis.py
--rw-r--r--   0        0        0       32 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/upload/nipt/__init__.py
--rw-r--r--   0        0        0      696 2024-04-25 07:25:49.707614 cg-60.4.0/cg/meta/upload/nipt/models.py
--rw-r--r--   0        0        0     8106 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/upload/nipt/nipt.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/upload/scout/__init__.py
--rw-r--r--   0        0        0     4009 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/upload/scout/balsamic_config_builder.py
--rw-r--r--   0        0        0     1491 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/upload/scout/balsamic_umi_config_builder.py
--rw-r--r--   0        0        0     3322 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/upload/scout/hk_tags.py
--rw-r--r--   0        0        0     9103 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/upload/scout/mip_config_builder.py
--rw-r--r--   0        0        0     3495 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/upload/scout/rnafusion_config_builder.py
--rw-r--r--   0        0        0     7231 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/upload/scout/scout_config_builder.py
--rw-r--r--   0        0        0    23146 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/upload/scout/uploadscoutapi.py
--rw-r--r--   0        0        0     3197 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/upload/upload_api.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/__init__.py
--rw-r--r--   0        0        0    29231 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/analysis.py
--rw-r--r--   0        0        0    27751 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/balsamic.py
--rw-r--r--   0        0        0     2700 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/balsamic_pon.py
--rw-r--r--   0        0        0      553 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/balsamic_qc.py
--rw-r--r--   0        0        0      556 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/balsamic_umi.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/downsample/__init__.py
--rw-r--r--   0        0        0     3922 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/downsample/downsample.py
--rw-r--r--   0        0        0      711 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/downsample/sbatch.py
--rw-r--r--   0        0        0     8913 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/fastq.py
--rw-r--r--   0        0        0    10603 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/fluffy.py
--rw-r--r--   0        0        0      521 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/jasen.py
--rw-r--r--   0        0        0       70 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/microsalt/__init__.py
--rw-r--r--   0        0        0      116 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/microsalt/constants.py
--rw-r--r--   0        0        0      174 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/microsalt/metrics_parser/__init__.py
--rw-r--r--   0        0        0      366 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/microsalt/metrics_parser/metrics_parser.py
--rw-r--r--   0        0        0      903 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/microsalt/metrics_parser/models.py
--rw-r--r--   0        0        0    13173 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/microsalt/microsalt.py
--rw-r--r--   0        0        0      113 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/microsalt/quality_controller/__init__.py
--rw-r--r--   0        0        0      712 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/microsalt/quality_controller/models.py
--rw-r--r--   0        0        0     5697 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/microsalt/quality_controller/quality_controller.py
--rw-r--r--   0        0        0     1217 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/microsalt/quality_controller/report_generator.py
--rw-r--r--   0        0        0     2373 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/microsalt/quality_controller/result_logger.py
--rw-r--r--   0        0        0     5641 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/microsalt/quality_controller/utils.py
--rw-r--r--   0        0        0     1220 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/microsalt/utils.py
--rw-r--r--   0        0        0    13587 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/mip.py
--rw-r--r--   0        0        0     2908 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/mip_dna.py
--rw-r--r--   0        0        0     2084 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/mip_rna.py
--rw-r--r--   0        0        0    10974 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/mutant.py
--rw-r--r--   0        0        0    35481 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/nf_analysis.py
--rw-r--r--   0        0        0     6161 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/nf_handlers.py
--rw-r--r--   0        0        0     6357 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/prepare_fastq.py
--rw-r--r--   0        0        0     5988 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/raredisease.py
--rw-r--r--   0        0        0     5214 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/rnafusion.py
--rw-r--r--   0        0        0     4607 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/taxprofiler.py
--rw-r--r--   0        0        0     3204 2024-04-25 07:25:49.711614 cg-60.4.0/cg/meta/workflow/tomte.py
--rw-r--r--   0        0        0      113 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/__init__.py
--rw-r--r--   0        0        0      367 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/analysis.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/balsamic/__init__.py
--rw-r--r--   0        0        0      459 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/balsamic/analysis.py
--rw-r--r--   0        0        0     4550 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/balsamic/config.py
--rw-r--r--   0        0        0     1986 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/balsamic/metrics.py
--rw-r--r--   0        0        0    17539 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/cg_config.py
--rw-r--r--   0        0        0     4302 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/compression_data.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/deliverables/__init__.py
--rw-r--r--   0        0        0     5213 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/deliverables/metric_deliverables.py
--rw-r--r--   0        0        0      243 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/delivery/delivery.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/demultiplex/__init__.py
--rw-r--r--   0        0        0    12040 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/demultiplex/run_parameters.py
--rw-r--r--   0        0        0      539 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/demultiplex/sbatch.py
--rw-r--r--   0        0        0     7006 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/downsample/downsample_data.py
--rw-r--r--   0        0        0      255 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/email.py
--rw-r--r--   0        0        0     1046 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/fastq.py
--rw-r--r--   0        0        0     2157 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/file_data.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/flow_cell/__init__.py
--rw-r--r--   0        0        0     9984 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/flow_cell/flow_cell.py
--rw-r--r--   0        0        0      317 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/flow_cell/utils.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/invoice/__init__.py
--rw-r--r--   0        0        0     1254 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/invoice/invoice.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/lims/__init__.py
--rw-r--r--   0        0        0     2019 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/lims/sample.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/mip/__init__.py
--rw-r--r--   0        0        0      337 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/mip/mip_analysis.py
--rw-r--r--   0        0        0     1564 2024-04-25 07:25:49.711614 cg-60.4.0/cg/models/mip/mip_config.py
--rw-r--r--   0        0        0     4696 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/mip/mip_metrics_deliverables.py
--rw-r--r--   0        0        0     2550 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/mip/mip_sample_info.py
--rw-r--r--   0        0        0     2472 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/nf_analysis.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/observations/__init__.py
--rw-r--r--   0        0        0      688 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/observations/input_files.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/orders/__init__.py
--rw-r--r--   0        0        0     2659 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/orders/constants.py
--rw-r--r--   0        0        0     5604 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/orders/excel_sample.py
--rw-r--r--   0        0        0      898 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/orders/json_sample.py
--rw-r--r--   0        0        0     1449 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/orders/order.py
--rw-r--r--   0        0        0      811 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/orders/orderform_schema.py
--rw-r--r--   0        0        0     4212 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/orders/sample_base.py
--rw-r--r--   0        0        0     9668 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/orders/samples.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/orders/validators/__init__.py
--rw-r--r--   0        0        0     2300 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/orders/validators/excel_sample_validators.py
--rw-r--r--   0        0        0      576 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/orders/validators/json_sample_validators.py
--rw-r--r--   0        0        0       71 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/orders/validators/sample_base_validators.py
--rw-r--r--   0        0        0      101 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/qc_metrics.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/raredisease/__init__.py
--rw-r--r--   0        0        0     1875 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/raredisease/raredisease.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/report/__init__.py
--rw-r--r--   0        0        0     7461 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/report/metadata.py
--rw-r--r--   0        0        0     6180 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/report/report.py
--rw-r--r--   0        0        0     5221 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/report/sample.py
--rw-r--r--   0        0        0     3004 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/report/validators.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/rnafusion/__init__.py
--rw-r--r--   0        0        0     1865 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/rnafusion/rnafusion.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/scout/__init__.py
--rw-r--r--   0        0        0     4783 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/scout/scout_load_config.py
--rw-r--r--   0        0        0      116 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/scout/validators.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/slurm/__init__.py
--rw-r--r--   0        0        0      617 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/slurm/sbatch.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/taxprofiler/__init__.py
--rw-r--r--   0        0        0     2443 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/taxprofiler/taxprofiler.py
--rw-r--r--   0        0        0     1774 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/tomte/tomte.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/workflow/__init__.py
--rw-r--r--   0        0        0      685 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/workflow/mutant.py
--rw-r--r--   0        0        0       70 2024-04-25 07:25:49.715614 cg-60.4.0/cg/models/workflow/validators.py
--rw-r--r--   0        0        0      842 2024-04-25 07:25:49.715614 cg-60.4.0/cg/resources/__init__.py
--rw-r--r--   0        0        0     3493 2024-04-25 07:25:49.715614 cg-60.4.0/cg/resources/rnafusion_bundle_filenames.yaml
--rw-r--r--   0        0        0     2434 2024-04-25 07:25:49.715614 cg-60.4.0/cg/resources/taxprofiler_bundle_filenames.yaml
--rw-r--r--   0        0        0     3732 2024-04-25 07:25:49.715614 cg-60.4.0/cg/resources/tomte_bundle_filenames.yaml
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/__init__.py
--rw-r--r--   0        0        0    20241 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/admin.py
--rw-r--r--   0        0        0    22743 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/api.py
--rw-r--r--   0        0        0     4887 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/app.py
--rw-r--r--   0        0        0       48 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/auto.py
--rw-r--r--   0        0        0     1184 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/config.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/dto/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/dto/delivery_message/__init__.py
--rw-r--r--   0        0        0      300 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/dto/delivery_message/delivery_message_request.py
--rw-r--r--   0        0        0      183 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/dto/delivery_message/delivery_message_response.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/dto/orders/__init__.py
--rw-r--r--   0        0        0      165 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/dto/orders/order_delivery_update_request.py
--rw-r--r--   0        0        0       91 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/dto/orders/order_patch_request.py
--rw-r--r--   0        0        0      662 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/dto/orders/orders_request.py
--rw-r--r--   0        0        0      413 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/dto/orders/orders_response.py
--rw-r--r--   0        0        0     2598 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/ext.py
--rw-r--r--   0        0        0       29 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/invoices/__init__.py
--rw-r--r--   0        0        0     4793 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/invoices/templates/invoices/index.html
--rw-r--r--   0        0        0     8171 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/invoices/templates/invoices/invoice.html
--rw-r--r--   0        0        0     2838 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/invoices/templates/invoices/layout.html
--rw-r--r--   0        0        0     4956 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/invoices/templates/invoices/new.html
--rw-r--r--   0        0        0     7708 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/invoices/views.py
--rw-r--r--   0        0        0      354 2024-04-25 07:25:49.715614 cg-60.4.0/cg/server/templates/admin/index.html
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.715614 cg-60.4.0/cg/services/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.715614 cg-60.4.0/cg/services/analysis_service/__init__.py
--rw-r--r--   0        0        0      482 2024-04-25 07:25:49.715614 cg-60.4.0/cg/services/analysis_service/analysis_service.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.715614 cg-60.4.0/cg/services/delivery_message/__init__.py
--rw-r--r--   0        0        0     2531 2024-04-25 07:25:49.715614 cg-60.4.0/cg/services/delivery_message/delivery_message_service.py
--rw-r--r--   0        0        0      792 2024-04-25 07:25:49.715614 cg-60.4.0/cg/services/delivery_message/messages/__init__.py
--rw-r--r--   0        0        0     1366 2024-04-25 07:25:49.715614 cg-60.4.0/cg/services/delivery_message/messages/analysis_scout_message.py
--rw-r--r--   0        0        0      791 2024-04-25 07:25:49.715614 cg-60.4.0/cg/services/delivery_message/messages/covid_message.py
--rw-r--r--   0        0        0      189 2024-04-25 07:25:49.715614 cg-60.4.0/cg/services/delivery_message/messages/delivery_message.py
--rw-r--r--   0        0        0     1391 2024-04-25 07:25:49.715614 cg-60.4.0/cg/services/delivery_message/messages/fastq_analysis_scout_message.py
--rw-r--r--   0        0        0      535 2024-04-25 07:25:49.715614 cg-60.4.0/cg/services/delivery_message/messages/fastq_message.py
--rw-r--r--   0        0        0     1358 2024-04-25 07:25:49.715614 cg-60.4.0/cg/services/delivery_message/messages/fastq_scout_message.py
--rw-r--r--   0        0        0      604 2024-04-25 07:25:49.715614 cg-60.4.0/cg/services/delivery_message/messages/microsalt_mwr_message.py
--rw-r--r--   0        0        0      592 2024-04-25 07:25:49.715614 cg-60.4.0/cg/services/delivery_message/messages/microsalt_mwx_message.py
--rw-r--r--   0        0        0      903 2024-04-25 07:25:49.715614 cg-60.4.0/cg/services/delivery_message/messages/scout_message.py
--rw-r--r--   0        0        0      512 2024-04-25 07:25:49.715614 cg-60.4.0/cg/services/delivery_message/messages/statina_message.py
--rw-r--r--   0        0        0      779 2024-04-25 07:25:49.715614 cg-60.4.0/cg/services/delivery_message/messages/utils.py
--rw-r--r--   0        0        0     3300 2024-04-25 07:25:49.715614 cg-60.4.0/cg/services/delivery_message/utils.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.715614 cg-60.4.0/cg/services/fastq_file_service/__init__.py
--rw-r--r--   0        0        0      101 2024-04-25 07:25:49.715614 cg-60.4.0/cg/services/fastq_file_service/exceptions.py
--rw-r--r--   0        0        0     1092 2024-04-25 07:25:49.715614 cg-60.4.0/cg/services/fastq_file_service/fastq_file_service.py
--rw-r--r--   0        0        0     2991 2024-04-25 07:25:49.715614 cg-60.4.0/cg/services/fastq_file_service/utils.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.719615 cg-60.4.0/cg/services/orders/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.719615 cg-60.4.0/cg/services/orders/order_service/__init__.py
--rw-r--r--   0        0        0     2684 2024-04-25 07:25:49.719615 cg-60.4.0/cg/services/orders/order_service/order_service.py
--rw-r--r--   0        0        0     1214 2024-04-25 07:25:49.719615 cg-60.4.0/cg/services/orders/order_service/utils.py
--rw-r--r--   0        0        0       94 2024-04-25 07:25:49.719615 cg-60.4.0/cg/services/orders/order_status_service/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.719615 cg-60.4.0/cg/services/orders/order_status_service/dto/__init__.py
--rw-r--r--   0        0        0      192 2024-04-25 07:25:49.719615 cg-60.4.0/cg/services/orders/order_status_service/dto/case_summary.py
--rw-r--r--   0        0        0      289 2024-04-25 07:25:49.719615 cg-60.4.0/cg/services/orders/order_status_service/dto/order_summary.py
--rw-r--r--   0        0        0     1768 2024-04-25 07:25:49.719615 cg-60.4.0/cg/services/orders/order_status_service/order_summary_service.py
--rw-r--r--   0        0        0     1737 2024-04-25 07:25:49.719615 cg-60.4.0/cg/services/orders/order_status_service/utils.py
--rw-r--r--   0        0        0       95 2024-04-25 07:25:49.719615 cg-60.4.0/cg/services/quality_controller/__init__.py
--rw-r--r--   0        0        0     1819 2024-04-25 07:25:49.719615 cg-60.4.0/cg/services/quality_controller/quality_checks/checks.py
--rw-r--r--   0        0        0     4987 2024-04-25 07:25:49.719615 cg-60.4.0/cg/services/quality_controller/quality_checks/utils.py
--rw-r--r--   0        0        0     1040 2024-04-25 07:25:49.719615 cg-60.4.0/cg/services/quality_controller/quality_controller_service.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.719615 cg-60.4.0/cg/services/slurm_service/__init__.py
--rw-r--r--   0        0        0      703 2024-04-25 07:25:49.719615 cg-60.4.0/cg/services/slurm_service/slurm_cli_service.py
--rw-r--r--   0        0        0      242 2024-04-25 07:25:49.719615 cg-60.4.0/cg/services/slurm_service/slurm_service.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.719615 cg-60.4.0/cg/services/slurm_upload_service/__init__.py
--rw-r--r--   0        0        0      175 2024-04-25 07:25:49.719615 cg-60.4.0/cg/services/slurm_upload_service/slurm_upload_config.py
--rw-r--r--   0        0        0     2074 2024-04-25 07:25:49.719615 cg-60.4.0/cg/services/slurm_upload_service/slurm_upload_service.py
--rw-r--r--   0        0        0      203 2024-04-25 07:25:49.719615 cg-60.4.0/cg/services/slurm_upload_service/utils.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/__init__.py
--rw-r--r--   0        0        0     4650 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/base.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/crud/__init__.py
--rw-r--r--   0        0        0    13100 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/crud/create.py
--rw-r--r--   0        0        0     2144 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/crud/delete.py
--rw-r--r--   0        0        0    60036 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/crud/read.py
--rw-r--r--   0        0        0     1121 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/crud/update.py
--rw-r--r--   0        0        0     1662 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/database.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/filters/__init__.py
--rw-r--r--   0        0        0     5371 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/filters/status_analysis_filters.py
--rw-r--r--   0        0        0     1712 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/filters/status_application_filters.py
--rw-r--r--   0        0        0     1440 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/filters/status_application_limitations_filters.py
--rw-r--r--   0        0        0     2523 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/filters/status_application_version_filters.py
--rw-r--r--   0        0        0     1390 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/filters/status_bed_filters.py
--rw-r--r--   0        0        0     1317 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/filters/status_bed_version_filters.py
--rw-r--r--   0        0        0    10787 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/filters/status_case_filters.py
--rw-r--r--   0        0        0     3272 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/filters/status_case_sample_filters.py
--rw-r--r--   0        0        0      903 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/filters/status_collaboration_filters.py
--rw-r--r--   0        0        0     1412 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/filters/status_customer_filters.py
--rw-r--r--   0        0        0     1880 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/filters/status_flow_cell_filters.py
--rw-r--r--   0        0        0     1255 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/filters/status_invoice_filters.py
--rw-r--r--   0        0        0     2792 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/filters/status_metrics_filters.py
--rw-r--r--   0        0        0     3225 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/filters/status_order_filters.py
--rw-r--r--   0        0        0      851 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/filters/status_organism_filters.py
--rw-r--r--   0        0        0      783 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/filters/status_panel_filters.py
--rw-r--r--   0        0        0     3923 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/filters/status_pool_filters.py
--rw-r--r--   0        0        0     8660 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/filters/status_sample_filters.py
--rw-r--r--   0        0        0      731 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/filters/status_user_filters.py
--rw-r--r--   0        0        0    36081 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/models.py
--rw-r--r--   0        0        0      593 2024-04-25 07:25:49.719615 cg-60.4.0/cg/store/store.py
--rw-r--r--   0        0        0       30 2024-04-25 07:25:49.719615 cg-60.4.0/cg/utils/__init__.py
--rw-r--r--   0        0        0      187 2024-04-25 07:25:49.719615 cg-60.4.0/cg/utils/calculations.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.719615 cg-60.4.0/cg/utils/checksum/__init__.py
--rw-r--r--   0        0        0     1579 2024-04-25 07:25:49.719615 cg-60.4.0/cg/utils/checksum/checksum.py
--rw-r--r--   0        0        0     1655 2024-04-25 07:25:49.719615 cg-60.4.0/cg/utils/click/EnumChoice.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.719615 cg-60.4.0/cg/utils/click/__init__.py
--rw-r--r--   0        0        0     4910 2024-04-25 07:25:49.719615 cg-60.4.0/cg/utils/commands.py
--rw-r--r--   0        0        0     1811 2024-04-25 07:25:49.719615 cg-60.4.0/cg/utils/date.py
--rw-r--r--   0        0        0      635 2024-04-25 07:25:49.719615 cg-60.4.0/cg/utils/dict.py
--rw-r--r--   0        0        0     2111 2024-04-25 07:25:49.719615 cg-60.4.0/cg/utils/dispatcher.py
--rw-r--r--   0        0        0     1251 2024-04-25 07:25:49.719615 cg-60.4.0/cg/utils/email.py
--rw-r--r--   0        0        0      134 2024-04-25 07:25:49.719615 cg-60.4.0/cg/utils/enums.py
--rw-r--r--   0        0        0     3178 2024-04-25 07:25:49.719615 cg-60.4.0/cg/utils/files.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.719615 cg-60.4.0/cg/utils/flask/__init__.py
--rw-r--r--   0        0        0     1052 2024-04-25 07:25:49.719615 cg-60.4.0/cg/utils/flask/enum.py
--rw-r--r--   0        0        0      233 2024-04-25 07:25:49.719615 cg-60.4.0/cg/utils/flow_cell.py
--rw-r--r--   0        0        0      834 2024-04-25 07:25:49.719615 cg-60.4.0/cg/utils/time.py
--rw-r--r--   0        0        0     1224 2024-04-25 07:25:49.719615 cg-60.4.0/cg/utils/utils.py
--rw-r--r--   0        0        0     1697 2024-04-25 07:25:49.723615 cg-60.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.723615 cg-60.4.0/tests/__init__.py
--rw-r--r--   0        0        0     1158 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/conftest.py
--rw-r--r--   0        0        0      231 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/coverage/conftest.py
--rw-r--r--   0        0        0     6188 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/coverage/test_coverage.py
--rw-r--r--   0        0        0     1693 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/crunchy/conftest.py
--rw-r--r--   0        0        0     5438 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/crunchy/test_compress_fastq.py
--rw-r--r--   0        0        0     2283 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/crunchy/test_config.py
--rw-r--r--   0        0        0    14032 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/crunchy/test_crunchy.py
--rw-r--r--   0        0        0     9109 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/crunchy/test_spring_decompression.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/demultiplex/__init__.py
--rw-r--r--   0        0        0     4994 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/demultiplex/conftest.py
--rw-r--r--   0        0        0     4010 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0        0        0     7986 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/demultiplex/test_demultiplex_api.py
--rw-r--r--   0        0        0     4782 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/demultiplex/test_index.py
--rw-r--r--   0        0        0     9468 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/demultiplex/test_override_cycles_validator.py
--rw-r--r--   0        0        0     4042 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/demultiplex/test_read_sample_sheet.py
--rw-r--r--   0        0        0    12389 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/demultiplex/test_sample_models.py
--rw-r--r--   0        0        0      951 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/demultiplex/test_sample_sheet_creator.py
--rw-r--r--   0        0        0     3175 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/demultiplex/test_sample_sheet_models.py
--rw-r--r--   0        0        0    10932 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/demultiplex/test_sample_sheet_validator.py
--rw-r--r--   0        0        0     4896 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/demultiplex/test_translate_sample_sheet.py
--rw-r--r--   0        0        0     1450 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/demultiplex/test_validate.py
--rw-r--r--   0        0        0     5094 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/downsample/test_downsample.py
--rw-r--r--   0        0        0     1419 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/downsample/test_downsample_utils.py
--rw-r--r--   0        0        0     1716 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/gens/test_gens_api.py
--rw-r--r--   0        0        0     1950 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/gt/conftest.py
--rw-r--r--   0        0        0     4276 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/gt/test_gt_api.py
--rw-r--r--   0        0        0     1453 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/hk/conftest.py
--rw-r--r--   0        0        0      684 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/hk/test__getattr__.py
--rw-r--r--   0        0        0     1593 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/hk/test_add_file.py
--rw-r--r--   0        0        0     3523 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/hk/test_bundles.py
--rw-r--r--   0        0        0      871 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/hk/test_core.py
--rw-r--r--   0        0        0    31172 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/hk/test_file.py
--rw-r--r--   0        0        0     5080 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/hk/test_version.py
--rw-r--r--   0        0        0     1840 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/lims/conftest.py
--rw-r--r--   0        0        0     3197 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/lims/test_api.py
--rw-r--r--   0        0        0     1451 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/lims/test_sample_sheet.py
--rw-r--r--   0        0        0     9223 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/loqus/conftest.py
--rw-r--r--   0        0        0     8994 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/loqus/test_loqusdb_api.py
--rw-r--r--   0        0        0     2439 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/madeline/conftest.py
--rw-r--r--   0        0        0     4653 2024-04-25 07:25:49.723615 cg-60.4.0/tests/apps/madeline/test_madeline.py
--rw-r--r--   0        0        0     3328 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/mip/conftest.py
--rw-r--r--   0        0        0     2487 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/mip/test_config_mip.py
--rw-r--r--   0        0        0      883 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/mutacc_auto/conftest.py
--rw-r--r--   0        0        0     2473 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/mutacc_auto/test_mutacc_auto.py
--rw-r--r--   0        0        0    11930 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/orderform/conftest.py
--rw-r--r--   0        0        0     9484 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/orderform/test_excel_orderform_parser.py
--rw-r--r--   0        0        0     4351 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/orderform/test_excel_sample_schema.py
--rw-r--r--   0        0        0     1032 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/orderform/test_json_orderform_parser.py
--rw-r--r--   0        0        0     2474 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/orderform/test_orderform_parser.py
--rw-r--r--   0        0        0    16002 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/orderform/validators/test_excel_sample_validators.py
--rw-r--r--   0        0        0     3670 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/scout/conftest.py
--rw-r--r--   0        0        0     2269 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/scout/test_get_causative_variants.py
--rw-r--r--   0        0        0     1376 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/scout/test_get_scout_cases.py
--rw-r--r--   0        0        0     1840 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/scout/test_scout_load_config.py
--rw-r--r--   0        0        0     7047 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/scout/test_scout_models.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0        0        0     2639 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/sequencing_metrics_parser/conftest.py
--rw-r--r--   0        0        0     7069 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
--rw-r--r--   0        0        0     2958 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/sequencing_metrics_parser/parsers/test_sequencing_metrics_parser_api.py
--rw-r--r--   0        0        0     1131 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/slurm/conftest.py
--rw-r--r--   0        0        0     4412 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/slurm/test_slurm_api.py
--rw-r--r--   0        0        0      831 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/test_apps_environ.py
--rw-r--r--   0        0        0      957 2024-04-25 07:25:49.727615 cg-60.4.0/tests/apps/test_osticket.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/add/__init__.py
--rw-r--r--   0        0        0     1174 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/add/test_cli_add.py
--rw-r--r--   0        0        0     2471 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/add/test_cli_add_customer.py
--rw-r--r--   0        0        0     6841 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/add/test_cli_add_family.py
--rw-r--r--   0        0        0     7588 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/add/test_cli_add_relationship.py
--rw-r--r--   0        0        0     8382 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/add/test_cli_add_sample.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/backup/__init__.py
--rw-r--r--   0        0        0      705 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/backup/conftest.py
--rw-r--r--   0        0        0    11101 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/backup/test_backup_command.py
--rw-r--r--   0        0        0     6865 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/clean/conftest.py
--rw-r--r--   0        0        0     5536 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/clean/test_balsamic_clean.py
--rw-r--r--   0        0        0     2557 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/clean/test_clean_flow_cell.py
--rw-r--r--   0        0        0     1830 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/clean/test_clean_hk_bundle_files.py
--rw-r--r--   0        0        0     2098 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/clean/test_hk_bundle_files.py
--rw-r--r--   0        0        0     4610 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/clean/test_hk_case_bundle_files.py
--rw-r--r--   0        0        0     3585 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/clean/test_microbial_clean.py
--rw-r--r--   0        0        0     1881 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/clean/test_rsync_past_run_dirs.py
--rw-r--r--   0        0        0     9707 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/compress/conftest.py
--rw-r--r--   0        0        0     7709 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/compress/test_cli_compress_fastq.py
--rw-r--r--   0        0        0     1416 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/compress/test_cli_decompress_spring.py
--rw-r--r--   0        0        0     5205 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/compress/test_compress_helpers.py
--rw-r--r--   0        0        0     1239 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/compress/test_store_fastq.py
--rw-r--r--   0        0        0     7558 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/conftest.py
--rw-r--r--   0        0        0    12747 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/delete/test_cli_delete_case.py
--rw-r--r--   0        0        0     1873 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/delete/test_cli_delete_cases.py
--rw-r--r--   0        0        0     3794 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/deliver/conftest.py
--rw-r--r--   0        0        0     4428 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/deliver/test_deliver_base.py
--rw-r--r--   0        0        0     1166 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/deliver/test_rsync_base.py
--rw-r--r--   0        0        0     8569 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/deliver/test_run_deliver_cmd.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/demultiplex/__init__.py
--rw-r--r--   0        0        0     5109 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0        0        0     4773 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/demultiplex/test_demultiplex_flowcell.py
--rw-r--r--   0        0        0     1607 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/demultiplex/test_finish_demux.py
--rw-r--r--   0        0        0     2989 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/demultiplex/test_validate_sample_sheet.py
--rw-r--r--   0        0        0     4423 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/demultiplex/test_verify_syncing.py
--rw-r--r--   0        0        0     1585 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/downsample/test_cli_downsample.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/generate/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/generate/report/__init__.py
--rw-r--r--   0        0        0     1622 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/generate/report/conftest.py
--rw-r--r--   0        0        0     2477 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/generate/report/test_cli_delivery_report.py
--rw-r--r--   0        0        0     2760 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/generate/report/test_utils.py
--rw-r--r--   0        0        0      563 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/generate/test_cli_base.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/get/__init__.py
--rw-r--r--   0        0        0      863 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/get/test_cli_get.py
--rw-r--r--   0        0        0     1526 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/get/test_cli_get_analysis.py
--rw-r--r--   0        0        0     1242 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/get/test_cli_get_case.py
--rw-r--r--   0        0        0     6208 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/get/test_cli_get_flow_cell.py
--rw-r--r--   0        0        0     8835 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/get/test_cli_get_sample.py
--rw-r--r--   0        0        0     1364 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/set/conftest.py
--rw-r--r--   0        0        0     7311 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/set/test_cli_set_case.py
--rw-r--r--   0        0        0     1460 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/set/test_cli_set_cases.py
--rw-r--r--   0        0        0     2016 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/set/test_cli_set_flowcell.py
--rw-r--r--   0        0        0     1685 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/set/test_cli_set_list_keys.py
--rw-r--r--   0        0        0    12450 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/set/test_cli_set_sample.py
--rw-r--r--   0        0        0     6124 2024-04-25 07:25:49.727615 cg-60.4.0/tests/cli/set/test_cli_set_samples.py
--rw-r--r--   0        0        0     7015 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/store/test_store.py
--rw-r--r--   0        0        0     2332 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/test_base.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/upload/__init__.py
--rw-r--r--   0        0        0    10057 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/upload/conftest.py
--rw-r--r--   0        0        0     2295 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/upload/test_cli_scout.py
--rw-r--r--   0        0        0     1789 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/upload/test_cli_upload.py
--rw-r--r--   0        0        0      971 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/upload/test_cli_upload_auto.py
--rw-r--r--   0        0        0     1669 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/upload/test_cli_upload_delivery_report.py
--rw-r--r--   0        0        0      895 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/upload/test_cli_upload_fastq.py
--rw-r--r--   0        0        0     1199 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/upload/test_cli_upload_genotype.py
--rw-r--r--   0        0        0      694 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/upload/test_cli_upload_gens.py
--rw-r--r--   0        0        0     9965 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/upload/test_cli_upload_nipt.py
--rw-r--r--   0        0        0     4684 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/upload/test_cli_upload_nipt_ftp.py
--rw-r--r--   0        0        0     1839 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/upload/test_cli_upload_nipt_statina.py
--rw-r--r--   0        0        0     6177 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/upload/test_cli_upload_observations.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/__init__.py
--rw-r--r--   0        0        0    31369 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/balsamic/conftest.py
--rw-r--r--   0        0        0    13938 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
--rw-r--r--   0        0        0     7984 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/balsamic/test_compound_commands.py
--rw-r--r--   0        0        0     2336 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/balsamic/test_link.py
--rw-r--r--   0        0        0     3554 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/balsamic/test_report_deliver.py
--rw-r--r--   0        0        0     6209 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/balsamic/test_run.py
--rw-r--r--   0        0        0     6934 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/balsamic/test_store_housekeeper.py
--rw-r--r--   0        0        0     8458 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/conftest.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/fastq/__init__.py
--rw-r--r--   0        0        0     2332 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/fastq/test_fastq_base.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/fluffy/__init__.py
--rw-r--r--   0        0        0     5237 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/fluffy/conftest.py
--rw-r--r--   0        0        0     5687 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
--rw-r--r--   0        0        0     3302 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/fluffy/test_cli_link.py
--rw-r--r--   0        0        0     1896 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/fluffy/test_cli_run.py
--rw-r--r--   0        0        0     2968 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/fluffy/test_cli_start.py
--rw-r--r--   0        0        0     7815 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/fluffy/test_cli_store.py
--rw-r--r--   0        0        0     2775 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/microsalt/conftest.py
--rw-r--r--   0        0        0     6926 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/microsalt/test_microsalt_case_config.py
--rw-r--r--   0        0        0     1000 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/microsalt/test_microsalt_run.py
--rw-r--r--   0        0        0     6544 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/mip/conftest.py
--rw-r--r--   0        0        0     7011 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/mip/test_cli_mip_base.py
--rw-r--r--   0        0        0     1542 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
--rw-r--r--   0        0        0      431 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/mip/test_cli_mip_dna_link.py
--rw-r--r--   0        0        0     2108 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py
--rw-r--r--   0        0        0     1273 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
--rw-r--r--   0        0        0     3595 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/mip/test_cli_mip_dna_run.py
--rw-r--r--   0        0        0     3884 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/mip/test_cli_mip_dna_start.py
--rw-r--r--   0        0        0     1004 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
--rw-r--r--   0        0        0      527 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/mip/test_cli_mip_rna_link.py
--rw-r--r--   0        0        0      716 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/mip/test_cli_mip_rna_run.py
--rw-r--r--   0        0        0     8559 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/mip/test_cli_mip_store.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/nf_analysis/__init__.py
--rw-r--r--   0        0        0     7365 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/nf_analysis/test_cli_config_case.py
--rw-r--r--   0        0        0     3831 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py
--rw-r--r--   0        0        0     5087 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py
--rw-r--r--   0        0        0     9211 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/nf_analysis/test_cli_run.py
--rw-r--r--   0        0        0     2994 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/nf_analysis/test_cli_start.py
--rw-r--r--   0        0        0     9877 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/nf_analysis/test_cli_store.py
--rw-r--r--   0        0        0    10373 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py
--rw-r--r--   0        0        0      978 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/raredisease/__init__.py
--rw-r--r--   0        0        0     3940 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py
--rw-r--r--   0        0        0      921 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/test_cli_workflow.py
--rw-r--r--   0        0        0     4310 2024-04-25 07:25:49.731615 cg-60.4.0/tests/cli/workflow/test_cli_workflow_clean.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.731615 cg-60.4.0/tests/clients/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.731615 cg-60.4.0/tests/clients/arnold/__init__.py
--rw-r--r--   0        0        0     1080 2024-04-25 07:25:49.731615 cg-60.4.0/tests/clients/arnold/conftest.py
--rw-r--r--   0        0        0     1503 2024-04-25 07:25:49.731615 cg-60.4.0/tests/clients/arnold/test_arnold_api_client.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.731615 cg-60.4.0/tests/clients/janus/__init__.py
--rw-r--r--   0        0        0     2381 2024-04-25 07:25:49.731615 cg-60.4.0/tests/clients/janus/conftest.py
--rw-r--r--   0        0        0     1716 2024-04-25 07:25:49.731615 cg-60.4.0/tests/clients/janus/test_janus_api_client.py
--rw-r--r--   0        0        0   133086 2024-04-25 07:25:49.731615 cg-60.4.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.731615 cg-60.4.0/tests/fixture_plugins/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.731615 cg-60.4.0/tests/fixture_plugins/delivery_fixtures/__init__.py
--rw-r--r--   0        0        0     2653 2024-04-25 07:25:49.731615 cg-60.4.0/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py
--rw-r--r--   0        0        0     4972 2024-04-25 07:25:49.731615 cg-60.4.0/tests/fixture_plugins/delivery_fixtures/context_fixtures.py
--rw-r--r--   0        0        0     1494 2024-04-25 07:25:49.731615 cg-60.4.0/tests/fixture_plugins/delivery_fixtures/path_fixtures.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixture_plugins/demultiplex_fixtures/__init__.py
--rw-r--r--   0        0        0     4625 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py
--rw-r--r--   0        0        0     3467 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py
--rw-r--r--   0        0        0    19179 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py
--rw-r--r--   0        0        0     3699 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py
--rw-r--r--   0        0        0     6000 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py
--rw-r--r--   0        0        0     8960 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py
--rw-r--r--   0        0        0     3174 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_check_scenario.py
--rw-r--r--   0        0        0     4801 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_fixtures.py
--rw-r--r--   0        0        0     1304 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixture_plugins/timestamp_fixtures.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
--rw-r--r--   0        0        0    14644 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
--rw-r--r--   0        0        0    15921 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/mip/dna/ADM2.cram
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/mip/dna/ADM3.cram
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/mip/dna/adm1.cram
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/mip/dna/adm1.mt.bam
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/mip/dna/multiqc.html
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/mip/dna/report.pdf
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/mip/dna/smn.vcf
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/mip/dna/snv.vcf
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/mip/dna/snv_research.vcf
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/mip/dna/str.vcf
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/mip/dna/sv.vcf
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/mip/dna/sv_research.vcf
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
--rw-r--r--   0        0        0       70 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/nf-analysis/pipeline_params.config
--rw-r--r--   0        0        0      195 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/nf-analysis/pipeline_resource_optimisation.config
--rw-r--r--   0        0        0      195 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/nf-analysis/platform.config
--rw-r--r--   0        0        0     8173 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/raredisease/multiqc_data.json
--rw-r--r--   0        0        0    20005 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml
--rw-r--r--   0        0        0     5497 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/rnafusion/multiqc_data.json
--rw-r--r--   0        0        0    12499 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml
--rw-r--r--   0        0        0     2873 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/sample_coverage.bed
--rw-r--r--   0        0        0     6506 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/taxprofiler/multiqc_data.json
--rw-r--r--   0        0        0    10513 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml
--rw-r--r--   0        0        0     5771 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/tomte/multiqc_data.json
--rw-r--r--   0        0        0    14859 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml
--rw-r--r--   0        0        0    10961 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/balsamic/case/config.json
--rw-r--r--   0        0        0     3465 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/balsamic/case/metadata.yml
--rw-r--r--   0        0        0       63 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/balsamic/case/metadata_directory.yml
--rw-r--r--   0        0        0      165 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
--rw-r--r--   0        0        0     2705 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
--rw-r--r--   0        0        0      692 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/crunchy/spring_metadata.json
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0      412 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      484 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      658 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/demuxcomplete.txt
--rw-r--r--   0        0        0     1757 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0        0        0        7 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0     6034 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0        0        0     1172 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0        0        0        7 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_1.fastq.gz
--rw-r--r--   0        0        0        7 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_2.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0      288 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      361 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      414 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/demuxcomplete.txt
--rw-r--r--   0        0        0      315 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      434 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0     8624 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml
--rw-r--r--   0        0        0      568 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0      220 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      463 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      622 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0      345 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      650 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      896 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0      619 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0      303 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      364 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      427 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/demuxcomplete.txt
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0     4439 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0        0        0     1172 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0     5127 2024-04-25 07:25:49.735615 cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
--rw-r--r--   0        0        0       43 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz
--rw-r--r--   0        0        0       67 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz.md5
--rw-r--r--   0        0        0   338370 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz
--rw-r--r--   0        0        0       67 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz.md5
--rw-r--r--   0        0        0   338349 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/CopyComplete.txt
--rw-r--r--   0        0        0     2126 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json
--rw-r--r--   0        0        0     1827 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json
--rw-r--r--   0        0        0       90 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/README.txt
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAComplete.txt
--rw-r--r--   0        0        0     6895 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml
--rw-r--r--   0        0        0       37 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead1Complete.txt
--rw-r--r--   0        0        0       36 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead2Complete.txt
--rw-r--r--   0        0        0       36 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead3Complete.txt
--rw-r--r--   0        0        0    24755 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml
--rw-r--r--   0        0        0      692 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
--rw-r--r--   0        0        0      724 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0       61 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SequencingComplete.txt
--rw-r--r--   0        0        0     5775 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.739615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/CopyComplete.txt
--rw-r--r--   0        0        0     2282 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json
--rw-r--r--   0        0        0     1632 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json
--rw-r--r--   0        0        0       75 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/README.txt
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAComplete.txt
--rw-r--r--   0        0        0     6912 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml
--rw-r--r--   0        0        0       36 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead1Complete.txt
--rw-r--r--   0        0        0       36 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead2Complete.txt
--rw-r--r--   0        0        0       36 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead3Complete.txt
--rw-r--r--   0        0        0       36 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead4Complete.txt
--rw-r--r--   0        0        0    24814 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml
--rw-r--r--   0        0        0      814 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv
--rw-r--r--   0        0        0      660 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0       61 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SequencingComplete.txt
--rw-r--r--   0        0        0     5853 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/CopyComplete.txt
--rw-r--r--   0        0        0    21848 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json
--rw-r--r--   0        0        0    15512 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json
--rw-r--r--   0        0        0       79 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/README.txt
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RTAComplete.txt
--rw-r--r--   0        0        0      756 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml
--rw-r--r--   0        0        0     4118 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv
--rw-r--r--   0        0        0     1408 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0     5326 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/CopyComplete.txt
--rw-r--r--   0        0        0    15041 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json
--rw-r--r--   0        0        0    10649 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json
--rw-r--r--   0        0        0       80 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/README.txt
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RTAComplete.txt
--rw-r--r--   0        0        0      755 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml
--rw-r--r--   0        0        0     2878 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv
--rw-r--r--   0        0        0      928 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0     5359 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CopyComplete.txt
--rw-r--r--   0        0        0    27887 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv
--rw-r--r--   0        0        0   141870 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json
--rwxr-xr-x   0        0        0   122682 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json
--rw-r--r--   0        0        0      243 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/README.txt
--rw-r--r--   0        0        0    28230 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTAComplete.txt
--rw-r--r--   0        0        0    94426 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml
--rw-r--r--   0        0        0     5819 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/SequenceComplete.txt
--rw-r--r--   0        0        0     1757 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0        0        0     1757 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stdout
--rw-r--r--   0        0        0       12 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/README.txt
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RTAComplete.txt
--rw-r--r--   0        0        0     5945 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml
--rw-r--r--   0        0        0      260 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/copycomplete.txt
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/demuxstarted.txt
--rw-r--r--   0        0        0     1757 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0        0        0     1757 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout
--rw-r--r--   0        0        0    47522 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json
--rw-r--r--   0        0        0       12 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/README.txt
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0        0        0     6666 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0        0        0      254 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/copycomplete.txt
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/delivery.txt
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/demuxstarted.txt
--rwxr-xr-x   0        0        0    47434 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CopyComplete.txt
--rw-r--r--   0        0        0    10950 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv
--rw-r--r--   0        0        0      225 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/Manifest.tsv
--rw-r--r--   0        0        0       55 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/README.txt
--rwxr-xr-x   0        0        0     2493 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg
--rwxr-xr-x   0        0        0        1 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAComplete.txt
--rwxr-xr-x   0        0        0        2 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAExited.txt
--rwxr-xr-x   0        0        0      730 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml
--rwxr-xr-x   0        0        0    79277 2024-04-25 07:25:49.743615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml
--rwxr-xr-x   0        0        0     2694 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
--rw-r--r--   0        0        0    10950 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
--rw-r--r--   0        0        0      619 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0        0        0       12 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/README.txt
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0        0        0      399 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CopyComplete.txt
--rw-r--r--   0        0        0     4941 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv
--rwxr-xr-x   0        0        0    20050 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stderr
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stdout
--rw-r--r--   0        0        0      244 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/README.txt
--rw-r--r--   0        0        0     6391 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTAComplete.txt
--rw-r--r--   0        0        0    16428 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml
--rw-r--r--   0        0        0     6728 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
--rw-r--r--   0        0        0     5127 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SequenceComplete.txt
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/demuxstarted.txt
--rw-r--r--   0        0        0      133 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/README.txt
--rw-r--r--   0        0        0      724 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
--rw-r--r--   0        0        0     5775 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
--rw-r--r--   0        0        0      124 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/180509_D00450_0598_BHGYFNBCX2/README.txt
--rw-r--r--   0        0        0      310 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/README.txt
--rw-r--r--   0        0        0     5819 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
--rw-r--r--   0        0        0      122 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/README.txt
--rwxr-xr-x   0        0        0     2694 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
--rw-r--r--   0        0        0      311 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/README.txt
--rw-r--r--   0        0        0     6728 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0        0        0      399 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
--rw-r--r--   0        0        0      399 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_0.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_1.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/final_summary_PAS86456_72d9fceb_8a4fd683.txt
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_0.pod5
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_1.pod5
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_0.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_1.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/final_summary_PAS97781_595b5663_efc7f02e.txt
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_0.pod5
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_1.pod5
--rw-r--r--   0        0        0   111989 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
--rw-r--r--   0        0        0     5319 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml
--rw-r--r--   0        0        0     5944 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
--rwxr-xr-x   0        0        0     2603 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
--rwxr-xr-x   0        0        0     2597 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml
--rw-r--r--   0        0        0     5899 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
--rw-r--r--   0        0        0     4941 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv
--rw-r--r--   0        0        0    10950 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/spring/dummy_run_001.spring
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/spring/dummy_run_002.spring
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/demultiplexing/spring/dummy_spring_meta_data.json
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
--rw-r--r--   0        0        0     5554 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/fluffy/SampleSheet.csv
--rw-r--r--   0        0        0      901 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/fluffy/deliverables.yaml
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/fluffy/multiqc_report.html
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/fluffy/summary.csv
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/gt/yellowhog.bcf
--rw-r--r--   0        0        0     5114 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/madeline/madeline.xml
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/mip/case_file.txt
--rw-r--r--   0        0        0     3241 2024-04-25 07:25:49.747615 cg-60.4.0/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
--rw-r--r--   0        0        0    21811 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/mip/dna/store/case_config.yaml
--rw-r--r--   0        0        0    23364 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
--rw-r--r--   0        0        0    37367 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
--rw-r--r--   0        0        0       16 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
--rw-r--r--   0        0        0       16 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
--rw-r--r--   0        0        0       16 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
--rw-r--r--   0        0        0      123 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
--rw-r--r--   0        0        0    62741 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
--rw-r--r--   0        0        0    11242 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/mip/rna/case_config.yaml
--rw-r--r--   0        0        0    12164 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
--rw-r--r--   0        0        0     5231 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
--rw-r--r--   0        0        0     9774 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/mip/rna/store/case_config.yaml
--rw-r--r--   0        0        0     4624 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
--rw-r--r--   0        0        0    13666 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/mip/sample_file.txt
--rw-r--r--   0        0        0     1885 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/scout/643594.config.yaml
--rw-r--r--   0        0        0     6027 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/scout/case_export.json
--rw-r--r--   0        0        0     9349 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/scout/export_causatives.json
--rw-r--r--   0        0        0     1315 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/scout/none_case_export.json
--rw-r--r--   0        0        0     3518 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/scout/other_sex_case.json
--rw-r--r--   0        0        0     8874 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/scout/panel_export.bed
--rw-r--r--   0        0        0     4169 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/scout/panel_export.csv
--rw-r--r--   0        0        0      619 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/SampleSheet.csv
--rw-r--r--   0        0        0    63569 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0    42478 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0    69708 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0       42 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/apps/shipping/scout-deploy.yaml
--rw-r--r--   0        0        0     1036 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/cgweb_orders/balsamic.json
--rw-r--r--   0        0        0     1104 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/cgweb_orders/fastq.json
--rw-r--r--   0        0        0     1313 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/cgweb_orders/metagenome.json
--rw-r--r--   0        0        0     3038 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/cgweb_orders/microsalt.json
--rw-r--r--   0        0        0     3705 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/cgweb_orders/mip.json
--rw-r--r--   0        0        0     1364 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/cgweb_orders/mip_rna.json
--rw-r--r--   0        0        0     2125 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/cgweb_orders/rml.json
--rw-r--r--   0        0        0     1368 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/cgweb_orders/rnafusion.json
--rw-r--r--   0        0        0     4684 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/cgweb_orders/sarscov2.json
--rw-r--r--   0        0        0     5609 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/data/SampleSheet.csv
--rw-r--r--   0        0        0      511 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/data/bcl_convert_sample_sheet.csv
--rw-r--r--   0        0        0   258048 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/data/cgfixture.db
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.751615 cg-60.4.0/tests/fixtures/data/fastq.fastq.gz
--rw-r--r--   0        0        0    49152 2024-04-25 07:25:49.755615 cg-60.4.0/tests/fixtures/data/hkstore.db
--rw-r--r--   0        0        0       73 2024-04-25 07:25:49.755615 cg-60.4.0/tests/fixtures/data/yellowhog/pedigree.yaml
--rw-r--r--   0        0        0       76 2024-04-25 07:25:49.755615 cg-60.4.0/tests/fixtures/io/casava_five_parts.fastq.gz
--rw-r--r--   0        0        0       90 2024-04-25 07:25:49.755615 cg-60.4.0/tests/fixtures/io/casava_seven_parts.fastq.gz
--rw-r--r--   0        0        0       96 2024-04-25 07:25:49.755615 cg-60.4.0/tests/fixtures/io/casava_ten_parts.fastq.gz
--rw-r--r--   0        0        0      153 2024-04-25 07:25:49.755615 cg-60.4.0/tests/fixtures/io/example.csv
--rw-r--r--   0        0        0       46 2024-04-25 07:25:49.755615 cg-60.4.0/tests/fixtures/io/example.gz
--rw-r--r--   0        0        0      147 2024-04-25 07:25:49.755615 cg-60.4.0/tests/fixtures/io/example.tsv
--rw-r--r--   0        0        0       20 2024-04-25 07:25:49.755615 cg-60.4.0/tests/fixtures/io/example.txt
--rw-r--r--   0        0        0       20 2024-04-25 07:25:49.755615 cg-60.4.0/tests/fixtures/io/example2.txt
--rw-r--r--   0        0        0      582 2024-04-25 07:25:49.755615 cg-60.4.0/tests/fixtures/io/example_json.json
--rw-r--r--   0        0        0      103 2024-04-25 07:25:49.755615 cg-60.4.0/tests/fixtures/io/example_xml.xml
--rw-r--r--   0        0        0       20 2024-04-25 07:25:49.755615 cg-60.4.0/tests/fixtures/meta/qc_metrics/file_with_right_tags.json
--rw-r--r--   0        0        0       20 2024-04-25 07:25:49.755615 cg-60.4.0/tests/fixtures/meta/qc_metrics/file_without_right_tags.json
--rw-r--r--   0        0        0   156910 2024-04-25 07:25:49.755615 cg-60.4.0/tests/fixtures/orderforms/1508.30.balsamic.xlsx
--rw-r--r--   0        0        0   156770 2024-04-25 07:25:49.755615 cg-60.4.0/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx
--rw-r--r--   0        0        0   156737 2024-04-25 07:25:49.755615 cg-60.4.0/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx
--rw-r--r--   0        0        0   156582 2024-04-25 07:25:49.755615 cg-60.4.0/tests/fixtures/orderforms/1508.30.fastq.xlsx
--rw-r--r--   0        0        0   155627 2024-04-25 07:25:49.755615 cg-60.4.0/tests/fixtures/orderforms/1508.30.metagenome.xlsx
--rw-r--r--   0        0        0   156850 2024-04-25 07:25:49.759615 cg-60.4.0/tests/fixtures/orderforms/1508.30.mip.xlsx
--rw-r--r--   0        0        0   258580 2024-04-25 07:25:49.759615 cg-60.4.0/tests/fixtures/orderforms/1508.30.mip_rna.xlsx
--rw-r--r--   0        0        0   258342 2024-04-25 07:25:49.759615 cg-60.4.0/tests/fixtures/orderforms/1508.30.rnafusion.xlsx
--rw-r--r--   0        0        0    82677 2024-04-25 07:25:49.759615 cg-60.4.0/tests/fixtures/orderforms/1603.11.microbial.xlsx
--rw-r--r--   0        0        0   149394 2024-04-25 07:25:49.759615 cg-60.4.0/tests/fixtures/orderforms/1604.17.rml.xlsx
--rw-r--r--   0        0        0   223184 2024-04-25 07:25:49.759615 cg-60.4.0/tests/fixtures/orderforms/2184.9.sarscov2.xlsx
--rw-r--r--   0        0        0    18639 2024-04-25 07:25:49.759615 cg-60.4.0/tests/fixtures/orderforms/NIPT-json.json
--rw-r--r--   0        0        0     6052 2024-04-25 07:25:49.759615 cg-60.4.0/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
--rw-r--r--   0        0        0     6611 2024-04-25 07:25:49.759615 cg-60.4.0/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
--rw-r--r--   0        0        0     1417 2024-04-25 07:25:49.763615 cg-60.4.0/tests/fixtures/report/case_data.json
--rw-r--r--   0        0        0     1109 2024-04-25 07:25:49.763615 cg-60.4.0/tests/fixtures/report/lims_exported_samples.json
--rw-r--r--   0        0        0     1562 2024-04-25 07:25:49.763615 cg-60.4.0/tests/fixtures/report/lims_family.json
--rw-r--r--   0        0        0     3296 2024-04-25 07:25:49.763615 cg-60.4.0/tests/io/conftest.py
--rw-r--r--   0        0        0      431 2024-04-25 07:25:49.763615 cg-60.4.0/tests/io/test_io_config.py
--rw-r--r--   0        0        0     8639 2024-04-25 07:25:49.763615 cg-60.4.0/tests/io/test_io_controller.py
--rw-r--r--   0        0        0     3877 2024-04-25 07:25:49.763615 cg-60.4.0/tests/io/test_io_csv.py
--rw-r--r--   0        0        0      482 2024-04-25 07:25:49.763615 cg-60.4.0/tests/io/test_io_gzip.py
--rw-r--r--   0        0        0     1779 2024-04-25 07:25:49.763615 cg-60.4.0/tests/io/test_io_json.py
--rw-r--r--   0        0        0     2914 2024-04-25 07:25:49.763615 cg-60.4.0/tests/io/test_io_txt.py
--rw-r--r--   0        0        0     1027 2024-04-25 07:25:49.763615 cg-60.4.0/tests/io/test_io_xml.py
--rw-r--r--   0        0        0     2131 2024-04-25 07:25:49.763615 cg-60.4.0/tests/io/test_io_yaml.py
--rw-r--r--   0        0        0     1233 2024-04-25 07:25:49.763615 cg-60.4.0/tests/io/test_validate_path.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/archive/__init__.py
--rw-r--r--   0        0        0    13131 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/archive/conftest.py
--rw-r--r--   0        0        0    16858 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/archive/test_archive_api.py
--rw-r--r--   0        0        0    10246 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/archive/test_archive_cli.py
--rw-r--r--   0        0        0    15766 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/archive/test_archiving.py
--rw-r--r--   0        0        0     3807 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/backup/conftest.py
--rw-r--r--   0        0        0    26368 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/backup/test_meta_backup.py
--rw-r--r--   0        0        0    10055 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/backup/test_meta_pdc.py
--rw-r--r--   0        0        0    12546 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/clean/conftest.py
--rw-r--r--   0        0        0    16944 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/clean/test_clean_flow_cells_api.py
--rw-r--r--   0        0        0     2286 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/clean/test_clean_retrieved_spring_files.py
--rw-r--r--   0        0        0     7691 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/compress/conftest.py
--rw-r--r--   0        0        0     7961 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/compress/test_clean_fastq.py
--rw-r--r--   0        0        0     1778 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/compress/test_compress_files.py
--rw-r--r--   0        0        0     3644 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/compress/test_compress_meta_fastq.py
--rw-r--r--   0        0        0     1180 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/compress/test_decompress_spring_meta.py
--rw-r--r--   0        0        0     7013 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/compress/test_meta_compress_update_hk.py
--rw-r--r--   0        0        0     8269 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/conftest.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/deliver/__init__.py
--rw-r--r--   0        0        0     3471 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/deliver/conftest.py
--rw-r--r--   0        0        0     5533 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/deliver/test_deliver_ticket.py
--rw-r--r--   0        0        0    10277 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/deliver/test_delivery_api.py
--rw-r--r--   0        0        0     1057 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/deliver/test_fastq_path_generator.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/delivery/__init__.py
--rw-r--r--   0        0        0    16660 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/delivery/test_delivery_api.py
--rw-r--r--   0        0        0     8874 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/demultiplex/conftest.py
--rw-r--r--   0        0        0     5382 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/demultiplex/test_combine_sequencing_metrics.py
--rw-r--r--   0        0        0     8339 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/demultiplex/test_demux_post_processing.py
--rw-r--r--   0        0        0    12406 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/demultiplex/test_housekeeper_storage_functions.py
--rw-r--r--   0        0        0     4392 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/demultiplex/test_status_db_storage_functions.py
--rw-r--r--   0        0        0    22837 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/demultiplex/test_utils.py
--rw-r--r--   0        0        0     6193 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/demultiplex/test_validation.py
--rw-r--r--   0        0        0     4943 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/encryption/conftest.py
--rw-r--r--   0        0        0    18133 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/encryption/test_encryption.py
--rw-r--r--   0        0        0     3122 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/observations/conftest.py
--rw-r--r--   0        0        0    16164 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/observations/test_meta_upload_observations.py
--rw-r--r--   0        0        0     4974 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/orders/conftest.py
--rw-r--r--   0        0        0     1749 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/orders/test_PoolSubmitter_validate_order.py
--rw-r--r--   0        0        0     1470 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
--rw-r--r--   0        0        0     1768 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/orders/test_SarsCov2Submitter_store_order.py
--rw-r--r--   0        0        0     2032 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
--rw-r--r--   0        0        0    19783 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/orders/test_meta_orders_api.py
--rw-r--r--   0        0        0     7086 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/orders/test_meta_orders_lims.py
--rw-r--r--   0        0        0    29515 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/orders/test_meta_orders_status.py
--rw-r--r--   0        0        0     1677 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/orders/test_rnafusion_submitter.py
--rw-r--r--   0        0        0     1068 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/orders/test_ticket_handler.py
--rw-r--r--   0        0        0     4336 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/qc_metrics/conftest.py
--rw-r--r--   0        0        0     1972 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/qc_metrics/test_collect_qc_metrics.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/report/__init__.py
--rw-r--r--   0        0        0     6512 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/report/conftest.py
--rw-r--r--   0        0        0      434 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/report/helper.py
--rw-r--r--   0        0        0     2604 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/report/test_balsamic_api.py
--rw-r--r--   0        0        0     4056 2024-04-25 07:25:49.763615 cg-60.4.0/tests/meta/report/test_field_validators.py
--rw-r--r--   0        0        0     2858 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/report/test_mip_dna_api.py
--rw-r--r--   0        0        0    16042 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/report/test_report_api.py
--rw-r--r--   0        0        0     1365 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/report/test_rnafusion_api.py
--rw-r--r--   0        0        0     1250 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/report/test_tomte_api.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/rsync/__init__.py
--rw-r--r--   0        0        0      916 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/rsync/conftest.py
--rw-r--r--   0        0        0     9442 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/rsync/test_rsync.py
--rw-r--r--   0        0        0     3147 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/test_invoice.py
--rw-r--r--   0        0        0     1220 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/transfer/conftest.py
--rw-r--r--   0        0        0     9892 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/transfer/test_external_data.py
--rw-r--r--   0        0        0     4395 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/transfer/test_meta_transfer_lims.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/__init__.py
--rw-r--r--   0        0        0     2210 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/balsamic/test_balsamic.py
--rw-r--r--   0        0        0     4002 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/conftest.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/gisaid/__init__.py
--rw-r--r--   0        0        0     2557 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/gisaid/fixtures/four_samples.csv
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
--rw-r--r--   0        0        0      211 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
--rw-r--r--   0        0        0      371 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/mutacc/__init__.py
--rw-r--r--   0        0        0     3684 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/mutacc/conftest.py
--rw-r--r--   0        0        0     4188 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
--rw-r--r--   0        0        0     1149 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/nipt/conftest.py
--rw-r--r--   0        0        0     1683 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/nipt/test_models.py
--rw-r--r--   0        0        0     1242 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/nipt/test_nipt_upload_api.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/scout/__init__.py
--rw-r--r--   0        0        0    23954 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/scout/conftest.py
--rw-r--r--   0        0        0     4734 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/scout/test_generate_load_config.py
--rw-r--r--   0        0        0     4182 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/scout/test_meta_upload_scoutapi.py
--rw-r--r--   0        0        0    33260 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
--rw-r--r--   0        0        0     7372 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/scout/test_scout_config_builder.py
--rw-r--r--   0        0        0     2511 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/test_meta_upload_coverage.py
--rw-r--r--   0        0        0     1473 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/test_upload_api.py
--rw-r--r--   0        0        0     2547 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/upload/test_upload_genotypes_api.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/workflow/__init__.py
--rw-r--r--   0        0        0    10262 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/workflow/conftest.py
--rw-r--r--   0        0        0     3679 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/workflow/microsalt/conftest.py
--rw-r--r--   0        0        0      318 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/workflow/microsalt/test_parsing_metrics.py
--rw-r--r--   0        0        0     3759 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/workflow/microsalt/test_quality_controller.py
--rw-r--r--   0        0        0    14367 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/workflow/microsalt/test_quality_controller_utils.py
--rw-r--r--   0        0        0      825 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/workflow/microsalt/test_report_generation.py
--rw-r--r--   0        0        0    20860 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/workflow/test_analysis.py
--rw-r--r--   0        0        0     7934 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/workflow/test_balsamic.py
--rw-r--r--   0        0        0     3034 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/workflow/test_fastq.py
--rw-r--r--   0        0        0     1532 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/workflow/test_microsalt.py
--rw-r--r--   0        0        0     2721 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/workflow/test_nf_analysis.py
--rw-r--r--   0        0        0     7741 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/workflow/test_prepare_fastq_api.py
--rw-r--r--   0        0        0     1920 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/workflow/test_raredisease.py
--rw-r--r--   0        0        0     1674 2024-04-25 07:25:49.767615 cg-60.4.0/tests/meta/workflow/test_rnafusion.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.767615 cg-60.4.0/tests/mocks/__init__.py
--rw-r--r--   0        0        0     1168 2024-04-25 07:25:49.767615 cg-60.4.0/tests/mocks/balsamic_analysis_mock.py
--rw-r--r--   0        0        0     3500 2024-04-25 07:25:49.767615 cg-60.4.0/tests/mocks/crunchy.py
--rw-r--r--   0        0        0    21778 2024-04-25 07:25:49.767615 cg-60.4.0/tests/mocks/hk_mock.py
--rw-r--r--   0        0        0     4106 2024-04-25 07:25:49.767615 cg-60.4.0/tests/mocks/limsmock.py
--rw-r--r--   0        0        0      572 2024-04-25 07:25:49.767615 cg-60.4.0/tests/mocks/madeline.py
--rw-r--r--   0        0        0     1297 2024-04-25 07:25:49.767615 cg-60.4.0/tests/mocks/mip_analysis_mock.py
--rw-r--r--   0        0        0     1525 2024-04-25 07:25:49.767615 cg-60.4.0/tests/mocks/osticket.py
--rw-r--r--   0        0        0     3239 2024-04-25 07:25:49.767615 cg-60.4.0/tests/mocks/process_mock.py
--rw-r--r--   0        0        0     4713 2024-04-25 07:25:49.767615 cg-60.4.0/tests/mocks/report.py
--rw-r--r--   0        0        0     3915 2024-04-25 07:25:49.767615 cg-60.4.0/tests/mocks/scout.py
--rw-r--r--   0        0        0      750 2024-04-25 07:25:49.767615 cg-60.4.0/tests/mocks/store_model.py
--rw-r--r--   0        0        0     1620 2024-04-25 07:25:49.767615 cg-60.4.0/tests/mocks/tb_mock.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.767615 cg-60.4.0/tests/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.767615 cg-60.4.0/tests/models/balsamic/__init__.py
--rw-r--r--   0        0        0     1194 2024-04-25 07:25:49.767615 cg-60.4.0/tests/models/balsamic/conftest.py
--rw-r--r--   0        0        0     1030 2024-04-25 07:25:49.767615 cg-60.4.0/tests/models/balsamic/test_balsamic_analysis.py
--rw-r--r--   0        0        0     1050 2024-04-25 07:25:49.767615 cg-60.4.0/tests/models/conftest.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.767615 cg-60.4.0/tests/models/demultiplexing/__init__.py
--rw-r--r--   0        0        0    11446 2024-04-25 07:25:49.767615 cg-60.4.0/tests/models/demultiplexing/test_run_parameters.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.767615 cg-60.4.0/tests/models/downsample/__init__.py
--rw-r--r--   0        0        0     2096 2024-04-25 07:25:49.767615 cg-60.4.0/tests/models/downsample/test_down_sample_meta_data.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.767615 cg-60.4.0/tests/models/flow_cell/__init__.py
--rw-r--r--   0        0        0     6659 2024-04-25 07:25:49.767615 cg-60.4.0/tests/models/flow_cell/test_flowcell_model.py
--rw-r--r--   0        0        0     6637 2024-04-25 07:25:49.767615 cg-60.4.0/tests/models/mip/conftest.py
--rw-r--r--   0        0        0     1239 2024-04-25 07:25:49.767615 cg-60.4.0/tests/models/mip/test_mip_analysis.py
--rw-r--r--   0        0        0     2348 2024-04-25 07:25:49.767615 cg-60.4.0/tests/models/mip/test_mip_config.py
--rw-r--r--   0        0        0     6392 2024-04-25 07:25:49.767615 cg-60.4.0/tests/models/mip/test_mip_metrics_deliverables.py
--rw-r--r--   0        0        0     3959 2024-04-25 07:25:49.767615 cg-60.4.0/tests/models/mip/test_mip_sample_info.py
--rw-r--r--   0        0        0     3314 2024-04-25 07:25:49.771615 cg-60.4.0/tests/models/nextflow/test_nextflow_deliver.py
--rw-r--r--   0        0        0     1602 2024-04-25 07:25:49.771615 cg-60.4.0/tests/models/observations/conftest.py
--rw-r--r--   0        0        0     2579 2024-04-25 07:25:49.771615 cg-60.4.0/tests/models/observations/test_observations_input_files.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.771615 cg-60.4.0/tests/models/report/__init__.py
--rw-r--r--   0        0        0     7327 2024-04-25 07:25:49.771615 cg-60.4.0/tests/models/report/test_validators.py
--rw-r--r--   0        0        0     3855 2024-04-25 07:25:49.771615 cg-60.4.0/tests/models/rnafusion/test_rnafusion_sample.py
--rw-r--r--   0        0        0     1374 2024-04-25 07:25:49.771615 cg-60.4.0/tests/models/test_cg_models.py
--rw-r--r--   0        0        0      990 2024-04-25 07:25:49.771615 cg-60.4.0/tests/models/test_compression_data.py
--rw-r--r--   0        0        0      729 2024-04-25 07:25:49.771615 cg-60.4.0/tests/models/test_fastq.py
--rw-r--r--   0        0        0     2860 2024-04-25 07:25:49.771615 cg-60.4.0/tests/models/test_file_data.py
--rw-r--r--   0        0        0     4539 2024-04-25 07:25:49.771615 cg-60.4.0/tests/server/conftest.py
--rw-r--r--   0        0        0     3135 2024-04-25 07:25:49.771615 cg-60.4.0/tests/server/endpoints/test_delivery_message_endpoint.py
--rw-r--r--   0        0        0     3239 2024-04-25 07:25:49.771615 cg-60.4.0/tests/server/endpoints/test_orders_endpoint.py
--rw-r--r--   0        0        0      271 2024-04-25 07:25:49.771615 cg-60.4.0/tests/server/test_server_auto.py
--rw-r--r--   0        0        0     1047 2024-04-25 07:25:49.771615 cg-60.4.0/tests/services/fastq_file_service/conftest.py
--rw-r--r--   0        0        0     3634 2024-04-25 07:25:49.771615 cg-60.4.0/tests/services/fastq_file_service/test_fastq_file_service.py
--rw-r--r--   0        0        0     4861 2024-04-25 07:25:49.771615 cg-60.4.0/tests/services/orders/order_status_service/conftest.py
--rw-r--r--   0        0        0     2865 2024-04-25 07:25:49.771615 cg-60.4.0/tests/services/orders/order_status_service/test_order_summary_service.py
--rw-r--r--   0        0        0     9595 2024-04-25 07:25:49.771615 cg-60.4.0/tests/services/quality_controller/test_sequencing_quality_checks_utils.py
--rw-r--r--   0        0        0      318 2024-04-25 07:25:49.771615 cg-60.4.0/tests/small_helpers.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/api/__init__.py
--rw-r--r--   0        0        0     3032 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/api/conftest.py
--rw-r--r--   0        0        0     1557 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/api/test_base.py
--rw-r--r--   0        0        0    20096 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/conftest.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/crud/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/crud/add/__init__.py
--rw-r--r--   0        0        0     1497 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/crud/add/test_store_add_application_version.py
--rw-r--r--   0        0        0     3958 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/crud/add/test_store_add_base.py
--rw-r--r--   0        0        0     2502 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/crud/add/test_store_add_customer.py
--rw-r--r--   0        0        0     1704 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/crud/add/test_store_add_flow_celll.py
--rw-r--r--   0        0        0    12290 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/crud/conftest.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/crud/delete/__init__.py
--rw-r--r--   0        0        0     5611 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/crud/delete/test_delete.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/crud/read/__init__.py
--rw-r--r--   0        0        0    56077 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/crud/read/test_read.py
--rw-r--r--   0        0        0     5461 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/crud/read/test_read_analyses_to_clean.py
--rw-r--r--   0        0        0     3553 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/crud/read/test_read_analyses_to_delivery_report.py
--rw-r--r--   0        0        0    17328 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/crud/read/test_read_analysis.py
--rw-r--r--   0        0        0     2743 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/crud/read/test_read_application_version.py
--rw-r--r--   0        0        0     1105 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/crud/read/test_read_customer.py
--rw-r--r--   0        0        0     1530 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/crud/read/test_read_pool.py
--rw-r--r--   0        0        0    21503 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/crud/read/test_read_sample.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/crud/update/__init__.py
--rw-r--r--   0        0        0      737 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/crud/update/test_update.py
--rw-r--r--   0        0        0    11693 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/filters/test_status_analyses_filters.py
--rw-r--r--   0        0        0     3397 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/filters/test_status_application_filters.py
--rw-r--r--   0        0        0     2073 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/filters/test_status_application_limitations_filters.py
--rw-r--r--   0        0        0    10452 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/filters/test_status_application_version_filters.py
--rw-r--r--   0        0        0     2804 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/filters/test_status_bed_filters.py
--rw-r--r--   0        0        0     2362 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/filters/test_status_bed_version_filters.py
--rw-r--r--   0        0        0     3495 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/filters/test_status_case_sample_filters.py
--rw-r--r--   0        0        0    39100 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/filters/test_status_cases_filters.py
--rw-r--r--   0        0        0     1345 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/filters/test_status_collaboration_filters.py
--rw-r--r--   0        0        0     2482 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/filters/test_status_customer_filters.py
--rw-r--r--   0        0        0     5153 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/filters/test_status_flow_cell_filters.py
--rw-r--r--   0        0        0     2226 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/filters/test_status_invoice_filters.py
--rw-r--r--   0        0        0     5871 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/filters/test_status_metrics_filters.py
--rw-r--r--   0        0        0     2404 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/filters/test_status_organism_filters.py
--rw-r--r--   0        0        0     1804 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/filters/test_status_panel_filters.py
--rw-r--r--   0        0        0     8720 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/filters/test_status_pool_filters.py
--rw-r--r--   0        0        0    22875 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/filters/test_status_samples_filters.py
--rw-r--r--   0        0        0     1576 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/filters/test_status_user_filters.py
--rw-r--r--   0        0        0     2147 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/test_delivery.py
--rw-r--r--   0        0        0     4127 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store/test_store_models.py
--rw-r--r--   0        0        0    37125 2024-04-25 07:25:49.771615 cg-60.4.0/tests/store_helpers.py
--rw-r--r--   0        0        0     4930 2024-04-25 07:25:49.771615 cg-60.4.0/tests/test_copy_novaseqx_flow_cell.py
--rw-r--r--   0        0        0      911 2024-04-25 07:25:49.771615 cg-60.4.0/tests/test_store_helpers.py
--rw-r--r--   0        0        0        0 2024-04-25 07:25:49.771615 cg-60.4.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     1754 2024-04-25 07:25:49.775615 cg-60.4.0/tests/utils/conftest.py
--rw-r--r--   0        0        0      371 2024-04-25 07:25:49.775615 cg-60.4.0/tests/utils/test_calculations.py
--rw-r--r--   0        0        0     2920 2024-04-25 07:25:49.775615 cg-60.4.0/tests/utils/test_commands.py
--rw-r--r--   0        0        0      953 2024-04-25 07:25:49.775615 cg-60.4.0/tests/utils/test_date.py
--rw-r--r--   0        0        0     1508 2024-04-25 07:25:49.775615 cg-60.4.0/tests/utils/test_dict.py
--rw-r--r--   0        0        0     7154 2024-04-25 07:25:49.775615 cg-60.4.0/tests/utils/test_dispatcher.py
--rw-r--r--   0        0        0     4100 2024-04-25 07:25:49.775615 cg-60.4.0/tests/utils/test_files.py
--rw-r--r--   0        0        0     1170 2024-04-25 07:25:49.775615 cg-60.4.0/tests/utils/test_time.py
--rw-r--r--   0        0        0     2366 2024-04-25 07:25:49.775615 cg-60.4.0/tests/utils/test_utils.py
--rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 cg-60.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2686 2024-04-25 12:07:50.743335 cg-60.4.1/README.md
+-rw-r--r--   0        0        0       40 2024-04-25 12:07:50.743335 cg-60.4.1/cg/__init__.py
+-rw-r--r--   0        0        0      315 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/coverage/__init__.py
+-rw-r--r--   0        0        0     2940 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/coverage/api.py
+-rw-r--r--   0        0        0       56 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/crunchy/__init__.py
+-rw-r--r--   0        0        0    12783 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/crunchy/crunchy.py
+-rw-r--r--   0        0        0     4502 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/crunchy/files.py
+-rw-r--r--   0        0        0      430 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/crunchy/models.py
+-rw-r--r--   0        0        0      910 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/crunchy/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/demultiplex/__init__.py
+-rw-r--r--   0        0        0    11299 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/demultiplex/demultiplex_api.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/demultiplex/sample_sheet/__init__.py
+-rw-r--r--   0        0        0    11227 2024-04-25 12:07:50.743335 cg-60.4.1/cg/apps/demultiplex/sample_sheet/api.py
+-rw-r--r--   0        0        0     2183 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/demultiplex/sample_sheet/index.py
+-rw-r--r--   0        0        0     7341 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py
+-rw-r--r--   0        0        0     3188 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py
+-rw-r--r--   0        0        0     7071 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/demultiplex/sample_sheet/sample_models.py
+-rw-r--r--   0        0        0     6076 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py
+-rw-r--r--   0        0        0     1372 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py
+-rw-r--r--   0        0        0     8092 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py
+-rw-r--r--   0        0        0      824 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/demultiplex/sample_sheet/validators.py
+-rw-r--r--   0        0        0      677 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/demultiplex/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/downsample/__init__.py
+-rw-r--r--   0        0        0     6160 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/downsample/downsample.py
+-rw-r--r--   0        0        0     2125 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/downsample/utils.py
+-rw-r--r--   0        0        0      298 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/environ.py
+-rw-r--r--   0        0        0     1741 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/gens.py
+-rw-r--r--   0        0        0     3419 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/gt.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/hermes/__init__.py
+-rw-r--r--   0        0        0     2249 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/hermes/hermes_api.py
+-rw-r--r--   0        0        0     1298 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/hermes/models.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/housekeeper/__init__.py
+-rw-r--r--   0        0        0    30395 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/housekeeper/hk.py
+-rw-r--r--   0        0        0      326 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/housekeeper/models.py
+-rw-r--r--   0        0        0       32 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/invoice/__init__.py
+-rw-r--r--   0        0        0     4804 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/invoice/render.py
+-rw-r--r--   0        0        0   113467 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/invoice/templates/KI_pool_invoice.xlsx
+-rw-r--r--   0        0        0    75562 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/invoice/templates/KI_sample_invoice.xlsx
+-rw-r--r--   0        0        0   113512 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
+-rw-r--r--   0        0        0    75459 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
+-rw-r--r--   0        0        0       25 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/lims/__init__.py
+-rw-r--r--   0        0        0    18873 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/lims/api.py
+-rw-r--r--   0        0        0     2652 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/lims/batch.py
+-rw-r--r--   0        0        0     8129 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/lims/order.py
+-rw-r--r--   0        0        0     3118 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/lims/sample_sheet.py
+-rw-r--r--   0        0        0     4866 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/loqus.py
+-rw-r--r--   0        0        0       35 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/madeline/__init__.py
+-rw-r--r--   0        0        0     3213 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/madeline/api.py
+-rw-r--r--   0        0        0       23 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/mip/__init__.py
+-rw-r--r--   0        0        0     3564 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/mip/confighandler.py
+-rw-r--r--   0        0        0     2207 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/mutacc_auto.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/orderform/__init__.py
+-rw-r--r--   0        0        0     9498 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/orderform/excel_orderform_parser.py
+-rw-r--r--   0        0        0     3051 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/orderform/json_orderform_parser.py
+-rw-r--r--   0        0        0     6419 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/orderform/orderform_parser.py
+-rw-r--r--   0        0        0      252 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/orderform/utils.py
+-rw-r--r--   0        0        0     2537 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/osticket.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/scout/__init__.py
+-rw-r--r--   0        0        0     3177 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/scout/scout_export.py
+-rw-r--r--   0        0        0    11108 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/scout/scoutapi.py
+-rw-r--r--   0        0        0      444 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/scout/validators.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0        0        0     3457 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/sequencing_metrics_parser/api.py
+-rw-r--r--   0        0        0      923 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/sequencing_metrics_parser/models.py
+-rw-r--r--   0        0        0     6658 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/sequencing_metrics_parser/parser.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/slurm/__init__.py
+-rw-r--r--   0        0        0     1277 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/slurm/sbatch.py
+-rw-r--r--   0        0        0     3559 2024-04-25 12:07:50.747335 cg-60.4.1/cg/apps/slurm/slurm_api.py
+-rw-r--r--   0        0        0       32 2024-04-25 12:07:50.751335 cg-60.4.1/cg/apps/tb/__init__.py
+-rw-r--r--   0        0        0     7995 2024-04-25 12:07:50.751335 cg-60.4.1/cg/apps/tb/api.py
+-rw-r--r--   0        0        0      152 2024-04-25 12:07:50.751335 cg-60.4.1/cg/apps/tb/dto/create_job_request.py
+-rw-r--r--   0        0        0      250 2024-04-25 12:07:50.751335 cg-60.4.1/cg/apps/tb/dto/summary_response.py
+-rw-r--r--   0        0        0     1305 2024-04-25 12:07:50.751335 cg-60.4.1/cg/apps/tb/models.py
+-rw-r--r--   0        0        0      305 2024-04-25 12:07:50.751335 cg-60.4.1/cg/apps/tb/validators.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/__init__.py
+-rw-r--r--   0        0        0    11558 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/add.py
+-rw-r--r--   0        0        0     2653 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/archive.py
+-rw-r--r--   0        0        0    10118 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/backup.py
+-rw-r--r--   0        0        0     3852 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/base.py
+-rw-r--r--   0        0        0    10506 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/clean.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/compress/__init__.py
+-rw-r--r--   0        0        0     2135 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/compress/base.py
+-rw-r--r--   0        0        0     6706 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/compress/fastq.py
+-rw-r--r--   0        0        0     8163 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/compress/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/delete/__init__.py
+-rw-r--r--   0        0        0      564 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/delete/base.py
+-rw-r--r--   0        0        0     4603 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/delete/case.py
+-rw-r--r--   0        0        0     1884 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/delete/cases.py
+-rw-r--r--   0        0        0     2633 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/delete/observations.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/deliver/__init__.py
+-rw-r--r--   0        0        0     6030 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/deliver/base.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/demultiplex/__init__.py
+-rw-r--r--   0        0        0      829 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/demultiplex/base.py
+-rw-r--r--   0        0        0     4905 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py
+-rw-r--r--   0        0        0     7726 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/demultiplex/demux.py
+-rw-r--r--   0        0        0     1473 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/demultiplex/finish.py
+-rw-r--r--   0        0        0     3119 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/demultiplex/sample_sheet.py
+-rw-r--r--   0        0        0     2995 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/downsample.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/generate/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/generate/base.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/generate/report/__init__.py
+-rw-r--r--   0        0        0     4636 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/generate/report/base.py
+-rw-r--r--   0        0        0      854 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/generate/report/options.py
+-rw-r--r--   0        0        0     5340 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/generate/report/utils.py
+-rw-r--r--   0        0        0     8327 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/get.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/set/__init__.py
+-rw-r--r--   0        0        0     9856 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/set/base.py
+-rw-r--r--   0        0        0     4384 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/set/case.py
+-rw-r--r--   0        0        0     2595 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/set/cases.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/store/__init__.py
+-rw-r--r--   0        0        0     1093 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/store/base.py
+-rw-r--r--   0        0        0     6191 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/store/store.py
+-rw-r--r--   0        0        0     1761 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/transfer.py
+-rw-r--r--   0        0        0        1 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/__init__.py
+-rw-r--r--   0        0        0     5706 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/base.py
+-rw-r--r--   0        0        0     5503 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/clinical_delivery.py
+-rw-r--r--   0        0        0     1175 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/coverage.py
+-rw-r--r--   0        0        0     1528 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/delivery_report.py
+-rw-r--r--   0        0        0     4022 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/fohm.py
+-rw-r--r--   0        0        0     1463 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/genotype.py
+-rw-r--r--   0        0        0     1885 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/gens.py
+-rw-r--r--   0        0        0      584 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/gisaid.py
+-rw-r--r--   0        0        0     2645 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/mutacc.py
+-rw-r--r--   0        0        0       23 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/nipt/__init__.py
+-rw-r--r--   0        0        0     3006 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/nipt/base.py
+-rw-r--r--   0        0        0     2275 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/nipt/ftp.py
+-rw-r--r--   0        0        0     1596 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/nipt/statina.py
+-rw-r--r--   0        0        0      112 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/observations/__init__.py
+-rw-r--r--   0        0        0     2672 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/observations/observations.py
+-rw-r--r--   0        0        0     2904 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/observations/utils.py
+-rw-r--r--   0        0        0     9970 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/scout.py
+-rw-r--r--   0        0        0      650 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/utils.py
+-rw-r--r--   0        0        0     1667 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/upload/validate.py
+-rw-r--r--   0        0        0      105 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/utils.py
+-rw-r--r--   0        0        0       18 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/balsamic/__init__.py
+-rw-r--r--   0        0        0     8925 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/balsamic/base.py
+-rw-r--r--   0        0        0     1980 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/balsamic/options.py
+-rw-r--r--   0        0        0      881 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/balsamic/pon.py
+-rw-r--r--   0        0        0     1162 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/balsamic/qc.py
+-rw-r--r--   0        0        0     1177 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/balsamic/umi.py
+-rw-r--r--   0        0        0     1342 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/base.py
+-rw-r--r--   0        0        0    12379 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/commands.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/fastq/__init__.py
+-rw-r--r--   0        0        0     1490 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/fastq/base.py
+-rw-r--r--   0        0        0     1787 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/fastq/fastq_service.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0        0        0     4177 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/fluffy/base.py
+-rw-r--r--   0        0        0       22 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/jasen/__init__.py
+-rw-r--r--   0        0        0      535 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/jasen/base.py
+-rw-r--r--   0        0        0       22 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/microsalt/__init__.py
+-rw-r--r--   0        0        0     7810 2024-04-25 12:07:50.751335 cg-60.4.1/cg/cli/workflow/microsalt/base.py
+-rw-r--r--   0        0        0       22 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/mip/__init__.py
+-rw-r--r--   0        0        0     6596 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/mip/base.py
+-rw-r--r--   0        0        0     1268 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/mip/options.py
+-rw-r--r--   0        0        0       22 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/mip_dna/__init__.py
+-rw-r--r--   0        0        0     1013 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/mip_dna/base.py
+-rw-r--r--   0        0        0       22 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/mip_rna/__init__.py
+-rw-r--r--   0        0        0      916 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/mip_rna/base.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/mutant/__init__.py
+-rw-r--r--   0        0        0     3413 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/mutant/base.py
+-rw-r--r--   0        0        0     9010 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/nf_analysis.py
+-rw-r--r--   0        0        0       22 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/raredisease/__init__.py
+-rw-r--r--   0        0        0     2210 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/raredisease/base.py
+-rw-r--r--   0        0        0       22 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/rnafusion/__init__.py
+-rw-r--r--   0        0        0     1179 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/rnafusion/base.py
+-rw-r--r--   0        0        0       22 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/taxprofiler/__init__.py
+-rw-r--r--   0        0        0     1211 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/taxprofiler/base.py
+-rw-r--r--   0        0        0     1111 2024-04-25 12:07:50.755335 cg-60.4.1/cg/cli/workflow/tomte/base.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.755335 cg-60.4.1/cg/clients/__init__.py
+-rw-r--r--   0        0        0     1363 2024-04-25 12:07:50.755335 cg-60.4.1/cg/clients/arnold/api.py
+-rw-r--r--   0        0        0      160 2024-04-25 12:07:50.755335 cg-60.4.1/cg/clients/arnold/dto/create_case_request.py
+-rw-r--r--   0        0        0      384 2024-04-25 12:07:50.755335 cg-60.4.1/cg/clients/arnold/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.755335 cg-60.4.1/cg/clients/janus/__init__.py
+-rw-r--r--   0        0        0     1246 2024-04-25 12:07:50.755335 cg-60.4.1/cg/clients/janus/api.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.755335 cg-60.4.1/cg/clients/janus/dto/__init__.py
+-rw-r--r--   0        0        0      503 2024-04-25 12:07:50.755335 cg-60.4.1/cg/clients/janus/dto/create_qc_metrics_request.py
+-rw-r--r--   0        0        0      420 2024-04-25 12:07:50.755335 cg-60.4.1/cg/clients/janus/exceptions.py
+-rw-r--r--   0        0        0      937 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/__init__.py
+-rw-r--r--   0        0        0      253 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/archiving.py
+-rw-r--r--   0        0        0       35 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/backup.py
+-rw-r--r--   0        0        0      769 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/bcl_convert_metrics.py
+-rw-r--r--   0        0        0      469 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/compression.py
+-rw-r--r--   0        0        0     6613 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/constants.py
+-rw-r--r--   0        0        0     6033 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/delivery.py
+-rw-r--r--   0        0        0     7387 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/demultiplexing.py
+-rw-r--r--   0        0        0     1422 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/encryption.py
+-rw-r--r--   0        0        0      372 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/extraction.py
+-rw-r--r--   0        0        0     2157 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/gene_panel.py
+-rw-r--r--   0        0        0     6704 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/housekeeper_tags.py
+-rw-r--r--   0        0        0       95 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/invoice.py
+-rw-r--r--   0        0        0     5815 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/lims.py
+-rw-r--r--   0        0        0      743 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/metrics.py
+-rw-r--r--   0        0        0      231 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/nanopore_files.py
+-rw-r--r--   0        0        0      650 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/nextflow.py
+-rw-r--r--   0        0        0     1529 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/nf_analysis.py
+-rw-r--r--   0        0        0       19 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/nipt.py
+-rw-r--r--   0        0        0     2257 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/observations.py
+-rw-r--r--   0        0        0     1216 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/orderforms.py
+-rw-r--r--   0        0        0       96 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/paths.py
+-rw-r--r--   0        0        0      266 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/pdc.py
+-rw-r--r--   0        0        0      160 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/pedigree.py
+-rw-r--r--   0        0        0     1044 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/priority.py
+-rw-r--r--   0        0        0       79 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/process.py
+-rw-r--r--   0        0        0     5474 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/report.py
+-rw-r--r--   0        0        0      569 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/sample_sources.py
+-rw-r--r--   0        0        0     3111 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/scout.py
+-rw-r--r--   0        0        0     1669 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/sequencing.py
+-rw-r--r--   0        0        0      313 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/slurm.py
+-rw-r--r--   0        0        0      529 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/subject.py
+-rw-r--r--   0        0        0       55 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/symbols.py
+-rw-r--r--   0        0        0      435 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/tb.py
+-rw-r--r--   0        0        0      161 2024-04-25 12:07:50.755335 cg-60.4.1/cg/constants/time.py
+-rw-r--r--   0        0        0     6639 2024-04-25 12:07:50.755335 cg-60.4.1/cg/exc.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/__init__.py
+-rw-r--r--   0        0        0     1037 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/api.py
+-rw-r--r--   0        0        0      621 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/config.py
+-rw-r--r--   0        0        0     2978 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/controller.py
+-rw-r--r--   0        0        0     1763 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/csv.py
+-rw-r--r--   0        0        0      210 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/gzip.py
+-rw-r--r--   0        0        0      662 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/json.py
+-rw-r--r--   0        0        0      525 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/png.py
+-rw-r--r--   0        0        0     1094 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/txt.py
+-rw-r--r--   0        0        0      552 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/validate_path.py
+-rw-r--r--   0        0        0     1289 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/xml.py
+-rw-r--r--   0        0        0     1153 2024-04-25 12:07:50.755335 cg-60.4.1/cg/io/yaml.py
+-rw-r--r--   0        0        0      281 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/archive/__init__.py
+-rw-r--r--   0        0        0    15193 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/archive/archive.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/archive/ddn/__init__.py
+-rw-r--r--   0        0        0     1727 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/archive/ddn/constants.py
+-rw-r--r--   0        0        0    10852 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/archive/ddn/ddn_data_flow_client.py
+-rw-r--r--   0        0        0     3704 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/archive/ddn/models.py
+-rw-r--r--   0        0        0     1250 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/archive/ddn/utils.py
+-rw-r--r--   0        0        0     2024 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/archive/models.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/backup/__init__.py
+-rw-r--r--   0        0        0    17426 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/backup/backup.py
+-rw-r--r--   0        0        0     5397 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/backup/pdc.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/clean/__init__.py
+-rw-r--r--   0        0        0     3901 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/clean/api.py
+-rw-r--r--   0        0        0     7738 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/clean/clean_flow_cells.py
+-rw-r--r--   0        0        0     1841 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/clean/clean_retrieved_spring_files.py
+-rw-r--r--   0        0        0       34 2024-04-25 12:07:50.755335 cg-60.4.1/cg/meta/compress/__init__.py
+-rw-r--r--   0        0        0    14557 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/compress/compress.py
+-rw-r--r--   0        0        0     4947 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/compress/files.py
+-rw-r--r--   0        0        0       77 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/deliver/__init__.py
+-rw-r--r--   0        0        0    14905 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/deliver/deliver.py
+-rw-r--r--   0        0        0     4502 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/deliver/deliver_ticket.py
+-rw-r--r--   0        0        0      904 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/deliver/fastq_path_generator.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/delivery/__init__.py
+-rw-r--r--   0        0        0     8458 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/delivery/delivery.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/demultiplex/__init__.py
+-rw-r--r--   0        0        0     2592 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/demultiplex/combine_sequencing_metrics.py
+-rw-r--r--   0        0        0     5719 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/demultiplex/demux_post_processing.py
+-rw-r--r--   0        0        0     4135 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/demultiplex/files.py
+-rw-r--r--   0        0        0     7777 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/demultiplex/housekeeper_storage_functions.py
+-rw-r--r--   0        0        0     6126 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/demultiplex/status_db_storage_functions.py
+-rw-r--r--   0        0        0    10690 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/demultiplex/utils.py
+-rw-r--r--   0        0        0     2855 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/demultiplex/validation.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/encryption/__init__.py
+-rw-r--r--   0        0        0    20271 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/encryption/encryption.py
+-rw-r--r--   0        0        0      537 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/encryption/sbatch.py
+-rw-r--r--   0        0        0    10922 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/invoice.py
+-rw-r--r--   0        0        0     2360 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/meta.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/observations/__init__.py
+-rw-r--r--   0        0        0     6008 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/observations/balsamic_observations_api.py
+-rw-r--r--   0        0        0     5277 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/observations/mip_dna_observations_api.py
+-rw-r--r--   0        0        0     5364 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/observations/observations_api.py
+-rw-r--r--   0        0        0       27 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/__init__.py
+-rw-r--r--   0        0        0     3637 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/api.py
+-rw-r--r--   0        0        0      121 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/balsamic_qc_submitter.py
+-rw-r--r--   0        0        0      107 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/balsamic_submitter.py
+-rw-r--r--   0        0        0      122 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/balsamic_umi_submitter.py
+-rw-r--r--   0        0        0    15262 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/case_submitter.py
+-rw-r--r--   0        0        0     6102 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/fastq_submitter.py
+-rw-r--r--   0        0        0      105 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/fluffy_submitter.py
+-rw-r--r--   0        0        0     1254 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/lims.py
+-rw-r--r--   0        0        0     5782 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/metagenome_submitter.py
+-rw-r--r--   0        0        0     6337 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/microbial_submitter.py
+-rw-r--r--   0        0        0      123 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/microsalt_submitter.py
+-rw-r--r--   0        0        0      105 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/mip_dna_submitter.py
+-rw-r--r--   0        0        0      105 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/mip_rna_submitter.py
+-rw-r--r--   0        0        0     7761 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/pool_submitter.py
+-rw-r--r--   0        0        0      102 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/rml_submitter.py
+-rw-r--r--   0        0        0      718 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/rnafusion_submitter.py
+-rw-r--r--   0        0        0     1268 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/sars_cov_2_submitter.py
+-rw-r--r--   0        0        0     1754 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/submitter.py
+-rw-r--r--   0        0        0     7880 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/orders/ticket_handler.py
+-rw-r--r--   0        0        0     4105 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/qc_metrics/collect_qc_metrics.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/__init__.py
+-rw-r--r--   0        0        0     8168 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/balsamic.py
+-rw-r--r--   0        0        0      562 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/balsamic_qc.py
+-rw-r--r--   0        0        0      717 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/balsamic_umi.py
+-rw-r--r--   0        0        0     4171 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/field_validators.py
+-rw-r--r--   0        0        0     6620 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/mip_dna.py
+-rw-r--r--   0        0        0    18543 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/report_api.py
+-rw-r--r--   0        0        0     5625 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/rnafusion.py
+-rw-r--r--   0        0        0     1911 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/delivery-report.html
+-rw-r--r--   0        0        0     4236 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/data_analysis/data_analysis.html
+-rw-r--r--   0        0        0     1049 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/data_analysis/limitations.html
+-rw-r--r--   0        0        0     3351 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html
+-rw-r--r--   0        0        0     1364 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html
+-rw-r--r--   0        0        0      753 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html
+-rw-r--r--   0        0        0     3284 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html
+-rw-r--r--   0        0        0     3670 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html
+-rw-r--r--   0        0        0     2332 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/header.html
+-rw-r--r--   0        0        0     2066 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/order.html
+-rw-r--r--   0        0        0     2243 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/sample_prep.html
+-rw-r--r--   0        0        0      472 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/ticket_system.html
+-rw-r--r--   0        0        0     1165 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html
+-rw-r--r--   0        0        0     1538 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html
+-rw-r--r--   0        0        0      428 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/uploaded_files/rnafusion_uploaded_files.html
+-rw-r--r--   0        0        0     4266 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html
+-rw-r--r--   0        0        0       80 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/partials/footer.html
+-rw-r--r--   0        0        0      172 2024-04-25 12:07:50.759335 cg-60.4.1/cg/meta/report/templates/partials/signature.html
+-rw-r--r--   0        0        0   232803 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/report/templates/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0       33 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/report/templates/static/css/custom.css
+-rw-r--r--   0        0        0    30068 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/report/templates/static/images/SWEDAC_logo.png
+-rw-r--r--   0        0        0     3925 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/report/tomte.py
+-rw-r--r--   0        0        0       32 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/rsync/__init__.py
+-rw-r--r--   0        0        0    12291 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/rsync/rsync_api.py
+-rw-r--r--   0        0        0      387 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/rsync/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/tar/__init__.py
+-rw-r--r--   0        0        0     1694 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/tar/tar.py
+-rw-r--r--   0        0        0       71 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/transfer/__init__.py
+-rw-r--r--   0        0        0    10016 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/transfer/external_data.py
+-rw-r--r--   0        0        0     5814 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/transfer/lims.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/balsamic/__init__.py
+-rw-r--r--   0        0        0     3107 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/balsamic/balsamic.py
+-rw-r--r--   0        0        0     2224 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/coverage.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/fohm/__init__.py
+-rw-r--r--   0        0        0    12102 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/fohm/fohm.py
+-rw-r--r--   0        0        0       30 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/gisaid/__init__.py
+-rw-r--r--   0        0        0      928 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/gisaid/constants.py
+-rw-r--r--   0        0        0    13521 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/gisaid/gisaid.py
+-rw-r--r--   0        0        0     3312 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/gisaid/models.py
+-rw-r--r--   0        0        0     5310 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/gt.py
+-rw-r--r--   0        0        0      898 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/microsalt/microsalt_upload_api.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/mip/__init__.py
+-rw-r--r--   0        0        0     2546 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/mip/mip_dna.py
+-rw-r--r--   0        0        0     1400 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/mip/mip_rna.py
+-rw-r--r--   0        0        0     7294 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/mutacc.py
+-rw-r--r--   0        0        0     1853 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/nf_analysis.py
+-rw-r--r--   0        0        0       32 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/nipt/__init__.py
+-rw-r--r--   0        0        0      696 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/nipt/models.py
+-rw-r--r--   0        0        0     8106 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/nipt/nipt.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/scout/__init__.py
+-rw-r--r--   0        0        0     4009 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/scout/balsamic_config_builder.py
+-rw-r--r--   0        0        0     1491 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/scout/balsamic_umi_config_builder.py
+-rw-r--r--   0        0        0     3322 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/scout/hk_tags.py
+-rw-r--r--   0        0        0     9103 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/scout/mip_config_builder.py
+-rw-r--r--   0        0        0     3495 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/scout/rnafusion_config_builder.py
+-rw-r--r--   0        0        0     7231 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/scout/scout_config_builder.py
+-rw-r--r--   0        0        0    23146 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/scout/uploadscoutapi.py
+-rw-r--r--   0        0        0     3197 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/upload/upload_api.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/__init__.py
+-rw-r--r--   0        0        0    31068 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/analysis.py
+-rw-r--r--   0        0        0    27751 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/balsamic.py
+-rw-r--r--   0        0        0     2700 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/balsamic_pon.py
+-rw-r--r--   0        0        0      553 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/balsamic_qc.py
+-rw-r--r--   0        0        0      556 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/balsamic_umi.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/downsample/__init__.py
+-rw-r--r--   0        0        0     3922 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/downsample/downsample.py
+-rw-r--r--   0        0        0      711 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/downsample/sbatch.py
+-rw-r--r--   0        0        0     8913 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/fastq.py
+-rw-r--r--   0        0        0    10603 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/fluffy.py
+-rw-r--r--   0        0        0      521 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/jasen.py
+-rw-r--r--   0        0        0       70 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/microsalt/__init__.py
+-rw-r--r--   0        0        0      116 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/microsalt/constants.py
+-rw-r--r--   0        0        0      174 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/microsalt/metrics_parser/__init__.py
+-rw-r--r--   0        0        0      366 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/microsalt/metrics_parser/metrics_parser.py
+-rw-r--r--   0        0        0      903 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/microsalt/metrics_parser/models.py
+-rw-r--r--   0        0        0    13173 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/microsalt/microsalt.py
+-rw-r--r--   0        0        0      113 2024-04-25 12:07:50.763335 cg-60.4.1/cg/meta/workflow/microsalt/quality_controller/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/microsalt/quality_controller/models.py
+-rw-r--r--   0        0        0     5697 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/microsalt/quality_controller/quality_controller.py
+-rw-r--r--   0        0        0     1217 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/microsalt/quality_controller/report_generator.py
+-rw-r--r--   0        0        0     2373 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/microsalt/quality_controller/result_logger.py
+-rw-r--r--   0        0        0     5641 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/microsalt/quality_controller/utils.py
+-rw-r--r--   0        0        0     1220 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/microsalt/utils.py
+-rw-r--r--   0        0        0    12611 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/mip.py
+-rw-r--r--   0        0        0     2948 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/mip_dna.py
+-rw-r--r--   0        0        0     2124 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/mip_rna.py
+-rw-r--r--   0        0        0    10974 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/mutant.py
+-rw-r--r--   0        0        0    37948 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/nf_analysis.py
+-rw-r--r--   0        0        0     6161 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/nf_handlers.py
+-rw-r--r--   0        0        0     6357 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/prepare_fastq.py
+-rw-r--r--   0        0        0     4965 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/raredisease.py
+-rw-r--r--   0        0        0     5403 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/rnafusion.py
+-rw-r--r--   0        0        0     4607 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/taxprofiler.py
+-rw-r--r--   0        0        0     3576 2024-04-25 12:07:50.767335 cg-60.4.1/cg/meta/workflow/tomte.py
+-rw-r--r--   0        0        0      113 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/__init__.py
+-rw-r--r--   0        0        0      367 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/analysis.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/balsamic/__init__.py
+-rw-r--r--   0        0        0      459 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/balsamic/analysis.py
+-rw-r--r--   0        0        0     4550 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/balsamic/config.py
+-rw-r--r--   0        0        0     1986 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/balsamic/metrics.py
+-rw-r--r--   0        0        0    17539 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/cg_config.py
+-rw-r--r--   0        0        0     4302 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/compression_data.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/deliverables/__init__.py
+-rw-r--r--   0        0        0     5213 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/deliverables/metric_deliverables.py
+-rw-r--r--   0        0        0      243 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/delivery/delivery.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/demultiplex/__init__.py
+-rw-r--r--   0        0        0    12040 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/demultiplex/run_parameters.py
+-rw-r--r--   0        0        0      539 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/demultiplex/sbatch.py
+-rw-r--r--   0        0        0     7006 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/downsample/downsample_data.py
+-rw-r--r--   0        0        0      255 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/email.py
+-rw-r--r--   0        0        0     1046 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/fastq.py
+-rw-r--r--   0        0        0     2157 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/file_data.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/flow_cell/__init__.py
+-rw-r--r--   0        0        0     9984 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/flow_cell/flow_cell.py
+-rw-r--r--   0        0        0      317 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/flow_cell/utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/invoice/__init__.py
+-rw-r--r--   0        0        0     1254 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/invoice/invoice.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/lims/__init__.py
+-rw-r--r--   0        0        0     2019 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/lims/sample.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/mip/__init__.py
+-rw-r--r--   0        0        0      337 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/mip/mip_analysis.py
+-rw-r--r--   0        0        0     1564 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/mip/mip_config.py
+-rw-r--r--   0        0        0     4696 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/mip/mip_metrics_deliverables.py
+-rw-r--r--   0        0        0     2550 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/mip/mip_sample_info.py
+-rw-r--r--   0        0        0     2472 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/nf_analysis.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/observations/__init__.py
+-rw-r--r--   0        0        0      688 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/observations/input_files.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/__init__.py
+-rw-r--r--   0        0        0     2659 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/constants.py
+-rw-r--r--   0        0        0     5604 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/excel_sample.py
+-rw-r--r--   0        0        0      898 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/json_sample.py
+-rw-r--r--   0        0        0     1449 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/order.py
+-rw-r--r--   0        0        0      811 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/orderform_schema.py
+-rw-r--r--   0        0        0     4212 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/sample_base.py
+-rw-r--r--   0        0        0     9668 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/samples.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/validators/__init__.py
+-rw-r--r--   0        0        0     2300 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/validators/excel_sample_validators.py
+-rw-r--r--   0        0        0      576 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/validators/json_sample_validators.py
+-rw-r--r--   0        0        0       71 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/orders/validators/sample_base_validators.py
+-rw-r--r--   0        0        0      101 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/qc_metrics.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/raredisease/__init__.py
+-rw-r--r--   0        0        0     1875 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/raredisease/raredisease.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/report/__init__.py
+-rw-r--r--   0        0        0     7461 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/report/metadata.py
+-rw-r--r--   0        0        0     6180 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/report/report.py
+-rw-r--r--   0        0        0     5221 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/report/sample.py
+-rw-r--r--   0        0        0     3004 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/report/validators.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/rnafusion/__init__.py
+-rw-r--r--   0        0        0     1865 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/rnafusion/rnafusion.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/scout/__init__.py
+-rw-r--r--   0        0        0     4783 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/scout/scout_load_config.py
+-rw-r--r--   0        0        0      116 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/scout/validators.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/slurm/__init__.py
+-rw-r--r--   0        0        0      617 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/slurm/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/taxprofiler/__init__.py
+-rw-r--r--   0        0        0     2443 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/taxprofiler/taxprofiler.py
+-rw-r--r--   0        0        0     2588 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/tomte/tomte.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/workflow/__init__.py
+-rw-r--r--   0        0        0      685 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/workflow/mutant.py
+-rw-r--r--   0        0        0       70 2024-04-25 12:07:50.767335 cg-60.4.1/cg/models/workflow/validators.py
+-rw-r--r--   0        0        0      842 2024-04-25 12:07:50.771335 cg-60.4.1/cg/resources/__init__.py
+-rw-r--r--   0        0        0     3493 2024-04-25 12:07:50.771335 cg-60.4.1/cg/resources/rnafusion_bundle_filenames.yaml
+-rw-r--r--   0        0        0     2434 2024-04-25 12:07:50.771335 cg-60.4.1/cg/resources/taxprofiler_bundle_filenames.yaml
+-rw-r--r--   0        0        0     3732 2024-04-25 12:07:50.771335 cg-60.4.1/cg/resources/tomte_bundle_filenames.yaml
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/__init__.py
+-rw-r--r--   0        0        0    20241 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/admin.py
+-rw-r--r--   0        0        0    22743 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/api.py
+-rw-r--r--   0        0        0     4887 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/app.py
+-rw-r--r--   0        0        0       48 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/auto.py
+-rw-r--r--   0        0        0     1184 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/config.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/dto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/dto/delivery_message/__init__.py
+-rw-r--r--   0        0        0      300 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/dto/delivery_message/delivery_message_request.py
+-rw-r--r--   0        0        0      183 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/dto/delivery_message/delivery_message_response.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/dto/orders/__init__.py
+-rw-r--r--   0        0        0      165 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/dto/orders/order_delivery_update_request.py
+-rw-r--r--   0        0        0       91 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/dto/orders/order_patch_request.py
+-rw-r--r--   0        0        0      662 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/dto/orders/orders_request.py
+-rw-r--r--   0        0        0      413 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/dto/orders/orders_response.py
+-rw-r--r--   0        0        0     2598 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/ext.py
+-rw-r--r--   0        0        0       29 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/invoices/__init__.py
+-rw-r--r--   0        0        0     4793 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/invoices/templates/invoices/index.html
+-rw-r--r--   0        0        0     8171 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/invoices/templates/invoices/invoice.html
+-rw-r--r--   0        0        0     2838 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/invoices/templates/invoices/layout.html
+-rw-r--r--   0        0        0     4956 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/invoices/templates/invoices/new.html
+-rw-r--r--   0        0        0     7708 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/invoices/views.py
+-rw-r--r--   0        0        0      354 2024-04-25 12:07:50.771335 cg-60.4.1/cg/server/templates/admin/index.html
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/analysis_service/__init__.py
+-rw-r--r--   0        0        0      482 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/analysis_service/analysis_service.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/__init__.py
+-rw-r--r--   0        0        0     2531 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/delivery_message_service.py
+-rw-r--r--   0        0        0      792 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/__init__.py
+-rw-r--r--   0        0        0     1366 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/analysis_scout_message.py
+-rw-r--r--   0        0        0      791 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/covid_message.py
+-rw-r--r--   0        0        0      189 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/delivery_message.py
+-rw-r--r--   0        0        0     1391 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/fastq_analysis_scout_message.py
+-rw-r--r--   0        0        0      535 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/fastq_message.py
+-rw-r--r--   0        0        0     1358 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/fastq_scout_message.py
+-rw-r--r--   0        0        0      604 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/microsalt_mwr_message.py
+-rw-r--r--   0        0        0      592 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/microsalt_mwx_message.py
+-rw-r--r--   0        0        0      903 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/scout_message.py
+-rw-r--r--   0        0        0      512 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/statina_message.py
+-rw-r--r--   0        0        0      779 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/messages/utils.py
+-rw-r--r--   0        0        0     3300 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/delivery_message/utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/fastq_file_service/__init__.py
+-rw-r--r--   0        0        0      101 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/fastq_file_service/exceptions.py
+-rw-r--r--   0        0        0     1092 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/fastq_file_service/fastq_file_service.py
+-rw-r--r--   0        0        0     2991 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/fastq_file_service/utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/orders/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/orders/order_service/__init__.py
+-rw-r--r--   0        0        0     2684 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/orders/order_service/order_service.py
+-rw-r--r--   0        0        0     1214 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/orders/order_service/utils.py
+-rw-r--r--   0        0        0       94 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/orders/order_status_service/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/orders/order_status_service/dto/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/orders/order_status_service/dto/case_summary.py
+-rw-r--r--   0        0        0      289 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/orders/order_status_service/dto/order_summary.py
+-rw-r--r--   0        0        0     1768 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/orders/order_status_service/order_summary_service.py
+-rw-r--r--   0        0        0     1737 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/orders/order_status_service/utils.py
+-rw-r--r--   0        0        0       95 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/quality_controller/__init__.py
+-rw-r--r--   0        0        0     1819 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/quality_controller/quality_checks/checks.py
+-rw-r--r--   0        0        0     4987 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/quality_controller/quality_checks/utils.py
+-rw-r--r--   0        0        0     1040 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/quality_controller/quality_controller_service.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/slurm_service/__init__.py
+-rw-r--r--   0        0        0      703 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/slurm_service/slurm_cli_service.py
+-rw-r--r--   0        0        0      242 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/slurm_service/slurm_service.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/slurm_upload_service/__init__.py
+-rw-r--r--   0        0        0      175 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/slurm_upload_service/slurm_upload_config.py
+-rw-r--r--   0        0        0     2074 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/slurm_upload_service/slurm_upload_service.py
+-rw-r--r--   0        0        0      203 2024-04-25 12:07:50.771335 cg-60.4.1/cg/services/slurm_upload_service/utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/__init__.py
+-rw-r--r--   0        0        0     4650 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/base.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/crud/__init__.py
+-rw-r--r--   0        0        0    13100 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/crud/create.py
+-rw-r--r--   0        0        0     2144 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/crud/delete.py
+-rw-r--r--   0        0        0    60036 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/crud/read.py
+-rw-r--r--   0        0        0     1121 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/crud/update.py
+-rw-r--r--   0        0        0     1662 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/database.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/filters/__init__.py
+-rw-r--r--   0        0        0     5371 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/filters/status_analysis_filters.py
+-rw-r--r--   0        0        0     1712 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/filters/status_application_filters.py
+-rw-r--r--   0        0        0     1440 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/filters/status_application_limitations_filters.py
+-rw-r--r--   0        0        0     2523 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/filters/status_application_version_filters.py
+-rw-r--r--   0        0        0     1390 2024-04-25 12:07:50.771335 cg-60.4.1/cg/store/filters/status_bed_filters.py
+-rw-r--r--   0        0        0     1317 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_bed_version_filters.py
+-rw-r--r--   0        0        0    10787 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_case_filters.py
+-rw-r--r--   0        0        0     3272 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_case_sample_filters.py
+-rw-r--r--   0        0        0      903 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_collaboration_filters.py
+-rw-r--r--   0        0        0     1412 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_customer_filters.py
+-rw-r--r--   0        0        0     1880 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_flow_cell_filters.py
+-rw-r--r--   0        0        0     1255 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_invoice_filters.py
+-rw-r--r--   0        0        0     2792 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_metrics_filters.py
+-rw-r--r--   0        0        0     3225 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_order_filters.py
+-rw-r--r--   0        0        0      851 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_organism_filters.py
+-rw-r--r--   0        0        0      783 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_panel_filters.py
+-rw-r--r--   0        0        0     3923 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_pool_filters.py
+-rw-r--r--   0        0        0     8660 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_sample_filters.py
+-rw-r--r--   0        0        0      731 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/filters/status_user_filters.py
+-rw-r--r--   0        0        0    36081 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/models.py
+-rw-r--r--   0        0        0      593 2024-04-25 12:07:50.775335 cg-60.4.1/cg/store/store.py
+-rw-r--r--   0        0        0       30 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/__init__.py
+-rw-r--r--   0        0        0      187 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/calculations.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/checksum/__init__.py
+-rw-r--r--   0        0        0     1579 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/checksum/checksum.py
+-rw-r--r--   0        0        0     1655 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/click/EnumChoice.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/click/__init__.py
+-rw-r--r--   0        0        0     4910 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/commands.py
+-rw-r--r--   0        0        0     1811 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/date.py
+-rw-r--r--   0        0        0      635 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/dict.py
+-rw-r--r--   0        0        0     2111 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/dispatcher.py
+-rw-r--r--   0        0        0     1251 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/email.py
+-rw-r--r--   0        0        0      134 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/enums.py
+-rw-r--r--   0        0        0     3178 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/files.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/flask/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/flask/enum.py
+-rw-r--r--   0        0        0      233 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/flow_cell.py
+-rw-r--r--   0        0        0      834 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/time.py
+-rw-r--r--   0        0        0     1410 2024-04-25 12:07:50.775335 cg-60.4.1/cg/utils/utils.py
+-rw-r--r--   0        0        0     1697 2024-04-25 12:07:50.775335 cg-60.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.775335 cg-60.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     1158 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/conftest.py
+-rw-r--r--   0        0        0      231 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/coverage/conftest.py
+-rw-r--r--   0        0        0     6188 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/coverage/test_coverage.py
+-rw-r--r--   0        0        0     1693 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/crunchy/conftest.py
+-rw-r--r--   0        0        0     5438 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/crunchy/test_compress_fastq.py
+-rw-r--r--   0        0        0     2283 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/crunchy/test_config.py
+-rw-r--r--   0        0        0    14032 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/crunchy/test_crunchy.py
+-rw-r--r--   0        0        0     9109 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/crunchy/test_spring_decompression.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/__init__.py
+-rw-r--r--   0        0        0     4994 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/conftest.py
+-rw-r--r--   0        0        0     4010 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0        0        0     7986 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/test_demultiplex_api.py
+-rw-r--r--   0        0        0     4782 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/test_index.py
+-rw-r--r--   0        0        0     9468 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/test_override_cycles_validator.py
+-rw-r--r--   0        0        0     4042 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/test_read_sample_sheet.py
+-rw-r--r--   0        0        0    12389 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/test_sample_models.py
+-rw-r--r--   0        0        0      951 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/test_sample_sheet_creator.py
+-rw-r--r--   0        0        0     3175 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/test_sample_sheet_models.py
+-rw-r--r--   0        0        0    10932 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/test_sample_sheet_validator.py
+-rw-r--r--   0        0        0     4896 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/test_translate_sample_sheet.py
+-rw-r--r--   0        0        0     1450 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/demultiplex/test_validate.py
+-rw-r--r--   0        0        0     5094 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/downsample/test_downsample.py
+-rw-r--r--   0        0        0     1419 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/downsample/test_downsample_utils.py
+-rw-r--r--   0        0        0     1716 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/gens/test_gens_api.py
+-rw-r--r--   0        0        0     1950 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/gt/conftest.py
+-rw-r--r--   0        0        0     4276 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/gt/test_gt_api.py
+-rw-r--r--   0        0        0     1453 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/hk/conftest.py
+-rw-r--r--   0        0        0      684 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/hk/test__getattr__.py
+-rw-r--r--   0        0        0     1593 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/hk/test_add_file.py
+-rw-r--r--   0        0        0     3523 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/hk/test_bundles.py
+-rw-r--r--   0        0        0      871 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/hk/test_core.py
+-rw-r--r--   0        0        0    31172 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/hk/test_file.py
+-rw-r--r--   0        0        0     5080 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/hk/test_version.py
+-rw-r--r--   0        0        0     1840 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/lims/conftest.py
+-rw-r--r--   0        0        0     3197 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/lims/test_api.py
+-rw-r--r--   0        0        0     1451 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/lims/test_sample_sheet.py
+-rw-r--r--   0        0        0     9223 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/loqus/conftest.py
+-rw-r--r--   0        0        0     8994 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/loqus/test_loqusdb_api.py
+-rw-r--r--   0        0        0     2439 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/madeline/conftest.py
+-rw-r--r--   0        0        0     4653 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/madeline/test_madeline.py
+-rw-r--r--   0        0        0     3328 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/mip/conftest.py
+-rw-r--r--   0        0        0     2487 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/mip/test_config_mip.py
+-rw-r--r--   0        0        0      883 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/mutacc_auto/conftest.py
+-rw-r--r--   0        0        0     2473 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/mutacc_auto/test_mutacc_auto.py
+-rw-r--r--   0        0        0    11930 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/orderform/conftest.py
+-rw-r--r--   0        0        0     9484 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/orderform/test_excel_orderform_parser.py
+-rw-r--r--   0        0        0     4351 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/orderform/test_excel_sample_schema.py
+-rw-r--r--   0        0        0     1032 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/orderform/test_json_orderform_parser.py
+-rw-r--r--   0        0        0     2474 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/orderform/test_orderform_parser.py
+-rw-r--r--   0        0        0    16002 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/orderform/validators/test_excel_sample_validators.py
+-rw-r--r--   0        0        0     3670 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/scout/conftest.py
+-rw-r--r--   0        0        0     2269 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/scout/test_get_causative_variants.py
+-rw-r--r--   0        0        0     1376 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/scout/test_get_scout_cases.py
+-rw-r--r--   0        0        0     1840 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/scout/test_scout_load_config.py
+-rw-r--r--   0        0        0     7047 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/scout/test_scout_models.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0        0        0     2639 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/sequencing_metrics_parser/conftest.py
+-rw-r--r--   0        0        0     7069 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
+-rw-r--r--   0        0        0     2958 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/sequencing_metrics_parser/parsers/test_sequencing_metrics_parser_api.py
+-rw-r--r--   0        0        0     1131 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/slurm/conftest.py
+-rw-r--r--   0        0        0     4412 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/slurm/test_slurm_api.py
+-rw-r--r--   0        0        0      831 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/test_apps_environ.py
+-rw-r--r--   0        0        0      957 2024-04-25 12:07:50.779335 cg-60.4.1/tests/apps/test_osticket.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/add/__init__.py
+-rw-r--r--   0        0        0     1174 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/add/test_cli_add.py
+-rw-r--r--   0        0        0     2471 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/add/test_cli_add_customer.py
+-rw-r--r--   0        0        0     6841 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/add/test_cli_add_family.py
+-rw-r--r--   0        0        0     7588 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/add/test_cli_add_relationship.py
+-rw-r--r--   0        0        0     8382 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/add/test_cli_add_sample.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/backup/__init__.py
+-rw-r--r--   0        0        0      705 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/backup/conftest.py
+-rw-r--r--   0        0        0    11101 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/backup/test_backup_command.py
+-rw-r--r--   0        0        0     6865 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/clean/conftest.py
+-rw-r--r--   0        0        0     5536 2024-04-25 12:07:50.779335 cg-60.4.1/tests/cli/clean/test_balsamic_clean.py
+-rw-r--r--   0        0        0     2557 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/clean/test_clean_flow_cell.py
+-rw-r--r--   0        0        0     1830 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/clean/test_clean_hk_bundle_files.py
+-rw-r--r--   0        0        0     2098 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/clean/test_hk_bundle_files.py
+-rw-r--r--   0        0        0     4610 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/clean/test_hk_case_bundle_files.py
+-rw-r--r--   0        0        0     3585 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/clean/test_microbial_clean.py
+-rw-r--r--   0        0        0     1881 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/clean/test_rsync_past_run_dirs.py
+-rw-r--r--   0        0        0     9707 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/compress/conftest.py
+-rw-r--r--   0        0        0     7709 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/compress/test_cli_compress_fastq.py
+-rw-r--r--   0        0        0     1416 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/compress/test_cli_decompress_spring.py
+-rw-r--r--   0        0        0     5205 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/compress/test_compress_helpers.py
+-rw-r--r--   0        0        0     1239 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/compress/test_store_fastq.py
+-rw-r--r--   0        0        0     7558 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/conftest.py
+-rw-r--r--   0        0        0    12747 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/delete/test_cli_delete_case.py
+-rw-r--r--   0        0        0     1873 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/delete/test_cli_delete_cases.py
+-rw-r--r--   0        0        0     3794 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/deliver/conftest.py
+-rw-r--r--   0        0        0     4428 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/deliver/test_deliver_base.py
+-rw-r--r--   0        0        0     1166 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/deliver/test_rsync_base.py
+-rw-r--r--   0        0        0     8569 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/deliver/test_run_deliver_cmd.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/demultiplex/__init__.py
+-rw-r--r--   0        0        0     5109 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0        0        0     4773 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/demultiplex/test_demultiplex_flowcell.py
+-rw-r--r--   0        0        0     1607 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/demultiplex/test_finish_demux.py
+-rw-r--r--   0        0        0     2989 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/demultiplex/test_validate_sample_sheet.py
+-rw-r--r--   0        0        0     4423 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/demultiplex/test_verify_syncing.py
+-rw-r--r--   0        0        0     1585 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/downsample/test_cli_downsample.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/generate/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/generate/report/__init__.py
+-rw-r--r--   0        0        0     1622 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/generate/report/conftest.py
+-rw-r--r--   0        0        0     2477 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/generate/report/test_cli_delivery_report.py
+-rw-r--r--   0        0        0     2760 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/generate/report/test_utils.py
+-rw-r--r--   0        0        0      563 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/generate/test_cli_base.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/get/__init__.py
+-rw-r--r--   0        0        0      863 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/get/test_cli_get.py
+-rw-r--r--   0        0        0     1526 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/get/test_cli_get_analysis.py
+-rw-r--r--   0        0        0     1242 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/get/test_cli_get_case.py
+-rw-r--r--   0        0        0     6208 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/get/test_cli_get_flow_cell.py
+-rw-r--r--   0        0        0     8835 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/get/test_cli_get_sample.py
+-rw-r--r--   0        0        0     1364 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/set/conftest.py
+-rw-r--r--   0        0        0     7311 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/set/test_cli_set_case.py
+-rw-r--r--   0        0        0     1460 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/set/test_cli_set_cases.py
+-rw-r--r--   0        0        0     2016 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/set/test_cli_set_flowcell.py
+-rw-r--r--   0        0        0     1685 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/set/test_cli_set_list_keys.py
+-rw-r--r--   0        0        0    12450 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/set/test_cli_set_sample.py
+-rw-r--r--   0        0        0     6124 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/set/test_cli_set_samples.py
+-rw-r--r--   0        0        0     7015 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/store/test_store.py
+-rw-r--r--   0        0        0     2332 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/test_base.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/__init__.py
+-rw-r--r--   0        0        0    10057 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/conftest.py
+-rw-r--r--   0        0        0     2295 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/test_cli_scout.py
+-rw-r--r--   0        0        0     1789 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/test_cli_upload.py
+-rw-r--r--   0        0        0      971 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/test_cli_upload_auto.py
+-rw-r--r--   0        0        0     1669 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/test_cli_upload_delivery_report.py
+-rw-r--r--   0        0        0      895 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/test_cli_upload_fastq.py
+-rw-r--r--   0        0        0     1199 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/test_cli_upload_genotype.py
+-rw-r--r--   0        0        0      694 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/test_cli_upload_gens.py
+-rw-r--r--   0        0        0     9965 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/test_cli_upload_nipt.py
+-rw-r--r--   0        0        0     4684 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/test_cli_upload_nipt_ftp.py
+-rw-r--r--   0        0        0     1839 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/test_cli_upload_nipt_statina.py
+-rw-r--r--   0        0        0     6177 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/upload/test_cli_upload_observations.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/__init__.py
+-rw-r--r--   0        0        0    31369 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/balsamic/conftest.py
+-rw-r--r--   0        0        0    13938 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
+-rw-r--r--   0        0        0     7984 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/balsamic/test_compound_commands.py
+-rw-r--r--   0        0        0     2336 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/balsamic/test_link.py
+-rw-r--r--   0        0        0     3554 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/balsamic/test_report_deliver.py
+-rw-r--r--   0        0        0     6209 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/balsamic/test_run.py
+-rw-r--r--   0        0        0     6934 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/balsamic/test_store_housekeeper.py
+-rw-r--r--   0        0        0     8458 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/fastq/__init__.py
+-rw-r--r--   0        0        0     2332 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/fastq/test_fastq_base.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0        0        0     5237 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/fluffy/conftest.py
+-rw-r--r--   0        0        0     5687 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
+-rw-r--r--   0        0        0     3302 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/fluffy/test_cli_link.py
+-rw-r--r--   0        0        0     1896 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/fluffy/test_cli_run.py
+-rw-r--r--   0        0        0     2968 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/fluffy/test_cli_start.py
+-rw-r--r--   0        0        0     7815 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/fluffy/test_cli_store.py
+-rw-r--r--   0        0        0     2775 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/microsalt/conftest.py
+-rw-r--r--   0        0        0     6926 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/microsalt/test_microsalt_case_config.py
+-rw-r--r--   0        0        0     1000 2024-04-25 12:07:50.783335 cg-60.4.1/tests/cli/workflow/microsalt/test_microsalt_run.py
+-rw-r--r--   0        0        0     6544 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/conftest.py
+-rw-r--r--   0        0        0     7011 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_base.py
+-rw-r--r--   0        0        0     1542 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
+-rw-r--r--   0        0        0      431 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_dna_link.py
+-rw-r--r--   0        0        0     2108 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py
+-rw-r--r--   0        0        0     1273 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
+-rw-r--r--   0        0        0     3595 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_dna_run.py
+-rw-r--r--   0        0        0     3884 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_dna_start.py
+-rw-r--r--   0        0        0     1004 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
+-rw-r--r--   0        0        0      527 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_rna_link.py
+-rw-r--r--   0        0        0      716 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_rna_run.py
+-rw-r--r--   0        0        0     8559 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_store.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/nf_analysis/__init__.py
+-rw-r--r--   0        0        0     9318 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_config_case.py
+-rw-r--r--   0        0        0     3831 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py
+-rw-r--r--   0        0        0     5087 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py
+-rw-r--r--   0        0        0     9211 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_run.py
+-rw-r--r--   0        0        0     3267 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_start.py
+-rw-r--r--   0        0        0     9877 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_store.py
+-rw-r--r--   0        0        0    10373 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py
+-rw-r--r--   0        0        0      978 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/raredisease/__init__.py
+-rw-r--r--   0        0        0     3940 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py
+-rw-r--r--   0        0        0      921 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/test_cli_workflow.py
+-rw-r--r--   0        0        0     4310 2024-04-25 12:07:50.787335 cg-60.4.1/tests/cli/workflow/test_cli_workflow_clean.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/clients/arnold/__init__.py
+-rw-r--r--   0        0        0     1080 2024-04-25 12:07:50.787335 cg-60.4.1/tests/clients/arnold/conftest.py
+-rw-r--r--   0        0        0     1503 2024-04-25 12:07:50.787335 cg-60.4.1/tests/clients/arnold/test_arnold_api_client.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/clients/janus/__init__.py
+-rw-r--r--   0        0        0     2381 2024-04-25 12:07:50.787335 cg-60.4.1/tests/clients/janus/conftest.py
+-rw-r--r--   0        0        0     1716 2024-04-25 12:07:50.787335 cg-60.4.1/tests/clients/janus/test_janus_api_client.py
+-rw-r--r--   0        0        0   133992 2024-04-25 12:07:50.787335 cg-60.4.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/delivery_fixtures/__init__.py
+-rw-r--r--   0        0        0     2653 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py
+-rw-r--r--   0        0        0     4972 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/delivery_fixtures/context_fixtures.py
+-rw-r--r--   0        0        0     1494 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/delivery_fixtures/path_fixtures.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/__init__.py
+-rw-r--r--   0        0        0     4625 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py
+-rw-r--r--   0        0        0     3467 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py
+-rw-r--r--   0        0        0    19179 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py
+-rw-r--r--   0        0        0     3699 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py
+-rw-r--r--   0        0        0     6000 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py
+-rw-r--r--   0        0        0     8960 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py
+-rw-r--r--   0        0        0     3174 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_check_scenario.py
+-rw-r--r--   0        0        0     4801 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_fixtures.py
+-rw-r--r--   0        0        0     1304 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixture_plugins/timestamp_fixtures.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
+-rw-r--r--   0        0        0    14644 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
+-rw-r--r--   0        0        0    15921 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/ADM2.cram
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/ADM3.cram
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/adm1.cram
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/adm1.mt.bam
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/multiqc.html
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/report.pdf
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/smn.vcf
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/snv.vcf
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/snv_research.vcf
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/str.vcf
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/sv.vcf
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/sv_research.vcf
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
+-rw-r--r--   0        0        0       70 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/nf-analysis/pipeline_params.config
+-rw-r--r--   0        0        0      195 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/nf-analysis/pipeline_resource_optimisation.config
+-rw-r--r--   0        0        0      195 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/nf-analysis/platform.config
+-rw-r--r--   0        0        0     8173 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/raredisease/multiqc_data.json
+-rw-r--r--   0        0        0    20005 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml
+-rw-r--r--   0        0        0     5497 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/rnafusion/multiqc_data.json
+-rw-r--r--   0        0        0    12499 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml
+-rw-r--r--   0        0        0     2873 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/sample_coverage.bed
+-rw-r--r--   0        0        0     6506 2024-04-25 12:07:50.787335 cg-60.4.1/tests/fixtures/analysis/taxprofiler/multiqc_data.json
+-rw-r--r--   0        0        0    10513 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0     5771 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/analysis/tomte/multiqc_data.json
+-rw-r--r--   0        0        0    14859 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml
+-rw-r--r--   0        0        0    10961 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/balsamic/case/config.json
+-rw-r--r--   0        0        0     3465 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/balsamic/case/metadata.yml
+-rw-r--r--   0        0        0       63 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/balsamic/case/metadata_directory.yml
+-rw-r--r--   0        0        0      165 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
+-rw-r--r--   0        0        0     2705 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
+-rw-r--r--   0        0        0      692 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/crunchy/spring_metadata.json
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0      412 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      484 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      658 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/demuxcomplete.txt
+-rw-r--r--   0        0        0     1757 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0        0        0        7 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0     6034 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0        0        0     1172 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0        0        0        7 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_1.fastq.gz
+-rw-r--r--   0        0        0        7 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_2.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0      288 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      361 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      414 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/demuxcomplete.txt
+-rw-r--r--   0        0        0      315 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      434 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0     8624 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml
+-rw-r--r--   0        0        0      568 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0      220 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      463 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      622 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0      345 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      650 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      896 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0      619 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0      303 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      364 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      427 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/demuxcomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0     4439 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0        0        0     1172 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0     5127 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
+-rw-r--r--   0        0        0       43 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz
+-rw-r--r--   0        0        0       67 2024-04-25 12:07:50.791335 cg-60.4.1/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz.md5
+-rw-r--r--   0        0        0   338370 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz
+-rw-r--r--   0        0        0       67 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz.md5
+-rw-r--r--   0        0        0   338349 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/CopyComplete.txt
+-rw-r--r--   0        0        0     2126 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json
+-rw-r--r--   0        0        0     1827 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json
+-rw-r--r--   0        0        0       90 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/README.txt
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAComplete.txt
+-rw-r--r--   0        0        0     6895 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml
+-rw-r--r--   0        0        0       37 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead1Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead2Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead3Complete.txt
+-rw-r--r--   0        0        0    24755 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml
+-rw-r--r--   0        0        0      692 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
+-rw-r--r--   0        0        0      724 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0       61 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SequencingComplete.txt
+-rw-r--r--   0        0        0     5775 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/CopyComplete.txt
+-rw-r--r--   0        0        0     2282 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json
+-rw-r--r--   0        0        0     1632 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json
+-rw-r--r--   0        0        0       75 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/README.txt
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAComplete.txt
+-rw-r--r--   0        0        0     6912 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml
+-rw-r--r--   0        0        0       36 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead1Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead2Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead3Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead4Complete.txt
+-rw-r--r--   0        0        0    24814 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml
+-rw-r--r--   0        0        0      814 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv
+-rw-r--r--   0        0        0      660 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0       61 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SequencingComplete.txt
+-rw-r--r--   0        0        0     5853 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/CopyComplete.txt
+-rw-r--r--   0        0        0    21848 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json
+-rw-r--r--   0        0        0    15512 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json
+-rw-r--r--   0        0        0       79 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/README.txt
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RTAComplete.txt
+-rw-r--r--   0        0        0      756 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml
+-rw-r--r--   0        0        0     4118 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv
+-rw-r--r--   0        0        0     1408 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0     5326 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/CopyComplete.txt
+-rw-r--r--   0        0        0    15041 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json
+-rw-r--r--   0        0        0    10649 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json
+-rw-r--r--   0        0        0       80 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/README.txt
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RTAComplete.txt
+-rw-r--r--   0        0        0      755 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml
+-rw-r--r--   0        0        0     2878 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv
+-rw-r--r--   0        0        0      928 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0     5359 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CopyComplete.txt
+-rw-r--r--   0        0        0    27887 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv
+-rw-r--r--   0        0        0   141870 2024-04-25 12:07:50.795335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json
+-rwxr-xr-x   0        0        0   122682 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json
+-rw-r--r--   0        0        0      243 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/README.txt
+-rw-r--r--   0        0        0    28230 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTAComplete.txt
+-rw-r--r--   0        0        0    94426 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml
+-rw-r--r--   0        0        0     5819 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/SequenceComplete.txt
+-rw-r--r--   0        0        0     1757 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0        0        0     1757 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stdout
+-rw-r--r--   0        0        0       12 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/README.txt
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RTAComplete.txt
+-rw-r--r--   0        0        0     5945 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml
+-rw-r--r--   0        0        0      260 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/copycomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/demuxstarted.txt
+-rw-r--r--   0        0        0     1757 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0        0        0     1757 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout
+-rw-r--r--   0        0        0    47522 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json
+-rw-r--r--   0        0        0       12 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/README.txt
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0        0        0     6666 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0        0        0      254 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/copycomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/delivery.txt
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/demuxstarted.txt
+-rwxr-xr-x   0        0        0    47434 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CopyComplete.txt
+-rw-r--r--   0        0        0    10950 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv
+-rw-r--r--   0        0        0      225 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/Manifest.tsv
+-rw-r--r--   0        0        0       55 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/README.txt
+-rwxr-xr-x   0        0        0     2493 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg
+-rwxr-xr-x   0        0        0        1 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAComplete.txt
+-rwxr-xr-x   0        0        0        2 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAExited.txt
+-rwxr-xr-x   0        0        0      730 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml
+-rwxr-xr-x   0        0        0    79277 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml
+-rwxr-xr-x   0        0        0     2694 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
+-rw-r--r--   0        0        0    10950 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
+-rw-r--r--   0        0        0      619 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0        0        0       12 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/README.txt
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0        0        0      399 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CopyComplete.txt
+-rw-r--r--   0        0        0     4941 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv
+-rwxr-xr-x   0        0        0    20050 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stderr
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stdout
+-rw-r--r--   0        0        0      244 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/README.txt
+-rw-r--r--   0        0        0     6391 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTAComplete.txt
+-rw-r--r--   0        0        0    16428 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml
+-rw-r--r--   0        0        0     6728 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
+-rw-r--r--   0        0        0     5127 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SequenceComplete.txt
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/demuxstarted.txt
+-rw-r--r--   0        0        0      133 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/README.txt
+-rw-r--r--   0        0        0      724 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
+-rw-r--r--   0        0        0     5775 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
+-rw-r--r--   0        0        0      124 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/180509_D00450_0598_BHGYFNBCX2/README.txt
+-rw-r--r--   0        0        0      310 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/README.txt
+-rw-r--r--   0        0        0     5819 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
+-rw-r--r--   0        0        0      122 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/README.txt
+-rwxr-xr-x   0        0        0     2694 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
+-rw-r--r--   0        0        0      311 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/README.txt
+-rw-r--r--   0        0        0     6728 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0        0        0      399 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.799335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
+-rw-r--r--   0        0        0      399 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_0.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_1.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/final_summary_PAS86456_72d9fceb_8a4fd683.txt
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_0.pod5
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_1.pod5
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_0.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_1.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/final_summary_PAS97781_595b5663_efc7f02e.txt
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_0.pod5
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_1.pod5
+-rw-r--r--   0        0        0   111989 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
+-rw-r--r--   0        0        0     5319 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml
+-rw-r--r--   0        0        0     5944 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
+-rwxr-xr-x   0        0        0     2603 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
+-rwxr-xr-x   0        0        0     2597 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml
+-rw-r--r--   0        0        0     5899 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
+-rw-r--r--   0        0        0     4941 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv
+-rw-r--r--   0        0        0    10950 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/spring/dummy_run_001.spring
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/spring/dummy_run_002.spring
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/demultiplexing/spring/dummy_spring_meta_data.json
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
+-rw-r--r--   0        0        0     5554 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/fluffy/SampleSheet.csv
+-rw-r--r--   0        0        0      901 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/fluffy/deliverables.yaml
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/fluffy/multiqc_report.html
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/fluffy/summary.csv
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/gt/yellowhog.bcf
+-rw-r--r--   0        0        0     5114 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/madeline/madeline.xml
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/case_file.txt
+-rw-r--r--   0        0        0     3241 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0    21811 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/dna/store/case_config.yaml
+-rw-r--r--   0        0        0    23364 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
+-rw-r--r--   0        0        0    37367 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
+-rw-r--r--   0        0        0       16 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
+-rw-r--r--   0        0        0       16 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0       16 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
+-rw-r--r--   0        0        0      123 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
+-rw-r--r--   0        0        0    62741 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
+-rw-r--r--   0        0        0    11242 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/rna/case_config.yaml
+-rw-r--r--   0        0        0    12164 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
+-rw-r--r--   0        0        0     5231 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
+-rw-r--r--   0        0        0     9774 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/rna/store/case_config.yaml
+-rw-r--r--   0        0        0     4624 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
+-rw-r--r--   0        0        0    13666 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/mip/sample_file.txt
+-rw-r--r--   0        0        0     1885 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/scout/643594.config.yaml
+-rw-r--r--   0        0        0     6027 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/scout/case_export.json
+-rw-r--r--   0        0        0     9349 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/scout/export_causatives.json
+-rw-r--r--   0        0        0     1315 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/scout/none_case_export.json
+-rw-r--r--   0        0        0     3518 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/scout/other_sex_case.json
+-rw-r--r--   0        0        0     8874 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/scout/panel_export.bed
+-rw-r--r--   0        0        0     4169 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/scout/panel_export.csv
+-rw-r--r--   0        0        0      619 2024-04-25 12:07:50.803335 cg-60.4.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/SampleSheet.csv
+-rw-r--r--   0        0        0    63569 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0    42478 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0    69708 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0       42 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/apps/shipping/scout-deploy.yaml
+-rw-r--r--   0        0        0     1036 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/cgweb_orders/balsamic.json
+-rw-r--r--   0        0        0     1104 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/cgweb_orders/fastq.json
+-rw-r--r--   0        0        0     1313 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/cgweb_orders/metagenome.json
+-rw-r--r--   0        0        0     3038 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/cgweb_orders/microsalt.json
+-rw-r--r--   0        0        0     3705 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/cgweb_orders/mip.json
+-rw-r--r--   0        0        0     1364 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/cgweb_orders/mip_rna.json
+-rw-r--r--   0        0        0     2125 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/cgweb_orders/rml.json
+-rw-r--r--   0        0        0     1368 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/cgweb_orders/rnafusion.json
+-rw-r--r--   0        0        0     4684 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/cgweb_orders/sarscov2.json
+-rw-r--r--   0        0        0     5609 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/data/SampleSheet.csv
+-rw-r--r--   0        0        0      511 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/data/bcl_convert_sample_sheet.csv
+-rw-r--r--   0        0        0   258048 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/data/cgfixture.db
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/data/fastq.fastq.gz
+-rw-r--r--   0        0        0    49152 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/data/hkstore.db
+-rw-r--r--   0        0        0       73 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/data/yellowhog/pedigree.yaml
+-rw-r--r--   0        0        0       76 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/io/casava_five_parts.fastq.gz
+-rw-r--r--   0        0        0       90 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/io/casava_seven_parts.fastq.gz
+-rw-r--r--   0        0        0       96 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/io/casava_ten_parts.fastq.gz
+-rw-r--r--   0        0        0      153 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/io/example.csv
+-rw-r--r--   0        0        0       46 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/io/example.gz
+-rw-r--r--   0        0        0      147 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/io/example.tsv
+-rw-r--r--   0        0        0       20 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/io/example.txt
+-rw-r--r--   0        0        0       20 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/io/example2.txt
+-rw-r--r--   0        0        0      582 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/io/example_json.json
+-rw-r--r--   0        0        0      103 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/io/example_xml.xml
+-rw-r--r--   0        0        0       20 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/meta/qc_metrics/file_with_right_tags.json
+-rw-r--r--   0        0        0       20 2024-04-25 12:07:50.807335 cg-60.4.1/tests/fixtures/meta/qc_metrics/file_without_right_tags.json
+-rw-r--r--   0        0        0   156910 2024-04-25 12:07:50.811334 cg-60.4.1/tests/fixtures/orderforms/1508.30.balsamic.xlsx
+-rw-r--r--   0        0        0   156770 2024-04-25 12:07:50.811334 cg-60.4.1/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx
+-rw-r--r--   0        0        0   156737 2024-04-25 12:07:50.811334 cg-60.4.1/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx
+-rw-r--r--   0        0        0   156582 2024-04-25 12:07:50.811334 cg-60.4.1/tests/fixtures/orderforms/1508.30.fastq.xlsx
+-rw-r--r--   0        0        0   155627 2024-04-25 12:07:50.811334 cg-60.4.1/tests/fixtures/orderforms/1508.30.metagenome.xlsx
+-rw-r--r--   0        0        0   156850 2024-04-25 12:07:50.811334 cg-60.4.1/tests/fixtures/orderforms/1508.30.mip.xlsx
+-rw-r--r--   0        0        0   258580 2024-04-25 12:07:50.811334 cg-60.4.1/tests/fixtures/orderforms/1508.30.mip_rna.xlsx
+-rw-r--r--   0        0        0   258342 2024-04-25 12:07:50.815335 cg-60.4.1/tests/fixtures/orderforms/1508.30.rnafusion.xlsx
+-rw-r--r--   0        0        0    82677 2024-04-25 12:07:50.815335 cg-60.4.1/tests/fixtures/orderforms/1603.11.microbial.xlsx
+-rw-r--r--   0        0        0   149394 2024-04-25 12:07:50.815335 cg-60.4.1/tests/fixtures/orderforms/1604.17.rml.xlsx
+-rw-r--r--   0        0        0   223184 2024-04-25 12:07:50.815335 cg-60.4.1/tests/fixtures/orderforms/2184.9.sarscov2.xlsx
+-rw-r--r--   0        0        0    18639 2024-04-25 12:07:50.815335 cg-60.4.1/tests/fixtures/orderforms/NIPT-json.json
+-rw-r--r--   0        0        0     6052 2024-04-25 12:07:50.815335 cg-60.4.1/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
+-rw-r--r--   0        0        0     6611 2024-04-25 12:07:50.815335 cg-60.4.1/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
+-rw-r--r--   0        0        0     1417 2024-04-25 12:07:50.815335 cg-60.4.1/tests/fixtures/report/case_data.json
+-rw-r--r--   0        0        0     1109 2024-04-25 12:07:50.815335 cg-60.4.1/tests/fixtures/report/lims_exported_samples.json
+-rw-r--r--   0        0        0     1562 2024-04-25 12:07:50.815335 cg-60.4.1/tests/fixtures/report/lims_family.json
+-rw-r--r--   0        0        0     3296 2024-04-25 12:07:50.815335 cg-60.4.1/tests/io/conftest.py
+-rw-r--r--   0        0        0      431 2024-04-25 12:07:50.815335 cg-60.4.1/tests/io/test_io_config.py
+-rw-r--r--   0        0        0     8639 2024-04-25 12:07:50.815335 cg-60.4.1/tests/io/test_io_controller.py
+-rw-r--r--   0        0        0     3877 2024-04-25 12:07:50.815335 cg-60.4.1/tests/io/test_io_csv.py
+-rw-r--r--   0        0        0      482 2024-04-25 12:07:50.815335 cg-60.4.1/tests/io/test_io_gzip.py
+-rw-r--r--   0        0        0     1779 2024-04-25 12:07:50.815335 cg-60.4.1/tests/io/test_io_json.py
+-rw-r--r--   0        0        0     2914 2024-04-25 12:07:50.815335 cg-60.4.1/tests/io/test_io_txt.py
+-rw-r--r--   0        0        0     1027 2024-04-25 12:07:50.815335 cg-60.4.1/tests/io/test_io_xml.py
+-rw-r--r--   0        0        0     2131 2024-04-25 12:07:50.815335 cg-60.4.1/tests/io/test_io_yaml.py
+-rw-r--r--   0        0        0     1233 2024-04-25 12:07:50.815335 cg-60.4.1/tests/io/test_validate_path.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/archive/__init__.py
+-rw-r--r--   0        0        0    13131 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/archive/conftest.py
+-rw-r--r--   0        0        0    16858 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/archive/test_archive_api.py
+-rw-r--r--   0        0        0    10246 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/archive/test_archive_cli.py
+-rw-r--r--   0        0        0    15766 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/archive/test_archiving.py
+-rw-r--r--   0        0        0     3807 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/backup/conftest.py
+-rw-r--r--   0        0        0    26368 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/backup/test_meta_backup.py
+-rw-r--r--   0        0        0    10055 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/backup/test_meta_pdc.py
+-rw-r--r--   0        0        0    12546 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/clean/conftest.py
+-rw-r--r--   0        0        0    16944 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/clean/test_clean_flow_cells_api.py
+-rw-r--r--   0        0        0     2286 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/clean/test_clean_retrieved_spring_files.py
+-rw-r--r--   0        0        0     7691 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/compress/conftest.py
+-rw-r--r--   0        0        0     7961 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/compress/test_clean_fastq.py
+-rw-r--r--   0        0        0     1778 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/compress/test_compress_files.py
+-rw-r--r--   0        0        0     3644 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/compress/test_compress_meta_fastq.py
+-rw-r--r--   0        0        0     1180 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/compress/test_decompress_spring_meta.py
+-rw-r--r--   0        0        0     7013 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/compress/test_meta_compress_update_hk.py
+-rw-r--r--   0        0        0     8269 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/deliver/__init__.py
+-rw-r--r--   0        0        0     3471 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/deliver/conftest.py
+-rw-r--r--   0        0        0     5533 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/deliver/test_deliver_ticket.py
+-rw-r--r--   0        0        0    10277 2024-04-25 12:07:50.815335 cg-60.4.1/tests/meta/deliver/test_delivery_api.py
+-rw-r--r--   0        0        0     1057 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/deliver/test_fastq_path_generator.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/delivery/__init__.py
+-rw-r--r--   0        0        0    16660 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/delivery/test_delivery_api.py
+-rw-r--r--   0        0        0     8874 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/demultiplex/conftest.py
+-rw-r--r--   0        0        0     5382 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/demultiplex/test_combine_sequencing_metrics.py
+-rw-r--r--   0        0        0     8339 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/demultiplex/test_demux_post_processing.py
+-rw-r--r--   0        0        0    12406 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/demultiplex/test_housekeeper_storage_functions.py
+-rw-r--r--   0        0        0     4392 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/demultiplex/test_status_db_storage_functions.py
+-rw-r--r--   0        0        0    22837 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/demultiplex/test_utils.py
+-rw-r--r--   0        0        0     6193 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/demultiplex/test_validation.py
+-rw-r--r--   0        0        0     4943 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/encryption/conftest.py
+-rw-r--r--   0        0        0    18133 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/encryption/test_encryption.py
+-rw-r--r--   0        0        0     3122 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/observations/conftest.py
+-rw-r--r--   0        0        0    16164 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/observations/test_meta_upload_observations.py
+-rw-r--r--   0        0        0     4974 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/orders/conftest.py
+-rw-r--r--   0        0        0     1749 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/orders/test_PoolSubmitter_validate_order.py
+-rw-r--r--   0        0        0     1470 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
+-rw-r--r--   0        0        0     1768 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/orders/test_SarsCov2Submitter_store_order.py
+-rw-r--r--   0        0        0     2032 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
+-rw-r--r--   0        0        0    19783 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/orders/test_meta_orders_api.py
+-rw-r--r--   0        0        0     7086 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/orders/test_meta_orders_lims.py
+-rw-r--r--   0        0        0    29515 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/orders/test_meta_orders_status.py
+-rw-r--r--   0        0        0     1677 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/orders/test_rnafusion_submitter.py
+-rw-r--r--   0        0        0     1068 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/orders/test_ticket_handler.py
+-rw-r--r--   0        0        0     4336 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/qc_metrics/conftest.py
+-rw-r--r--   0        0        0     1972 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/qc_metrics/test_collect_qc_metrics.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/report/__init__.py
+-rw-r--r--   0        0        0     6512 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/report/conftest.py
+-rw-r--r--   0        0        0      434 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/report/helper.py
+-rw-r--r--   0        0        0     2604 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/report/test_balsamic_api.py
+-rw-r--r--   0        0        0     4056 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/report/test_field_validators.py
+-rw-r--r--   0        0        0     2858 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/report/test_mip_dna_api.py
+-rw-r--r--   0        0        0    16042 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/report/test_report_api.py
+-rw-r--r--   0        0        0     1365 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/report/test_rnafusion_api.py
+-rw-r--r--   0        0        0     1250 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/report/test_tomte_api.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/rsync/__init__.py
+-rw-r--r--   0        0        0      916 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/rsync/conftest.py
+-rw-r--r--   0        0        0     9442 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/rsync/test_rsync.py
+-rw-r--r--   0        0        0     3147 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/test_invoice.py
+-rw-r--r--   0        0        0     1220 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/transfer/conftest.py
+-rw-r--r--   0        0        0     9892 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/transfer/test_external_data.py
+-rw-r--r--   0        0        0     4395 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/transfer/test_meta_transfer_lims.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/__init__.py
+-rw-r--r--   0        0        0     2210 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/balsamic/test_balsamic.py
+-rw-r--r--   0        0        0     4002 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/gisaid/__init__.py
+-rw-r--r--   0        0        0     2557 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/gisaid/fixtures/four_samples.csv
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
+-rw-r--r--   0        0        0      211 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
+-rw-r--r--   0        0        0      371 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/mutacc/__init__.py
+-rw-r--r--   0        0        0     3684 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/mutacc/conftest.py
+-rw-r--r--   0        0        0     4188 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
+-rw-r--r--   0        0        0     1149 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/nipt/conftest.py
+-rw-r--r--   0        0        0     1683 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/nipt/test_models.py
+-rw-r--r--   0        0        0     1242 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/nipt/test_nipt_upload_api.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/scout/__init__.py
+-rw-r--r--   0        0        0    23954 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/scout/conftest.py
+-rw-r--r--   0        0        0     4734 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/scout/test_generate_load_config.py
+-rw-r--r--   0        0        0     4182 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/scout/test_meta_upload_scoutapi.py
+-rw-r--r--   0        0        0    33260 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
+-rw-r--r--   0        0        0     7372 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/scout/test_scout_config_builder.py
+-rw-r--r--   0        0        0     2511 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/test_meta_upload_coverage.py
+-rw-r--r--   0        0        0     1473 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/test_upload_api.py
+-rw-r--r--   0        0        0     2547 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/upload/test_upload_genotypes_api.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/workflow/__init__.py
+-rw-r--r--   0        0        0    10262 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/workflow/conftest.py
+-rw-r--r--   0        0        0     3679 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/workflow/microsalt/conftest.py
+-rw-r--r--   0        0        0      318 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/workflow/microsalt/test_parsing_metrics.py
+-rw-r--r--   0        0        0     3759 2024-04-25 12:07:50.819335 cg-60.4.1/tests/meta/workflow/microsalt/test_quality_controller.py
+-rw-r--r--   0        0        0    14367 2024-04-25 12:07:50.823335 cg-60.4.1/tests/meta/workflow/microsalt/test_quality_controller_utils.py
+-rw-r--r--   0        0        0      825 2024-04-25 12:07:50.823335 cg-60.4.1/tests/meta/workflow/microsalt/test_report_generation.py
+-rw-r--r--   0        0        0    20860 2024-04-25 12:07:50.823335 cg-60.4.1/tests/meta/workflow/test_analysis.py
+-rw-r--r--   0        0        0     7934 2024-04-25 12:07:50.823335 cg-60.4.1/tests/meta/workflow/test_balsamic.py
+-rw-r--r--   0        0        0     3034 2024-04-25 12:07:50.823335 cg-60.4.1/tests/meta/workflow/test_fastq.py
+-rw-r--r--   0        0        0     1532 2024-04-25 12:07:50.823335 cg-60.4.1/tests/meta/workflow/test_microsalt.py
+-rw-r--r--   0        0        0     2721 2024-04-25 12:07:50.823335 cg-60.4.1/tests/meta/workflow/test_nf_analysis.py
+-rw-r--r--   0        0        0     7741 2024-04-25 12:07:50.823335 cg-60.4.1/tests/meta/workflow/test_prepare_fastq_api.py
+-rw-r--r--   0        0        0     1920 2024-04-25 12:07:50.823335 cg-60.4.1/tests/meta/workflow/test_raredisease.py
+-rw-r--r--   0        0        0     1674 2024-04-25 12:07:50.823335 cg-60.4.1/tests/meta/workflow/test_rnafusion.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/__init__.py
+-rw-r--r--   0        0        0     1168 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/balsamic_analysis_mock.py
+-rw-r--r--   0        0        0     3500 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/crunchy.py
+-rw-r--r--   0        0        0    21778 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/hk_mock.py
+-rw-r--r--   0        0        0     4106 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/limsmock.py
+-rw-r--r--   0        0        0      572 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/madeline.py
+-rw-r--r--   0        0        0     1297 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/mip_analysis_mock.py
+-rw-r--r--   0        0        0     1525 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/osticket.py
+-rw-r--r--   0        0        0     3239 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/process_mock.py
+-rw-r--r--   0        0        0     4713 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/report.py
+-rw-r--r--   0        0        0     3915 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/scout.py
+-rw-r--r--   0        0        0      750 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/store_model.py
+-rw-r--r--   0        0        0     1620 2024-04-25 12:07:50.823335 cg-60.4.1/tests/mocks/tb_mock.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/balsamic/__init__.py
+-rw-r--r--   0        0        0     1194 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/balsamic/conftest.py
+-rw-r--r--   0        0        0     1030 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/balsamic/test_balsamic_analysis.py
+-rw-r--r--   0        0        0     1050 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/demultiplexing/__init__.py
+-rw-r--r--   0        0        0    11446 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/demultiplexing/test_run_parameters.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/downsample/__init__.py
+-rw-r--r--   0        0        0     2096 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/downsample/test_down_sample_meta_data.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/flow_cell/__init__.py
+-rw-r--r--   0        0        0     6659 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/flow_cell/test_flowcell_model.py
+-rw-r--r--   0        0        0     6637 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/mip/conftest.py
+-rw-r--r--   0        0        0     1239 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/mip/test_mip_analysis.py
+-rw-r--r--   0        0        0     2348 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/mip/test_mip_config.py
+-rw-r--r--   0        0        0     6392 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/mip/test_mip_metrics_deliverables.py
+-rw-r--r--   0        0        0     3959 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/mip/test_mip_sample_info.py
+-rw-r--r--   0        0        0     3314 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/nextflow/test_nextflow_deliver.py
+-rw-r--r--   0        0        0     1602 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/observations/conftest.py
+-rw-r--r--   0        0        0     2579 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/observations/test_observations_input_files.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/report/__init__.py
+-rw-r--r--   0        0        0     7327 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/report/test_validators.py
+-rw-r--r--   0        0        0     3855 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/rnafusion/test_rnafusion_sample.py
+-rw-r--r--   0        0        0     1374 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/test_cg_models.py
+-rw-r--r--   0        0        0      990 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/test_compression_data.py
+-rw-r--r--   0        0        0      729 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/test_fastq.py
+-rw-r--r--   0        0        0     2860 2024-04-25 12:07:50.823335 cg-60.4.1/tests/models/test_file_data.py
+-rw-r--r--   0        0        0     4539 2024-04-25 12:07:50.823335 cg-60.4.1/tests/server/conftest.py
+-rw-r--r--   0        0        0     3135 2024-04-25 12:07:50.823335 cg-60.4.1/tests/server/endpoints/test_delivery_message_endpoint.py
+-rw-r--r--   0        0        0     3239 2024-04-25 12:07:50.823335 cg-60.4.1/tests/server/endpoints/test_orders_endpoint.py
+-rw-r--r--   0        0        0      271 2024-04-25 12:07:50.823335 cg-60.4.1/tests/server/test_server_auto.py
+-rw-r--r--   0        0        0     1047 2024-04-25 12:07:50.823335 cg-60.4.1/tests/services/fastq_file_service/conftest.py
+-rw-r--r--   0        0        0     3634 2024-04-25 12:07:50.823335 cg-60.4.1/tests/services/fastq_file_service/test_fastq_file_service.py
+-rw-r--r--   0        0        0     4861 2024-04-25 12:07:50.823335 cg-60.4.1/tests/services/orders/order_status_service/conftest.py
+-rw-r--r--   0        0        0     2865 2024-04-25 12:07:50.823335 cg-60.4.1/tests/services/orders/order_status_service/test_order_summary_service.py
+-rw-r--r--   0        0        0     9595 2024-04-25 12:07:50.823335 cg-60.4.1/tests/services/quality_controller/test_sequencing_quality_checks_utils.py
+-rw-r--r--   0        0        0      318 2024-04-25 12:07:50.823335 cg-60.4.1/tests/small_helpers.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/api/__init__.py
+-rw-r--r--   0        0        0     3032 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/api/conftest.py
+-rw-r--r--   0        0        0     1557 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/api/test_base.py
+-rw-r--r--   0        0        0    20096 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/crud/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/crud/add/__init__.py
+-rw-r--r--   0        0        0     1497 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/crud/add/test_store_add_application_version.py
+-rw-r--r--   0        0        0     3958 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/crud/add/test_store_add_base.py
+-rw-r--r--   0        0        0     2502 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/crud/add/test_store_add_customer.py
+-rw-r--r--   0        0        0     1704 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/crud/add/test_store_add_flow_celll.py
+-rw-r--r--   0        0        0    12290 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/crud/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/crud/delete/__init__.py
+-rw-r--r--   0        0        0     5611 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/crud/delete/test_delete.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.823335 cg-60.4.1/tests/store/crud/read/__init__.py
+-rw-r--r--   0        0        0    56077 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/crud/read/test_read.py
+-rw-r--r--   0        0        0     5461 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/crud/read/test_read_analyses_to_clean.py
+-rw-r--r--   0        0        0     3553 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/crud/read/test_read_analyses_to_delivery_report.py
+-rw-r--r--   0        0        0    17328 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/crud/read/test_read_analysis.py
+-rw-r--r--   0        0        0     2743 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/crud/read/test_read_application_version.py
+-rw-r--r--   0        0        0     1105 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/crud/read/test_read_customer.py
+-rw-r--r--   0        0        0     1530 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/crud/read/test_read_pool.py
+-rw-r--r--   0        0        0    21503 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/crud/read/test_read_sample.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/crud/update/__init__.py
+-rw-r--r--   0        0        0      737 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/crud/update/test_update.py
+-rw-r--r--   0        0        0    11693 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_analyses_filters.py
+-rw-r--r--   0        0        0     3397 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_application_filters.py
+-rw-r--r--   0        0        0     2073 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_application_limitations_filters.py
+-rw-r--r--   0        0        0    10452 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_application_version_filters.py
+-rw-r--r--   0        0        0     2804 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_bed_filters.py
+-rw-r--r--   0        0        0     2362 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_bed_version_filters.py
+-rw-r--r--   0        0        0     3495 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_case_sample_filters.py
+-rw-r--r--   0        0        0    39100 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_cases_filters.py
+-rw-r--r--   0        0        0     1345 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_collaboration_filters.py
+-rw-r--r--   0        0        0     2482 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_customer_filters.py
+-rw-r--r--   0        0        0     5153 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_flow_cell_filters.py
+-rw-r--r--   0        0        0     2226 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_invoice_filters.py
+-rw-r--r--   0        0        0     5871 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_metrics_filters.py
+-rw-r--r--   0        0        0     2404 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_organism_filters.py
+-rw-r--r--   0        0        0     1804 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_panel_filters.py
+-rw-r--r--   0        0        0     8720 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_pool_filters.py
+-rw-r--r--   0        0        0    22875 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_samples_filters.py
+-rw-r--r--   0        0        0     1576 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/filters/test_status_user_filters.py
+-rw-r--r--   0        0        0     2147 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/test_delivery.py
+-rw-r--r--   0        0        0     4127 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store/test_store_models.py
+-rw-r--r--   0        0        0    37125 2024-04-25 12:07:50.827335 cg-60.4.1/tests/store_helpers.py
+-rw-r--r--   0        0        0     4930 2024-04-25 12:07:50.827335 cg-60.4.1/tests/test_copy_novaseqx_flow_cell.py
+-rw-r--r--   0        0        0      911 2024-04-25 12:07:50.827335 cg-60.4.1/tests/test_store_helpers.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:07:50.827335 cg-60.4.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1754 2024-04-25 12:07:50.827335 cg-60.4.1/tests/utils/conftest.py
+-rw-r--r--   0        0        0      371 2024-04-25 12:07:50.827335 cg-60.4.1/tests/utils/test_calculations.py
+-rw-r--r--   0        0        0     2920 2024-04-25 12:07:50.827335 cg-60.4.1/tests/utils/test_commands.py
+-rw-r--r--   0        0        0      953 2024-04-25 12:07:50.827335 cg-60.4.1/tests/utils/test_date.py
+-rw-r--r--   0        0        0     1508 2024-04-25 12:07:50.827335 cg-60.4.1/tests/utils/test_dict.py
+-rw-r--r--   0        0        0     7154 2024-04-25 12:07:50.827335 cg-60.4.1/tests/utils/test_dispatcher.py
+-rw-r--r--   0        0        0     4100 2024-04-25 12:07:50.827335 cg-60.4.1/tests/utils/test_files.py
+-rw-r--r--   0        0        0     1170 2024-04-25 12:07:50.827335 cg-60.4.1/tests/utils/test_time.py
+-rw-r--r--   0        0        0     2366 2024-04-25 12:07:50.827335 cg-60.4.1/tests/utils/test_utils.py
+-rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 cg-60.4.1/PKG-INFO
```

### Comparing `cg-60.4.0/README.md` & `cg-60.4.1/README.md`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/coverage/api.py` & `cg-60.4.1/cg/apps/coverage/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/crunchy/crunchy.py` & `cg-60.4.1/cg/apps/crunchy/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/crunchy/files.py` & `cg-60.4.1/cg/apps/crunchy/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/crunchy/sbatch.py` & `cg-60.4.1/cg/apps/crunchy/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/demultiplex/demultiplex_api.py` & `cg-60.4.1/cg/apps/demultiplex/demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/demultiplex/sample_sheet/api.py` & `cg-60.4.1/cg/apps/demultiplex/sample_sheet/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/demultiplex/sample_sheet/index.py` & `cg-60.4.1/cg/apps/demultiplex/sample_sheet/index.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py` & `cg-60.4.1/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py` & `cg-60.4.1/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/demultiplex/sample_sheet/sample_models.py` & `cg-60.4.1/cg/apps/demultiplex/sample_sheet/sample_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py` & `cg-60.4.1/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py` & `cg-60.4.1/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py` & `cg-60.4.1/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/demultiplex/sample_sheet/validators.py` & `cg-60.4.1/cg/apps/demultiplex/sample_sheet/validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/demultiplex/sbatch.py` & `cg-60.4.1/cg/apps/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/downsample/downsample.py` & `cg-60.4.1/cg/apps/downsample/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/downsample/utils.py` & `cg-60.4.1/cg/apps/downsample/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/gens.py` & `cg-60.4.1/cg/apps/gens.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/gt.py` & `cg-60.4.1/cg/apps/gt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/hermes/hermes_api.py` & `cg-60.4.1/cg/apps/hermes/hermes_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/hermes/models.py` & `cg-60.4.1/cg/apps/hermes/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/housekeeper/hk.py` & `cg-60.4.1/cg/apps/housekeeper/hk.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/invoice/render.py` & `cg-60.4.1/cg/apps/invoice/render.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/invoice/templates/KI_pool_invoice.xlsx` & `cg-60.4.1/cg/apps/invoice/templates/KI_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/invoice/templates/KI_sample_invoice.xlsx` & `cg-60.4.1/cg/apps/invoice/templates/KI_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/invoice/templates/KTH_pool_invoice.xlsx` & `cg-60.4.1/cg/apps/invoice/templates/KTH_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/invoice/templates/KTH_sample_invoice.xlsx` & `cg-60.4.1/cg/apps/invoice/templates/KTH_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/lims/api.py` & `cg-60.4.1/cg/apps/lims/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,18 @@
 from typing import Any
 
 from dateutil.parser import parse as parse_date
 from genologics.entities import Artifact, Process, Researcher, Sample
 from genologics.lims import Lims
 from requests.exceptions import HTTPError
 
-from cg.constants.lims import (
-    MASTER_STEPS_UDFS,
-    PROP2UDF,
-    DocumentationMethod,
-    LimsArtifactTypes,
-)
+from cg.constants import Priority
+from cg.constants.lims import MASTER_STEPS_UDFS, PROP2UDF, DocumentationMethod, LimsArtifactTypes
 from cg.exc import LimsDataError
 
-from ...constants import Priority
 from .order import OrderHandler
 
 SEX_MAP = {"F": "female", "M": "male", "Unknown": "unknown", "unknown": "unknown"}
 REV_SEX_MAP = {value: key for key, value in SEX_MAP.items()}
 AM_METHODS = {
     "1464": "Automated TruSeq DNA PCR-free library preparation method",
     "1317": "HiSeq X Sequencing method at Clinical Genomics",
@@ -64,14 +59,21 @@
             LOG.warning(f"Sample {lims_id} not found in LIMS: {error}")
         return lims_sample
 
     def samples_in_pools(self, pool_name, projectname):
         """Fetch all samples from a pool"""
         return self.get_samples(udf={"pool name": str(pool_name)}, projectname=projectname)
 
+    def get_source(self, lims_id: str) -> str | None:
+        """Return the source from LIMS for a given sample ID.
+        Return 'None' if no source information is set or
+        if sample is not found or cannot be fetched from LIMS."""
+        lims_sample: dict[str, Any] = self.sample(lims_id=lims_id)
+        return lims_sample.get("source")
+
     @staticmethod
     def _export_project(lims_project) -> dict:
         """Fetch relevant information from a lims project object"""
         return {
             "id": lims_project.id,
             "name": lims_project.name,
             "date": parse_date(lims_project.open_date) if lims_project.open_date else None,
```

### Comparing `cg-60.4.0/cg/apps/lims/batch.py` & `cg-60.4.1/cg/apps/lims/batch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/lims/order.py` & `cg-60.4.1/cg/apps/lims/order.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/lims/sample_sheet.py` & `cg-60.4.1/cg/apps/lims/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/loqus.py` & `cg-60.4.1/cg/apps/loqus.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/madeline/api.py` & `cg-60.4.1/cg/apps/madeline/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/mip/confighandler.py` & `cg-60.4.1/cg/apps/mip/confighandler.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/mutacc_auto.py` & `cg-60.4.1/cg/apps/mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/orderform/excel_orderform_parser.py` & `cg-60.4.1/cg/apps/orderform/excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/orderform/json_orderform_parser.py` & `cg-60.4.1/cg/apps/orderform/json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/orderform/orderform_parser.py` & `cg-60.4.1/cg/apps/orderform/orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/osticket.py` & `cg-60.4.1/cg/apps/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/scout/scout_export.py` & `cg-60.4.1/cg/apps/scout/scout_export.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/scout/scoutapi.py` & `cg-60.4.1/cg/apps/scout/scoutapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,27 +45,29 @@
                 existing_date = existing_case.analysis_date.date()
                 LOG.warning(f"Analysis of case already loaded: {existing_date}")
                 return
         LOG.debug("load new Scout case")
         self.process.run_command(load_command)
         LOG.debug("Case loaded successfully to Scout")
 
-    def export_panels(self, panels: list[str], build: str = GENOME_BUILD_37) -> list[str]:
+    def export_panels(
+        self, panels: list[str], build: str = GENOME_BUILD_37, dry_run: bool = False
+    ) -> list[str]:
         """Pass through to export of a list of gene panels.
 
         Return list of lines in bed format
         """
         export_panels_command = ["export", "panel", "--bed"]
         export_panels_command.extend(iter(panels))
 
         if build:
             export_panels_command.extend(["--build", build])
 
         try:
-            self.process.run_command(export_panels_command)
+            self.process.run_command(export_panels_command, dry_run=dry_run)
             if not self.process.stdout:
                 return []
         except CalledProcessError:
             LOG.info("Could not find panels")
             return []
 
         return list(self.process.stdout_lines())
```

### Comparing `cg-60.4.0/cg/apps/sequencing_metrics_parser/api.py` & `cg-60.4.1/cg/apps/sequencing_metrics_parser/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/sequencing_metrics_parser/models.py` & `cg-60.4.1/cg/apps/sequencing_metrics_parser/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/sequencing_metrics_parser/parser.py` & `cg-60.4.1/cg/apps/sequencing_metrics_parser/parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/slurm/sbatch.py` & `cg-60.4.1/cg/apps/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/slurm/slurm_api.py` & `cg-60.4.1/cg/apps/slurm/slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/tb/api.py` & `cg-60.4.1/cg/apps/tb/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/apps/tb/models.py` & `cg-60.4.1/cg/apps/tb/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/add.py` & `cg-60.4.1/cg/cli/add.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/archive.py` & `cg-60.4.1/cg/cli/archive.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/backup.py` & `cg-60.4.1/cg/cli/backup.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/base.py` & `cg-60.4.1/cg/cli/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/clean.py` & `cg-60.4.1/cg/cli/clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/compress/base.py` & `cg-60.4.1/cg/cli/compress/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/compress/fastq.py` & `cg-60.4.1/cg/cli/compress/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/compress/helpers.py` & `cg-60.4.1/cg/cli/compress/helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/delete/base.py` & `cg-60.4.1/cg/cli/delete/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/delete/case.py` & `cg-60.4.1/cg/cli/delete/case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/delete/cases.py` & `cg-60.4.1/cg/cli/delete/cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/delete/observations.py` & `cg-60.4.1/cg/cli/delete/observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/deliver/base.py` & `cg-60.4.1/cg/cli/deliver/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/demultiplex/base.py` & `cg-60.4.1/cg/cli/demultiplex/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py` & `cg-60.4.1/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/demultiplex/demux.py` & `cg-60.4.1/cg/cli/demultiplex/demux.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/demultiplex/finish.py` & `cg-60.4.1/cg/cli/demultiplex/finish.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/demultiplex/sample_sheet.py` & `cg-60.4.1/cg/cli/demultiplex/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/downsample.py` & `cg-60.4.1/cg/cli/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/generate/report/base.py` & `cg-60.4.1/cg/cli/generate/report/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/generate/report/options.py` & `cg-60.4.1/cg/cli/generate/report/options.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/generate/report/utils.py` & `cg-60.4.1/cg/cli/generate/report/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/get.py` & `cg-60.4.1/cg/cli/get.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/set/base.py` & `cg-60.4.1/cg/cli/set/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/set/case.py` & `cg-60.4.1/cg/cli/set/case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/set/cases.py` & `cg-60.4.1/cg/cli/set/cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/store/base.py` & `cg-60.4.1/cg/cli/store/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/store/store.py` & `cg-60.4.1/cg/cli/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/transfer.py` & `cg-60.4.1/cg/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/upload/base.py` & `cg-60.4.1/cg/cli/upload/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/upload/clinical_delivery.py` & `cg-60.4.1/cg/cli/upload/clinical_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/upload/coverage.py` & `cg-60.4.1/cg/cli/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/upload/delivery_report.py` & `cg-60.4.1/cg/cli/upload/delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/upload/fohm.py` & `cg-60.4.1/cg/cli/upload/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/upload/genotype.py` & `cg-60.4.1/cg/cli/upload/genotype.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/upload/gens.py` & `cg-60.4.1/cg/cli/upload/gens.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/upload/gisaid.py` & `cg-60.4.1/cg/cli/upload/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/upload/mutacc.py` & `cg-60.4.1/cg/cli/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/upload/nipt/base.py` & `cg-60.4.1/cg/cli/upload/nipt/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/upload/nipt/ftp.py` & `cg-60.4.1/cg/cli/upload/nipt/ftp.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/upload/nipt/statina.py` & `cg-60.4.1/cg/cli/upload/nipt/statina.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/upload/observations/observations.py` & `cg-60.4.1/cg/cli/upload/observations/observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/upload/observations/utils.py` & `cg-60.4.1/cg/cli/upload/observations/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/upload/scout.py` & `cg-60.4.1/cg/cli/upload/scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/upload/utils.py` & `cg-60.4.1/cg/cli/upload/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/upload/validate.py` & `cg-60.4.1/cg/cli/upload/validate.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/workflow/balsamic/base.py` & `cg-60.4.1/cg/cli/workflow/balsamic/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/workflow/balsamic/options.py` & `cg-60.4.1/cg/cli/workflow/balsamic/options.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/workflow/balsamic/pon.py` & `cg-60.4.1/cg/cli/workflow/balsamic/pon.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/workflow/balsamic/qc.py` & `cg-60.4.1/cg/cli/workflow/balsamic/qc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/workflow/balsamic/umi.py` & `cg-60.4.1/cg/cli/workflow/balsamic/umi.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/workflow/base.py` & `cg-60.4.1/cg/cli/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/workflow/commands.py` & `cg-60.4.1/cg/cli/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/workflow/fastq/base.py` & `cg-60.4.1/cg/cli/workflow/fastq/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/workflow/fastq/fastq_service.py` & `cg-60.4.1/cg/cli/workflow/fastq/fastq_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/workflow/fluffy/base.py` & `cg-60.4.1/cg/cli/workflow/fluffy/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/workflow/jasen/base.py` & `cg-60.4.1/cg/cli/workflow/jasen/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/workflow/microsalt/base.py` & `cg-60.4.1/cg/cli/workflow/microsalt/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/workflow/mip/base.py` & `cg-60.4.1/cg/cli/workflow/mip/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/workflow/mip/options.py` & `cg-60.4.1/cg/cli/workflow/mip/options.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/workflow/mip_dna/base.py` & `cg-60.4.1/cg/cli/workflow/mip_dna/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/workflow/mip_rna/base.py` & `cg-60.4.1/cg/cli/workflow/mip_rna/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/workflow/mutant/base.py` & `cg-60.4.1/cg/cli/workflow/mutant/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/workflow/nf_analysis.py` & `cg-60.4.1/cg/cli/workflow/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/workflow/raredisease/base.py` & `cg-60.4.1/cg/cli/workflow/raredisease/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/workflow/rnafusion/base.py` & `cg-60.4.1/cg/cli/workflow/rnafusion/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/workflow/taxprofiler/base.py` & `cg-60.4.1/cg/cli/workflow/taxprofiler/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/cli/workflow/tomte/base.py` & `cg-60.4.1/cg/cli/workflow/tomte/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/clients/arnold/api.py` & `cg-60.4.1/cg/clients/arnold/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/clients/janus/api.py` & `cg-60.4.1/cg/clients/janus/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/constants/__init__.py` & `cg-60.4.1/cg/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/constants/bcl_convert_metrics.py` & `cg-60.4.1/cg/constants/bcl_convert_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/constants/constants.py` & `cg-60.4.1/cg/constants/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/constants/delivery.py` & `cg-60.4.1/cg/constants/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/constants/demultiplexing.py` & `cg-60.4.1/cg/constants/demultiplexing.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/constants/encryption.py` & `cg-60.4.1/cg/constants/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/constants/gene_panel.py` & `cg-60.4.1/cg/constants/gene_panel.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
 from cg.constants.constants import CustomerId
 
 GENOME_BUILD_37: str = "37"
 GENOME_BUILD_38: str = "GRCh38"
 
 
+class GenePanelGenomeBuild(StrEnum):
+    hg19: str = GENOME_BUILD_37
+    hg38: str = GENOME_BUILD_38
+
+
 class GenePanelMasterList(StrEnum):
     BRAIN: str = "BRAIN"
     CARDIOLOGY: str = "Cardiology"
     CILM: str = "CILM"
     CH: str = "CH"
     CTD: str = "CTD"
     DIAB: str = "DIAB"
```

### Comparing `cg-60.4.0/cg/constants/housekeeper_tags.py` & `cg-60.4.1/cg/constants/housekeeper_tags.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/constants/lims.py` & `cg-60.4.1/cg/constants/lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/constants/metrics.py` & `cg-60.4.1/cg/constants/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/constants/nextflow.py` & `cg-60.4.1/cg/constants/nextflow.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/constants/nf_analysis.py` & `cg-60.4.1/cg/constants/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/constants/observations.py` & `cg-60.4.1/cg/constants/observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/constants/orderforms.py` & `cg-60.4.1/cg/constants/orderforms.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/constants/priority.py` & `cg-60.4.1/cg/constants/priority.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/constants/report.py` & `cg-60.4.1/cg/constants/report.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/constants/scout.py` & `cg-60.4.1/cg/constants/scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/constants/sequencing.py` & `cg-60.4.1/cg/constants/sequencing.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/constants/subject.py` & `cg-60.4.1/cg/constants/subject.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/exc.py` & `cg-60.4.1/cg/exc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/io/api.py` & `cg-60.4.1/cg/io/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/io/config.py` & `cg-60.4.1/cg/io/config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/io/controller.py` & `cg-60.4.1/cg/io/controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/io/csv.py` & `cg-60.4.1/cg/io/csv.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/io/json.py` & `cg-60.4.1/cg/io/json.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/io/png.py` & `cg-60.4.1/cg/io/png.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/io/txt.py` & `cg-60.4.1/cg/io/txt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/io/validate_path.py` & `cg-60.4.1/cg/io/validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/io/xml.py` & `cg-60.4.1/cg/io/xml.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/io/yaml.py` & `cg-60.4.1/cg/io/yaml.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/archive/archive.py` & `cg-60.4.1/cg/meta/archive/archive.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/archive/ddn/constants.py` & `cg-60.4.1/cg/meta/archive/ddn/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/archive/ddn/ddn_data_flow_client.py` & `cg-60.4.1/cg/meta/archive/ddn/ddn_data_flow_client.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/archive/ddn/models.py` & `cg-60.4.1/cg/meta/archive/ddn/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/archive/ddn/utils.py` & `cg-60.4.1/cg/meta/archive/ddn/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/archive/models.py` & `cg-60.4.1/cg/meta/archive/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/backup/backup.py` & `cg-60.4.1/cg/meta/backup/backup.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/backup/pdc.py` & `cg-60.4.1/cg/meta/backup/pdc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/clean/api.py` & `cg-60.4.1/cg/meta/clean/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/clean/clean_flow_cells.py` & `cg-60.4.1/cg/meta/clean/clean_flow_cells.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/clean/clean_retrieved_spring_files.py` & `cg-60.4.1/cg/meta/clean/clean_retrieved_spring_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/compress/compress.py` & `cg-60.4.1/cg/meta/compress/compress.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/compress/files.py` & `cg-60.4.1/cg/meta/compress/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/deliver/deliver.py` & `cg-60.4.1/cg/meta/deliver/deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/deliver/deliver_ticket.py` & `cg-60.4.1/cg/meta/deliver/deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/deliver/fastq_path_generator.py` & `cg-60.4.1/cg/meta/deliver/fastq_path_generator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/delivery/delivery.py` & `cg-60.4.1/cg/meta/delivery/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/demultiplex/combine_sequencing_metrics.py` & `cg-60.4.1/cg/meta/demultiplex/combine_sequencing_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/demultiplex/demux_post_processing.py` & `cg-60.4.1/cg/meta/demultiplex/demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/demultiplex/files.py` & `cg-60.4.1/cg/meta/demultiplex/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/demultiplex/housekeeper_storage_functions.py` & `cg-60.4.1/cg/meta/demultiplex/housekeeper_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/demultiplex/status_db_storage_functions.py` & `cg-60.4.1/cg/meta/demultiplex/status_db_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/demultiplex/utils.py` & `cg-60.4.1/cg/meta/demultiplex/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/demultiplex/validation.py` & `cg-60.4.1/cg/meta/demultiplex/validation.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/encryption/encryption.py` & `cg-60.4.1/cg/meta/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/encryption/sbatch.py` & `cg-60.4.1/cg/meta/encryption/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/invoice.py` & `cg-60.4.1/cg/meta/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/meta.py` & `cg-60.4.1/cg/meta/meta.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/observations/balsamic_observations_api.py` & `cg-60.4.1/cg/meta/observations/balsamic_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/observations/mip_dna_observations_api.py` & `cg-60.4.1/cg/meta/observations/mip_dna_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/observations/observations_api.py` & `cg-60.4.1/cg/meta/observations/observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/orders/api.py` & `cg-60.4.1/cg/meta/orders/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/orders/case_submitter.py` & `cg-60.4.1/cg/meta/orders/case_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/orders/fastq_submitter.py` & `cg-60.4.1/cg/meta/orders/fastq_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/orders/lims.py` & `cg-60.4.1/cg/meta/orders/lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/orders/metagenome_submitter.py` & `cg-60.4.1/cg/meta/orders/metagenome_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/orders/microbial_submitter.py` & `cg-60.4.1/cg/meta/orders/microbial_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/orders/pool_submitter.py` & `cg-60.4.1/cg/meta/orders/pool_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/orders/rnafusion_submitter.py` & `cg-60.4.1/cg/meta/orders/rnafusion_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/orders/sars_cov_2_submitter.py` & `cg-60.4.1/cg/meta/orders/sars_cov_2_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/orders/submitter.py` & `cg-60.4.1/cg/meta/orders/submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/orders/ticket_handler.py` & `cg-60.4.1/cg/meta/orders/ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/qc_metrics/collect_qc_metrics.py` & `cg-60.4.1/cg/meta/qc_metrics/collect_qc_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/balsamic.py` & `cg-60.4.1/cg/meta/report/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/balsamic_qc.py` & `cg-60.4.1/cg/meta/report/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/balsamic_umi.py` & `cg-60.4.1/cg/meta/report/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/field_validators.py` & `cg-60.4.1/cg/meta/report/field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/mip_dna.py` & `cg-60.4.1/cg/meta/report/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/report_api.py` & `cg-60.4.1/cg/meta/report/report_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,43 +11,28 @@
 
 from cg.constants import DELIVERY_REPORT_FILE_NAME, SWEDAC_LOGO_PATH, Workflow
 from cg.constants.constants import MAX_ITEMS_TO_RETRIEVE, FileFormat
 from cg.constants.housekeeper_tags import HK_DELIVERY_REPORT_TAG, HermesFileTag
 from cg.exc import DeliveryReportError
 from cg.io.controller import ReadFile, WriteStream
 from cg.meta.meta import MetaAPI
-from cg.meta.report.field_validators import (
-    get_empty_report_data,
-    get_missing_report_data,
-)
+from cg.meta.report.field_validators import get_empty_report_data, get_missing_report_data
 from cg.meta.workflow.analysis import AnalysisAPI
 from cg.models.analysis import AnalysisModel
 from cg.models.cg_config import CGConfig
 from cg.models.report.metadata import SampleMetadataModel
 from cg.models.report.report import (
     CaseModel,
     CustomerModel,
     DataAnalysisModel,
     ReportModel,
     ScoutReportFiles,
 )
-from cg.models.report.sample import (
-    ApplicationModel,
-    MethodsModel,
-    SampleModel,
-    TimestampModel,
-)
-from cg.store.models import (
-    Analysis,
-    Application,
-    ApplicationLimitations,
-    Case,
-    CaseSample,
-    Sample,
-)
+from cg.models.report.sample import ApplicationModel, MethodsModel, SampleModel, TimestampModel
+from cg.store.models import Analysis, Application, ApplicationLimitations, Case, CaseSample, Sample
 
 LOG = logging.getLogger(__name__)
 
 
 class ReportAPI(MetaAPI):
     """Common Delivery Report API."""
```

### Comparing `cg-60.4.0/cg/meta/report/rnafusion.py` & `cg-60.4.1/cg/meta/report/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/templates/delivery-report.html` & `cg-60.4.1/cg/meta/report/templates/delivery-report.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/templates/macros/data_analysis/data_analysis.html` & `cg-60.4.1/cg/meta/report/templates/macros/data_analysis/data_analysis.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/templates/macros/data_analysis/limitations.html` & `cg-60.4.1/cg/meta/report/templates/macros/data_analysis/limitations.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html` & `cg-60.4.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html` & `cg-60.4.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html` & `cg-60.4.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html` & `cg-60.4.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html` & `cg-60.4.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/templates/macros/header.html` & `cg-60.4.1/cg/meta/report/templates/macros/header.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/templates/macros/order.html` & `cg-60.4.1/cg/meta/report/templates/macros/order.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/templates/macros/sample_prep.html` & `cg-60.4.1/cg/meta/report/templates/macros/sample_prep.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html` & `cg-60.4.1/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html` & `cg-60.4.1/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html` & `cg-60.4.1/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/templates/static/css/bootstrap.min.css` & `cg-60.4.1/cg/meta/report/templates/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/templates/static/images/SWEDAC_logo.png` & `cg-60.4.1/cg/meta/report/templates/static/images/SWEDAC_logo.png`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/report/tomte.py` & `cg-60.4.1/cg/meta/report/tomte.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/rsync/rsync_api.py` & `cg-60.4.1/cg/meta/rsync/rsync_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/tar/tar.py` & `cg-60.4.1/cg/meta/tar/tar.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/transfer/external_data.py` & `cg-60.4.1/cg/meta/transfer/external_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/transfer/lims.py` & `cg-60.4.1/cg/meta/transfer/lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/upload/balsamic/balsamic.py` & `cg-60.4.1/cg/meta/upload/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/upload/coverage.py` & `cg-60.4.1/cg/meta/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/upload/fohm/fohm.py` & `cg-60.4.1/cg/meta/upload/fohm/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/upload/gisaid/constants.py` & `cg-60.4.1/cg/meta/upload/gisaid/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/upload/gisaid/gisaid.py` & `cg-60.4.1/cg/meta/upload/gisaid/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/upload/gisaid/models.py` & `cg-60.4.1/cg/meta/upload/gisaid/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/upload/gt.py` & `cg-60.4.1/cg/meta/upload/gt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/upload/microsalt/microsalt_upload_api.py` & `cg-60.4.1/cg/meta/upload/microsalt/microsalt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/upload/mip/mip_dna.py` & `cg-60.4.1/cg/meta/upload/mip/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/upload/mip/mip_rna.py` & `cg-60.4.1/cg/meta/upload/mip/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/upload/mutacc.py` & `cg-60.4.1/cg/meta/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/upload/nf_analysis.py` & `cg-60.4.1/cg/meta/upload/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/upload/nipt/models.py` & `cg-60.4.1/cg/meta/upload/nipt/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/upload/nipt/nipt.py` & `cg-60.4.1/cg/meta/upload/nipt/nipt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/upload/scout/balsamic_config_builder.py` & `cg-60.4.1/cg/meta/upload/scout/balsamic_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/upload/scout/balsamic_umi_config_builder.py` & `cg-60.4.1/cg/meta/upload/scout/balsamic_umi_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/upload/scout/hk_tags.py` & `cg-60.4.1/cg/meta/upload/scout/hk_tags.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/upload/scout/mip_config_builder.py` & `cg-60.4.1/cg/meta/upload/scout/mip_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/upload/scout/rnafusion_config_builder.py` & `cg-60.4.1/cg/meta/upload/scout/rnafusion_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/upload/scout/scout_config_builder.py` & `cg-60.4.1/cg/meta/upload/scout/scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/upload/scout/uploadscoutapi.py` & `cg-60.4.1/cg/meta/upload/scout/uploadscoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/upload/upload_api.py` & `cg-60.4.1/cg/meta/upload/upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/workflow/analysis.py` & `cg-60.4.1/cg/meta/workflow/analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 import datetime as dt
 import logging
 import os
 import shutil
 from pathlib import Path
 from subprocess import CalledProcessError
-from typing import Any
+from typing import Any, Iterator
 
 import click
+import requests
 from housekeeper.store.models import Bundle, Version
 
 from cg.apps.environ import environ_email
 from cg.constants import EXIT_FAIL, EXIT_SUCCESS, Priority, SequencingFileTag, Workflow
-from cg.constants.constants import (
-    AnalysisType,
-    CaseActions,
-    FileFormat,
-    WorkflowManager,
-)
-from cg.constants.gene_panel import GenePanelCombo
+from cg.constants.constants import AnalysisType, CaseActions, FileFormat, WorkflowManager
+from cg.constants.gene_panel import GenePanelCombo, GenePanelMasterList
 from cg.constants.scout import ScoutExportFileName
 from cg.constants.tb import AnalysisStatus
 from cg.exc import AnalysisNotReadyError, BundleAlreadyAddedError, CgDataError, CgError
 from cg.io.controller import WriteFile
 from cg.meta.archive.archive import SpringArchiveAPI
 from cg.meta.meta import MetaAPI
 from cg.services.quality_controller import QualityControllerService
@@ -185,14 +181,28 @@
         if len(application_types) > 1:
             raise CgError(
                 f"Different application_types found for case: {case_id} ({application_types})"
             )
 
         return application_types.pop()
 
+    def get_case_source_type(self, case_id: str) -> str | None:
+        """Returns the source type for samples in a case.
+        Raises:
+            CgError: If different sources are set for the samples linked to a case."""
+        sample_ids: Iterator[str] = self.status_db.get_sample_ids_by_case_id(case_id=case_id)
+        source_types: set[str | None] = {
+            self.lims_api.get_source(lims_id=sample_id) for sample_id in sample_ids
+        }
+
+        if len(source_types) > 1:
+            raise CgError(f"Different source types found for case: {case_id} ({source_types})")
+
+        return source_types.pop()
+
     def has_case_only_exome_samples(self, case_id: str) -> bool:
         """Returns True if the application type for all samples in a case is WES."""
         application_type: str = self.get_case_application_type(case_id)
         return application_type == AnalysisType.WHOLE_EXOME_SEQUENCING
 
     def upload_bundle_housekeeper(self, case_id: str, dry_run: bool = False) -> None:
         """Storing bundle data in Housekeeper for CASE_ID"""
@@ -627,34 +637,57 @@
             content="\n".join(content),
             file_format=FileFormat.TXT,
             file_path=Path(out_dir, ScoutExportFileName.MANAGED_VARIANTS),
         )
 
     @staticmethod
     def _write_panel(out_dir: Path, content: list[str]) -> None:
-        """Write the managed variants to case dir."""
+        """Write the gene panel to case dir."""
         out_dir.mkdir(parents=True, exist_ok=True)
         WriteFile.write_file_from_content(
             content="\n".join(content),
             file_format=FileFormat.TXT,
             file_path=Path(out_dir, ScoutExportFileName.PANELS),
         )
 
-    def _get_gene_panel(self, case_id: str, genome_build: str) -> list[str]:
+    def _get_gene_panel(self, case_id: str, genome_build: str, dry_run: bool = False) -> list[str]:
         """Create and return the aggregated gene panel file."""
         case: Case = self.status_db.get_case_by_internal_id(internal_id=case_id)
         all_panels: list[str] = self.get_aggregated_panels(
             customer_id=case.customer.internal_id, default_panels=set(case.panels)
         )
-        return self.scout_api.export_panels(build=genome_build, panels=all_panels)
+        return self.scout_api.export_panels(build=genome_build, panels=all_panels, dry_run=dry_run)
+
+    def get_gene_panel(self, case_id: str, dry_run: bool = False) -> list[str]:
+        """Create and return the aggregated gene panel file."""
+        raise NotImplementedError
 
     def _get_managed_variants(self, genome_build: str) -> list[str]:
         """Create and return the managed variants."""
         return self.scout_api.export_managed_variants(genome_build=genome_build)
 
+    def write_panel(self, case_id: str, content: list[str]) -> None:
+        """Write the gene panel to case dir."""
+        self._write_panel(out_dir=Path(self.root, case_id), content=content)
+
+    @staticmethod
+    def get_aggregated_panels(customer_id: str, default_panels: set[str]) -> list[str]:
+        """Check if customer should use the gene panel master list
+        and if all default panels are included in the gene panel master list.
+        If not, add gene panel combo and OMIM-AUTO.
+        Return an aggregated gene panel."""
+        master_list: list[str] = GenePanelMasterList.get_panel_names()
+        if customer_id in GenePanelMasterList.collaborators() and default_panels.issubset(
+            master_list
+        ):
+            return master_list
+        all_panels: set[str] = add_gene_panel_combo(default_panels=default_panels)
+        all_panels |= {GenePanelMasterList.OMIM_AUTO, GenePanelMasterList.PANELAPP_GREEN}
+        return list(all_panels)
+
     def run_analysis(self, *args, **kwargs):
         raise NotImplementedError
 
     def get_data_analysis_type(self, case_id: str) -> str | None:
         """Return data analysis type carried out."""
         case_sample: Sample = self.status_db.get_case_samples_by_case_id(case_internal_id=case_id)[
             0
```

### Comparing `cg-60.4.0/cg/meta/workflow/balsamic.py` & `cg-60.4.1/cg/meta/workflow/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/workflow/balsamic_pon.py` & `cg-60.4.1/cg/meta/workflow/balsamic_pon.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/workflow/balsamic_qc.py` & `cg-60.4.1/cg/meta/workflow/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/workflow/balsamic_umi.py` & `cg-60.4.1/cg/meta/workflow/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/workflow/downsample/downsample.py` & `cg-60.4.1/cg/meta/workflow/downsample/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/workflow/downsample/sbatch.py` & `cg-60.4.1/cg/meta/workflow/downsample/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/workflow/fastq.py` & `cg-60.4.1/cg/meta/workflow/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/workflow/fluffy.py` & `cg-60.4.1/cg/meta/workflow/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/workflow/jasen.py` & `cg-60.4.1/cg/meta/workflow/jasen.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/workflow/microsalt/metrics_parser/models.py` & `cg-60.4.1/cg/meta/workflow/microsalt/metrics_parser/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/workflow/microsalt/microsalt.py` & `cg-60.4.1/cg/meta/workflow/microsalt/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/workflow/microsalt/quality_controller/models.py` & `cg-60.4.1/cg/meta/workflow/microsalt/quality_controller/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/workflow/microsalt/quality_controller/quality_controller.py` & `cg-60.4.1/cg/meta/workflow/microsalt/quality_controller/quality_controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/workflow/microsalt/quality_controller/report_generator.py` & `cg-60.4.1/cg/meta/workflow/microsalt/quality_controller/report_generator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/workflow/microsalt/quality_controller/result_logger.py` & `cg-60.4.1/cg/meta/workflow/microsalt/quality_controller/result_logger.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/workflow/microsalt/quality_controller/utils.py` & `cg-60.4.1/cg/meta/workflow/microsalt/quality_controller/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/workflow/microsalt/utils.py` & `cg-60.4.1/cg/meta/workflow/microsalt/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/workflow/mip.py` & `cg-60.4.1/cg/meta/workflow/mip.py`

 * *Files 9% similar despite different names*

```diff
@@ -145,33 +145,14 @@
         )
 
     def link_fastq_files(self, case_id: str, dry_run: bool = False) -> None:
         case: Case = self.status_db.get_case_by_internal_id(internal_id=case_id)
         for link in case.links:
             self.link_fastq_files_for_sample(case=case, sample=link.sample)
 
-    def write_panel(self, case_id: str, content: list[str]) -> None:
-        """Write the gene panel to case dir."""
-        self._write_panel(out_dir=Path(self.root, case_id), content=content)
-
-    @staticmethod
-    def get_aggregated_panels(customer_id: str, default_panels: set[str]) -> list[str]:
-        """Check if customer should use the gene panel master list
-        and if all default panels are included in the gene panel master list.
-        If not, add gene panel combo and OMIM-AUTO.
-        Return an aggregated gene panel."""
-        master_list: list[str] = GenePanelMasterList.get_panel_names()
-        if customer_id in GenePanelMasterList.collaborators() and default_panels.issubset(
-            master_list
-        ):
-            return master_list
-        all_panels: set[str] = add_gene_panel_combo(default_panels=default_panels)
-        all_panels |= {GenePanelMasterList.OMIM_AUTO, GenePanelMasterList.PANELAPP_GREEN}
-        return list(all_panels)
-
     def _get_latest_raw_file(self, family_id: str, tags: list[str]) -> Any:
         """Get a python object file for a tag and a family ."""
 
         last_version = self.housekeeper_api.last_version(bundle=family_id)
 
         analysis_files = self.housekeeper_api.files(
             bundle=family_id, version=last_version.id, tags=tags
```

### Comparing `cg-60.4.0/cg/meta/workflow/mip_dna.py` & `cg-60.4.1/cg/meta/workflow/mip_dna.py`

 * *Files 14% similar despite different names*

```diff
@@ -57,17 +57,17 @@
             )
         if link_obj.mother:
             sample_data[Pedigree.MOTHER.value]: str = link_obj.mother.internal_id
         if link_obj.father:
             sample_data[Pedigree.FATHER.value]: str = link_obj.father.internal_id
         return sample_data
 
-    def get_gene_panel(self, case_id: str) -> list[str]:
+    def get_gene_panel(self, case_id: str, dry_run: bool = False) -> list[str]:
         """Create and return the aggregated gene panel file."""
-        return self._get_gene_panel(case_id=case_id, genome_build=GENOME_BUILD_37)
+        return self._get_gene_panel(case_id=case_id, genome_build=GENOME_BUILD_37, dry_run=dry_run)
 
     def get_managed_variants(self) -> list[str]:
         """Create and return the managed variants."""
         return self._get_managed_variants(genome_build=GENOME_BUILD_37)
 
     def get_genome_build(self, case_id: str) -> str:
         """Return the reference genome build version of a MIP-DNA analysis."""
```

### Comparing `cg-60.4.0/cg/meta/workflow/mip_rna.py` & `cg-60.4.1/cg/meta/workflow/mip_rna.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,14 @@
         sample_data: dict[str, str | int] = self.get_sample_data(link_obj)
         if link_obj.mother:
             sample_data[Pedigree.MOTHER.value]: str = link_obj.mother.internal_id
         if link_obj.father:
             sample_data[Pedigree.FATHER.value]: str = link_obj.father.internal_id
         return sample_data
 
-    def get_gene_panel(self, case_id: str) -> list[str]:
+    def get_gene_panel(self, case_id: str, dry_run: bool = False) -> list[str]:
         """Create and return the aggregated gene panel file."""
-        return self._get_gene_panel(case_id=case_id, genome_build=GENOME_BUILD_38)
+        return self._get_gene_panel(case_id=case_id, genome_build=GENOME_BUILD_38, dry_run=dry_run)
 
     def get_managed_variants(self) -> list[str]:
         """Create and return the managed variants."""
         return self._get_managed_variants(genome_build=GENOME_BUILD_38)
```

### Comparing `cg-60.4.0/cg/meta/workflow/mutant.py` & `cg-60.4.1/cg/meta/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/workflow/nf_analysis.py` & `cg-60.4.1/cg/meta/workflow/nf_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,26 +10,27 @@
     CaseActions,
     FileExtensions,
     FileFormat,
     GenomeVersion,
     MultiQC,
     WorkflowManager,
 )
+from cg.constants.gene_panel import GenePanelGenomeBuild
 from cg.constants.nextflow import NFX_WORK_DIR
 from cg.constants.nf_analysis import NfTowerStatus
 from cg.constants.tb import AnalysisStatus
 from cg.exc import CgError, HousekeeperStoreError, MetricsQCError
 from cg.io.config import write_config_nextflow_style
 from cg.io.controller import ReadFile, WriteFile
 from cg.io.json import read_json
 from cg.io.txt import concat_txt, write_txt
 from cg.io.yaml import write_yaml_nextflow_style
 from cg.meta.workflow.analysis import AnalysisAPI
 from cg.meta.workflow.nf_handlers import NextflowHandler, NfTowerHandler
-from cg.models.analysis import NextflowAnalysis, AnalysisModel
+from cg.models.analysis import NextflowAnalysis
 from cg.models.cg_config import CGConfig
 from cg.models.deliverables.metric_deliverables import (
     MetricsBase,
     MetricsDeliverablesCondition,
     MultiqcDataJson,
 )
 from cg.models.fastq import FastqFileMeta
@@ -107,14 +108,19 @@
 
     @property
     def is_multiqc_pattern_search_exact(self) -> bool:
         """Return True if only exact pattern search is allowed to collect metrics information from MultiQC file.
         If false, pattern must be present but does not need to be exact."""
         return False
 
+    @property
+    def is_gene_panel_required(self) -> bool:
+        """Return True if a gene panel is needs to be created using the information in StatusDB and exporting it from Scout."""
+        return False
+
     def get_profile(self, profile: str | None = None) -> str:
         """Get NF profiles."""
         return profile or self.profile
 
     def get_workflow_manager(self) -> str:
         """Get workflow manager from Tower."""
         return WorkflowManager.Tower.value
@@ -211,14 +217,20 @@
 
     def get_workdir_path(self, case_id: str, work_dir: Path | None = None) -> Path:
         """Path to NF work directory."""
         if work_dir:
             return work_dir.absolute()
         return Path(self.get_case_path(case_id), NFX_WORK_DIR)
 
+    def get_gene_panels_path(self, case_id: str) -> Path:
+        """Path to gene panels bed file exported from Scout."""
+        return Path(self.get_case_path(case_id=case_id), "gene_panels").with_suffix(
+            FileExtensions.BED
+        )
+
     def set_cluster_options(self, case_id: str) -> str:
         return f'process.clusterOptions = "-A {self.account} --qos={self.get_slurm_qos_for_case(case_id=case_id)}"\n'
 
     @staticmethod
     def extract_read_files(
         metadata: list[FastqFileMeta], forward_read: bool = False, reverse_read: bool = False
     ) -> list[str]:
@@ -348,23 +360,35 @@
             if dry_run:
                 return
             write_txt(
                 content=content,
                 file_path=self.get_nextflow_config_path(case_id=case_id),
             )
 
+    def create_gene_panel(self, case_id: str, dry_run: bool) -> None:
+        """Create and write an aggregated gene panel file exported from Scout."""
+        LOG.info("Creating gene panel file")
+        bed_lines: list[str] = self.get_gene_panel(case_id=case_id, dry_run=dry_run)
+        if dry_run:
+            bed_lines: str = "\n".join(bed_lines)
+            LOG.debug(f"{bed_lines}")
+            return
+        self.write_panel(case_id=case_id, content=bed_lines)
+
     def config_case(self, case_id: str, dry_run: bool):
         """Create directory and config files required by a workflow for a case."""
         if dry_run:
             LOG.info("Dry run: Config files will not be written")
         self.status_db.verify_case_exists(case_internal_id=case_id)
         self.create_case_directory(case_id=case_id, dry_run=dry_run)
         self.create_sample_sheet(case_id=case_id, dry_run=dry_run)
         self.create_params_file(case_id=case_id, dry_run=dry_run)
         self.create_nextflow_config(case_id=case_id, dry_run=dry_run)
+        if self.is_gene_panel_required:
+            self.create_gene_panel(case_id=case_id, dry_run=dry_run)
 
     def _run_analysis_with_nextflow(
         self, case_id: str, command_args: NfCommandArgs, dry_run: bool
     ) -> None:
         """Run analysis with given options using Nextflow."""
         self.process = Process(
             binary=self.nextflow_binary_path,
@@ -808,25 +832,55 @@
         return [
             case
             for case in self.status_db.get_running_cases_in_workflow(workflow=self.workflow)
             if self.trailblazer_api.is_latest_analysis_completed(case_id=case.internal_id)
             or self.trailblazer_api.is_latest_analysis_qc(case_id=case.internal_id)
         ]
 
+    def get_genome_build(self, case_id: str) -> GenomeVersion:
+        """Return reference genome version for a case.
+        Raises CgError if this information is missing or inconsistent for the samples linked to a case.
+        """
+        reference_genome: set[str] = {
+            sample.reference_genome
+            for sample in self.status_db.get_samples_by_case_id(case_id=case_id)
+        }
+        if len(reference_genome) == 1:
+            return reference_genome.pop()
+        if len(reference_genome) > 1:
+            raise CgError(
+                f"Samples linked to case {case_id} have different reference genome versions set"
+            )
+        raise CgError(f"No reference genome specified for case {case_id}")
+
+    def get_gene_panel_genome_build(self, case_id: str) -> GenePanelGenomeBuild:
+        """Return build version of the gene panel for a case."""
+        reference_genome: GenomeVersion = self.get_genome_build(case_id=case_id)
+        try:
+            return getattr(GenePanelGenomeBuild, reference_genome)
+        except AttributeError as error:
+            raise CgError(
+                f"Reference {reference_genome} has no associated genome build for panels: {error}"
+            ) from error
+
+    def get_gene_panel(self, case_id: str, dry_run: bool = False) -> list[str]:
+        """Create and return the aggregated gene panel file."""
+        return self._get_gene_panel(
+            case_id=case_id,
+            genome_build=self.get_gene_panel_genome_build(case_id=case_id),
+            dry_run=dry_run,
+        )
+
     def parse_analysis(self, qc_metrics_raw: list[MetricsBase], **kwargs) -> NextflowAnalysis:
         """Parse Nextflow output analysis files and return an analysis model."""
         sample_metrics: dict[str, dict] = {}
         for metric in qc_metrics_raw:
             try:
                 sample_metrics[metric.id].update({metric.name.lower(): metric.value})
             except KeyError:
                 sample_metrics[metric.id] = {metric.name.lower(): metric.value}
         return NextflowAnalysis(sample_metrics=sample_metrics)
 
     def get_latest_metadata(self, case_id: str) -> NextflowAnalysis:
         """Return analysis output of a Nextflow case."""
         qc_metrics: list[MetricsBase] = self.get_multiqc_json_metrics(case_id)
         return self.parse_analysis(qc_metrics_raw=qc_metrics)
-
-    def get_genome_build(self, case_id: str) -> str:
-        """Return the reference genome build version of Nextflow analysis."""
-        return GenomeVersion.hg38.value
```

### Comparing `cg-60.4.0/cg/meta/workflow/nf_handlers.py` & `cg-60.4.1/cg/meta/workflow/nf_handlers.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/workflow/prepare_fastq.py` & `cg-60.4.1/cg/meta/workflow/prepare_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/workflow/raredisease.py` & `cg-60.4.1/cg/meta/workflow/raredisease.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Module for Raredisease Analysis API."""
 
 import logging
 from pathlib import Path
 
-from cg.constants import GenePanelMasterList, Workflow
-from cg.constants.subject import PlinkPhenotypeStatus, PlinkSex
-from cg.constants.gene_panel import GENOME_BUILD_37
+from cg.constants import Workflow
+from cg.constants.constants import GenomeVersion
+from cg.constants.gene_panel import GenePanelGenomeBuild
 from cg.constants.nf_analysis import RAREDISEASE_METRIC_CONDITIONS
-from cg.meta.workflow.analysis import add_gene_panel_combo
+from cg.constants.subject import PlinkPhenotypeStatus, PlinkSex
 from cg.meta.workflow.nf_analysis import NfAnalysisAPI
 from cg.models.cg_config import CGConfig
+from cg.models.nf_analysis import WorkflowParameters
 from cg.models.raredisease.raredisease import (
     RarediseaseSampleSheetEntry,
     RarediseaseSampleSheetHeaders,
 )
-from cg.models.nf_analysis import WorkflowParameters
 from cg.store.models import CaseSample
 
 LOG = logging.getLogger(__name__)
 
 
 class RarediseaseAnalysisAPI(NfAnalysisAPI):
     """Handles communication between RAREDISEASE processes
@@ -53,14 +53,18 @@
         return RarediseaseSampleSheetHeaders.list()
 
     @property
     def is_multiple_samples_allowed(self) -> bool:
         """Return whether the analysis supports multiple samples to be linked to the case."""
         return True
 
+    def get_genome_build(self, case_id: str) -> GenomeVersion:
+        """Return reference genome for a case. Currently fixed for hg19."""
+        return GenomeVersion.hg19
+
     def get_sample_sheet_content_per_sample(self, case_sample: CaseSample) -> list[list[str]]:
         """Collect and format information required to build a sample sheet for a single sample."""
         fastq_forward_read_paths, fastq_reverse_read_paths = self.get_paired_read_paths(
             sample=case_sample.sample
         )
         sample_sheet_entry = RarediseaseSampleSheetEntry(
             name=case_sample.sample.internal_id,
@@ -104,36 +108,13 @@
     @property
     def root(self) -> str:
         return self.config.raredisease.root
 
     def write_managed_variants(self, case_id: str, content: list[str]) -> None:
         self._write_managed_variants(out_dir=Path(self.root, case_id), content=content)
 
-    def write_panel(self, case_id: str, content: list[str]) -> None:
-        """Write the gene panel to case dir."""
-        self._write_panel(out_dir=Path(self.root, case_id), content=content)
-
-    @staticmethod
-    def get_aggregated_panels(customer_id: str, default_panels: set[str]) -> list[str]:
-        """Check if customer should use the gene panel master list
-        and if all default panels are included in the gene panel master list.
-        If not, add gene panel combo and OMIM-AUTO.
-        Return an aggregated gene panel."""
-        master_list: list[str] = GenePanelMasterList.get_panel_names()
-        if customer_id in GenePanelMasterList.collaborators() and default_panels.issubset(
-            master_list
-        ):
-            return master_list
-        all_panels: set[str] = add_gene_panel_combo(default_panels=default_panels)
-        all_panels |= {GenePanelMasterList.OMIM_AUTO, GenePanelMasterList.PANELAPP_GREEN}
-        return list(all_panels)
-
-    def get_gene_panel(self, case_id: str) -> list[str]:
-        """Create and return the aggregated gene panel file."""
-        return self._get_gene_panel(case_id=case_id, genome_build=GENOME_BUILD_37)
-
     def get_managed_variants(self) -> list[str]:
         """Create and return the managed variants."""
-        return self._get_managed_variants(genome_build=GENOME_BUILD_37)
+        return self._get_managed_variants(genome_build=GenePanelGenomeBuild.hg19)
 
     def get_workflow_metrics(self) -> dict:
         return RAREDISEASE_METRIC_CONDITIONS
```

### Comparing `cg-60.4.0/cg/meta/workflow/rnafusion.py` & `cg-60.4.1/cg/meta/workflow/rnafusion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module for Rnafusion Analysis API."""
 
 import logging
 from pathlib import Path
 
 from cg.constants import Workflow
-from cg.constants.constants import Strandedness
+from cg.constants.constants import GenomeVersion, Strandedness
 from cg.constants.nf_analysis import MULTIQC_NEXFLOW_CONFIG, RNAFUSION_METRIC_CONDITIONS
 from cg.exc import MissingMetrics
 from cg.meta.workflow.nf_analysis import NfAnalysisAPI
 from cg.models.analysis import AnalysisModel
 from cg.models.cg_config import CGConfig
 from cg.models.deliverables.metric_deliverables import MetricsBase
 from cg.models.rnafusion.rnafusion import RnafusionParameters, RnafusionSampleSheetEntry
@@ -53,14 +53,18 @@
         return False
 
     @property
     def is_multiple_samples_allowed(self) -> bool:
         """Return whether the analysis supports multiple samples to be linked to the case."""
         return False
 
+    def get_genome_build(self, case_id: str) -> GenomeVersion:
+        """Return reference genome for a case. Currently fixed for hg38."""
+        return GenomeVersion.hg38
+
     def get_nextflow_config_content(self, case_id: str) -> str:
         """Return nextflow config content."""
         return MULTIQC_NEXFLOW_CONFIG
 
     @staticmethod
     def get_bundle_filenames_path() -> Path:
         """Return Rnafusion bundle filenames path."""
```

### Comparing `cg-60.4.0/cg/meta/workflow/taxprofiler.py` & `cg-60.4.1/cg/meta/workflow/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/meta/workflow/tomte.py` & `cg-60.4.1/cg/meta/workflow/tomte.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 from pathlib import Path
 
 from cg.constants import Workflow
 from cg.constants.constants import Strandedness
 from cg.constants.nf_analysis import TOMTE_METRIC_CONDITIONS
 from cg.meta.workflow.nf_analysis import NfAnalysisAPI
 from cg.models.cg_config import CGConfig
-from cg.models.nf_analysis import WorkflowParameters
-from cg.models.tomte.tomte import TomteSampleSheetEntry, TomteSampleSheetHeaders
+from cg.models.tomte.tomte import TomteParameters, TomteSampleSheetEntry, TomteSampleSheetHeaders
 from cg.resources import TOMTE_BUNDLE_FILENAMES_PATH
 from cg.store.models import CaseSample
 
 LOG = logging.getLogger(__name__)
 
 
 class TomteAnalysisAPI(NfAnalysisAPI):
@@ -43,14 +42,19 @@
         self.nextflow_binary_path: str = config.tomte.binary_path
 
     @property
     def sample_sheet_headers(self) -> list[str]:
         """Headers for sample sheet."""
         return TomteSampleSheetHeaders.list()
 
+    @property
+    def is_gene_panel_required(self) -> bool:
+        """Return True if a gene panel is needs to be created using the information in StatusDB and exporting it from Scout."""
+        return True
+
     @staticmethod
     def get_bundle_filenames_path() -> Path:
         """Return path to bundle template."""
         return TOMTE_BUNDLE_FILENAMES_PATH
 
     def get_sample_sheet_content_per_sample(self, case_sample: CaseSample) -> list[list[str]]:
         """Collect and format information required to build a sample sheet for a single sample."""
@@ -62,16 +66,19 @@
             name=case_sample.sample.internal_id,
             fastq_forward_read_paths=fastq_forward_read_paths,
             fastq_reverse_read_paths=fastq_reverse_read_paths,
             strandedness=Strandedness.REVERSE,
         )
         return sample_sheet_entry.reformat_sample_content
 
-    def get_workflow_parameters(self, case_id: str) -> WorkflowParameters:
+    def get_workflow_parameters(self, case_id: str) -> TomteParameters:
         """Return parameters."""
-        return WorkflowParameters(
+        return TomteParameters(
             input=self.get_sample_sheet_path(case_id=case_id),
             outdir=self.get_case_path(case_id=case_id),
+            gene_panel_clinical_filter=self.get_gene_panels_path(case_id=case_id),
+            tissue=self.get_case_source_type(case_id=case_id),
+            genome=self.get_genome_build(case_id=case_id),
         )
 
     def get_workflow_metrics(self) -> dict:
         return TOMTE_METRIC_CONDITIONS
```

### Comparing `cg-60.4.0/cg/models/balsamic/config.py` & `cg-60.4.1/cg/models/balsamic/config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/balsamic/metrics.py` & `cg-60.4.1/cg/models/balsamic/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/cg_config.py` & `cg-60.4.1/cg/models/cg_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/compression_data.py` & `cg-60.4.1/cg/models/compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/deliverables/metric_deliverables.py` & `cg-60.4.1/cg/models/deliverables/metric_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/demultiplex/run_parameters.py` & `cg-60.4.1/cg/models/demultiplex/run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/demultiplex/sbatch.py` & `cg-60.4.1/cg/models/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/downsample/downsample_data.py` & `cg-60.4.1/cg/models/downsample/downsample_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/fastq.py` & `cg-60.4.1/cg/models/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/file_data.py` & `cg-60.4.1/cg/models/file_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/flow_cell/flow_cell.py` & `cg-60.4.1/cg/models/flow_cell/flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/invoice/invoice.py` & `cg-60.4.1/cg/models/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/lims/sample.py` & `cg-60.4.1/cg/models/lims/sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/mip/mip_config.py` & `cg-60.4.1/cg/models/mip/mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/mip/mip_metrics_deliverables.py` & `cg-60.4.1/cg/models/mip/mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/mip/mip_sample_info.py` & `cg-60.4.1/cg/models/mip/mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/nf_analysis.py` & `cg-60.4.1/cg/models/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/observations/input_files.py` & `cg-60.4.1/cg/models/observations/input_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/orders/constants.py` & `cg-60.4.1/cg/models/orders/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/orders/excel_sample.py` & `cg-60.4.1/cg/models/orders/excel_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/orders/json_sample.py` & `cg-60.4.1/cg/models/orders/json_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/orders/order.py` & `cg-60.4.1/cg/models/orders/order.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/orders/orderform_schema.py` & `cg-60.4.1/cg/models/orders/orderform_schema.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/orders/sample_base.py` & `cg-60.4.1/cg/models/orders/sample_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/orders/samples.py` & `cg-60.4.1/cg/models/orders/samples.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/orders/validators/excel_sample_validators.py` & `cg-60.4.1/cg/models/orders/validators/excel_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/orders/validators/json_sample_validators.py` & `cg-60.4.1/cg/models/orders/validators/json_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/raredisease/raredisease.py` & `cg-60.4.1/cg/models/raredisease/raredisease.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/report/metadata.py` & `cg-60.4.1/cg/models/report/metadata.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/report/report.py` & `cg-60.4.1/cg/models/report/report.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/report/sample.py` & `cg-60.4.1/cg/models/report/sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/report/validators.py` & `cg-60.4.1/cg/models/report/validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/rnafusion/rnafusion.py` & `cg-60.4.1/cg/models/rnafusion/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/scout/scout_load_config.py` & `cg-60.4.1/cg/models/scout/scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/slurm/sbatch.py` & `cg-60.4.1/cg/models/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/taxprofiler/taxprofiler.py` & `cg-60.4.1/cg/models/taxprofiler/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/models/workflow/mutant.py` & `cg-60.4.1/cg/models/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/resources/__init__.py` & `cg-60.4.1/cg/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/resources/rnafusion_bundle_filenames.yaml` & `cg-60.4.1/cg/resources/rnafusion_bundle_filenames.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/resources/taxprofiler_bundle_filenames.yaml` & `cg-60.4.1/cg/resources/taxprofiler_bundle_filenames.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/resources/tomte_bundle_filenames.yaml` & `cg-60.4.1/cg/resources/tomte_bundle_filenames.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/server/admin.py` & `cg-60.4.1/cg/server/admin.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/server/api.py` & `cg-60.4.1/cg/server/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/server/app.py` & `cg-60.4.1/cg/server/app.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/server/config.py` & `cg-60.4.1/cg/server/config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/server/dto/orders/orders_request.py` & `cg-60.4.1/cg/server/dto/orders/orders_request.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/server/ext.py` & `cg-60.4.1/cg/server/ext.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/server/invoices/templates/invoices/index.html` & `cg-60.4.1/cg/server/invoices/templates/invoices/index.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/server/invoices/templates/invoices/invoice.html` & `cg-60.4.1/cg/server/invoices/templates/invoices/invoice.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/server/invoices/templates/invoices/layout.html` & `cg-60.4.1/cg/server/invoices/templates/invoices/layout.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/server/invoices/templates/invoices/new.html` & `cg-60.4.1/cg/server/invoices/templates/invoices/new.html`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/server/invoices/views.py` & `cg-60.4.1/cg/server/invoices/views.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/delivery_message/delivery_message_service.py` & `cg-60.4.1/cg/services/delivery_message/delivery_message_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/delivery_message/messages/__init__.py` & `cg-60.4.1/cg/services/delivery_message/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/delivery_message/messages/analysis_scout_message.py` & `cg-60.4.1/cg/services/delivery_message/messages/analysis_scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/delivery_message/messages/covid_message.py` & `cg-60.4.1/cg/services/delivery_message/messages/covid_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/delivery_message/messages/fastq_analysis_scout_message.py` & `cg-60.4.1/cg/services/delivery_message/messages/fastq_analysis_scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/delivery_message/messages/fastq_message.py` & `cg-60.4.1/cg/services/delivery_message/messages/fastq_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/delivery_message/messages/fastq_scout_message.py` & `cg-60.4.1/cg/services/delivery_message/messages/fastq_scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/delivery_message/messages/microsalt_mwr_message.py` & `cg-60.4.1/cg/services/delivery_message/messages/microsalt_mwr_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/delivery_message/messages/microsalt_mwx_message.py` & `cg-60.4.1/cg/services/delivery_message/messages/microsalt_mwx_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/delivery_message/messages/scout_message.py` & `cg-60.4.1/cg/services/delivery_message/messages/scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/delivery_message/messages/statina_message.py` & `cg-60.4.1/cg/services/delivery_message/messages/statina_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/delivery_message/messages/utils.py` & `cg-60.4.1/cg/services/delivery_message/messages/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/delivery_message/utils.py` & `cg-60.4.1/cg/services/delivery_message/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/fastq_file_service/fastq_file_service.py` & `cg-60.4.1/cg/services/fastq_file_service/fastq_file_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/fastq_file_service/utils.py` & `cg-60.4.1/cg/services/fastq_file_service/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/orders/order_service/order_service.py` & `cg-60.4.1/cg/services/orders/order_service/order_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/orders/order_service/utils.py` & `cg-60.4.1/cg/services/orders/order_service/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/orders/order_status_service/order_summary_service.py` & `cg-60.4.1/cg/services/orders/order_status_service/order_summary_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/orders/order_status_service/utils.py` & `cg-60.4.1/cg/services/orders/order_status_service/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/quality_controller/quality_checks/checks.py` & `cg-60.4.1/cg/services/quality_controller/quality_checks/checks.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/quality_controller/quality_checks/utils.py` & `cg-60.4.1/cg/services/quality_controller/quality_checks/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/quality_controller/quality_controller_service.py` & `cg-60.4.1/cg/services/quality_controller/quality_controller_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/slurm_service/slurm_cli_service.py` & `cg-60.4.1/cg/services/slurm_service/slurm_cli_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/services/slurm_upload_service/slurm_upload_service.py` & `cg-60.4.1/cg/services/slurm_upload_service/slurm_upload_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/base.py` & `cg-60.4.1/cg/store/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/crud/create.py` & `cg-60.4.1/cg/store/crud/create.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/crud/delete.py` & `cg-60.4.1/cg/store/crud/delete.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/crud/read.py` & `cg-60.4.1/cg/store/crud/read.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/crud/update.py` & `cg-60.4.1/cg/store/crud/update.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/database.py` & `cg-60.4.1/cg/store/database.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/filters/status_analysis_filters.py` & `cg-60.4.1/cg/store/filters/status_analysis_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/filters/status_application_filters.py` & `cg-60.4.1/cg/store/filters/status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/filters/status_application_limitations_filters.py` & `cg-60.4.1/cg/store/filters/status_application_limitations_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/filters/status_application_version_filters.py` & `cg-60.4.1/cg/store/filters/status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/filters/status_bed_filters.py` & `cg-60.4.1/cg/store/filters/status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/filters/status_bed_version_filters.py` & `cg-60.4.1/cg/store/filters/status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/filters/status_case_filters.py` & `cg-60.4.1/cg/store/filters/status_case_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/filters/status_case_sample_filters.py` & `cg-60.4.1/cg/store/filters/status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/filters/status_collaboration_filters.py` & `cg-60.4.1/cg/store/filters/status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/filters/status_customer_filters.py` & `cg-60.4.1/cg/store/filters/status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/filters/status_flow_cell_filters.py` & `cg-60.4.1/cg/store/filters/status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/filters/status_invoice_filters.py` & `cg-60.4.1/cg/store/filters/status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/filters/status_metrics_filters.py` & `cg-60.4.1/cg/store/filters/status_metrics_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/filters/status_order_filters.py` & `cg-60.4.1/cg/store/filters/status_order_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/filters/status_organism_filters.py` & `cg-60.4.1/cg/store/filters/status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/filters/status_panel_filters.py` & `cg-60.4.1/cg/store/filters/status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/filters/status_pool_filters.py` & `cg-60.4.1/cg/store/filters/status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/filters/status_sample_filters.py` & `cg-60.4.1/cg/store/filters/status_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/filters/status_user_filters.py` & `cg-60.4.1/cg/store/filters/status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/models.py` & `cg-60.4.1/cg/store/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/store/store.py` & `cg-60.4.1/cg/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/utils/checksum/checksum.py` & `cg-60.4.1/cg/utils/checksum/checksum.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/utils/click/EnumChoice.py` & `cg-60.4.1/cg/utils/click/EnumChoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/utils/commands.py` & `cg-60.4.1/cg/utils/commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/utils/date.py` & `cg-60.4.1/cg/utils/date.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/utils/dict.py` & `cg-60.4.1/cg/utils/dict.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/utils/dispatcher.py` & `cg-60.4.1/cg/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/utils/email.py` & `cg-60.4.1/cg/utils/email.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/utils/files.py` & `cg-60.4.1/cg/utils/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/utils/flask/enum.py` & `cg-60.4.1/cg/utils/flask/enum.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/utils/time.py` & `cg-60.4.1/cg/utils/time.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/cg/utils/utils.py` & `cg-60.4.1/cg/utils/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Helper functions."""
 
+import re
+
 
 def get_string_from_list_by_pattern(strings: list[str], pattern: str) -> str | None:
     """Returns the full string from a list given a specific pattern."""
 
     return next((string for string in strings if pattern in string), None) if strings else None
 
 
@@ -25,7 +27,12 @@
 
     Raises:
         KeyError: When the strings have the same length.
     """
     if len(str_1) != len(str_2):
         raise KeyError("The two strings must have the same length to calculate distance!")
     return sum(n1 != n2 for n1, n2 in zip(str_1, str_2))
+
+
+def replace_non_alphanumeric(string: str, replace_by="_") -> str:
+    """Replace non-alphanumeric characters from a string."""
+    return re.sub(r"\W+", replace_by, string)
```

### Comparing `cg-60.4.0/pyproject.toml` & `cg-60.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cg"
-version = "60.4.0"
+version = "60.4.1"
 description = "Clinical Genomics command center"
 authors = ["Clinical Genomics <support@clinicalgenomics.se>"]
 readme = "README.md"
 homepage = "https://github.com/Clinical-Genomics/cg"
 repository = "https://github.com/Clinical-Genomics/cg"
 classifiers = [
   "Programming Language :: Python",
```

### Comparing `cg-60.4.0/tests/apps/conftest.py` & `cg-60.4.1/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/coverage/test_coverage.py` & `cg-60.4.1/tests/apps/coverage/test_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/crunchy/conftest.py` & `cg-60.4.1/tests/apps/crunchy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/crunchy/test_compress_fastq.py` & `cg-60.4.1/tests/apps/crunchy/test_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/crunchy/test_config.py` & `cg-60.4.1/tests/apps/crunchy/test_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/crunchy/test_crunchy.py` & `cg-60.4.1/tests/apps/crunchy/test_crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/crunchy/test_spring_decompression.py` & `cg-60.4.1/tests/apps/crunchy/test_spring_decompression.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/demultiplex/conftest.py` & `cg-60.4.1/tests/apps/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/demultiplex/test_create_sample_sheet.py` & `cg-60.4.1/tests/apps/demultiplex/test_create_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/demultiplex/test_demultiplex_api.py` & `cg-60.4.1/tests/apps/demultiplex/test_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/demultiplex/test_index.py` & `cg-60.4.1/tests/apps/demultiplex/test_index.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/demultiplex/test_override_cycles_validator.py` & `cg-60.4.1/tests/apps/demultiplex/test_override_cycles_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/demultiplex/test_read_sample_sheet.py` & `cg-60.4.1/tests/apps/demultiplex/test_read_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/demultiplex/test_sample_models.py` & `cg-60.4.1/tests/apps/demultiplex/test_sample_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/demultiplex/test_sample_sheet_creator.py` & `cg-60.4.1/tests/apps/demultiplex/test_sample_sheet_creator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/demultiplex/test_sample_sheet_models.py` & `cg-60.4.1/tests/apps/demultiplex/test_sample_sheet_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/demultiplex/test_sample_sheet_validator.py` & `cg-60.4.1/tests/apps/demultiplex/test_sample_sheet_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/demultiplex/test_translate_sample_sheet.py` & `cg-60.4.1/tests/apps/demultiplex/test_translate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/demultiplex/test_validate.py` & `cg-60.4.1/tests/apps/demultiplex/test_validate.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/downsample/test_downsample.py` & `cg-60.4.1/tests/apps/downsample/test_downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/downsample/test_downsample_utils.py` & `cg-60.4.1/tests/apps/downsample/test_downsample_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/gens/test_gens_api.py` & `cg-60.4.1/tests/apps/gens/test_gens_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/gt/conftest.py` & `cg-60.4.1/tests/apps/gt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/gt/test_gt_api.py` & `cg-60.4.1/tests/apps/gt/test_gt_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/hk/conftest.py` & `cg-60.4.1/tests/apps/hk/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/hk/test__getattr__.py` & `cg-60.4.1/tests/apps/hk/test__getattr__.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/hk/test_add_file.py` & `cg-60.4.1/tests/apps/hk/test_add_file.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/hk/test_bundles.py` & `cg-60.4.1/tests/apps/hk/test_bundles.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/hk/test_core.py` & `cg-60.4.1/tests/apps/hk/test_core.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/hk/test_file.py` & `cg-60.4.1/tests/apps/hk/test_file.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/hk/test_version.py` & `cg-60.4.1/tests/apps/hk/test_version.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/lims/conftest.py` & `cg-60.4.1/tests/apps/lims/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/lims/test_api.py` & `cg-60.4.1/tests/apps/lims/test_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/lims/test_sample_sheet.py` & `cg-60.4.1/tests/apps/lims/test_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/loqus/conftest.py` & `cg-60.4.1/tests/apps/loqus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/loqus/test_loqusdb_api.py` & `cg-60.4.1/tests/apps/loqus/test_loqusdb_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/madeline/conftest.py` & `cg-60.4.1/tests/apps/madeline/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/madeline/test_madeline.py` & `cg-60.4.1/tests/apps/madeline/test_madeline.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/mip/conftest.py` & `cg-60.4.1/tests/apps/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/mip/test_config_mip.py` & `cg-60.4.1/tests/apps/mip/test_config_mip.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/mutacc_auto/conftest.py` & `cg-60.4.1/tests/apps/mutacc_auto/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/mutacc_auto/test_mutacc_auto.py` & `cg-60.4.1/tests/apps/mutacc_auto/test_mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/orderform/conftest.py` & `cg-60.4.1/tests/apps/orderform/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/orderform/test_excel_orderform_parser.py` & `cg-60.4.1/tests/apps/orderform/test_excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/orderform/test_excel_sample_schema.py` & `cg-60.4.1/tests/apps/orderform/test_excel_sample_schema.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/orderform/test_json_orderform_parser.py` & `cg-60.4.1/tests/apps/orderform/test_json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/orderform/test_orderform_parser.py` & `cg-60.4.1/tests/apps/orderform/test_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/orderform/validators/test_excel_sample_validators.py` & `cg-60.4.1/tests/apps/orderform/validators/test_excel_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/scout/conftest.py` & `cg-60.4.1/tests/apps/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/scout/test_get_causative_variants.py` & `cg-60.4.1/tests/apps/scout/test_get_causative_variants.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/scout/test_get_scout_cases.py` & `cg-60.4.1/tests/apps/scout/test_get_scout_cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/scout/test_scout_load_config.py` & `cg-60.4.1/tests/apps/scout/test_scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/scout/test_scout_models.py` & `cg-60.4.1/tests/apps/scout/test_scout_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/sequencing_metrics_parser/conftest.py` & `cg-60.4.1/tests/apps/sequencing_metrics_parser/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py` & `cg-60.4.1/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/sequencing_metrics_parser/parsers/test_sequencing_metrics_parser_api.py` & `cg-60.4.1/tests/apps/sequencing_metrics_parser/parsers/test_sequencing_metrics_parser_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/slurm/conftest.py` & `cg-60.4.1/tests/apps/slurm/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/slurm/test_slurm_api.py` & `cg-60.4.1/tests/apps/slurm/test_slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/test_apps_environ.py` & `cg-60.4.1/tests/apps/test_apps_environ.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/apps/test_osticket.py` & `cg-60.4.1/tests/apps/test_osticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/add/test_cli_add.py` & `cg-60.4.1/tests/cli/add/test_cli_add.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/add/test_cli_add_customer.py` & `cg-60.4.1/tests/cli/add/test_cli_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/add/test_cli_add_family.py` & `cg-60.4.1/tests/cli/add/test_cli_add_family.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/add/test_cli_add_relationship.py` & `cg-60.4.1/tests/cli/add/test_cli_add_relationship.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/add/test_cli_add_sample.py` & `cg-60.4.1/tests/cli/add/test_cli_add_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/backup/conftest.py` & `cg-60.4.1/tests/cli/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/backup/test_backup_command.py` & `cg-60.4.1/tests/cli/backup/test_backup_command.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/clean/conftest.py` & `cg-60.4.1/tests/cli/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/clean/test_balsamic_clean.py` & `cg-60.4.1/tests/cli/clean/test_balsamic_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/clean/test_clean_flow_cell.py` & `cg-60.4.1/tests/cli/clean/test_clean_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/clean/test_clean_hk_bundle_files.py` & `cg-60.4.1/tests/cli/clean/test_clean_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/clean/test_hk_bundle_files.py` & `cg-60.4.1/tests/cli/clean/test_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/clean/test_hk_case_bundle_files.py` & `cg-60.4.1/tests/cli/clean/test_hk_case_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/clean/test_microbial_clean.py` & `cg-60.4.1/tests/cli/clean/test_microbial_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/clean/test_rsync_past_run_dirs.py` & `cg-60.4.1/tests/cli/clean/test_rsync_past_run_dirs.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/compress/conftest.py` & `cg-60.4.1/tests/cli/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/compress/test_cli_compress_fastq.py` & `cg-60.4.1/tests/cli/compress/test_cli_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/compress/test_cli_decompress_spring.py` & `cg-60.4.1/tests/cli/compress/test_cli_decompress_spring.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/compress/test_compress_helpers.py` & `cg-60.4.1/tests/cli/compress/test_compress_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/compress/test_store_fastq.py` & `cg-60.4.1/tests/cli/compress/test_store_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/conftest.py` & `cg-60.4.1/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/delete/test_cli_delete_case.py` & `cg-60.4.1/tests/cli/delete/test_cli_delete_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/delete/test_cli_delete_cases.py` & `cg-60.4.1/tests/cli/delete/test_cli_delete_cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/deliver/conftest.py` & `cg-60.4.1/tests/cli/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/deliver/test_deliver_base.py` & `cg-60.4.1/tests/cli/deliver/test_deliver_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/deliver/test_rsync_base.py` & `cg-60.4.1/tests/cli/deliver/test_rsync_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/deliver/test_run_deliver_cmd.py` & `cg-60.4.1/tests/cli/deliver/test_run_deliver_cmd.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/demultiplex/test_create_sample_sheet.py` & `cg-60.4.1/tests/cli/demultiplex/test_create_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/demultiplex/test_demultiplex_flowcell.py` & `cg-60.4.1/tests/cli/demultiplex/test_demultiplex_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/demultiplex/test_finish_demux.py` & `cg-60.4.1/tests/cli/demultiplex/test_finish_demux.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/demultiplex/test_validate_sample_sheet.py` & `cg-60.4.1/tests/cli/demultiplex/test_validate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/demultiplex/test_verify_syncing.py` & `cg-60.4.1/tests/cli/demultiplex/test_verify_syncing.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/downsample/test_cli_downsample.py` & `cg-60.4.1/tests/cli/downsample/test_cli_downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/generate/report/conftest.py` & `cg-60.4.1/tests/cli/generate/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/generate/report/test_cli_delivery_report.py` & `cg-60.4.1/tests/cli/generate/report/test_cli_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/generate/report/test_utils.py` & `cg-60.4.1/tests/cli/generate/report/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/generate/test_cli_base.py` & `cg-60.4.1/tests/cli/generate/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/get/test_cli_get.py` & `cg-60.4.1/tests/cli/get/test_cli_get.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/get/test_cli_get_analysis.py` & `cg-60.4.1/tests/cli/get/test_cli_get_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/get/test_cli_get_case.py` & `cg-60.4.1/tests/cli/get/test_cli_get_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/get/test_cli_get_flow_cell.py` & `cg-60.4.1/tests/cli/get/test_cli_get_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/get/test_cli_get_sample.py` & `cg-60.4.1/tests/cli/get/test_cli_get_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/set/conftest.py` & `cg-60.4.1/tests/cli/set/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/set/test_cli_set_case.py` & `cg-60.4.1/tests/cli/set/test_cli_set_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/set/test_cli_set_cases.py` & `cg-60.4.1/tests/cli/set/test_cli_set_cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/set/test_cli_set_flowcell.py` & `cg-60.4.1/tests/cli/set/test_cli_set_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/set/test_cli_set_list_keys.py` & `cg-60.4.1/tests/cli/set/test_cli_set_list_keys.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/set/test_cli_set_sample.py` & `cg-60.4.1/tests/cli/set/test_cli_set_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/set/test_cli_set_samples.py` & `cg-60.4.1/tests/cli/set/test_cli_set_samples.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/store/test_store.py` & `cg-60.4.1/tests/cli/store/test_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/test_base.py` & `cg-60.4.1/tests/cli/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/upload/conftest.py` & `cg-60.4.1/tests/cli/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/upload/test_cli_scout.py` & `cg-60.4.1/tests/cli/upload/test_cli_scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/upload/test_cli_upload.py` & `cg-60.4.1/tests/cli/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/upload/test_cli_upload_auto.py` & `cg-60.4.1/tests/cli/upload/test_cli_upload_auto.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/upload/test_cli_upload_delivery_report.py` & `cg-60.4.1/tests/cli/upload/test_cli_upload_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/upload/test_cli_upload_fastq.py` & `cg-60.4.1/tests/cli/upload/test_cli_upload_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/upload/test_cli_upload_genotype.py` & `cg-60.4.1/tests/cli/upload/test_cli_upload_genotype.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/upload/test_cli_upload_gens.py` & `cg-60.4.1/tests/cli/upload/test_cli_upload_gens.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/upload/test_cli_upload_nipt.py` & `cg-60.4.1/tests/cli/upload/test_cli_upload_nipt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/upload/test_cli_upload_nipt_ftp.py` & `cg-60.4.1/tests/cli/upload/test_cli_upload_nipt_ftp.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/upload/test_cli_upload_nipt_statina.py` & `cg-60.4.1/tests/cli/upload/test_cli_upload_nipt_statina.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/upload/test_cli_upload_observations.py` & `cg-60.4.1/tests/cli/upload/test_cli_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/balsamic/conftest.py` & `cg-60.4.1/tests/cli/workflow/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py` & `cg-60.4.1/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/balsamic/test_compound_commands.py` & `cg-60.4.1/tests/cli/workflow/balsamic/test_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/balsamic/test_link.py` & `cg-60.4.1/tests/cli/workflow/balsamic/test_link.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/balsamic/test_report_deliver.py` & `cg-60.4.1/tests/cli/workflow/balsamic/test_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/balsamic/test_run.py` & `cg-60.4.1/tests/cli/workflow/balsamic/test_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/balsamic/test_store_housekeeper.py` & `cg-60.4.1/tests/cli/workflow/balsamic/test_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/conftest.py` & `cg-60.4.1/tests/cli/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/fastq/test_fastq_base.py` & `cg-60.4.1/tests/cli/workflow/fastq/test_fastq_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/fluffy/conftest.py` & `cg-60.4.1/tests/cli/workflow/fluffy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py` & `cg-60.4.1/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/fluffy/test_cli_link.py` & `cg-60.4.1/tests/cli/workflow/fluffy/test_cli_link.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/fluffy/test_cli_run.py` & `cg-60.4.1/tests/cli/workflow/fluffy/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/fluffy/test_cli_start.py` & `cg-60.4.1/tests/cli/workflow/fluffy/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/fluffy/test_cli_store.py` & `cg-60.4.1/tests/cli/workflow/fluffy/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/microsalt/conftest.py` & `cg-60.4.1/tests/cli/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/microsalt/test_microsalt_case_config.py` & `cg-60.4.1/tests/cli/workflow/microsalt/test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/microsalt/test_microsalt_run.py` & `cg-60.4.1/tests/cli/workflow/microsalt/test_microsalt_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/mip/conftest.py` & `cg-60.4.1/tests/cli/workflow/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/mip/test_cli_mip_base.py` & `cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py` & `cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py` & `cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/mip/test_cli_mip_dna_panel.py` & `cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_dna_panel.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/mip/test_cli_mip_dna_run.py` & `cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_dna_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/mip/test_cli_mip_dna_start.py` & `cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_dna_start.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py` & `cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/mip/test_cli_mip_rna_link.py` & `cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_rna_link.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/mip/test_cli_mip_rna_run.py` & `cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_rna_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/mip/test_cli_mip_store.py` & `cg-60.4.1/tests/cli/workflow/mip/test_cli_mip_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/nf_analysis/test_cli_config_case.py` & `cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_config_case.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 from pathlib import Path
 
 import pytest
 from _pytest.fixtures import FixtureRequest
 from _pytest.logging import LogCaptureFixture
 from click.testing import CliRunner
 
+from cg.apps.lims import LimsAPI
 from cg.cli.workflow.base import workflow as workflow_cli
 from cg.constants import EXIT_SUCCESS, Workflow
-from cg.constants.constants import FileFormat
+from cg.constants.constants import FileFormat, MetaApis
 from cg.io.controller import ReadFile
+from cg.meta.workflow.nf_analysis import NfAnalysisAPI
 from cg.models.cg_config import CGConfig
-from cg.models.nf_analysis import WorkflowParameters
+from cg.utils import Process
 
 LOG = logging.getLogger(__name__)
 
 
 @pytest.mark.parametrize(
     "workflow",
     [Workflow.RAREDISEASE, Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.TOMTE],
@@ -96,31 +98,38 @@
     # THEN warning should be printed that no sample is found
     assert no_sample_case_id in caplog.text
     assert "has no samples" in caplog.text
 
 
 @pytest.mark.parametrize(
     "workflow",
-    [Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.RAREDISEASE, Workflow.TOMTE],
+    [Workflow.RAREDISEASE, Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.TOMTE],
 )
 def test_config_case_default_parameters(
     cli_runner: CliRunner,
     workflow: Workflow,
     caplog: LogCaptureFixture,
     request: FixtureRequest,
+    mocker,
 ):
     """Test that command generates config files."""
     caplog.set_level(logging.DEBUG)
     context: CGConfig = request.getfixturevalue(f"{workflow}_context")
     case_id: str = request.getfixturevalue(f"{workflow}_case_id")
     sample_sheet_path: Path = request.getfixturevalue(f"{workflow}_sample_sheet_path")
     params_file_path: Path = request.getfixturevalue(f"{workflow}_params_file_path")
     nexflow_config_file_path: Path = request.getfixturevalue(f"{workflow}_nexflow_config_file_path")
     sample_sheet_content_expected: str = request.getfixturevalue(f"{workflow}_sample_sheet_content")
 
+    # Mocking external Scout call
+    mocker.patch.object(Process, "run_command", return_value=None)
+
+    # GIVEN that the sample source in LIMS is set
+    mocker.patch.object(LimsAPI, "get_source", return_value="blood")
+
     # GIVEN a valid case
 
     # WHEN running config case
     result = cli_runner.invoke(workflow_cli, [workflow, "config-case", case_id], obj=context)
 
     # THEN command should exit successfully
     assert result.exit_code == EXIT_SUCCESS
@@ -143,56 +152,86 @@
 
     # THEN the sample sheet content should match the expected values
     sample_sheet_content_created: list[list[str]] = ReadFile.get_content_from_file(
         file_format=FileFormat.TXT, file_path=sample_sheet_path, read_to_string=True
     )
     assert sample_sheet_content_expected in sample_sheet_content_created
 
-    # WHEN workflow is not raredisease
+    # WHEN workflow is not raredisease nor tomte
     # Note this will need to be unified once all workflows are standarised
     if workflow not in {Workflow.RAREDISEASE, Workflow.TOMTE}:
         # THEN the params file should contain all parameters
         parameters_default = vars(request.getfixturevalue(f"{workflow}_parameters_default"))
         params_content: list[list[str]] = ReadFile.get_content_from_file(
             file_format=FileFormat.TXT, file_path=params_file_path, read_to_string=True
         )
         for parameter in parameters_default:
             assert parameter in params_content
 
+    # Check that parameters are written in the config file for tomte
+    # Note this will need to be unified once all workflows are standarised
+    if workflow in {Workflow.TOMTE}:
+        # THEN the params file should contain all parameters
+        parameters_default = vars(request.getfixturevalue(f"{workflow}_parameters_default"))
+        params_content: list[list[str]] = ReadFile.get_content_from_file(
+            file_format=FileFormat.TXT, file_path=nexflow_config_file_path, read_to_string=True
+        )
+        for parameter in parameters_default:
+            assert f"params.{parameter}" in params_content
+
+    # WHEN the workflow requires a gene panel
+    # THEN information about the panel being generated should be logged and the file should be written
+    analysis_api: NfAnalysisAPI = context.meta_apis[MetaApis.ANALYSIS_API]
+    if analysis_api.is_gene_panel_required:
+        assert "Creating gene panel file" in caplog.text
+        gene_panel_path: Path = request.getfixturevalue(f"{workflow}_gene_panel_path")
+        assert gene_panel_path.is_file()
+
 
 @pytest.mark.parametrize(
     "workflow",
-    [Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.RAREDISEASE, Workflow.TOMTE],
+    [Workflow.RAREDISEASE, Workflow.RNAFUSION, Workflow.TAXPROFILER, Workflow.TOMTE],
 )
 def test_config_case_dry_run(
     cli_runner: CliRunner,
     workflow: Workflow,
     caplog: LogCaptureFixture,
     request: FixtureRequest,
+    mocker,
 ):
     """Test dry-run."""
     caplog.set_level(logging.DEBUG)
     context: CGConfig = request.getfixturevalue(f"{workflow}_context")
     case_id: str = request.getfixturevalue(f"{workflow}_case_id")
     sample_sheet_path: Path = request.getfixturevalue(f"{workflow}_sample_sheet_path")
     params_file_path: Path = request.getfixturevalue(f"{workflow}_params_file_path")
     nexflow_config_file_path: Path = request.getfixturevalue(f"{workflow}_nexflow_config_file_path")
 
     # GIVEN a valid case
 
+    # GIVEN that the sample source in LIMS is set
+    mocker.patch.object(LimsAPI, "get_source", return_value="blood")
+
     # WHEN invoking the command with dry-run specified
     result = cli_runner.invoke(workflow_cli, [workflow, "config-case", case_id, "-d"], obj=context)
 
     # THEN command should exit successfully
     assert result.exit_code == EXIT_SUCCESS
 
     # THEN sample sheet and parameters information should be collected
     assert "Getting sample sheet information" in caplog.text
     assert "Getting parameters information" in caplog.text
 
     # THEN sample sheet and parameters information files should not be written
     assert "Dry run: Config files will not be written" in caplog.text
-    assert "Writing sample sheet" not in caplog.text
-    assert "Writing parameters file" not in caplog.text
     assert not sample_sheet_path.is_file()
     assert not params_file_path.is_file()
     assert not nexflow_config_file_path.is_file()
+
+    # WHEN the workflow requires a gene panel
+    # THEN information about the panel being generated should be logged but no file should be written
+    analysis_api: NfAnalysisAPI = context.meta_apis[MetaApis.ANALYSIS_API]
+    if analysis_api.is_gene_panel_required:
+        assert "Creating gene panel file" in caplog.text
+        assert "bin/scout --config scout-stage.yaml export panel" in caplog.text
+        gene_panel_path: Path = request.getfixturevalue(f"{workflow}_gene_panel_path")
+        assert not gene_panel_path.is_file()
```

### Comparing `cg-60.4.0/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py` & `cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py` & `cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/nf_analysis/test_cli_run.py` & `cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/nf_analysis/test_cli_start.py` & `cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_start.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 
 import pytest
 from _pytest.fixtures import FixtureRequest
 from _pytest.logging import LogCaptureFixture
 from click.testing import CliRunner
 
+from cg.apps.lims import LimsAPI
 from cg.cli.workflow.base import workflow as workflow_cli
 from cg.constants import EXIT_SUCCESS, Workflow
 from cg.meta.workflow.nf_analysis import NfAnalysisAPI
 from cg.models.cg_config import CGConfig
 from tests.cli.workflow.conftest import mock_analysis_flow_cell
 
 
@@ -32,14 +33,17 @@
     case_id: str = request.getfixturevalue(f"{workflow}_case_id")
 
     # GIVEN a mocked config
 
     # GIVEN decompression is not needed
     mocker.patch.object(NfAnalysisAPI, "resolve_decompression", return_value=None)
 
+    # GIVEN that the sample source in LIMS is set
+    mocker.patch.object(LimsAPI, "get_source", return_value="blood")
+
     # WHEN invoking the command with dry-run specified
     result = cli_runner.invoke(workflow_cli, [workflow, "start", case_id, "--dry-run"], obj=context)
 
     # THEN command should execute successfully
     assert result.exit_code == EXIT_SUCCESS
     assert case_id in caplog.text
 
@@ -71,14 +75,17 @@
     case_id: str = request.getfixturevalue(f"{workflow}_case_id")
 
     # GIVEN a mocked config
 
     # GIVEN decompression is not needed
     mocker.patch.object(NfAnalysisAPI, "resolve_decompression", return_value=None)
 
+    # GIVEN that the sample source in LIMS is set
+    mocker.patch.object(LimsAPI, "get_source", return_value="blood")
+
     # WHEN invoking the command with dry-run specified
     result = cli_runner.invoke(
         workflow_cli, [workflow, "start-available", "--dry-run"], obj=context
     )
 
     # THEN command exits successfully
     assert result.exit_code == EXIT_SUCCESS
```

### Comparing `cg-60.4.0/tests/cli/workflow/nf_analysis/test_cli_store.py` & `cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py` & `cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py` & `cg-60.4.1/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py` & `cg-60.4.1/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/test_cli_workflow.py` & `cg-60.4.1/tests/cli/workflow/test_cli_workflow.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/cli/workflow/test_cli_workflow_clean.py` & `cg-60.4.1/tests/cli/workflow/test_cli_workflow_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/clients/arnold/conftest.py` & `cg-60.4.1/tests/clients/arnold/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/clients/arnold/test_arnold_api_client.py` & `cg-60.4.1/tests/clients/arnold/test_arnold_api_client.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/clients/janus/conftest.py` & `cg-60.4.1/tests/clients/janus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/clients/janus/test_janus_api_client.py` & `cg-60.4.1/tests/clients/janus/test_janus_api_client.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/conftest.py` & `cg-60.4.1/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,17 @@
 from cg.apps.gt import GenotypeAPI
 from cg.apps.hermes.hermes_api import HermesApi
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.apps.housekeeper.models import InputBundle
 from cg.apps.lims import LimsAPI
 from cg.apps.slurm.slurm_api import SlurmAPI
 from cg.constants import FileExtensions, SequencingFileTag, Workflow
-from cg.constants.constants import CaseActions, FileFormat, Strandedness
+from cg.constants.constants import CaseActions, CustomerId, FileFormat, GenomeVersion, Strandedness
 from cg.constants.demultiplexing import DemultiplexingDirsAndFiles
+from cg.constants.gene_panel import GenePanelMasterList
 from cg.constants.housekeeper_tags import HK_DELIVERY_REPORT_TAG
 from cg.constants.priority import SlurmQos
 from cg.constants.sequencing import SequencingPlatform
 from cg.constants.subject import Sex
 from cg.io.controller import WriteFile
 from cg.io.json import read_json, write_json
 from cg.io.yaml import read_yaml, write_yaml
@@ -49,15 +50,15 @@
 from cg.models import CompressionData
 from cg.models.cg_config import CGConfig, PDCArchivingDirectory
 from cg.models.downsample.downsample_data import DownsampleData
 from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
 from cg.models.raredisease.raredisease import RarediseaseSampleSheetHeaders
 from cg.models.rnafusion.rnafusion import RnafusionParameters, RnafusionSampleSheetEntry
 from cg.models.taxprofiler.taxprofiler import TaxprofilerParameters, TaxprofilerSampleSheetEntry
-from cg.models.tomte.tomte import TomteSampleSheetHeaders
+from cg.models.tomte.tomte import TomteParameters, TomteSampleSheetHeaders
 from cg.store.database import create_all_tables, drop_all_tables, initialize_database
 from cg.store.models import Bed, BedVersion, Case, Customer, Order, Organism, Sample
 from cg.store.store import Store
 from cg.utils import Process
 from tests.mocks.crunchy import MockCrunchyAPI
 from tests.mocks.hk_mock import MockHousekeeperAPI
 from tests.mocks.limsmock import MockLimsAPI
@@ -3066,14 +3067,20 @@
     """Path to config file."""
     return Path(tomte_dir, tomte_case_id, f"{tomte_case_id}_nextflow_config").with_suffix(
         FileExtensions.JSON
     )
 
 
 @pytest.fixture(scope="function")
+def tomte_gene_panel_path(tomte_dir, tomte_case_id) -> Path:
+    """Path to gene panel file."""
+    return Path(tomte_dir, tomte_case_id, "gene_panels").with_suffix(FileExtensions.BED)
+
+
+@pytest.fixture(scope="function")
 def tomte_mock_config(tomte_dir: Path, tomte_case_id: str) -> None:
     """Create Tomte samplesheet.csv file for testing."""
     Path.mkdir(Path(tomte_dir, tomte_case_id), parents=True, exist_ok=True)
     Path(tomte_dir, tomte_case_id, f"{tomte_case_id}_samplesheet").with_suffix(
         FileExtensions.CSV
     ).touch(exist_ok=True)
 
@@ -3252,14 +3259,32 @@
             "created": timestamp_yesterday,
             "name": tomte_case_id,
         }
     )
 
 
 @pytest.fixture(scope="function")
+def tomte_parameters_default(
+    tomte_dir: Path,
+    tomte_case_id: str,
+    tomte_sample_sheet_path: Path,
+    tomte_gene_panel_path: Path,
+    existing_directory: Path,
+) -> TomteParameters:
+    """Return Tomte parameters."""
+    return TomteParameters(
+        input=tomte_sample_sheet_path,
+        outdir=Path(tomte_dir, tomte_case_id),
+        gene_panel_clinical_filter=tomte_gene_panel_path,
+        tissue="unkown",
+        genome="hg38",
+    )
+
+
+@pytest.fixture(scope="function")
 def tomte_context(
     cg_context: CGConfig,
     helpers: StoreHelpers,
     nf_analysis_housekeeper: HousekeeperAPI,
     trailblazer_api: MockTB,
     hermes_api: HermesApi,
     cg_dir: Path,
@@ -3283,22 +3308,24 @@
 
     # Create a textbook case with enough reads
     case_enough_reads: Case = helpers.add_case(
         store=status_db,
         internal_id=tomte_case_id,
         name=tomte_case_id,
         data_analysis=Workflow.TOMTE,
+        panels=[GenePanelMasterList.OMIM_AUTO],
     )
 
     sample_enough_reads: Sample = helpers.add_sample(
         status_db,
         application_tag=apptag_rna,
         internal_id=sample_id,
         reads=total_sequenced_reads_pass,
         last_sequenced_at=datetime.now(),
+        reference_genome=GenomeVersion.hg38,
     )
 
     helpers.add_relationship(
         status_db,
         case=case_enough_reads,
         sample=sample_enough_reads,
     )
```

### Comparing `cg-60.4.0/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py` & `cg-60.4.1/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixture_plugins/delivery_fixtures/context_fixtures.py` & `cg-60.4.1/tests/fixture_plugins/delivery_fixtures/context_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixture_plugins/delivery_fixtures/path_fixtures.py` & `cg-60.4.1/tests/fixture_plugins/delivery_fixtures/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py` & `cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py` & `cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py` & `cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py` & `cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py` & `cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py` & `cg-60.4.1/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_check_scenario.py` & `cg-60.4.1/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_check_scenario.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_fixtures.py` & `cg-60.4.1/tests/fixture_plugins/quality_controller_fixtures/sequencing_qc_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixture_plugins/timestamp_fixtures.py` & `cg-60.4.1/tests/fixture_plugins/timestamp_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json` & `cg-60.4.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json` & `cg-60.4.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/analysis/raredisease/multiqc_data.json` & `cg-60.4.1/tests/fixtures/analysis/raredisease/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml` & `cg-60.4.1/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/analysis/rnafusion/multiqc_data.json` & `cg-60.4.1/tests/fixtures/analysis/rnafusion/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml` & `cg-60.4.1/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/analysis/sample_coverage.bed` & `cg-60.4.1/tests/fixtures/analysis/sample_coverage.bed`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/analysis/taxprofiler/multiqc_data.json` & `cg-60.4.1/tests/fixtures/analysis/taxprofiler/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml` & `cg-60.4.1/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/analysis/tomte/multiqc_data.json` & `cg-60.4.1/tests/fixtures/analysis/tomte/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml` & `cg-60.4.1/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/balsamic/case/config.json` & `cg-60.4.1/tests/fixtures/apps/balsamic/case/config.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/balsamic/case/metadata.yml` & `cg-60.4.1/tests/fixtures/apps/balsamic/case/metadata.yml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml` & `cg-60.4.1/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/crunchy/spring_metadata.json` & `cg-60.4.1/tests/fixtures/apps/crunchy/spring_metadata.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stderr` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stdout` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RunParameters.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv` & `cg-60.4.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/fluffy/SampleSheet.csv` & `cg-60.4.1/tests/fixtures/apps/fluffy/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/fluffy/deliverables.yaml` & `cg-60.4.1/tests/fixtures/apps/fluffy/deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/madeline/madeline.xml` & `cg-60.4.1/tests/fixtures/apps/madeline/madeline.xml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/mip/case_metrics_deliverables.yaml` & `cg-60.4.1/tests/fixtures/apps/mip/case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/mip/dna/store/case_config.yaml` & `cg-60.4.1/tests/fixtures/apps/mip/dna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml` & `cg-60.4.1/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml` & `cg-60.4.1/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf` & `cg-60.4.1/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/mip/rna/case_config.yaml` & `cg-60.4.1/tests/fixtures/apps/mip/rna/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml` & `cg-60.4.1/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/mip/rna/store/bundle_data.yaml` & `cg-60.4.1/tests/fixtures/apps/mip/rna/store/bundle_data.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/mip/rna/store/case_config.yaml` & `cg-60.4.1/tests/fixtures/apps/mip/rna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml` & `cg-60.4.1/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml` & `cg-60.4.1/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/scout/643594.config.yaml` & `cg-60.4.1/tests/fixtures/apps/scout/643594.config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/scout/case_export.json` & `cg-60.4.1/tests/fixtures/apps/scout/case_export.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/scout/export_causatives.json` & `cg-60.4.1/tests/fixtures/apps/scout/export_causatives.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/scout/none_case_export.json` & `cg-60.4.1/tests/fixtures/apps/scout/none_case_export.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/scout/other_sex_case.json` & `cg-60.4.1/tests/fixtures/apps/scout/other_sex_case.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/scout/panel_export.bed` & `cg-60.4.1/tests/fixtures/apps/scout/panel_export.bed`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/scout/panel_export.csv` & `cg-60.4.1/tests/fixtures/apps/scout/panel_export.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/SampleSheet.csv` & `cg-60.4.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv` & `cg-60.4.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv` & `cg-60.4.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv` & `cg-60.4.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/cgweb_orders/balsamic.json` & `cg-60.4.1/tests/fixtures/cgweb_orders/balsamic.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/cgweb_orders/fastq.json` & `cg-60.4.1/tests/fixtures/cgweb_orders/fastq.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/cgweb_orders/metagenome.json` & `cg-60.4.1/tests/fixtures/cgweb_orders/metagenome.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/cgweb_orders/microsalt.json` & `cg-60.4.1/tests/fixtures/cgweb_orders/microsalt.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/cgweb_orders/mip.json` & `cg-60.4.1/tests/fixtures/cgweb_orders/mip.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/cgweb_orders/mip_rna.json` & `cg-60.4.1/tests/fixtures/cgweb_orders/mip_rna.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/cgweb_orders/rml.json` & `cg-60.4.1/tests/fixtures/cgweb_orders/rml.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/cgweb_orders/rnafusion.json` & `cg-60.4.1/tests/fixtures/cgweb_orders/rnafusion.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/cgweb_orders/sarscov2.json` & `cg-60.4.1/tests/fixtures/cgweb_orders/sarscov2.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/data/SampleSheet.csv` & `cg-60.4.1/tests/fixtures/data/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/data/cgfixture.db` & `cg-60.4.1/tests/fixtures/data/cgfixture.db`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/data/hkstore.db` & `cg-60.4.1/tests/fixtures/data/hkstore.db`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/io/example_json.json` & `cg-60.4.1/tests/fixtures/io/example_json.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/orderforms/1508.30.balsamic.xlsx` & `cg-60.4.1/tests/fixtures/orderforms/1508.30.balsamic.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx` & `cg-60.4.1/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx` & `cg-60.4.1/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/orderforms/1508.30.fastq.xlsx` & `cg-60.4.1/tests/fixtures/orderforms/1508.30.fastq.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/orderforms/1508.30.metagenome.xlsx` & `cg-60.4.1/tests/fixtures/orderforms/1508.30.metagenome.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/orderforms/1508.30.mip.xlsx` & `cg-60.4.1/tests/fixtures/orderforms/1508.30.mip.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/orderforms/1508.30.mip_rna.xlsx` & `cg-60.4.1/tests/fixtures/orderforms/1508.30.mip_rna.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/orderforms/1508.30.rnafusion.xlsx` & `cg-60.4.1/tests/fixtures/orderforms/1508.30.rnafusion.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/orderforms/1603.11.microbial.xlsx` & `cg-60.4.1/tests/fixtures/orderforms/1603.11.microbial.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/orderforms/1604.17.rml.xlsx` & `cg-60.4.1/tests/fixtures/orderforms/1604.17.rml.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/orderforms/2184.9.sarscov2.xlsx` & `cg-60.4.1/tests/fixtures/orderforms/2184.9.sarscov2.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/orderforms/NIPT-json.json` & `cg-60.4.1/tests/fixtures/orderforms/NIPT-json.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json` & `cg-60.4.1/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/orderforms/mip_uploaded_json_orderform.json` & `cg-60.4.1/tests/fixtures/orderforms/mip_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/report/case_data.json` & `cg-60.4.1/tests/fixtures/report/case_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/report/lims_exported_samples.json` & `cg-60.4.1/tests/fixtures/report/lims_exported_samples.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/fixtures/report/lims_family.json` & `cg-60.4.1/tests/fixtures/report/lims_family.json`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/io/conftest.py` & `cg-60.4.1/tests/io/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/io/test_io_controller.py` & `cg-60.4.1/tests/io/test_io_controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/io/test_io_csv.py` & `cg-60.4.1/tests/io/test_io_csv.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/io/test_io_json.py` & `cg-60.4.1/tests/io/test_io_json.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/io/test_io_txt.py` & `cg-60.4.1/tests/io/test_io_txt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/io/test_io_xml.py` & `cg-60.4.1/tests/io/test_io_xml.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/io/test_io_yaml.py` & `cg-60.4.1/tests/io/test_io_yaml.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/io/test_validate_path.py` & `cg-60.4.1/tests/io/test_validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/archive/conftest.py` & `cg-60.4.1/tests/meta/archive/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/archive/test_archive_api.py` & `cg-60.4.1/tests/meta/archive/test_archive_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/archive/test_archive_cli.py` & `cg-60.4.1/tests/meta/archive/test_archive_cli.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/archive/test_archiving.py` & `cg-60.4.1/tests/meta/archive/test_archiving.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/backup/conftest.py` & `cg-60.4.1/tests/meta/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/backup/test_meta_backup.py` & `cg-60.4.1/tests/meta/backup/test_meta_backup.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/backup/test_meta_pdc.py` & `cg-60.4.1/tests/meta/backup/test_meta_pdc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/clean/conftest.py` & `cg-60.4.1/tests/meta/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/clean/test_clean_flow_cells_api.py` & `cg-60.4.1/tests/meta/clean/test_clean_flow_cells_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/clean/test_clean_retrieved_spring_files.py` & `cg-60.4.1/tests/meta/clean/test_clean_retrieved_spring_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/compress/conftest.py` & `cg-60.4.1/tests/meta/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/compress/test_clean_fastq.py` & `cg-60.4.1/tests/meta/compress/test_clean_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/compress/test_compress_files.py` & `cg-60.4.1/tests/meta/compress/test_compress_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/compress/test_compress_meta_fastq.py` & `cg-60.4.1/tests/meta/compress/test_compress_meta_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/compress/test_decompress_spring_meta.py` & `cg-60.4.1/tests/meta/compress/test_decompress_spring_meta.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/compress/test_meta_compress_update_hk.py` & `cg-60.4.1/tests/meta/compress/test_meta_compress_update_hk.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/conftest.py` & `cg-60.4.1/tests/meta/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/deliver/conftest.py` & `cg-60.4.1/tests/meta/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/deliver/test_deliver_ticket.py` & `cg-60.4.1/tests/meta/deliver/test_deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/deliver/test_delivery_api.py` & `cg-60.4.1/tests/meta/deliver/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/deliver/test_fastq_path_generator.py` & `cg-60.4.1/tests/meta/deliver/test_fastq_path_generator.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/delivery/test_delivery_api.py` & `cg-60.4.1/tests/meta/delivery/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/demultiplex/conftest.py` & `cg-60.4.1/tests/meta/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/demultiplex/test_combine_sequencing_metrics.py` & `cg-60.4.1/tests/meta/demultiplex/test_combine_sequencing_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/demultiplex/test_demux_post_processing.py` & `cg-60.4.1/tests/meta/demultiplex/test_demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/demultiplex/test_housekeeper_storage_functions.py` & `cg-60.4.1/tests/meta/demultiplex/test_housekeeper_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/demultiplex/test_status_db_storage_functions.py` & `cg-60.4.1/tests/meta/demultiplex/test_status_db_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/demultiplex/test_utils.py` & `cg-60.4.1/tests/meta/demultiplex/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/demultiplex/test_validation.py` & `cg-60.4.1/tests/meta/demultiplex/test_validation.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/encryption/conftest.py` & `cg-60.4.1/tests/meta/encryption/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/encryption/test_encryption.py` & `cg-60.4.1/tests/meta/encryption/test_encryption.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/observations/conftest.py` & `cg-60.4.1/tests/meta/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/observations/test_meta_upload_observations.py` & `cg-60.4.1/tests/meta/observations/test_meta_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/orders/conftest.py` & `cg-60.4.1/tests/meta/orders/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/orders/test_PoolSubmitter_validate_order.py` & `cg-60.4.1/tests/meta/orders/test_PoolSubmitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py` & `cg-60.4.1/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/orders/test_SarsCov2Submitter_store_order.py` & `cg-60.4.1/tests/meta/orders/test_SarsCov2Submitter_store_order.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/orders/test_SarsCov2Submitter_validate_order.py` & `cg-60.4.1/tests/meta/orders/test_SarsCov2Submitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/orders/test_meta_orders_api.py` & `cg-60.4.1/tests/meta/orders/test_meta_orders_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/orders/test_meta_orders_lims.py` & `cg-60.4.1/tests/meta/orders/test_meta_orders_lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/orders/test_meta_orders_status.py` & `cg-60.4.1/tests/meta/orders/test_meta_orders_status.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/orders/test_rnafusion_submitter.py` & `cg-60.4.1/tests/meta/orders/test_rnafusion_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/orders/test_ticket_handler.py` & `cg-60.4.1/tests/meta/orders/test_ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/qc_metrics/conftest.py` & `cg-60.4.1/tests/meta/qc_metrics/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/qc_metrics/test_collect_qc_metrics.py` & `cg-60.4.1/tests/meta/qc_metrics/test_collect_qc_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/report/conftest.py` & `cg-60.4.1/tests/meta/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/report/test_balsamic_api.py` & `cg-60.4.1/tests/meta/report/test_balsamic_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/report/test_field_validators.py` & `cg-60.4.1/tests/meta/report/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/report/test_mip_dna_api.py` & `cg-60.4.1/tests/meta/report/test_mip_dna_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/report/test_report_api.py` & `cg-60.4.1/tests/meta/report/test_report_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/report/test_rnafusion_api.py` & `cg-60.4.1/tests/meta/report/test_rnafusion_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/report/test_tomte_api.py` & `cg-60.4.1/tests/meta/report/test_tomte_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/rsync/conftest.py` & `cg-60.4.1/tests/meta/rsync/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/rsync/test_rsync.py` & `cg-60.4.1/tests/meta/rsync/test_rsync.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/test_invoice.py` & `cg-60.4.1/tests/meta/test_invoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/transfer/conftest.py` & `cg-60.4.1/tests/meta/transfer/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/transfer/test_external_data.py` & `cg-60.4.1/tests/meta/transfer/test_external_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/transfer/test_meta_transfer_lims.py` & `cg-60.4.1/tests/meta/transfer/test_meta_transfer_lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/upload/balsamic/test_balsamic.py` & `cg-60.4.1/tests/meta/upload/balsamic/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/upload/conftest.py` & `cg-60.4.1/tests/meta/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/upload/gisaid/fixtures/four_samples.csv` & `cg-60.4.1/tests/meta/upload/gisaid/fixtures/four_samples.csv`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/upload/mutacc/conftest.py` & `cg-60.4.1/tests/meta/upload/mutacc/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/upload/mutacc/test_meta_upload_mutacc.py` & `cg-60.4.1/tests/meta/upload/mutacc/test_meta_upload_mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/upload/nipt/conftest.py` & `cg-60.4.1/tests/meta/upload/nipt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/upload/nipt/test_models.py` & `cg-60.4.1/tests/meta/upload/nipt/test_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/upload/nipt/test_nipt_upload_api.py` & `cg-60.4.1/tests/meta/upload/nipt/test_nipt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/upload/scout/conftest.py` & `cg-60.4.1/tests/meta/upload/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/upload/scout/test_generate_load_config.py` & `cg-60.4.1/tests/meta/upload/scout/test_generate_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/upload/scout/test_meta_upload_scoutapi.py` & `cg-60.4.1/tests/meta/upload/scout/test_meta_upload_scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py` & `cg-60.4.1/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/upload/scout/test_scout_config_builder.py` & `cg-60.4.1/tests/meta/upload/scout/test_scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/upload/test_meta_upload_coverage.py` & `cg-60.4.1/tests/meta/upload/test_meta_upload_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/upload/test_upload_api.py` & `cg-60.4.1/tests/meta/upload/test_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/upload/test_upload_genotypes_api.py` & `cg-60.4.1/tests/meta/upload/test_upload_genotypes_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/workflow/conftest.py` & `cg-60.4.1/tests/meta/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/workflow/microsalt/conftest.py` & `cg-60.4.1/tests/meta/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/workflow/microsalt/test_quality_controller.py` & `cg-60.4.1/tests/meta/workflow/microsalt/test_quality_controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/workflow/microsalt/test_quality_controller_utils.py` & `cg-60.4.1/tests/meta/workflow/microsalt/test_quality_controller_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/workflow/microsalt/test_report_generation.py` & `cg-60.4.1/tests/meta/workflow/microsalt/test_report_generation.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/workflow/test_analysis.py` & `cg-60.4.1/tests/meta/workflow/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/workflow/test_balsamic.py` & `cg-60.4.1/tests/meta/workflow/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/workflow/test_fastq.py` & `cg-60.4.1/tests/meta/workflow/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/workflow/test_microsalt.py` & `cg-60.4.1/tests/meta/workflow/test_microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/workflow/test_nf_analysis.py` & `cg-60.4.1/tests/meta/workflow/test_nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/workflow/test_prepare_fastq_api.py` & `cg-60.4.1/tests/meta/workflow/test_prepare_fastq_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/workflow/test_raredisease.py` & `cg-60.4.1/tests/meta/workflow/test_raredisease.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/meta/workflow/test_rnafusion.py` & `cg-60.4.1/tests/meta/workflow/test_rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/mocks/balsamic_analysis_mock.py` & `cg-60.4.1/tests/mocks/balsamic_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/mocks/crunchy.py` & `cg-60.4.1/tests/mocks/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/mocks/hk_mock.py` & `cg-60.4.1/tests/mocks/hk_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/mocks/limsmock.py` & `cg-60.4.1/tests/mocks/limsmock.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/mocks/madeline.py` & `cg-60.4.1/tests/mocks/madeline.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/mocks/mip_analysis_mock.py` & `cg-60.4.1/tests/mocks/mip_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/mocks/osticket.py` & `cg-60.4.1/tests/mocks/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/mocks/process_mock.py` & `cg-60.4.1/tests/mocks/process_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/mocks/report.py` & `cg-60.4.1/tests/mocks/report.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/mocks/scout.py` & `cg-60.4.1/tests/mocks/scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/mocks/store_model.py` & `cg-60.4.1/tests/mocks/store_model.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/mocks/tb_mock.py` & `cg-60.4.1/tests/mocks/tb_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/models/balsamic/conftest.py` & `cg-60.4.1/tests/models/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/models/balsamic/test_balsamic_analysis.py` & `cg-60.4.1/tests/models/balsamic/test_balsamic_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/models/conftest.py` & `cg-60.4.1/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/models/demultiplexing/test_run_parameters.py` & `cg-60.4.1/tests/models/demultiplexing/test_run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/models/downsample/test_down_sample_meta_data.py` & `cg-60.4.1/tests/models/downsample/test_down_sample_meta_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/models/flow_cell/test_flowcell_model.py` & `cg-60.4.1/tests/models/flow_cell/test_flowcell_model.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/models/mip/conftest.py` & `cg-60.4.1/tests/models/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/models/mip/test_mip_analysis.py` & `cg-60.4.1/tests/models/mip/test_mip_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/models/mip/test_mip_config.py` & `cg-60.4.1/tests/models/mip/test_mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/models/mip/test_mip_metrics_deliverables.py` & `cg-60.4.1/tests/models/mip/test_mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/models/mip/test_mip_sample_info.py` & `cg-60.4.1/tests/models/mip/test_mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/models/nextflow/test_nextflow_deliver.py` & `cg-60.4.1/tests/models/nextflow/test_nextflow_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/models/observations/conftest.py` & `cg-60.4.1/tests/models/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/models/observations/test_observations_input_files.py` & `cg-60.4.1/tests/models/observations/test_observations_input_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/models/report/test_validators.py` & `cg-60.4.1/tests/models/report/test_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/models/rnafusion/test_rnafusion_sample.py` & `cg-60.4.1/tests/models/rnafusion/test_rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/models/test_cg_models.py` & `cg-60.4.1/tests/models/test_cg_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/models/test_compression_data.py` & `cg-60.4.1/tests/models/test_compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/models/test_fastq.py` & `cg-60.4.1/tests/models/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/models/test_file_data.py` & `cg-60.4.1/tests/models/test_file_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/server/conftest.py` & `cg-60.4.1/tests/server/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/server/endpoints/test_delivery_message_endpoint.py` & `cg-60.4.1/tests/server/endpoints/test_delivery_message_endpoint.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/server/endpoints/test_orders_endpoint.py` & `cg-60.4.1/tests/server/endpoints/test_orders_endpoint.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/services/fastq_file_service/conftest.py` & `cg-60.4.1/tests/services/fastq_file_service/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/services/fastq_file_service/test_fastq_file_service.py` & `cg-60.4.1/tests/services/fastq_file_service/test_fastq_file_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/services/orders/order_status_service/conftest.py` & `cg-60.4.1/tests/services/orders/order_status_service/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/services/orders/order_status_service/test_order_summary_service.py` & `cg-60.4.1/tests/services/orders/order_status_service/test_order_summary_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/services/quality_controller/test_sequencing_quality_checks_utils.py` & `cg-60.4.1/tests/services/quality_controller/test_sequencing_quality_checks_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/api/conftest.py` & `cg-60.4.1/tests/store/api/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/api/test_base.py` & `cg-60.4.1/tests/store/api/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/conftest.py` & `cg-60.4.1/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/crud/add/test_store_add_application_version.py` & `cg-60.4.1/tests/store/crud/add/test_store_add_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/crud/add/test_store_add_base.py` & `cg-60.4.1/tests/store/crud/add/test_store_add_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/crud/add/test_store_add_customer.py` & `cg-60.4.1/tests/store/crud/add/test_store_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/crud/add/test_store_add_flow_celll.py` & `cg-60.4.1/tests/store/crud/add/test_store_add_flow_celll.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/crud/conftest.py` & `cg-60.4.1/tests/store/crud/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/crud/delete/test_delete.py` & `cg-60.4.1/tests/store/crud/delete/test_delete.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/crud/read/test_read.py` & `cg-60.4.1/tests/store/crud/read/test_read.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/crud/read/test_read_analyses_to_clean.py` & `cg-60.4.1/tests/store/crud/read/test_read_analyses_to_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/crud/read/test_read_analyses_to_delivery_report.py` & `cg-60.4.1/tests/store/crud/read/test_read_analyses_to_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/crud/read/test_read_analysis.py` & `cg-60.4.1/tests/store/crud/read/test_read_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/crud/read/test_read_application_version.py` & `cg-60.4.1/tests/store/crud/read/test_read_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/crud/read/test_read_customer.py` & `cg-60.4.1/tests/store/crud/read/test_read_customer.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/crud/read/test_read_pool.py` & `cg-60.4.1/tests/store/crud/read/test_read_pool.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/crud/read/test_read_sample.py` & `cg-60.4.1/tests/store/crud/read/test_read_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/crud/update/test_update.py` & `cg-60.4.1/tests/store/crud/update/test_update.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/filters/test_status_analyses_filters.py` & `cg-60.4.1/tests/store/filters/test_status_analyses_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/filters/test_status_application_filters.py` & `cg-60.4.1/tests/store/filters/test_status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/filters/test_status_application_limitations_filters.py` & `cg-60.4.1/tests/store/filters/test_status_application_limitations_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/filters/test_status_application_version_filters.py` & `cg-60.4.1/tests/store/filters/test_status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/filters/test_status_bed_filters.py` & `cg-60.4.1/tests/store/filters/test_status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/filters/test_status_bed_version_filters.py` & `cg-60.4.1/tests/store/filters/test_status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/filters/test_status_case_sample_filters.py` & `cg-60.4.1/tests/store/filters/test_status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/filters/test_status_cases_filters.py` & `cg-60.4.1/tests/store/filters/test_status_cases_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/filters/test_status_collaboration_filters.py` & `cg-60.4.1/tests/store/filters/test_status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/filters/test_status_customer_filters.py` & `cg-60.4.1/tests/store/filters/test_status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/filters/test_status_flow_cell_filters.py` & `cg-60.4.1/tests/store/filters/test_status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/filters/test_status_invoice_filters.py` & `cg-60.4.1/tests/store/filters/test_status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/filters/test_status_metrics_filters.py` & `cg-60.4.1/tests/store/filters/test_status_metrics_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/filters/test_status_organism_filters.py` & `cg-60.4.1/tests/store/filters/test_status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/filters/test_status_panel_filters.py` & `cg-60.4.1/tests/store/filters/test_status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/filters/test_status_pool_filters.py` & `cg-60.4.1/tests/store/filters/test_status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/filters/test_status_samples_filters.py` & `cg-60.4.1/tests/store/filters/test_status_samples_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/filters/test_status_user_filters.py` & `cg-60.4.1/tests/store/filters/test_status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/test_delivery.py` & `cg-60.4.1/tests/store/test_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store/test_store_models.py` & `cg-60.4.1/tests/store/test_store_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/store_helpers.py` & `cg-60.4.1/tests/store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/test_copy_novaseqx_flow_cell.py` & `cg-60.4.1/tests/test_copy_novaseqx_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/test_store_helpers.py` & `cg-60.4.1/tests/test_store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/utils/conftest.py` & `cg-60.4.1/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/utils/test_commands.py` & `cg-60.4.1/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/utils/test_date.py` & `cg-60.4.1/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/utils/test_dict.py` & `cg-60.4.1/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/utils/test_dispatcher.py` & `cg-60.4.1/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/utils/test_files.py` & `cg-60.4.1/tests/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/utils/test_time.py` & `cg-60.4.1/tests/utils/test_time.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/tests/utils/test_utils.py` & `cg-60.4.1/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.4.0/PKG-INFO` & `cg-60.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 60.4.0
+Version: 60.4.1
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

