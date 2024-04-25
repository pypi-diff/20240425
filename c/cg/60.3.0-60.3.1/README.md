# Comparing `tmp/cg-60.3.0.tar.gz` & `tmp/cg-60.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cg-60.3.0.tar", max compression
+gzip compressed data, was "cg-60.3.1.tar", max compression
```

## Comparing `cg-60.3.0.tar` & `cg-60.3.1.tar`

### file list

```diff
@@ -1,1369 +1,1369 @@
--rw-r--r--   0        0        0     2686 2024-04-24 09:24:14.188206 cg-60.3.0/README.md
--rw-r--r--   0        0        0       40 2024-04-24 09:24:14.192206 cg-60.3.0/cg/__init__.py
--rw-r--r--   0        0        0      315 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/__init__.py
--rw-r--r--   0        0        0       27 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/coverage/__init__.py
--rw-r--r--   0        0        0     2940 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/coverage/api.py
--rw-r--r--   0        0        0       56 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/crunchy/__init__.py
--rw-r--r--   0        0        0    12783 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/crunchy/crunchy.py
--rw-r--r--   0        0        0     4502 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/crunchy/files.py
--rw-r--r--   0        0        0      430 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/crunchy/models.py
--rw-r--r--   0        0        0      910 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/crunchy/sbatch.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/demultiplex/__init__.py
--rw-r--r--   0        0        0    11299 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/demultiplex/demultiplex_api.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/demultiplex/sample_sheet/__init__.py
--rw-r--r--   0        0        0    12410 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/demultiplex/sample_sheet/api.py
--rw-r--r--   0        0        0     3442 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/demultiplex/sample_sheet/index.py
--rw-r--r--   0        0        0     7341 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py
--rw-r--r--   0        0        0     4305 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py
--rw-r--r--   0        0        0    10542 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/demultiplex/sample_sheet/sample_models.py
--rw-r--r--   0        0        0     6180 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py
--rw-r--r--   0        0        0     1614 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py
--rw-r--r--   0        0        0     8346 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py
--rw-r--r--   0        0        0      824 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/demultiplex/sample_sheet/validators.py
--rw-r--r--   0        0        0      677 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/demultiplex/sbatch.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/downsample/__init__.py
--rw-r--r--   0        0        0     6160 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/downsample/downsample.py
--rw-r--r--   0        0        0     2125 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/downsample/utils.py
--rw-r--r--   0        0        0      298 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/environ.py
--rw-r--r--   0        0        0     1741 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/gens.py
--rw-r--r--   0        0        0     3419 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/gt.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/hermes/__init__.py
--rw-r--r--   0        0        0     2249 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/hermes/hermes_api.py
--rw-r--r--   0        0        0     1298 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/hermes/models.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/housekeeper/__init__.py
--rw-r--r--   0        0        0    30395 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/housekeeper/hk.py
--rw-r--r--   0        0        0      326 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/housekeeper/models.py
--rw-r--r--   0        0        0       32 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/invoice/__init__.py
--rw-r--r--   0        0        0     4804 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/invoice/render.py
--rw-r--r--   0        0        0   113467 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/invoice/templates/KI_pool_invoice.xlsx
--rw-r--r--   0        0        0    75562 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/invoice/templates/KI_sample_invoice.xlsx
--rw-r--r--   0        0        0   113512 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
--rw-r--r--   0        0        0    75459 2024-04-24 09:24:14.192206 cg-60.3.0/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
--rw-r--r--   0        0        0       25 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/lims/__init__.py
--rw-r--r--   0        0        0    18546 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/lims/api.py
--rw-r--r--   0        0        0     2652 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/lims/batch.py
--rw-r--r--   0        0        0     8129 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/lims/order.py
--rw-r--r--   0        0        0     3148 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/lims/sample_sheet.py
--rw-r--r--   0        0        0     4866 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/loqus.py
--rw-r--r--   0        0        0       35 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/madeline/__init__.py
--rw-r--r--   0        0        0     3213 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/madeline/api.py
--rw-r--r--   0        0        0       23 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/mip/__init__.py
--rw-r--r--   0        0        0     3564 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/mip/confighandler.py
--rw-r--r--   0        0        0     2207 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/mutacc_auto.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/orderform/__init__.py
--rw-r--r--   0        0        0     9498 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/orderform/excel_orderform_parser.py
--rw-r--r--   0        0        0     3051 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/orderform/json_orderform_parser.py
--rw-r--r--   0        0        0     6419 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/orderform/orderform_parser.py
--rw-r--r--   0        0        0      252 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/orderform/utils.py
--rw-r--r--   0        0        0     2537 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/osticket.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/scout/__init__.py
--rw-r--r--   0        0        0     3177 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/scout/scout_export.py
--rw-r--r--   0        0        0    11054 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/scout/scoutapi.py
--rw-r--r--   0        0        0      444 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/scout/validators.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0        0        0     3457 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/sequencing_metrics_parser/api.py
--rw-r--r--   0        0        0      923 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/sequencing_metrics_parser/models.py
--rw-r--r--   0        0        0     6670 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/sequencing_metrics_parser/parser.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/slurm/__init__.py
--rw-r--r--   0        0        0     1277 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/slurm/sbatch.py
--rw-r--r--   0        0        0     3559 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/slurm/slurm_api.py
--rw-r--r--   0        0        0       32 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/tb/__init__.py
--rw-r--r--   0        0        0     7995 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/tb/api.py
--rw-r--r--   0        0        0      152 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/tb/dto/create_job_request.py
--rw-r--r--   0        0        0      250 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/tb/dto/summary_response.py
--rw-r--r--   0        0        0     1305 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/tb/models.py
--rw-r--r--   0        0        0      305 2024-04-24 09:24:14.196206 cg-60.3.0/cg/apps/tb/validators.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/__init__.py
--rw-r--r--   0        0        0    11558 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/add.py
--rw-r--r--   0        0        0     2653 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/archive.py
--rw-r--r--   0        0        0    10118 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/backup.py
--rw-r--r--   0        0        0     3852 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/base.py
--rw-r--r--   0        0        0    10506 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/clean.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/compress/__init__.py
--rw-r--r--   0        0        0     2135 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/compress/base.py
--rw-r--r--   0        0        0     6706 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/compress/fastq.py
--rw-r--r--   0        0        0     8163 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/compress/helpers.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/delete/__init__.py
--rw-r--r--   0        0        0      564 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/delete/base.py
--rw-r--r--   0        0        0     4603 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/delete/case.py
--rw-r--r--   0        0        0     1884 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/delete/cases.py
--rw-r--r--   0        0        0     2633 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/delete/observations.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/deliver/__init__.py
--rw-r--r--   0        0        0     6030 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/deliver/base.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/demultiplex/__init__.py
--rw-r--r--   0        0        0      829 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/demultiplex/base.py
--rw-r--r--   0        0        0     4905 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py
--rw-r--r--   0        0        0     7726 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/demultiplex/demux.py
--rw-r--r--   0        0        0     1473 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/demultiplex/finish.py
--rw-r--r--   0        0        0     3119 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/demultiplex/sample_sheet.py
--rw-r--r--   0        0        0     2995 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/downsample.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/generate/__init__.py
--rw-r--r--   0        0        0      356 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/generate/base.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/generate/report/__init__.py
--rw-r--r--   0        0        0     4636 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/generate/report/base.py
--rw-r--r--   0        0        0      854 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/generate/report/options.py
--rw-r--r--   0        0        0     5340 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/generate/report/utils.py
--rw-r--r--   0        0        0     8327 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/get.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/set/__init__.py
--rw-r--r--   0        0        0     9856 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/set/base.py
--rw-r--r--   0        0        0     4384 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/set/case.py
--rw-r--r--   0        0        0     2595 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/set/cases.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/store/__init__.py
--rw-r--r--   0        0        0     1093 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/store/base.py
--rw-r--r--   0        0        0     6191 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/store/store.py
--rw-r--r--   0        0        0     1761 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/transfer.py
--rw-r--r--   0        0        0        1 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/upload/__init__.py
--rw-r--r--   0        0        0     5706 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/upload/base.py
--rw-r--r--   0        0        0     5503 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/upload/clinical_delivery.py
--rw-r--r--   0        0        0     1175 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/upload/coverage.py
--rw-r--r--   0        0        0     1528 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/upload/delivery_report.py
--rw-r--r--   0        0        0     4022 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/upload/fohm.py
--rw-r--r--   0        0        0     1463 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/upload/genotype.py
--rw-r--r--   0        0        0     1885 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/upload/gens.py
--rw-r--r--   0        0        0      584 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/upload/gisaid.py
--rw-r--r--   0        0        0     2645 2024-04-24 09:24:14.196206 cg-60.3.0/cg/cli/upload/mutacc.py
--rw-r--r--   0        0        0       23 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/upload/nipt/__init__.py
--rw-r--r--   0        0        0     3006 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/upload/nipt/base.py
--rw-r--r--   0        0        0     2275 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/upload/nipt/ftp.py
--rw-r--r--   0        0        0     1596 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/upload/nipt/statina.py
--rw-r--r--   0        0        0      112 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/upload/observations/__init__.py
--rw-r--r--   0        0        0     2672 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/upload/observations/observations.py
--rw-r--r--   0        0        0     2904 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/upload/observations/utils.py
--rw-r--r--   0        0        0     9970 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/upload/scout.py
--rw-r--r--   0        0        0      650 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/upload/utils.py
--rw-r--r--   0        0        0     1667 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/upload/validate.py
--rw-r--r--   0        0        0      105 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/utils.py
--rw-r--r--   0        0        0       18 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/__init__.py
--rw-r--r--   0        0        0       22 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/balsamic/__init__.py
--rw-r--r--   0        0        0     8925 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/balsamic/base.py
--rw-r--r--   0        0        0     1980 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/balsamic/options.py
--rw-r--r--   0        0        0      881 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/balsamic/pon.py
--rw-r--r--   0        0        0     1162 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/balsamic/qc.py
--rw-r--r--   0        0        0     1177 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/balsamic/umi.py
--rw-r--r--   0        0        0     1342 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/base.py
--rw-r--r--   0        0        0    12379 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/commands.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/fastq/__init__.py
--rw-r--r--   0        0        0     1367 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/fastq/base.py
--rw-r--r--   0        0        0     1787 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/fastq/fastq_service.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/fluffy/__init__.py
--rw-r--r--   0        0        0     4177 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/fluffy/base.py
--rw-r--r--   0        0        0       22 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/jasen/__init__.py
--rw-r--r--   0        0        0      535 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/jasen/base.py
--rw-r--r--   0        0        0       22 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/microsalt/__init__.py
--rw-r--r--   0        0        0     7810 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/microsalt/base.py
--rw-r--r--   0        0        0       22 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/mip/__init__.py
--rw-r--r--   0        0        0     6596 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/mip/base.py
--rw-r--r--   0        0        0     1268 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/mip/options.py
--rw-r--r--   0        0        0       22 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/mip_dna/__init__.py
--rw-r--r--   0        0        0     1013 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/mip_dna/base.py
--rw-r--r--   0        0        0       22 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/mip_rna/__init__.py
--rw-r--r--   0        0        0      916 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/mip_rna/base.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/mutant/__init__.py
--rw-r--r--   0        0        0     3413 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/mutant/base.py
--rw-r--r--   0        0        0     9002 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/nf_analysis.py
--rw-r--r--   0        0        0       22 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/raredisease/__init__.py
--rw-r--r--   0        0        0     2210 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/raredisease/base.py
--rw-r--r--   0        0        0       22 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/rnafusion/__init__.py
--rw-r--r--   0        0        0     1179 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/rnafusion/base.py
--rw-r--r--   0        0        0       22 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/taxprofiler/__init__.py
--rw-r--r--   0        0        0     1211 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/taxprofiler/base.py
--rw-r--r--   0        0        0     1111 2024-04-24 09:24:14.200206 cg-60.3.0/cg/cli/workflow/tomte/base.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.200206 cg-60.3.0/cg/clients/__init__.py
--rw-r--r--   0        0        0     1363 2024-04-24 09:24:14.200206 cg-60.3.0/cg/clients/arnold/api.py
--rw-r--r--   0        0        0      160 2024-04-24 09:24:14.200206 cg-60.3.0/cg/clients/arnold/dto/create_case_request.py
--rw-r--r--   0        0        0      384 2024-04-24 09:24:14.200206 cg-60.3.0/cg/clients/arnold/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.200206 cg-60.3.0/cg/clients/janus/__init__.py
--rw-r--r--   0        0        0     1246 2024-04-24 09:24:14.200206 cg-60.3.0/cg/clients/janus/api.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.200206 cg-60.3.0/cg/clients/janus/dto/__init__.py
--rw-r--r--   0        0        0      503 2024-04-24 09:24:14.200206 cg-60.3.0/cg/clients/janus/dto/create_qc_metrics_request.py
--rw-r--r--   0        0        0      420 2024-04-24 09:24:14.200206 cg-60.3.0/cg/clients/janus/exceptions.py
--rw-r--r--   0        0        0      937 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/__init__.py
--rw-r--r--   0        0        0      253 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/archiving.py
--rw-r--r--   0        0        0       35 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/backup.py
--rw-r--r--   0        0        0      769 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/bcl_convert_metrics.py
--rw-r--r--   0        0        0      469 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/compression.py
--rw-r--r--   0        0        0     6613 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/constants.py
--rw-r--r--   0        0        0     6033 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/delivery.py
--rw-r--r--   0        0        0     8120 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/demultiplexing.py
--rw-r--r--   0        0        0     1422 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/encryption.py
--rw-r--r--   0        0        0      372 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/extraction.py
--rw-r--r--   0        0        0     2054 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/gene_panel.py
--rw-r--r--   0        0        0     6704 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/housekeeper_tags.py
--rw-r--r--   0        0        0       95 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/invoice.py
--rw-r--r--   0        0        0     5815 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/lims.py
--rw-r--r--   0        0        0      743 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/metrics.py
--rw-r--r--   0        0        0      231 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/nanopore_files.py
--rw-r--r--   0        0        0      650 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/nextflow.py
--rw-r--r--   0        0        0     1529 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/nf_analysis.py
--rw-r--r--   0        0        0       19 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/nipt.py
--rw-r--r--   0        0        0     2257 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/observations.py
--rw-r--r--   0        0        0     1216 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/orderforms.py
--rw-r--r--   0        0        0       96 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/paths.py
--rw-r--r--   0        0        0      266 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/pdc.py
--rw-r--r--   0        0        0      160 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/pedigree.py
--rw-r--r--   0        0        0     1044 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/priority.py
--rw-r--r--   0        0        0       79 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/process.py
--rw-r--r--   0        0        0     5474 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/report.py
--rw-r--r--   0        0        0      485 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/sample_sources.py
--rw-r--r--   0        0        0     3111 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/scout.py
--rw-r--r--   0        0        0     1669 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/sequencing.py
--rw-r--r--   0        0        0      313 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/slurm.py
--rw-r--r--   0        0        0      529 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/subject.py
--rw-r--r--   0        0        0       55 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/symbols.py
--rw-r--r--   0        0        0      435 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/tb.py
--rw-r--r--   0        0        0      161 2024-04-24 09:24:14.200206 cg-60.3.0/cg/constants/time.py
--rw-r--r--   0        0        0     6639 2024-04-24 09:24:14.200206 cg-60.3.0/cg/exc.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.200206 cg-60.3.0/cg/io/__init__.py
--rw-r--r--   0        0        0     1037 2024-04-24 09:24:14.204206 cg-60.3.0/cg/io/api.py
--rw-r--r--   0        0        0      621 2024-04-24 09:24:14.204206 cg-60.3.0/cg/io/config.py
--rw-r--r--   0        0        0     2978 2024-04-24 09:24:14.204206 cg-60.3.0/cg/io/controller.py
--rw-r--r--   0        0        0     1763 2024-04-24 09:24:14.204206 cg-60.3.0/cg/io/csv.py
--rw-r--r--   0        0        0      210 2024-04-24 09:24:14.204206 cg-60.3.0/cg/io/gzip.py
--rw-r--r--   0        0        0      662 2024-04-24 09:24:14.204206 cg-60.3.0/cg/io/json.py
--rw-r--r--   0        0        0      525 2024-04-24 09:24:14.204206 cg-60.3.0/cg/io/png.py
--rw-r--r--   0        0        0     1094 2024-04-24 09:24:14.204206 cg-60.3.0/cg/io/txt.py
--rw-r--r--   0        0        0      552 2024-04-24 09:24:14.204206 cg-60.3.0/cg/io/validate_path.py
--rw-r--r--   0        0        0     1289 2024-04-24 09:24:14.204206 cg-60.3.0/cg/io/xml.py
--rw-r--r--   0        0        0     1153 2024-04-24 09:24:14.204206 cg-60.3.0/cg/io/yaml.py
--rw-r--r--   0        0        0      281 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/archive/__init__.py
--rw-r--r--   0        0        0    15193 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/archive/archive.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/archive/ddn/__init__.py
--rw-r--r--   0        0        0     1727 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/archive/ddn/constants.py
--rw-r--r--   0        0        0    10852 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/archive/ddn/ddn_data_flow_client.py
--rw-r--r--   0        0        0     3704 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/archive/ddn/models.py
--rw-r--r--   0        0        0     1250 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/archive/ddn/utils.py
--rw-r--r--   0        0        0     2024 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/archive/models.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/backup/__init__.py
--rw-r--r--   0        0        0    17426 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/backup/backup.py
--rw-r--r--   0        0        0     5397 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/backup/pdc.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/clean/__init__.py
--rw-r--r--   0        0        0     3901 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/clean/api.py
--rw-r--r--   0        0        0     7738 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/clean/clean_flow_cells.py
--rw-r--r--   0        0        0     1841 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/clean/clean_retrieved_spring_files.py
--rw-r--r--   0        0        0       34 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/compress/__init__.py
--rw-r--r--   0        0        0    14557 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/compress/compress.py
--rw-r--r--   0        0        0     4947 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/compress/files.py
--rw-r--r--   0        0        0       77 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/deliver/__init__.py
--rw-r--r--   0        0        0    14672 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/deliver/deliver.py
--rw-r--r--   0        0        0     4502 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/deliver/deliver_ticket.py
--rw-r--r--   0        0        0      904 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/deliver/fastq_path_generator.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/delivery/__init__.py
--rw-r--r--   0        0        0     8255 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/delivery/delivery.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/demultiplex/__init__.py
--rw-r--r--   0        0        0     2592 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/demultiplex/combine_sequencing_metrics.py
--rw-r--r--   0        0        0     5719 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/demultiplex/demux_post_processing.py
--rw-r--r--   0        0        0     4135 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/demultiplex/files.py
--rw-r--r--   0        0        0     7777 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/demultiplex/housekeeper_storage_functions.py
--rw-r--r--   0        0        0     6126 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/demultiplex/status_db_storage_functions.py
--rw-r--r--   0        0        0    10690 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/demultiplex/utils.py
--rw-r--r--   0        0        0     2855 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/demultiplex/validation.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/encryption/__init__.py
--rw-r--r--   0        0        0    20271 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/encryption/encryption.py
--rw-r--r--   0        0        0      537 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/encryption/sbatch.py
--rw-r--r--   0        0        0    10922 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/invoice.py
--rw-r--r--   0        0        0     2360 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/meta.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/observations/__init__.py
--rw-r--r--   0        0        0     6008 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/observations/balsamic_observations_api.py
--rw-r--r--   0        0        0     5277 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/observations/mip_dna_observations_api.py
--rw-r--r--   0        0        0     5364 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/observations/observations_api.py
--rw-r--r--   0        0        0       27 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/orders/__init__.py
--rw-r--r--   0        0        0     3637 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/orders/api.py
--rw-r--r--   0        0        0      121 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/orders/balsamic_qc_submitter.py
--rw-r--r--   0        0        0      107 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/orders/balsamic_submitter.py
--rw-r--r--   0        0        0      122 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/orders/balsamic_umi_submitter.py
--rw-r--r--   0        0        0    15262 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/orders/case_submitter.py
--rw-r--r--   0        0        0     6102 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/orders/fastq_submitter.py
--rw-r--r--   0        0        0      105 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/orders/fluffy_submitter.py
--rw-r--r--   0        0        0     1254 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/orders/lims.py
--rw-r--r--   0        0        0     5782 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/orders/metagenome_submitter.py
--rw-r--r--   0        0        0     6337 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/orders/microbial_submitter.py
--rw-r--r--   0        0        0      123 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/orders/microsalt_submitter.py
--rw-r--r--   0        0        0      105 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/orders/mip_dna_submitter.py
--rw-r--r--   0        0        0      105 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/orders/mip_rna_submitter.py
--rw-r--r--   0        0        0     7761 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/orders/pool_submitter.py
--rw-r--r--   0        0        0      102 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/orders/rml_submitter.py
--rw-r--r--   0        0        0      718 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/orders/rnafusion_submitter.py
--rw-r--r--   0        0        0     1268 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/orders/sars_cov_2_submitter.py
--rw-r--r--   0        0        0     1754 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/orders/submitter.py
--rw-r--r--   0        0        0     7880 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/orders/ticket_handler.py
--rw-r--r--   0        0        0     4105 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/qc_metrics/collect_qc_metrics.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/report/__init__.py
--rw-r--r--   0        0        0     8168 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/report/balsamic.py
--rw-r--r--   0        0        0      562 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/report/balsamic_qc.py
--rw-r--r--   0        0        0      717 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/report/balsamic_umi.py
--rw-r--r--   0        0        0     4171 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/report/field_validators.py
--rw-r--r--   0        0        0     6620 2024-04-24 09:24:14.204206 cg-60.3.0/cg/meta/report/mip_dna.py
--rw-r--r--   0        0        0    18606 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/report_api.py
--rw-r--r--   0        0        0     5625 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/rnafusion.py
--rw-r--r--   0        0        0     1911 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/templates/delivery-report.html
--rw-r--r--   0        0        0     4236 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/templates/macros/data_analysis/data_analysis.html
--rw-r--r--   0        0        0     1049 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/templates/macros/data_analysis/limitations.html
--rw-r--r--   0        0        0     3351 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html
--rw-r--r--   0        0        0     1364 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html
--rw-r--r--   0        0        0      753 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html
--rw-r--r--   0        0        0     3284 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html
--rw-r--r--   0        0        0     3670 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html
--rw-r--r--   0        0        0     2332 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/templates/macros/header.html
--rw-r--r--   0        0        0     2066 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/templates/macros/order.html
--rw-r--r--   0        0        0     2243 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/templates/macros/sample_prep.html
--rw-r--r--   0        0        0      472 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/templates/macros/ticket_system.html
--rw-r--r--   0        0        0     1165 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html
--rw-r--r--   0        0        0     1538 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html
--rw-r--r--   0        0        0      428 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/templates/macros/uploaded_files/rnafusion_uploaded_files.html
--rw-r--r--   0        0        0     4266 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html
--rw-r--r--   0        0        0       80 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/templates/partials/footer.html
--rw-r--r--   0        0        0      172 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/templates/partials/signature.html
--rw-r--r--   0        0        0   232803 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/templates/static/css/bootstrap.min.css
--rw-r--r--   0        0        0       33 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/templates/static/css/custom.css
--rw-r--r--   0        0        0    30068 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/templates/static/images/SWEDAC_logo.png
--rw-r--r--   0        0        0     3925 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/report/tomte.py
--rw-r--r--   0        0        0       32 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/rsync/__init__.py
--rw-r--r--   0        0        0    12291 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/rsync/rsync_api.py
--rw-r--r--   0        0        0      387 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/rsync/sbatch.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/tar/__init__.py
--rw-r--r--   0        0        0     1694 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/tar/tar.py
--rw-r--r--   0        0        0       71 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/transfer/__init__.py
--rw-r--r--   0        0        0    10016 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/transfer/external_data.py
--rw-r--r--   0        0        0     5814 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/transfer/lims.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/balsamic/__init__.py
--rw-r--r--   0        0        0     3107 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/balsamic/balsamic.py
--rw-r--r--   0        0        0     2224 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/coverage.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/fohm/__init__.py
--rw-r--r--   0        0        0    12102 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/fohm/fohm.py
--rw-r--r--   0        0        0       30 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/gisaid/__init__.py
--rw-r--r--   0        0        0      928 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/gisaid/constants.py
--rw-r--r--   0        0        0    13521 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/gisaid/gisaid.py
--rw-r--r--   0        0        0     3312 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/gisaid/models.py
--rw-r--r--   0        0        0     5310 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/gt.py
--rw-r--r--   0        0        0      898 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/microsalt/microsalt_upload_api.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/mip/__init__.py
--rw-r--r--   0        0        0     2546 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/mip/mip_dna.py
--rw-r--r--   0        0        0     1400 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/mip/mip_rna.py
--rw-r--r--   0        0        0     7294 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/mutacc.py
--rw-r--r--   0        0        0     1853 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/nf_analysis.py
--rw-r--r--   0        0        0       32 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/nipt/__init__.py
--rw-r--r--   0        0        0      696 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/nipt/models.py
--rw-r--r--   0        0        0     8106 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/nipt/nipt.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/scout/__init__.py
--rw-r--r--   0        0        0     4009 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/scout/balsamic_config_builder.py
--rw-r--r--   0        0        0     1491 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/scout/balsamic_umi_config_builder.py
--rw-r--r--   0        0        0     3322 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/scout/hk_tags.py
--rw-r--r--   0        0        0     9103 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/scout/mip_config_builder.py
--rw-r--r--   0        0        0     3495 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/scout/rnafusion_config_builder.py
--rw-r--r--   0        0        0     7231 2024-04-24 09:24:14.208206 cg-60.3.0/cg/meta/upload/scout/scout_config_builder.py
--rw-r--r--   0        0        0    23146 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/upload/scout/uploadscoutapi.py
--rw-r--r--   0        0        0     3197 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/upload/upload_api.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/__init__.py
--rw-r--r--   0        0        0    28043 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/analysis.py
--rw-r--r--   0        0        0    28188 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/balsamic.py
--rw-r--r--   0        0        0     2700 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/balsamic_pon.py
--rw-r--r--   0        0        0      553 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/balsamic_qc.py
--rw-r--r--   0        0        0      556 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/balsamic_umi.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/downsample/__init__.py
--rw-r--r--   0        0        0     3922 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/downsample/downsample.py
--rw-r--r--   0        0        0      711 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/downsample/sbatch.py
--rw-r--r--   0        0        0     8913 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/fastq.py
--rw-r--r--   0        0        0    10687 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/fluffy.py
--rw-r--r--   0        0        0      521 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/jasen.py
--rw-r--r--   0        0        0       70 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/microsalt/__init__.py
--rw-r--r--   0        0        0      116 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/microsalt/constants.py
--rw-r--r--   0        0        0      174 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/microsalt/metrics_parser/__init__.py
--rw-r--r--   0        0        0      366 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/microsalt/metrics_parser/metrics_parser.py
--rw-r--r--   0        0        0      903 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/microsalt/metrics_parser/models.py
--rw-r--r--   0        0        0    13062 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/microsalt/microsalt.py
--rw-r--r--   0        0        0       95 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/microsalt/quality_controller/__init__.py
--rw-r--r--   0        0        0      712 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/microsalt/quality_controller/models.py
--rw-r--r--   0        0        0     5688 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/microsalt/quality_controller/quality_controller.py
--rw-r--r--   0        0        0     1217 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/microsalt/quality_controller/report_generator.py
--rw-r--r--   0        0        0     2373 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/microsalt/quality_controller/result_logger.py
--rw-r--r--   0        0        0     5641 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/microsalt/quality_controller/utils.py
--rw-r--r--   0        0        0     1220 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/microsalt/utils.py
--rw-r--r--   0        0        0    13924 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/mip.py
--rw-r--r--   0        0        0     2991 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/mip_dna.py
--rw-r--r--   0        0        0     2167 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/mip_rna.py
--rw-r--r--   0        0        0    10587 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/mutant.py
--rw-r--r--   0        0        0    35481 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/nf_analysis.py
--rw-r--r--   0        0        0     6161 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/nf_handlers.py
--rw-r--r--   0        0        0     6394 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/prepare_fastq.py
--rw-r--r--   0        0        0     5988 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/raredisease.py
--rw-r--r--   0        0        0     5214 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/rnafusion.py
--rw-r--r--   0        0        0     4607 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/taxprofiler.py
--rw-r--r--   0        0        0     3204 2024-04-24 09:24:14.212206 cg-60.3.0/cg/meta/workflow/tomte.py
--rw-r--r--   0        0        0      113 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/__init__.py
--rw-r--r--   0        0        0      367 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/analysis.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/balsamic/__init__.py
--rw-r--r--   0        0        0      459 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/balsamic/analysis.py
--rw-r--r--   0        0        0     4550 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/balsamic/config.py
--rw-r--r--   0        0        0     1986 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/balsamic/metrics.py
--rw-r--r--   0        0        0    17539 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/cg_config.py
--rw-r--r--   0        0        0     4302 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/compression_data.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/deliverables/__init__.py
--rw-r--r--   0        0        0     5213 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/deliverables/metric_deliverables.py
--rw-r--r--   0        0        0      243 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/delivery/delivery.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/demultiplex/__init__.py
--rw-r--r--   0        0        0    12040 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/demultiplex/run_parameters.py
--rw-r--r--   0        0        0      539 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/demultiplex/sbatch.py
--rw-r--r--   0        0        0     7006 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/downsample/downsample_data.py
--rw-r--r--   0        0        0      255 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/email.py
--rw-r--r--   0        0        0     1046 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/fastq.py
--rw-r--r--   0        0        0     2157 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/file_data.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/flow_cell/__init__.py
--rw-r--r--   0        0        0    10373 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/flow_cell/flow_cell.py
--rw-r--r--   0        0        0      317 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/flow_cell/utils.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/invoice/__init__.py
--rw-r--r--   0        0        0     1254 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/invoice/invoice.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/lims/__init__.py
--rw-r--r--   0        0        0     2019 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/lims/sample.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/mip/__init__.py
--rw-r--r--   0        0        0      337 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/mip/mip_analysis.py
--rw-r--r--   0        0        0     1564 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/mip/mip_config.py
--rw-r--r--   0        0        0     4696 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/mip/mip_metrics_deliverables.py
--rw-r--r--   0        0        0     2550 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/mip/mip_sample_info.py
--rw-r--r--   0        0        0     2472 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/nf_analysis.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/observations/__init__.py
--rw-r--r--   0        0        0      688 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/observations/input_files.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/orders/__init__.py
--rw-r--r--   0        0        0     2659 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/orders/constants.py
--rw-r--r--   0        0        0     5604 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/orders/excel_sample.py
--rw-r--r--   0        0        0      898 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/orders/json_sample.py
--rw-r--r--   0        0        0     1449 2024-04-24 09:24:14.212206 cg-60.3.0/cg/models/orders/order.py
--rw-r--r--   0        0        0      811 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/orders/orderform_schema.py
--rw-r--r--   0        0        0     4212 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/orders/sample_base.py
--rw-r--r--   0        0        0     9668 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/orders/samples.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/orders/validators/__init__.py
--rw-r--r--   0        0        0     2300 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/orders/validators/excel_sample_validators.py
--rw-r--r--   0        0        0      576 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/orders/validators/json_sample_validators.py
--rw-r--r--   0        0        0       71 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/orders/validators/sample_base_validators.py
--rw-r--r--   0        0        0      101 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/qc_metrics.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/raredisease/__init__.py
--rw-r--r--   0        0        0     1875 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/raredisease/raredisease.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/report/__init__.py
--rw-r--r--   0        0        0     7461 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/report/metadata.py
--rw-r--r--   0        0        0     6180 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/report/report.py
--rw-r--r--   0        0        0     5221 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/report/sample.py
--rw-r--r--   0        0        0     3004 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/report/validators.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/rnafusion/__init__.py
--rw-r--r--   0        0        0     1865 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/rnafusion/rnafusion.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/scout/__init__.py
--rw-r--r--   0        0        0     4783 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/scout/scout_load_config.py
--rw-r--r--   0        0        0      116 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/scout/validators.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/slurm/__init__.py
--rw-r--r--   0        0        0      617 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/slurm/sbatch.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/taxprofiler/__init__.py
--rw-r--r--   0        0        0     2443 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/taxprofiler/taxprofiler.py
--rw-r--r--   0        0        0     1774 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/tomte/tomte.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/workflow/__init__.py
--rw-r--r--   0        0        0      685 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/workflow/mutant.py
--rw-r--r--   0        0        0       70 2024-04-24 09:24:14.216206 cg-60.3.0/cg/models/workflow/validators.py
--rw-r--r--   0        0        0      842 2024-04-24 09:24:14.216206 cg-60.3.0/cg/resources/__init__.py
--rw-r--r--   0        0        0     3493 2024-04-24 09:24:14.216206 cg-60.3.0/cg/resources/rnafusion_bundle_filenames.yaml
--rw-r--r--   0        0        0     2434 2024-04-24 09:24:14.216206 cg-60.3.0/cg/resources/taxprofiler_bundle_filenames.yaml
--rw-r--r--   0        0        0     3732 2024-04-24 09:24:14.216206 cg-60.3.0/cg/resources/tomte_bundle_filenames.yaml
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/__init__.py
--rw-r--r--   0        0        0    20241 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/admin.py
--rw-r--r--   0        0        0    22743 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/api.py
--rw-r--r--   0        0        0     4887 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/app.py
--rw-r--r--   0        0        0       48 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/auto.py
--rw-r--r--   0        0        0     1184 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/config.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/dto/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/dto/delivery_message/__init__.py
--rw-r--r--   0        0        0      300 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/dto/delivery_message/delivery_message_request.py
--rw-r--r--   0        0        0      183 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/dto/delivery_message/delivery_message_response.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/dto/orders/__init__.py
--rw-r--r--   0        0        0      165 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/dto/orders/order_delivery_update_request.py
--rw-r--r--   0        0        0       91 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/dto/orders/order_patch_request.py
--rw-r--r--   0        0        0      662 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/dto/orders/orders_request.py
--rw-r--r--   0        0        0      413 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/dto/orders/orders_response.py
--rw-r--r--   0        0        0     2598 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/ext.py
--rw-r--r--   0        0        0       29 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/invoices/__init__.py
--rw-r--r--   0        0        0     4793 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/invoices/templates/invoices/index.html
--rw-r--r--   0        0        0     8171 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/invoices/templates/invoices/invoice.html
--rw-r--r--   0        0        0     2838 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/invoices/templates/invoices/layout.html
--rw-r--r--   0        0        0     4956 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/invoices/templates/invoices/new.html
--rw-r--r--   0        0        0     7708 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/invoices/views.py
--rw-r--r--   0        0        0      354 2024-04-24 09:24:14.216206 cg-60.3.0/cg/server/templates/admin/index.html
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/analysis_service/__init__.py
--rw-r--r--   0        0        0      482 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/analysis_service/analysis_service.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/delivery_message/__init__.py
--rw-r--r--   0        0        0     2531 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/delivery_message/delivery_message_service.py
--rw-r--r--   0        0        0      792 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/delivery_message/messages/__init__.py
--rw-r--r--   0        0        0     1366 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/delivery_message/messages/analysis_scout_message.py
--rw-r--r--   0        0        0      791 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/delivery_message/messages/covid_message.py
--rw-r--r--   0        0        0      189 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/delivery_message/messages/delivery_message.py
--rw-r--r--   0        0        0     1391 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/delivery_message/messages/fastq_analysis_scout_message.py
--rw-r--r--   0        0        0      535 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/delivery_message/messages/fastq_message.py
--rw-r--r--   0        0        0     1358 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/delivery_message/messages/fastq_scout_message.py
--rw-r--r--   0        0        0      604 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/delivery_message/messages/microsalt_mwr_message.py
--rw-r--r--   0        0        0      592 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/delivery_message/messages/microsalt_mwx_message.py
--rw-r--r--   0        0        0      903 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/delivery_message/messages/scout_message.py
--rw-r--r--   0        0        0      512 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/delivery_message/messages/statina_message.py
--rw-r--r--   0        0        0      779 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/delivery_message/messages/utils.py
--rw-r--r--   0        0        0     3300 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/delivery_message/utils.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/fastq_file_service/__init__.py
--rw-r--r--   0        0        0      101 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/fastq_file_service/exceptions.py
--rw-r--r--   0        0        0     1092 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/fastq_file_service/fastq_file_service.py
--rw-r--r--   0        0        0     2991 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/fastq_file_service/utils.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/orders/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/orders/order_service/__init__.py
--rw-r--r--   0        0        0     2684 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/orders/order_service/order_service.py
--rw-r--r--   0        0        0     1214 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/orders/order_service/utils.py
--rw-r--r--   0        0        0       94 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/orders/order_status_service/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/orders/order_status_service/dto/__init__.py
--rw-r--r--   0        0        0      192 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/orders/order_status_service/dto/case_summary.py
--rw-r--r--   0        0        0      289 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/orders/order_status_service/dto/order_summary.py
--rw-r--r--   0        0        0     1768 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/orders/order_status_service/order_summary_service.py
--rw-r--r--   0        0        0     1737 2024-04-24 09:24:14.216206 cg-60.3.0/cg/services/orders/order_status_service/utils.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.220206 cg-60.3.0/cg/services/slurm_service/__init__.py
--rw-r--r--   0        0        0      703 2024-04-24 09:24:14.220206 cg-60.3.0/cg/services/slurm_service/slurm_cli_service.py
--rw-r--r--   0        0        0      242 2024-04-24 09:24:14.220206 cg-60.3.0/cg/services/slurm_service/slurm_service.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.220206 cg-60.3.0/cg/services/slurm_upload_service/__init__.py
--rw-r--r--   0        0        0      175 2024-04-24 09:24:14.220206 cg-60.3.0/cg/services/slurm_upload_service/slurm_upload_config.py
--rw-r--r--   0        0        0     2074 2024-04-24 09:24:14.220206 cg-60.3.0/cg/services/slurm_upload_service/slurm_upload_service.py
--rw-r--r--   0        0        0      203 2024-04-24 09:24:14.220206 cg-60.3.0/cg/services/slurm_upload_service/utils.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/__init__.py
--rw-r--r--   0        0        0     4650 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/base.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/crud/__init__.py
--rw-r--r--   0        0        0    13100 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/crud/create.py
--rw-r--r--   0        0        0     2144 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/crud/delete.py
--rw-r--r--   0        0        0    60188 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/crud/read.py
--rw-r--r--   0        0        0     1121 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/crud/update.py
--rw-r--r--   0        0        0     1662 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/database.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/filters/__init__.py
--rw-r--r--   0        0        0     5371 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/filters/status_analysis_filters.py
--rw-r--r--   0        0        0     1712 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/filters/status_application_filters.py
--rw-r--r--   0        0        0     1440 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/filters/status_application_limitations_filters.py
--rw-r--r--   0        0        0     2523 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/filters/status_application_version_filters.py
--rw-r--r--   0        0        0     1390 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/filters/status_bed_filters.py
--rw-r--r--   0        0        0     1317 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/filters/status_bed_version_filters.py
--rw-r--r--   0        0        0    10787 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/filters/status_case_filters.py
--rw-r--r--   0        0        0     3272 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/filters/status_case_sample_filters.py
--rw-r--r--   0        0        0      903 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/filters/status_collaboration_filters.py
--rw-r--r--   0        0        0     1412 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/filters/status_customer_filters.py
--rw-r--r--   0        0        0     1880 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/filters/status_flow_cell_filters.py
--rw-r--r--   0        0        0     1255 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/filters/status_invoice_filters.py
--rw-r--r--   0        0        0     2792 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/filters/status_metrics_filters.py
--rw-r--r--   0        0        0     3225 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/filters/status_order_filters.py
--rw-r--r--   0        0        0      851 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/filters/status_organism_filters.py
--rw-r--r--   0        0        0      783 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/filters/status_panel_filters.py
--rw-r--r--   0        0        0     3923 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/filters/status_pool_filters.py
--rw-r--r--   0        0        0     8660 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/filters/status_sample_filters.py
--rw-r--r--   0        0        0      731 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/filters/status_user_filters.py
--rw-r--r--   0        0        0    36844 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/models.py
--rw-r--r--   0        0        0      593 2024-04-24 09:24:14.220206 cg-60.3.0/cg/store/store.py
--rw-r--r--   0        0        0       30 2024-04-24 09:24:14.220206 cg-60.3.0/cg/utils/__init__.py
--rw-r--r--   0        0        0      187 2024-04-24 09:24:14.220206 cg-60.3.0/cg/utils/calculations.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.220206 cg-60.3.0/cg/utils/checksum/__init__.py
--rw-r--r--   0        0        0     1579 2024-04-24 09:24:14.220206 cg-60.3.0/cg/utils/checksum/checksum.py
--rw-r--r--   0        0        0     1655 2024-04-24 09:24:14.220206 cg-60.3.0/cg/utils/click/EnumChoice.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.220206 cg-60.3.0/cg/utils/click/__init__.py
--rw-r--r--   0        0        0     4910 2024-04-24 09:24:14.220206 cg-60.3.0/cg/utils/commands.py
--rw-r--r--   0        0        0     1811 2024-04-24 09:24:14.220206 cg-60.3.0/cg/utils/date.py
--rw-r--r--   0        0        0      635 2024-04-24 09:24:14.220206 cg-60.3.0/cg/utils/dict.py
--rw-r--r--   0        0        0     2111 2024-04-24 09:24:14.220206 cg-60.3.0/cg/utils/dispatcher.py
--rw-r--r--   0        0        0     1251 2024-04-24 09:24:14.220206 cg-60.3.0/cg/utils/email.py
--rw-r--r--   0        0        0      134 2024-04-24 09:24:14.220206 cg-60.3.0/cg/utils/enums.py
--rw-r--r--   0        0        0     3178 2024-04-24 09:24:14.220206 cg-60.3.0/cg/utils/files.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.220206 cg-60.3.0/cg/utils/flask/__init__.py
--rw-r--r--   0        0        0     1052 2024-04-24 09:24:14.220206 cg-60.3.0/cg/utils/flask/enum.py
--rw-r--r--   0        0        0      233 2024-04-24 09:24:14.220206 cg-60.3.0/cg/utils/flow_cell.py
--rw-r--r--   0        0        0      834 2024-04-24 09:24:14.220206 cg-60.3.0/cg/utils/time.py
--rw-r--r--   0        0        0     1224 2024-04-24 09:24:14.220206 cg-60.3.0/cg/utils/utils.py
--rw-r--r--   0        0        0     1697 2024-04-24 09:24:14.224206 cg-60.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.224206 cg-60.3.0/tests/__init__.py
--rw-r--r--   0        0        0     1158 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/conftest.py
--rw-r--r--   0        0        0      231 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/coverage/conftest.py
--rw-r--r--   0        0        0     6188 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/coverage/test_coverage.py
--rw-r--r--   0        0        0     1693 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/crunchy/conftest.py
--rw-r--r--   0        0        0     5438 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/crunchy/test_compress_fastq.py
--rw-r--r--   0        0        0     2283 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/crunchy/test_config.py
--rw-r--r--   0        0        0    14032 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/crunchy/test_crunchy.py
--rw-r--r--   0        0        0     9109 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/crunchy/test_spring_decompression.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/demultiplex/__init__.py
--rw-r--r--   0        0        0    10893 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/demultiplex/conftest.py
--rw-r--r--   0        0        0     4040 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0        0        0     7986 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/demultiplex/test_demultiplex_api.py
--rw-r--r--   0        0        0     5729 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/demultiplex/test_index.py
--rw-r--r--   0        0        0     9468 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/demultiplex/test_override_cycles_validator.py
--rw-r--r--   0        0        0     5290 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/demultiplex/test_read_sample_sheet.py
--rw-r--r--   0        0        0    15738 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/demultiplex/test_sample_models.py
--rw-r--r--   0        0        0     1050 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/demultiplex/test_sample_sheet_creator.py
--rw-r--r--   0        0        0     3245 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/demultiplex/test_sample_sheet_models.py
--rw-r--r--   0        0        0    10932 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/demultiplex/test_sample_sheet_validator.py
--rw-r--r--   0        0        0     7037 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/demultiplex/test_translate_sample_sheet.py
--rw-r--r--   0        0        0     1495 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/demultiplex/test_validate.py
--rw-r--r--   0        0        0     5094 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/downsample/test_downsample.py
--rw-r--r--   0        0        0     1419 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/downsample/test_downsample_utils.py
--rw-r--r--   0        0        0     1716 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/gens/test_gens_api.py
--rw-r--r--   0        0        0     1950 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/gt/conftest.py
--rw-r--r--   0        0        0     4276 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/gt/test_gt_api.py
--rw-r--r--   0        0        0     1453 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/hk/conftest.py
--rw-r--r--   0        0        0      684 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/hk/test__getattr__.py
--rw-r--r--   0        0        0     1593 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/hk/test_add_file.py
--rw-r--r--   0        0        0     3523 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/hk/test_bundles.py
--rw-r--r--   0        0        0      871 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/hk/test_core.py
--rw-r--r--   0        0        0    31172 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/hk/test_file.py
--rw-r--r--   0        0        0     5080 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/hk/test_version.py
--rw-r--r--   0        0        0     1840 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/lims/conftest.py
--rw-r--r--   0        0        0     3197 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/lims/test_api.py
--rw-r--r--   0        0        0     1451 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/lims/test_sample_sheet.py
--rw-r--r--   0        0        0     9223 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/loqus/conftest.py
--rw-r--r--   0        0        0     8994 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/loqus/test_loqusdb_api.py
--rw-r--r--   0        0        0     2439 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/madeline/conftest.py
--rw-r--r--   0        0        0     4653 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/madeline/test_madeline.py
--rw-r--r--   0        0        0     3328 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/mip/conftest.py
--rw-r--r--   0        0        0     2487 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/mip/test_config_mip.py
--rw-r--r--   0        0        0      883 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/mutacc_auto/conftest.py
--rw-r--r--   0        0        0     2473 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/mutacc_auto/test_mutacc_auto.py
--rw-r--r--   0        0        0    11930 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/orderform/conftest.py
--rw-r--r--   0        0        0     9484 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/orderform/test_excel_orderform_parser.py
--rw-r--r--   0        0        0     4351 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/orderform/test_excel_sample_schema.py
--rw-r--r--   0        0        0     1032 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/orderform/test_json_orderform_parser.py
--rw-r--r--   0        0        0     2474 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/orderform/test_orderform_parser.py
--rw-r--r--   0        0        0    16002 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/orderform/validators/test_excel_sample_validators.py
--rw-r--r--   0        0        0     3670 2024-04-24 09:24:14.224206 cg-60.3.0/tests/apps/scout/conftest.py
--rw-r--r--   0        0        0     2269 2024-04-24 09:24:14.228206 cg-60.3.0/tests/apps/scout/test_get_causative_variants.py
--rw-r--r--   0        0        0     1376 2024-04-24 09:24:14.228206 cg-60.3.0/tests/apps/scout/test_get_scout_cases.py
--rw-r--r--   0        0        0     1840 2024-04-24 09:24:14.228206 cg-60.3.0/tests/apps/scout/test_scout_load_config.py
--rw-r--r--   0        0        0     7047 2024-04-24 09:24:14.228206 cg-60.3.0/tests/apps/scout/test_scout_models.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.228206 cg-60.3.0/tests/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0        0        0     2639 2024-04-24 09:24:14.228206 cg-60.3.0/tests/apps/sequencing_metrics_parser/conftest.py
--rw-r--r--   0        0        0     2010 2024-04-24 09:24:14.228206 cg-60.3.0/tests/apps/sequencing_metrics_parser/parsers/conftest.py
--rw-r--r--   0        0        0     7105 2024-04-24 09:24:14.228206 cg-60.3.0/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
--rw-r--r--   0        0        0     3030 2024-04-24 09:24:14.228206 cg-60.3.0/tests/apps/sequencing_metrics_parser/parsers/test_sequencing_metrics_parser_api.py
--rw-r--r--   0        0        0     1131 2024-04-24 09:24:14.228206 cg-60.3.0/tests/apps/slurm/conftest.py
--rw-r--r--   0        0        0     4412 2024-04-24 09:24:14.228206 cg-60.3.0/tests/apps/slurm/test_slurm_api.py
--rw-r--r--   0        0        0      831 2024-04-24 09:24:14.228206 cg-60.3.0/tests/apps/test_apps_environ.py
--rw-r--r--   0        0        0      957 2024-04-24 09:24:14.228206 cg-60.3.0/tests/apps/test_osticket.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/add/__init__.py
--rw-r--r--   0        0        0     1174 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/add/test_cli_add.py
--rw-r--r--   0        0        0     2471 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/add/test_cli_add_customer.py
--rw-r--r--   0        0        0     6841 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/add/test_cli_add_family.py
--rw-r--r--   0        0        0     7588 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/add/test_cli_add_relationship.py
--rw-r--r--   0        0        0     8382 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/add/test_cli_add_sample.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/backup/__init__.py
--rw-r--r--   0        0        0      705 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/backup/conftest.py
--rw-r--r--   0        0        0    11101 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/backup/test_backup_command.py
--rw-r--r--   0        0        0     6865 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/clean/conftest.py
--rw-r--r--   0        0        0     5536 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/clean/test_balsamic_clean.py
--rw-r--r--   0        0        0     2557 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/clean/test_clean_flow_cell.py
--rw-r--r--   0        0        0     1830 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/clean/test_clean_hk_bundle_files.py
--rw-r--r--   0        0        0     2098 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/clean/test_hk_bundle_files.py
--rw-r--r--   0        0        0     4610 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/clean/test_hk_case_bundle_files.py
--rw-r--r--   0        0        0     3585 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/clean/test_microbial_clean.py
--rw-r--r--   0        0        0     1881 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/clean/test_rsync_past_run_dirs.py
--rw-r--r--   0        0        0     9707 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/compress/conftest.py
--rw-r--r--   0        0        0     7709 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/compress/test_cli_compress_fastq.py
--rw-r--r--   0        0        0     1416 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/compress/test_cli_decompress_spring.py
--rw-r--r--   0        0        0     5205 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/compress/test_compress_helpers.py
--rw-r--r--   0        0        0     1239 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/compress/test_store_fastq.py
--rw-r--r--   0        0        0     7558 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/conftest.py
--rw-r--r--   0        0        0    12747 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/delete/test_cli_delete_case.py
--rw-r--r--   0        0        0     1873 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/delete/test_cli_delete_cases.py
--rw-r--r--   0        0        0     3794 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/deliver/conftest.py
--rw-r--r--   0        0        0     4428 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/deliver/test_deliver_base.py
--rw-r--r--   0        0        0     1166 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/deliver/test_rsync_base.py
--rw-r--r--   0        0        0     8569 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/deliver/test_run_deliver_cmd.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/demultiplex/__init__.py
--rw-r--r--   0        0        0     5129 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0        0        0     4773 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/demultiplex/test_demultiplex_flowcell.py
--rw-r--r--   0        0        0     1607 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/demultiplex/test_finish_demux.py
--rw-r--r--   0        0        0     2989 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/demultiplex/test_validate_sample_sheet.py
--rw-r--r--   0        0        0     4423 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/demultiplex/test_verify_syncing.py
--rw-r--r--   0        0        0     1585 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/downsample/test_cli_downsample.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/generate/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/generate/report/__init__.py
--rw-r--r--   0        0        0     1622 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/generate/report/conftest.py
--rw-r--r--   0        0        0     2477 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/generate/report/test_cli_delivery_report.py
--rw-r--r--   0        0        0     2760 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/generate/report/test_utils.py
--rw-r--r--   0        0        0      563 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/generate/test_cli_base.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/get/__init__.py
--rw-r--r--   0        0        0      863 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/get/test_cli_get.py
--rw-r--r--   0        0        0     1526 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/get/test_cli_get_analysis.py
--rw-r--r--   0        0        0     1242 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/get/test_cli_get_case.py
--rw-r--r--   0        0        0     6208 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/get/test_cli_get_flow_cell.py
--rw-r--r--   0        0        0     8835 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/get/test_cli_get_sample.py
--rw-r--r--   0        0        0     1364 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/set/conftest.py
--rw-r--r--   0        0        0     7311 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/set/test_cli_set_case.py
--rw-r--r--   0        0        0     1460 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/set/test_cli_set_cases.py
--rw-r--r--   0        0        0     2016 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/set/test_cli_set_flowcell.py
--rw-r--r--   0        0        0     1685 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/set/test_cli_set_list_keys.py
--rw-r--r--   0        0        0    12450 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/set/test_cli_set_sample.py
--rw-r--r--   0        0        0     6124 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/set/test_cli_set_samples.py
--rw-r--r--   0        0        0     6934 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/store/test_store.py
--rw-r--r--   0        0        0     2332 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/test_base.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/upload/__init__.py
--rw-r--r--   0        0        0    10057 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/upload/conftest.py
--rw-r--r--   0        0        0     2295 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/upload/test_cli_scout.py
--rw-r--r--   0        0        0     1789 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/upload/test_cli_upload.py
--rw-r--r--   0        0        0      971 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/upload/test_cli_upload_auto.py
--rw-r--r--   0        0        0     1669 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/upload/test_cli_upload_delivery_report.py
--rw-r--r--   0        0        0      895 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/upload/test_cli_upload_fastq.py
--rw-r--r--   0        0        0     1199 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/upload/test_cli_upload_genotype.py
--rw-r--r--   0        0        0      694 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/upload/test_cli_upload_gens.py
--rw-r--r--   0        0        0     9965 2024-04-24 09:24:14.228206 cg-60.3.0/tests/cli/upload/test_cli_upload_nipt.py
--rw-r--r--   0        0        0     4684 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/upload/test_cli_upload_nipt_ftp.py
--rw-r--r--   0        0        0     1839 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/upload/test_cli_upload_nipt_statina.py
--rw-r--r--   0        0        0     6177 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/upload/test_cli_upload_observations.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/__init__.py
--rw-r--r--   0        0        0    30612 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/balsamic/conftest.py
--rw-r--r--   0        0        0    13938 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
--rw-r--r--   0        0        0     7957 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/balsamic/test_compound_commands.py
--rw-r--r--   0        0        0     2336 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/balsamic/test_link.py
--rw-r--r--   0        0        0     3554 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/balsamic/test_report_deliver.py
--rw-r--r--   0        0        0     6209 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/balsamic/test_run.py
--rw-r--r--   0        0        0     6934 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/balsamic/test_store_housekeeper.py
--rw-r--r--   0        0        0     8458 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/conftest.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/fastq/__init__.py
--rw-r--r--   0        0        0     2298 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/fastq/test_fastq_base.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/fluffy/__init__.py
--rw-r--r--   0        0        0     5291 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/fluffy/conftest.py
--rw-r--r--   0        0        0     5687 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
--rw-r--r--   0        0        0     3302 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/fluffy/test_cli_link.py
--rw-r--r--   0        0        0     1896 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/fluffy/test_cli_run.py
--rw-r--r--   0        0        0     2968 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/fluffy/test_cli_start.py
--rw-r--r--   0        0        0     7815 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/fluffy/test_cli_store.py
--rw-r--r--   0        0        0     2775 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/microsalt/conftest.py
--rw-r--r--   0        0        0     6926 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/microsalt/test_microsalt_case_config.py
--rw-r--r--   0        0        0     1000 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/microsalt/test_microsalt_run.py
--rw-r--r--   0        0        0     6544 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/mip/conftest.py
--rw-r--r--   0        0        0     7011 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/mip/test_cli_mip_base.py
--rw-r--r--   0        0        0     1542 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
--rw-r--r--   0        0        0      431 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/mip/test_cli_mip_dna_link.py
--rw-r--r--   0        0        0     2108 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py
--rw-r--r--   0        0        0     1273 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
--rw-r--r--   0        0        0     3595 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/mip/test_cli_mip_dna_run.py
--rw-r--r--   0        0        0     3884 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/mip/test_cli_mip_dna_start.py
--rw-r--r--   0        0        0     1004 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
--rw-r--r--   0        0        0      527 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/mip/test_cli_mip_rna_link.py
--rw-r--r--   0        0        0      716 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/mip/test_cli_mip_rna_run.py
--rw-r--r--   0        0        0     8559 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/mip/test_cli_mip_store.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/nf_analysis/__init__.py
--rw-r--r--   0        0        0     7365 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/nf_analysis/test_cli_config_case.py
--rw-r--r--   0        0        0     3831 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py
--rw-r--r--   0        0        0     5087 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py
--rw-r--r--   0        0        0     9211 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/nf_analysis/test_cli_run.py
--rw-r--r--   0        0        0     2994 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/nf_analysis/test_cli_start.py
--rw-r--r--   0        0        0     9877 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/nf_analysis/test_cli_store.py
--rw-r--r--   0        0        0    10373 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py
--rw-r--r--   0        0        0      978 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/raredisease/__init__.py
--rw-r--r--   0        0        0     3940 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py
--rw-r--r--   0        0        0      921 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/test_cli_workflow.py
--rw-r--r--   0        0        0     4310 2024-04-24 09:24:14.232206 cg-60.3.0/tests/cli/workflow/test_cli_workflow_clean.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.232206 cg-60.3.0/tests/clients/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.232206 cg-60.3.0/tests/clients/arnold/__init__.py
--rw-r--r--   0        0        0     1080 2024-04-24 09:24:14.232206 cg-60.3.0/tests/clients/arnold/conftest.py
--rw-r--r--   0        0        0     1503 2024-04-24 09:24:14.232206 cg-60.3.0/tests/clients/arnold/test_arnold_api_client.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.232206 cg-60.3.0/tests/clients/janus/__init__.py
--rw-r--r--   0        0        0     2381 2024-04-24 09:24:14.232206 cg-60.3.0/tests/clients/janus/conftest.py
--rw-r--r--   0        0        0     1716 2024-04-24 09:24:14.232206 cg-60.3.0/tests/clients/janus/test_janus_api_client.py
--rw-r--r--   0        0        0   133089 2024-04-24 09:24:14.232206 cg-60.3.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.232206 cg-60.3.0/tests/fixture_plugins/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.232206 cg-60.3.0/tests/fixture_plugins/delivery_fixtures/__init__.py
--rw-r--r--   0        0        0     2653 2024-04-24 09:24:14.232206 cg-60.3.0/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py
--rw-r--r--   0        0        0     4972 2024-04-24 09:24:14.232206 cg-60.3.0/tests/fixture_plugins/delivery_fixtures/context_fixtures.py
--rw-r--r--   0        0        0     1494 2024-04-24 09:24:14.232206 cg-60.3.0/tests/fixture_plugins/delivery_fixtures/path_fixtures.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.232206 cg-60.3.0/tests/fixture_plugins/demultiplex_fixtures/__init__.py
--rw-r--r--   0        0        0     4702 2024-04-24 09:24:14.232206 cg-60.3.0/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py
--rw-r--r--   0        0        0     6152 2024-04-24 09:24:14.232206 cg-60.3.0/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py
--rw-r--r--   0        0        0    22442 2024-04-24 09:24:14.232206 cg-60.3.0/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py
--rw-r--r--   0        0        0     3699 2024-04-24 09:24:14.232206 cg-60.3.0/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py
--rw-r--r--   0        0        0     6160 2024-04-24 09:24:14.232206 cg-60.3.0/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py
--rw-r--r--   0        0        0     6514 2024-04-24 09:24:14.232206 cg-60.3.0/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py
--rw-r--r--   0        0        0     1304 2024-04-24 09:24:14.232206 cg-60.3.0/tests/fixture_plugins/timestamp_fixtures.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.232206 cg-60.3.0/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.232206 cg-60.3.0/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.232206 cg-60.3.0/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.232206 cg-60.3.0/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
--rw-r--r--   0        0        0    14644 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
--rw-r--r--   0        0        0    15921 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/mip/dna/ADM2.cram
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/mip/dna/ADM3.cram
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/mip/dna/adm1.cram
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/mip/dna/adm1.mt.bam
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/mip/dna/multiqc.html
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/mip/dna/report.pdf
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/mip/dna/smn.vcf
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/mip/dna/snv.vcf
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/mip/dna/snv_research.vcf
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/mip/dna/str.vcf
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/mip/dna/sv.vcf
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/mip/dna/sv_research.vcf
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
--rw-r--r--   0        0        0       70 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/nf-analysis/pipeline_params.config
--rw-r--r--   0        0        0      195 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/nf-analysis/pipeline_resource_optimisation.config
--rw-r--r--   0        0        0      195 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/nf-analysis/platform.config
--rw-r--r--   0        0        0     8173 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/raredisease/multiqc_data.json
--rw-r--r--   0        0        0    20005 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml
--rw-r--r--   0        0        0     5497 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/rnafusion/multiqc_data.json
--rw-r--r--   0        0        0    12499 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml
--rw-r--r--   0        0        0     2873 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/sample_coverage.bed
--rw-r--r--   0        0        0     6506 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/taxprofiler/multiqc_data.json
--rw-r--r--   0        0        0    10513 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml
--rw-r--r--   0        0        0     5771 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/tomte/multiqc_data.json
--rw-r--r--   0        0        0    14859 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml
--rw-r--r--   0        0        0    10961 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/balsamic/case/config.json
--rw-r--r--   0        0        0     3465 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/balsamic/case/metadata.yml
--rw-r--r--   0        0        0       63 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/balsamic/case/metadata_directory.yml
--rw-r--r--   0        0        0      165 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
--rw-r--r--   0        0        0     2705 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
--rw-r--r--   0        0        0      692 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/crunchy/spring_metadata.json
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0      412 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      484 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      658 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/demuxcomplete.txt
--rw-r--r--   0        0        0     1757 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0        0        0        7 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0     6034 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0        0        0     1172 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0        0        0        7 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_1.fastq.gz
--rw-r--r--   0        0        0        7 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_2.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0      345 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      650 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      896 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0      602 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/demuxcomplete.txt
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0      288 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      361 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      414 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/demuxcomplete.txt
--rw-r--r--   0        0        0      315 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      434 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0     8624 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml
--rw-r--r--   0        0        0      568 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0      220 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      463 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      622 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0      345 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      650 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      896 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0      619 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0      303 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      364 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      427 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/demuxcomplete.txt
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0     4439 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0        0        0     1172 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0     5127 2024-04-24 09:24:14.236206 cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
--rw-r--r--   0        0        0       43 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz
--rw-r--r--   0        0        0       67 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz.md5
--rw-r--r--   0        0        0   338370 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz
--rw-r--r--   0        0        0       67 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz.md5
--rw-r--r--   0        0        0   338349 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/CopyComplete.txt
--rw-r--r--   0        0        0     2126 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json
--rw-r--r--   0        0        0     1827 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json
--rw-r--r--   0        0        0       90 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/README.txt
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAComplete.txt
--rw-r--r--   0        0        0     6895 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml
--rw-r--r--   0        0        0       37 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead1Complete.txt
--rw-r--r--   0        0        0       36 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead2Complete.txt
--rw-r--r--   0        0        0       36 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead3Complete.txt
--rw-r--r--   0        0        0    24755 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml
--rw-r--r--   0        0        0      692 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
--rw-r--r--   0        0        0      724 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0       61 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SequencingComplete.txt
--rw-r--r--   0        0        0     5775 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/CopyComplete.txt
--rw-r--r--   0        0        0     2282 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json
--rw-r--r--   0        0        0     1632 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json
--rw-r--r--   0        0        0       75 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/README.txt
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAComplete.txt
--rw-r--r--   0        0        0     6912 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml
--rw-r--r--   0        0        0       36 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead1Complete.txt
--rw-r--r--   0        0        0       36 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead2Complete.txt
--rw-r--r--   0        0        0       36 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead3Complete.txt
--rw-r--r--   0        0        0       36 2024-04-24 09:24:14.240206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead4Complete.txt
--rw-r--r--   0        0        0    24814 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml
--rw-r--r--   0        0        0      814 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv
--rw-r--r--   0        0        0      660 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0       61 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SequencingComplete.txt
--rw-r--r--   0        0        0     5853 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/CopyComplete.txt
--rw-r--r--   0        0        0    21848 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json
--rw-r--r--   0        0        0    15512 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json
--rw-r--r--   0        0        0       79 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/README.txt
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RTAComplete.txt
--rw-r--r--   0        0        0      756 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml
--rw-r--r--   0        0        0     4118 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv
--rw-r--r--   0        0        0     1408 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0     5326 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/CopyComplete.txt
--rw-r--r--   0        0        0    15041 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json
--rw-r--r--   0        0        0    10649 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json
--rw-r--r--   0        0        0       80 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/README.txt
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RTAComplete.txt
--rw-r--r--   0        0        0      755 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml
--rw-r--r--   0        0        0     2878 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv
--rw-r--r--   0        0        0      928 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0     5359 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CopyComplete.txt
--rw-r--r--   0        0        0    27887 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv
--rw-r--r--   0        0        0   141870 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json
--rwxr-xr-x   0        0        0   122682 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json
--rw-r--r--   0        0        0      243 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/README.txt
--rw-r--r--   0        0        0    28230 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTAComplete.txt
--rw-r--r--   0        0        0    94426 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml
--rw-r--r--   0        0        0     5819 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/SequenceComplete.txt
--rw-r--r--   0        0        0     1757 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0        0        0     1757 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stdout
--rw-r--r--   0        0        0       12 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/README.txt
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RTAComplete.txt
--rw-r--r--   0        0        0     5945 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml
--rw-r--r--   0        0        0      260 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/copycomplete.txt
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/demuxstarted.txt
--rw-r--r--   0        0        0     1757 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0        0        0     1757 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout
--rw-r--r--   0        0        0    47522 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json
--rw-r--r--   0        0        0       12 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/README.txt
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0        0        0     6666 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0        0        0      254 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/copycomplete.txt
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/delivery.txt
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/demuxstarted.txt
--rwxr-xr-x   0        0        0    47434 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CopyComplete.txt
--rw-r--r--   0        0        0    10950 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv
--rw-r--r--   0        0        0      225 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/Manifest.tsv
--rw-r--r--   0        0        0       55 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/README.txt
--rwxr-xr-x   0        0        0     2493 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg
--rwxr-xr-x   0        0        0        1 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAComplete.txt
--rwxr-xr-x   0        0        0        2 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAExited.txt
--rwxr-xr-x   0        0        0      730 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml
--rwxr-xr-x   0        0        0    79277 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml
--rwxr-xr-x   0        0        0     2694 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
--rw-r--r--   0        0        0    10950 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
--rw-r--r--   0        0        0      619 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0        0        0       12 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/README.txt
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-04-24 09:24:14.244206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0        0        0      399 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CopyComplete.txt
--rw-r--r--   0        0        0     4941 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv
--rwxr-xr-x   0        0        0    20050 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stderr
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stdout
--rw-r--r--   0        0        0      244 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/README.txt
--rw-r--r--   0        0        0     6391 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTAComplete.txt
--rw-r--r--   0        0        0    16428 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml
--rw-r--r--   0        0        0     6728 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
--rw-r--r--   0        0        0     5127 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SequenceComplete.txt
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/demuxstarted.txt
--rw-r--r--   0        0        0      133 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/README.txt
--rw-r--r--   0        0        0      724 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
--rw-r--r--   0        0        0     5775 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
--rw-r--r--   0        0        0      124 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/180509_D00450_0598_BHGYFNBCX2/README.txt
--rw-r--r--   0        0        0      310 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/README.txt
--rw-r--r--   0        0        0     5819 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
--rw-r--r--   0        0        0      122 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/README.txt
--rwxr-xr-x   0        0        0     2694 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
--rw-r--r--   0        0        0      311 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/README.txt
--rw-r--r--   0        0        0     6728 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0        0        0      399 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
--rw-r--r--   0        0        0      399 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_0.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_1.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/final_summary_PAS86456_72d9fceb_8a4fd683.txt
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_0.pod5
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_1.pod5
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_0.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_1.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/final_summary_PAS97781_595b5663_efc7f02e.txt
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_0.pod5
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_1.pod5
--rw-r--r--   0        0        0   111989 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
--rw-r--r--   0        0        0     5319 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml
--rw-r--r--   0        0        0     5944 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
--rwxr-xr-x   0        0        0     2481 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
--rwxr-xr-x   0        0        0     2474 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml
--rw-r--r--   0        0        0     5899 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
--rw-r--r--   0        0        0     4941 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv
--rw-r--r--   0        0        0    10950 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/spring/dummy_run_001.spring
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/spring/dummy_run_002.spring
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/demultiplexing/spring/dummy_spring_meta_data.json
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
--rw-r--r--   0        0        0     5554 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/fluffy/SampleSheet.csv
--rw-r--r--   0        0        0      901 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/fluffy/deliverables.yaml
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/fluffy/multiqc_report.html
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/fluffy/summary.csv
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/gt/yellowhog.bcf
--rw-r--r--   0        0        0     5114 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/madeline/madeline.xml
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/mip/case_file.txt
--rw-r--r--   0        0        0     3241 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
--rw-r--r--   0        0        0    21811 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/mip/dna/store/case_config.yaml
--rw-r--r--   0        0        0    23364 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
--rw-r--r--   0        0        0    37367 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
--rw-r--r--   0        0        0       16 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
--rw-r--r--   0        0        0       16 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
--rw-r--r--   0        0        0       16 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
--rw-r--r--   0        0        0      123 2024-04-24 09:24:14.248206 cg-60.3.0/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
--rw-r--r--   0        0        0    62741 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
--rw-r--r--   0        0        0    11242 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/apps/mip/rna/case_config.yaml
--rw-r--r--   0        0        0    12164 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
--rw-r--r--   0        0        0     5231 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
--rw-r--r--   0        0        0     9774 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/apps/mip/rna/store/case_config.yaml
--rw-r--r--   0        0        0     4624 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
--rw-r--r--   0        0        0    13666 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/apps/mip/sample_file.txt
--rw-r--r--   0        0        0     1885 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/apps/scout/643594.config.yaml
--rw-r--r--   0        0        0     6027 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/apps/scout/case_export.json
--rw-r--r--   0        0        0     9349 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/apps/scout/export_causatives.json
--rw-r--r--   0        0        0     1315 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/apps/scout/none_case_export.json
--rw-r--r--   0        0        0     3518 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/apps/scout/other_sex_case.json
--rw-r--r--   0        0        0     8874 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/apps/scout/panel_export.bed
--rw-r--r--   0        0        0     4169 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/apps/scout/panel_export.csv
--rw-r--r--   0        0        0      619 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/SampleSheet.csv
--rw-r--r--   0        0        0    63569 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0    42478 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0    69708 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0       42 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/apps/shipping/scout-deploy.yaml
--rw-r--r--   0        0        0     1036 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/cgweb_orders/balsamic.json
--rw-r--r--   0        0        0     1104 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/cgweb_orders/fastq.json
--rw-r--r--   0        0        0     1313 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/cgweb_orders/metagenome.json
--rw-r--r--   0        0        0     3038 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/cgweb_orders/microsalt.json
--rw-r--r--   0        0        0     3705 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/cgweb_orders/mip.json
--rw-r--r--   0        0        0     1364 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/cgweb_orders/mip_rna.json
--rw-r--r--   0        0        0     2125 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/cgweb_orders/rml.json
--rw-r--r--   0        0        0     1368 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/cgweb_orders/rnafusion.json
--rw-r--r--   0        0        0     4684 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/cgweb_orders/sarscov2.json
--rw-r--r--   0        0        0     5609 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/data/SampleSheet.csv
--rw-r--r--   0        0        0      511 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/data/bcl_convert_sample_sheet.csv
--rw-r--r--   0        0        0   258048 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/data/cgfixture.db
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.252206 cg-60.3.0/tests/fixtures/data/fastq.fastq.gz
--rw-r--r--   0        0        0    49152 2024-04-24 09:24:14.256206 cg-60.3.0/tests/fixtures/data/hkstore.db
--rw-r--r--   0        0        0       73 2024-04-24 09:24:14.256206 cg-60.3.0/tests/fixtures/data/yellowhog/pedigree.yaml
--rw-r--r--   0        0        0       76 2024-04-24 09:24:14.256206 cg-60.3.0/tests/fixtures/io/casava_five_parts.fastq.gz
--rw-r--r--   0        0        0       90 2024-04-24 09:24:14.256206 cg-60.3.0/tests/fixtures/io/casava_seven_parts.fastq.gz
--rw-r--r--   0        0        0       96 2024-04-24 09:24:14.256206 cg-60.3.0/tests/fixtures/io/casava_ten_parts.fastq.gz
--rw-r--r--   0        0        0      153 2024-04-24 09:24:14.256206 cg-60.3.0/tests/fixtures/io/example.csv
--rw-r--r--   0        0        0       46 2024-04-24 09:24:14.256206 cg-60.3.0/tests/fixtures/io/example.gz
--rw-r--r--   0        0        0      147 2024-04-24 09:24:14.256206 cg-60.3.0/tests/fixtures/io/example.tsv
--rw-r--r--   0        0        0       20 2024-04-24 09:24:14.256206 cg-60.3.0/tests/fixtures/io/example.txt
--rw-r--r--   0        0        0       20 2024-04-24 09:24:14.256206 cg-60.3.0/tests/fixtures/io/example2.txt
--rw-r--r--   0        0        0      582 2024-04-24 09:24:14.256206 cg-60.3.0/tests/fixtures/io/example_json.json
--rw-r--r--   0        0        0      103 2024-04-24 09:24:14.256206 cg-60.3.0/tests/fixtures/io/example_xml.xml
--rw-r--r--   0        0        0       20 2024-04-24 09:24:14.256206 cg-60.3.0/tests/fixtures/meta/qc_metrics/file_with_right_tags.json
--rw-r--r--   0        0        0       20 2024-04-24 09:24:14.256206 cg-60.3.0/tests/fixtures/meta/qc_metrics/file_without_right_tags.json
--rw-r--r--   0        0        0   156910 2024-04-24 09:24:14.256206 cg-60.3.0/tests/fixtures/orderforms/1508.30.balsamic.xlsx
--rw-r--r--   0        0        0   156770 2024-04-24 09:24:14.256206 cg-60.3.0/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx
--rw-r--r--   0        0        0   156737 2024-04-24 09:24:14.256206 cg-60.3.0/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx
--rw-r--r--   0        0        0   156582 2024-04-24 09:24:14.256206 cg-60.3.0/tests/fixtures/orderforms/1508.30.fastq.xlsx
--rw-r--r--   0        0        0   155627 2024-04-24 09:24:14.256206 cg-60.3.0/tests/fixtures/orderforms/1508.30.metagenome.xlsx
--rw-r--r--   0        0        0   156850 2024-04-24 09:24:14.256206 cg-60.3.0/tests/fixtures/orderforms/1508.30.mip.xlsx
--rw-r--r--   0        0        0   258580 2024-04-24 09:24:14.260206 cg-60.3.0/tests/fixtures/orderforms/1508.30.mip_rna.xlsx
--rw-r--r--   0        0        0   258342 2024-04-24 09:24:14.260206 cg-60.3.0/tests/fixtures/orderforms/1508.30.rnafusion.xlsx
--rw-r--r--   0        0        0    82677 2024-04-24 09:24:14.260206 cg-60.3.0/tests/fixtures/orderforms/1603.11.microbial.xlsx
--rw-r--r--   0        0        0   149394 2024-04-24 09:24:14.260206 cg-60.3.0/tests/fixtures/orderforms/1604.17.rml.xlsx
--rw-r--r--   0        0        0   223184 2024-04-24 09:24:14.260206 cg-60.3.0/tests/fixtures/orderforms/2184.9.sarscov2.xlsx
--rw-r--r--   0        0        0    18639 2024-04-24 09:24:14.260206 cg-60.3.0/tests/fixtures/orderforms/NIPT-json.json
--rw-r--r--   0        0        0     6052 2024-04-24 09:24:14.260206 cg-60.3.0/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
--rw-r--r--   0        0        0     6611 2024-04-24 09:24:14.260206 cg-60.3.0/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
--rw-r--r--   0        0        0     1417 2024-04-24 09:24:14.260206 cg-60.3.0/tests/fixtures/report/case_data.json
--rw-r--r--   0        0        0     1109 2024-04-24 09:24:14.260206 cg-60.3.0/tests/fixtures/report/lims_exported_samples.json
--rw-r--r--   0        0        0     1562 2024-04-24 09:24:14.260206 cg-60.3.0/tests/fixtures/report/lims_family.json
--rw-r--r--   0        0        0     3296 2024-04-24 09:24:14.260206 cg-60.3.0/tests/io/conftest.py
--rw-r--r--   0        0        0      431 2024-04-24 09:24:14.260206 cg-60.3.0/tests/io/test_io_config.py
--rw-r--r--   0        0        0     8639 2024-04-24 09:24:14.260206 cg-60.3.0/tests/io/test_io_controller.py
--rw-r--r--   0        0        0     3877 2024-04-24 09:24:14.260206 cg-60.3.0/tests/io/test_io_csv.py
--rw-r--r--   0        0        0      482 2024-04-24 09:24:14.260206 cg-60.3.0/tests/io/test_io_gzip.py
--rw-r--r--   0        0        0     1779 2024-04-24 09:24:14.260206 cg-60.3.0/tests/io/test_io_json.py
--rw-r--r--   0        0        0     2914 2024-04-24 09:24:14.260206 cg-60.3.0/tests/io/test_io_txt.py
--rw-r--r--   0        0        0     1027 2024-04-24 09:24:14.260206 cg-60.3.0/tests/io/test_io_xml.py
--rw-r--r--   0        0        0     2131 2024-04-24 09:24:14.260206 cg-60.3.0/tests/io/test_io_yaml.py
--rw-r--r--   0        0        0     1233 2024-04-24 09:24:14.260206 cg-60.3.0/tests/io/test_validate_path.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.260206 cg-60.3.0/tests/meta/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.260206 cg-60.3.0/tests/meta/archive/__init__.py
--rw-r--r--   0        0        0    13131 2024-04-24 09:24:14.260206 cg-60.3.0/tests/meta/archive/conftest.py
--rw-r--r--   0        0        0    16858 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/archive/test_archive_api.py
--rw-r--r--   0        0        0    10246 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/archive/test_archive_cli.py
--rw-r--r--   0        0        0    15766 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/archive/test_archiving.py
--rw-r--r--   0        0        0     3807 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/backup/conftest.py
--rw-r--r--   0        0        0    26368 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/backup/test_meta_backup.py
--rw-r--r--   0        0        0    10055 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/backup/test_meta_pdc.py
--rw-r--r--   0        0        0    12546 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/clean/conftest.py
--rw-r--r--   0        0        0    16944 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/clean/test_clean_flow_cells_api.py
--rw-r--r--   0        0        0     2286 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/clean/test_clean_retrieved_spring_files.py
--rw-r--r--   0        0        0     7691 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/compress/conftest.py
--rw-r--r--   0        0        0     7961 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/compress/test_clean_fastq.py
--rw-r--r--   0        0        0     1778 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/compress/test_compress_files.py
--rw-r--r--   0        0        0     3644 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/compress/test_compress_meta_fastq.py
--rw-r--r--   0        0        0     1180 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/compress/test_decompress_spring_meta.py
--rw-r--r--   0        0        0     6902 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/compress/test_meta_compress_update_hk.py
--rw-r--r--   0        0        0     8207 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/conftest.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/deliver/__init__.py
--rw-r--r--   0        0        0     3471 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/deliver/conftest.py
--rw-r--r--   0        0        0     5533 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/deliver/test_deliver_ticket.py
--rw-r--r--   0        0        0    10277 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/deliver/test_delivery_api.py
--rw-r--r--   0        0        0     1057 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/deliver/test_fastq_path_generator.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/delivery/__init__.py
--rw-r--r--   0        0        0    16660 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/delivery/test_delivery_api.py
--rw-r--r--   0        0        0     8729 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/demultiplex/conftest.py
--rw-r--r--   0        0        0     5382 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/demultiplex/test_combine_sequencing_metrics.py
--rw-r--r--   0        0        0     8339 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/demultiplex/test_demux_post_processing.py
--rw-r--r--   0        0        0    12330 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/demultiplex/test_housekeeper_storage_functions.py
--rw-r--r--   0        0        0     4392 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/demultiplex/test_status_db_storage_functions.py
--rw-r--r--   0        0        0    22705 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/demultiplex/test_utils.py
--rw-r--r--   0        0        0     6193 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/demultiplex/test_validation.py
--rw-r--r--   0        0        0     4943 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/encryption/conftest.py
--rw-r--r--   0        0        0    18133 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/encryption/test_encryption.py
--rw-r--r--   0        0        0     3122 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/observations/conftest.py
--rw-r--r--   0        0        0    16164 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/observations/test_meta_upload_observations.py
--rw-r--r--   0        0        0     4974 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/orders/conftest.py
--rw-r--r--   0        0        0     1749 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/orders/test_PoolSubmitter_validate_order.py
--rw-r--r--   0        0        0     1470 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
--rw-r--r--   0        0        0     1768 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/orders/test_SarsCov2Submitter_store_order.py
--rw-r--r--   0        0        0     2032 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
--rw-r--r--   0        0        0    19783 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/orders/test_meta_orders_api.py
--rw-r--r--   0        0        0     7086 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/orders/test_meta_orders_lims.py
--rw-r--r--   0        0        0    29515 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/orders/test_meta_orders_status.py
--rw-r--r--   0        0        0     1677 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/orders/test_rnafusion_submitter.py
--rw-r--r--   0        0        0     1068 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/orders/test_ticket_handler.py
--rw-r--r--   0        0        0     4336 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/qc_metrics/conftest.py
--rw-r--r--   0        0        0     1972 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/qc_metrics/test_collect_qc_metrics.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/report/__init__.py
--rw-r--r--   0        0        0     6512 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/report/conftest.py
--rw-r--r--   0        0        0      434 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/report/helper.py
--rw-r--r--   0        0        0     2604 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/report/test_balsamic_api.py
--rw-r--r--   0        0        0     4056 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/report/test_field_validators.py
--rw-r--r--   0        0        0     2858 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/report/test_mip_dna_api.py
--rw-r--r--   0        0        0    16042 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/report/test_report_api.py
--rw-r--r--   0        0        0     1365 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/report/test_rnafusion_api.py
--rw-r--r--   0        0        0     1250 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/report/test_tomte_api.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/rsync/__init__.py
--rw-r--r--   0        0        0      916 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/rsync/conftest.py
--rw-r--r--   0        0        0     9442 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/rsync/test_rsync.py
--rw-r--r--   0        0        0     3147 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/test_invoice.py
--rw-r--r--   0        0        0     1220 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/transfer/conftest.py
--rw-r--r--   0        0        0     9892 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/transfer/test_external_data.py
--rw-r--r--   0        0        0     4395 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/transfer/test_meta_transfer_lims.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/upload/__init__.py
--rw-r--r--   0        0        0     2210 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/upload/balsamic/test_balsamic.py
--rw-r--r--   0        0        0     4002 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/upload/conftest.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/upload/gisaid/__init__.py
--rw-r--r--   0        0        0     2557 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/upload/gisaid/fixtures/four_samples.csv
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.264206 cg-60.3.0/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
--rw-r--r--   0        0        0      211 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
--rw-r--r--   0        0        0      371 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/upload/mutacc/__init__.py
--rw-r--r--   0        0        0     3684 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/upload/mutacc/conftest.py
--rw-r--r--   0        0        0     4188 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
--rw-r--r--   0        0        0     1149 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/upload/nipt/conftest.py
--rw-r--r--   0        0        0     1683 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/upload/nipt/test_models.py
--rw-r--r--   0        0        0     1242 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/upload/nipt/test_nipt_upload_api.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/upload/scout/__init__.py
--rw-r--r--   0        0        0    23954 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/upload/scout/conftest.py
--rw-r--r--   0        0        0     4734 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/upload/scout/test_generate_load_config.py
--rw-r--r--   0        0        0     4182 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/upload/scout/test_meta_upload_scoutapi.py
--rw-r--r--   0        0        0    33260 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
--rw-r--r--   0        0        0     7372 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/upload/scout/test_scout_config_builder.py
--rw-r--r--   0        0        0     2511 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/upload/test_meta_upload_coverage.py
--rw-r--r--   0        0        0     1473 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/upload/test_upload_api.py
--rw-r--r--   0        0        0     2547 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/upload/test_upload_genotypes_api.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/workflow/__init__.py
--rw-r--r--   0        0        0    10262 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/workflow/conftest.py
--rw-r--r--   0        0        0     3652 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/workflow/microsalt/conftest.py
--rw-r--r--   0        0        0      318 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/workflow/microsalt/test_parsing_metrics.py
--rw-r--r--   0        0        0     3714 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/workflow/microsalt/test_quality_controller.py
--rw-r--r--   0        0        0    14367 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/workflow/microsalt/test_quality_controller_utils.py
--rw-r--r--   0        0        0      825 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/workflow/microsalt/test_report_generation.py
--rw-r--r--   0        0        0    20848 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/workflow/test_analysis.py
--rw-r--r--   0        0        0     7934 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/workflow/test_balsamic.py
--rw-r--r--   0        0        0     3034 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/workflow/test_fastq.py
--rw-r--r--   0        0        0     1532 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/workflow/test_microsalt.py
--rw-r--r--   0        0        0     2721 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/workflow/test_nf_analysis.py
--rw-r--r--   0        0        0     7741 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/workflow/test_prepare_fastq_api.py
--rw-r--r--   0        0        0     1920 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/workflow/test_raredisease.py
--rw-r--r--   0        0        0     1674 2024-04-24 09:24:14.268206 cg-60.3.0/tests/meta/workflow/test_rnafusion.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.268206 cg-60.3.0/tests/mocks/__init__.py
--rw-r--r--   0        0        0     1168 2024-04-24 09:24:14.268206 cg-60.3.0/tests/mocks/balsamic_analysis_mock.py
--rw-r--r--   0        0        0     3500 2024-04-24 09:24:14.268206 cg-60.3.0/tests/mocks/crunchy.py
--rw-r--r--   0        0        0    21778 2024-04-24 09:24:14.268206 cg-60.3.0/tests/mocks/hk_mock.py
--rw-r--r--   0        0        0     4106 2024-04-24 09:24:14.268206 cg-60.3.0/tests/mocks/limsmock.py
--rw-r--r--   0        0        0      572 2024-04-24 09:24:14.268206 cg-60.3.0/tests/mocks/madeline.py
--rw-r--r--   0        0        0     1297 2024-04-24 09:24:14.268206 cg-60.3.0/tests/mocks/mip_analysis_mock.py
--rw-r--r--   0        0        0     1525 2024-04-24 09:24:14.268206 cg-60.3.0/tests/mocks/osticket.py
--rw-r--r--   0        0        0     3239 2024-04-24 09:24:14.268206 cg-60.3.0/tests/mocks/process_mock.py
--rw-r--r--   0        0        0     4713 2024-04-24 09:24:14.268206 cg-60.3.0/tests/mocks/report.py
--rw-r--r--   0        0        0     3915 2024-04-24 09:24:14.268206 cg-60.3.0/tests/mocks/scout.py
--rw-r--r--   0        0        0      750 2024-04-24 09:24:14.268206 cg-60.3.0/tests/mocks/store_model.py
--rw-r--r--   0        0        0     1532 2024-04-24 09:24:14.268206 cg-60.3.0/tests/mocks/tb_mock.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/balsamic/__init__.py
--rw-r--r--   0        0        0     1194 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/balsamic/conftest.py
--rw-r--r--   0        0        0     1030 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/balsamic/test_balsamic_analysis.py
--rw-r--r--   0        0        0     1050 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/conftest.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/demultiplexing/__init__.py
--rw-r--r--   0        0        0      284 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/demultiplexing/conftest.py
--rw-r--r--   0        0        0    11446 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/demultiplexing/test_run_parameters.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/downsample/__init__.py
--rw-r--r--   0        0        0     2096 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/downsample/test_down_sample_meta_data.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/flow_cell/__init__.py
--rw-r--r--   0        0        0     6659 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/flow_cell/test_flowcell_model.py
--rw-r--r--   0        0        0     6637 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/mip/conftest.py
--rw-r--r--   0        0        0     1239 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/mip/test_mip_analysis.py
--rw-r--r--   0        0        0     2348 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/mip/test_mip_config.py
--rw-r--r--   0        0        0     6392 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/mip/test_mip_metrics_deliverables.py
--rw-r--r--   0        0        0     3959 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/mip/test_mip_sample_info.py
--rw-r--r--   0        0        0     3314 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/nextflow/test_nextflow_deliver.py
--rw-r--r--   0        0        0     1602 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/observations/conftest.py
--rw-r--r--   0        0        0     2579 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/observations/test_observations_input_files.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/report/__init__.py
--rw-r--r--   0        0        0     7327 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/report/test_validators.py
--rw-r--r--   0        0        0     3855 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/rnafusion/test_rnafusion_sample.py
--rw-r--r--   0        0        0     1374 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/test_cg_models.py
--rw-r--r--   0        0        0      990 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/test_compression_data.py
--rw-r--r--   0        0        0      729 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/test_fastq.py
--rw-r--r--   0        0        0     2860 2024-04-24 09:24:14.268206 cg-60.3.0/tests/models/test_file_data.py
--rw-r--r--   0        0        0     4539 2024-04-24 09:24:14.268206 cg-60.3.0/tests/server/conftest.py
--rw-r--r--   0        0        0     3135 2024-04-24 09:24:14.268206 cg-60.3.0/tests/server/endpoints/test_delivery_message_endpoint.py
--rw-r--r--   0        0        0     3239 2024-04-24 09:24:14.268206 cg-60.3.0/tests/server/endpoints/test_orders_endpoint.py
--rw-r--r--   0        0        0      271 2024-04-24 09:24:14.268206 cg-60.3.0/tests/server/test_server_auto.py
--rw-r--r--   0        0        0     1047 2024-04-24 09:24:14.268206 cg-60.3.0/tests/services/fastq_file_service/conftest.py
--rw-r--r--   0        0        0     3634 2024-04-24 09:24:14.268206 cg-60.3.0/tests/services/fastq_file_service/test_fastq_file_service.py
--rw-r--r--   0        0        0     4861 2024-04-24 09:24:14.272206 cg-60.3.0/tests/services/orders/order_status_service/conftest.py
--rw-r--r--   0        0        0     2865 2024-04-24 09:24:14.272206 cg-60.3.0/tests/services/orders/order_status_service/test_order_summary_service.py
--rw-r--r--   0        0        0      318 2024-04-24 09:24:14.272206 cg-60.3.0/tests/small_helpers.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/api/__init__.py
--rw-r--r--   0        0        0     2984 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/api/conftest.py
--rw-r--r--   0        0        0     1557 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/api/test_base.py
--rw-r--r--   0        0        0    20096 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/conftest.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/crud/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/crud/add/__init__.py
--rw-r--r--   0        0        0     1497 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/crud/add/test_store_add_application_version.py
--rw-r--r--   0        0        0     3958 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/crud/add/test_store_add_base.py
--rw-r--r--   0        0        0     2502 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/crud/add/test_store_add_customer.py
--rw-r--r--   0        0        0     1640 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/crud/add/test_store_add_flow_celll.py
--rw-r--r--   0        0        0    12212 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/crud/conftest.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/crud/delete/__init__.py
--rw-r--r--   0        0        0     5541 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/crud/delete/test_delete.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/crud/read/__init__.py
--rw-r--r--   0        0        0    57211 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/crud/read/test_read.py
--rw-r--r--   0        0        0     5461 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/crud/read/test_read_analyses_to_clean.py
--rw-r--r--   0        0        0     3553 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/crud/read/test_read_analyses_to_delivery_report.py
--rw-r--r--   0        0        0    18463 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/crud/read/test_read_analysis.py
--rw-r--r--   0        0        0     2743 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/crud/read/test_read_application_version.py
--rw-r--r--   0        0        0     1105 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/crud/read/test_read_customer.py
--rw-r--r--   0        0        0     1530 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/crud/read/test_read_pool.py
--rw-r--r--   0        0        0    21503 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/crud/read/test_read_sample.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/crud/update/__init__.py
--rw-r--r--   0        0        0      737 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/crud/update/test_update.py
--rw-r--r--   0        0        0    11693 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/filters/test_status_analyses_filters.py
--rw-r--r--   0        0        0     3397 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/filters/test_status_application_filters.py
--rw-r--r--   0        0        0     2073 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/filters/test_status_application_limitations_filters.py
--rw-r--r--   0        0        0    10452 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/filters/test_status_application_version_filters.py
--rw-r--r--   0        0        0     2804 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/filters/test_status_bed_filters.py
--rw-r--r--   0        0        0     2362 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/filters/test_status_bed_version_filters.py
--rw-r--r--   0        0        0     3495 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/filters/test_status_case_sample_filters.py
--rw-r--r--   0        0        0    39100 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/filters/test_status_cases_filters.py
--rw-r--r--   0        0        0     1345 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/filters/test_status_collaboration_filters.py
--rw-r--r--   0        0        0     2482 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/filters/test_status_customer_filters.py
--rw-r--r--   0        0        0     4907 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/filters/test_status_flow_cell_filters.py
--rw-r--r--   0        0        0     2226 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/filters/test_status_invoice_filters.py
--rw-r--r--   0        0        0     5871 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/filters/test_status_metrics_filters.py
--rw-r--r--   0        0        0     2404 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/filters/test_status_organism_filters.py
--rw-r--r--   0        0        0     1804 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/filters/test_status_panel_filters.py
--rw-r--r--   0        0        0     8720 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/filters/test_status_pool_filters.py
--rw-r--r--   0        0        0    22875 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/filters/test_status_samples_filters.py
--rw-r--r--   0        0        0     1576 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/filters/test_status_user_filters.py
--rw-r--r--   0        0        0     2147 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/test_delivery.py
--rw-r--r--   0        0        0     4127 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store/test_store_models.py
--rw-r--r--   0        0        0    37040 2024-04-24 09:24:14.272206 cg-60.3.0/tests/store_helpers.py
--rw-r--r--   0        0        0     4930 2024-04-24 09:24:14.272206 cg-60.3.0/tests/test_copy_novaseqx_flow_cell.py
--rw-r--r--   0        0        0      911 2024-04-24 09:24:14.272206 cg-60.3.0/tests/test_store_helpers.py
--rw-r--r--   0        0        0        0 2024-04-24 09:24:14.272206 cg-60.3.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     1754 2024-04-24 09:24:14.272206 cg-60.3.0/tests/utils/conftest.py
--rw-r--r--   0        0        0      371 2024-04-24 09:24:14.272206 cg-60.3.0/tests/utils/test_calculations.py
--rw-r--r--   0        0        0     2920 2024-04-24 09:24:14.272206 cg-60.3.0/tests/utils/test_commands.py
--rw-r--r--   0        0        0      953 2024-04-24 09:24:14.272206 cg-60.3.0/tests/utils/test_date.py
--rw-r--r--   0        0        0     1508 2024-04-24 09:24:14.272206 cg-60.3.0/tests/utils/test_dict.py
--rw-r--r--   0        0        0     7154 2024-04-24 09:24:14.272206 cg-60.3.0/tests/utils/test_dispatcher.py
--rw-r--r--   0        0        0     4100 2024-04-24 09:24:14.272206 cg-60.3.0/tests/utils/test_files.py
--rw-r--r--   0        0        0     1170 2024-04-24 09:24:14.272206 cg-60.3.0/tests/utils/test_time.py
--rw-r--r--   0        0        0     2366 2024-04-24 09:24:14.272206 cg-60.3.0/tests/utils/test_utils.py
--rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 cg-60.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2686 2024-04-24 11:46:39.943723 cg-60.3.1/README.md
+-rw-r--r--   0        0        0       40 2024-04-24 11:46:39.947723 cg-60.3.1/cg/__init__.py
+-rw-r--r--   0        0        0      315 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/coverage/__init__.py
+-rw-r--r--   0        0        0     2940 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/coverage/api.py
+-rw-r--r--   0        0        0       56 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/crunchy/__init__.py
+-rw-r--r--   0        0        0    12783 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/crunchy/crunchy.py
+-rw-r--r--   0        0        0     4502 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/crunchy/files.py
+-rw-r--r--   0        0        0      430 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/crunchy/models.py
+-rw-r--r--   0        0        0      910 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/crunchy/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/__init__.py
+-rw-r--r--   0        0        0    11299 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/demultiplex_api.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/sample_sheet/__init__.py
+-rw-r--r--   0        0        0    11249 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/sample_sheet/api.py
+-rw-r--r--   0        0        0     2183 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/sample_sheet/index.py
+-rw-r--r--   0        0        0     7341 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py
+-rw-r--r--   0        0        0     3188 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py
+-rw-r--r--   0        0        0     7071 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/sample_sheet/sample_models.py
+-rw-r--r--   0        0        0     6076 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py
+-rw-r--r--   0        0        0     1372 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py
+-rw-r--r--   0        0        0     8092 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py
+-rw-r--r--   0        0        0      824 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/sample_sheet/validators.py
+-rw-r--r--   0        0        0      677 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/downsample/__init__.py
+-rw-r--r--   0        0        0     6160 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/downsample/downsample.py
+-rw-r--r--   0        0        0     2125 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/downsample/utils.py
+-rw-r--r--   0        0        0      298 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/environ.py
+-rw-r--r--   0        0        0     1741 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/gens.py
+-rw-r--r--   0        0        0     3419 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/gt.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/hermes/__init__.py
+-rw-r--r--   0        0        0     2249 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/hermes/hermes_api.py
+-rw-r--r--   0        0        0     1298 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/hermes/models.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/housekeeper/__init__.py
+-rw-r--r--   0        0        0    30395 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/housekeeper/hk.py
+-rw-r--r--   0        0        0      326 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/housekeeper/models.py
+-rw-r--r--   0        0        0       32 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/invoice/__init__.py
+-rw-r--r--   0        0        0     4804 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/invoice/render.py
+-rw-r--r--   0        0        0   113467 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/invoice/templates/KI_pool_invoice.xlsx
+-rw-r--r--   0        0        0    75562 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/invoice/templates/KI_sample_invoice.xlsx
+-rw-r--r--   0        0        0   113512 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
+-rw-r--r--   0        0        0    75459 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
+-rw-r--r--   0        0        0       25 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/lims/__init__.py
+-rw-r--r--   0        0        0    18546 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/lims/api.py
+-rw-r--r--   0        0        0     2652 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/lims/batch.py
+-rw-r--r--   0        0        0     8129 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/lims/order.py
+-rw-r--r--   0        0        0     3118 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/lims/sample_sheet.py
+-rw-r--r--   0        0        0     4866 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/loqus.py
+-rw-r--r--   0        0        0       35 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/madeline/__init__.py
+-rw-r--r--   0        0        0     3213 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/madeline/api.py
+-rw-r--r--   0        0        0       23 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/mip/__init__.py
+-rw-r--r--   0        0        0     3564 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/mip/confighandler.py
+-rw-r--r--   0        0        0     2207 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/mutacc_auto.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/orderform/__init__.py
+-rw-r--r--   0        0        0     9498 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/orderform/excel_orderform_parser.py
+-rw-r--r--   0        0        0     3051 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/orderform/json_orderform_parser.py
+-rw-r--r--   0        0        0     6419 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/orderform/orderform_parser.py
+-rw-r--r--   0        0        0      252 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/orderform/utils.py
+-rw-r--r--   0        0        0     2537 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/osticket.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/scout/__init__.py
+-rw-r--r--   0        0        0     3177 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/scout/scout_export.py
+-rw-r--r--   0        0        0    11054 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/scout/scoutapi.py
+-rw-r--r--   0        0        0      444 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/scout/validators.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0        0        0     3457 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/sequencing_metrics_parser/api.py
+-rw-r--r--   0        0        0      923 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/sequencing_metrics_parser/models.py
+-rw-r--r--   0        0        0     6670 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/sequencing_metrics_parser/parser.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/slurm/__init__.py
+-rw-r--r--   0        0        0     1277 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/slurm/sbatch.py
+-rw-r--r--   0        0        0     3559 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/slurm/slurm_api.py
+-rw-r--r--   0        0        0       32 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/tb/__init__.py
+-rw-r--r--   0        0        0     7995 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/tb/api.py
+-rw-r--r--   0        0        0      152 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/tb/dto/create_job_request.py
+-rw-r--r--   0        0        0      250 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/tb/dto/summary_response.py
+-rw-r--r--   0        0        0     1305 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/tb/models.py
+-rw-r--r--   0        0        0      305 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/tb/validators.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.951723 cg-60.3.1/cg/cli/__init__.py
+-rw-r--r--   0        0        0    11558 2024-04-24 11:46:39.951723 cg-60.3.1/cg/cli/add.py
+-rw-r--r--   0        0        0     2653 2024-04-24 11:46:39.951723 cg-60.3.1/cg/cli/archive.py
+-rw-r--r--   0        0        0    10118 2024-04-24 11:46:39.951723 cg-60.3.1/cg/cli/backup.py
+-rw-r--r--   0        0        0     3852 2024-04-24 11:46:39.951723 cg-60.3.1/cg/cli/base.py
+-rw-r--r--   0        0        0    10506 2024-04-24 11:46:39.951723 cg-60.3.1/cg/cli/clean.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.951723 cg-60.3.1/cg/cli/compress/__init__.py
+-rw-r--r--   0        0        0     2135 2024-04-24 11:46:39.951723 cg-60.3.1/cg/cli/compress/base.py
+-rw-r--r--   0        0        0     6706 2024-04-24 11:46:39.951723 cg-60.3.1/cg/cli/compress/fastq.py
+-rw-r--r--   0        0        0     8163 2024-04-24 11:46:39.951723 cg-60.3.1/cg/cli/compress/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/delete/__init__.py
+-rw-r--r--   0        0        0      564 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/delete/base.py
+-rw-r--r--   0        0        0     4603 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/delete/case.py
+-rw-r--r--   0        0        0     1884 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/delete/cases.py
+-rw-r--r--   0        0        0     2633 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/delete/observations.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/deliver/__init__.py
+-rw-r--r--   0        0        0     6030 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/deliver/base.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/demultiplex/__init__.py
+-rw-r--r--   0        0        0      829 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/demultiplex/base.py
+-rw-r--r--   0        0        0     4905 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py
+-rw-r--r--   0        0        0     7726 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/demultiplex/demux.py
+-rw-r--r--   0        0        0     1473 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/demultiplex/finish.py
+-rw-r--r--   0        0        0     3119 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/demultiplex/sample_sheet.py
+-rw-r--r--   0        0        0     2995 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/downsample.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/generate/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/generate/base.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/generate/report/__init__.py
+-rw-r--r--   0        0        0     4636 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/generate/report/base.py
+-rw-r--r--   0        0        0      854 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/generate/report/options.py
+-rw-r--r--   0        0        0     5340 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/generate/report/utils.py
+-rw-r--r--   0        0        0     8327 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/get.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/set/__init__.py
+-rw-r--r--   0        0        0     9856 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/set/base.py
+-rw-r--r--   0        0        0     4384 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/set/case.py
+-rw-r--r--   0        0        0     2595 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/set/cases.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/store/__init__.py
+-rw-r--r--   0        0        0     1093 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/store/base.py
+-rw-r--r--   0        0        0     6191 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/store/store.py
+-rw-r--r--   0        0        0     1761 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/transfer.py
+-rw-r--r--   0        0        0        1 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/__init__.py
+-rw-r--r--   0        0        0     5706 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/base.py
+-rw-r--r--   0        0        0     5503 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/clinical_delivery.py
+-rw-r--r--   0        0        0     1175 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/coverage.py
+-rw-r--r--   0        0        0     1528 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/delivery_report.py
+-rw-r--r--   0        0        0     4022 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/fohm.py
+-rw-r--r--   0        0        0     1463 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/genotype.py
+-rw-r--r--   0        0        0     1885 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/gens.py
+-rw-r--r--   0        0        0      584 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/gisaid.py
+-rw-r--r--   0        0        0     2645 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/mutacc.py
+-rw-r--r--   0        0        0       23 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/nipt/__init__.py
+-rw-r--r--   0        0        0     3006 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/nipt/base.py
+-rw-r--r--   0        0        0     2275 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/nipt/ftp.py
+-rw-r--r--   0        0        0     1596 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/nipt/statina.py
+-rw-r--r--   0        0        0      112 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/observations/__init__.py
+-rw-r--r--   0        0        0     2672 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/observations/observations.py
+-rw-r--r--   0        0        0     2904 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/observations/utils.py
+-rw-r--r--   0        0        0     9970 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/scout.py
+-rw-r--r--   0        0        0      650 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/utils.py
+-rw-r--r--   0        0        0     1667 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/validate.py
+-rw-r--r--   0        0        0      105 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/utils.py
+-rw-r--r--   0        0        0       18 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/balsamic/__init__.py
+-rw-r--r--   0        0        0     8925 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/balsamic/base.py
+-rw-r--r--   0        0        0     1980 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/balsamic/options.py
+-rw-r--r--   0        0        0      881 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/balsamic/pon.py
+-rw-r--r--   0        0        0     1162 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/balsamic/qc.py
+-rw-r--r--   0        0        0     1177 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/balsamic/umi.py
+-rw-r--r--   0        0        0     1342 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/base.py
+-rw-r--r--   0        0        0    12379 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/commands.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/fastq/__init__.py
+-rw-r--r--   0        0        0     1367 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/fastq/base.py
+-rw-r--r--   0        0        0     1787 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/fastq/fastq_service.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0        0        0     4177 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/fluffy/base.py
+-rw-r--r--   0        0        0       22 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/jasen/__init__.py
+-rw-r--r--   0        0        0      535 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/jasen/base.py
+-rw-r--r--   0        0        0       22 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/microsalt/__init__.py
+-rw-r--r--   0        0        0     7810 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/microsalt/base.py
+-rw-r--r--   0        0        0       22 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/mip/__init__.py
+-rw-r--r--   0        0        0     6596 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/mip/base.py
+-rw-r--r--   0        0        0     1268 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/mip/options.py
+-rw-r--r--   0        0        0       22 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/mip_dna/__init__.py
+-rw-r--r--   0        0        0     1013 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/mip_dna/base.py
+-rw-r--r--   0        0        0       22 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/mip_rna/__init__.py
+-rw-r--r--   0        0        0      916 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/mip_rna/base.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/mutant/__init__.py
+-rw-r--r--   0        0        0     3413 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/mutant/base.py
+-rw-r--r--   0        0        0     9002 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/nf_analysis.py
+-rw-r--r--   0        0        0       22 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/raredisease/__init__.py
+-rw-r--r--   0        0        0     2210 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/raredisease/base.py
+-rw-r--r--   0        0        0       22 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/rnafusion/__init__.py
+-rw-r--r--   0        0        0     1179 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/rnafusion/base.py
+-rw-r--r--   0        0        0       22 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/taxprofiler/__init__.py
+-rw-r--r--   0        0        0     1211 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/taxprofiler/base.py
+-rw-r--r--   0        0        0     1111 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/tomte/base.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.959723 cg-60.3.1/cg/clients/__init__.py
+-rw-r--r--   0        0        0     1363 2024-04-24 11:46:39.959723 cg-60.3.1/cg/clients/arnold/api.py
+-rw-r--r--   0        0        0      160 2024-04-24 11:46:39.959723 cg-60.3.1/cg/clients/arnold/dto/create_case_request.py
+-rw-r--r--   0        0        0      384 2024-04-24 11:46:39.959723 cg-60.3.1/cg/clients/arnold/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.959723 cg-60.3.1/cg/clients/janus/__init__.py
+-rw-r--r--   0        0        0     1246 2024-04-24 11:46:39.959723 cg-60.3.1/cg/clients/janus/api.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.959723 cg-60.3.1/cg/clients/janus/dto/__init__.py
+-rw-r--r--   0        0        0      503 2024-04-24 11:46:39.959723 cg-60.3.1/cg/clients/janus/dto/create_qc_metrics_request.py
+-rw-r--r--   0        0        0      420 2024-04-24 11:46:39.959723 cg-60.3.1/cg/clients/janus/exceptions.py
+-rw-r--r--   0        0        0      937 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/__init__.py
+-rw-r--r--   0        0        0      253 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/archiving.py
+-rw-r--r--   0        0        0       35 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/backup.py
+-rw-r--r--   0        0        0      769 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/bcl_convert_metrics.py
+-rw-r--r--   0        0        0      469 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/compression.py
+-rw-r--r--   0        0        0     6613 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/constants.py
+-rw-r--r--   0        0        0     6033 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/delivery.py
+-rw-r--r--   0        0        0     8120 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/demultiplexing.py
+-rw-r--r--   0        0        0     1422 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/encryption.py
+-rw-r--r--   0        0        0      372 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/extraction.py
+-rw-r--r--   0        0        0     2054 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/gene_panel.py
+-rw-r--r--   0        0        0     6704 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/housekeeper_tags.py
+-rw-r--r--   0        0        0       95 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/invoice.py
+-rw-r--r--   0        0        0     5815 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/lims.py
+-rw-r--r--   0        0        0      743 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/metrics.py
+-rw-r--r--   0        0        0      231 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/nanopore_files.py
+-rw-r--r--   0        0        0      650 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/nextflow.py
+-rw-r--r--   0        0        0     1529 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/nf_analysis.py
+-rw-r--r--   0        0        0       19 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/nipt.py
+-rw-r--r--   0        0        0     2257 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/observations.py
+-rw-r--r--   0        0        0     1216 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/orderforms.py
+-rw-r--r--   0        0        0       96 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/paths.py
+-rw-r--r--   0        0        0      266 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/pdc.py
+-rw-r--r--   0        0        0      160 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/pedigree.py
+-rw-r--r--   0        0        0     1044 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/priority.py
+-rw-r--r--   0        0        0       79 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/process.py
+-rw-r--r--   0        0        0     5474 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/report.py
+-rw-r--r--   0        0        0      485 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/sample_sources.py
+-rw-r--r--   0        0        0     3111 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/scout.py
+-rw-r--r--   0        0        0     1669 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/sequencing.py
+-rw-r--r--   0        0        0      313 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/slurm.py
+-rw-r--r--   0        0        0      529 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/subject.py
+-rw-r--r--   0        0        0       55 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/symbols.py
+-rw-r--r--   0        0        0      435 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/tb.py
+-rw-r--r--   0        0        0      161 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/time.py
+-rw-r--r--   0        0        0     6639 2024-04-24 11:46:39.959723 cg-60.3.1/cg/exc.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/__init__.py
+-rw-r--r--   0        0        0     1037 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/api.py
+-rw-r--r--   0        0        0      621 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/config.py
+-rw-r--r--   0        0        0     2978 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/controller.py
+-rw-r--r--   0        0        0     1763 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/csv.py
+-rw-r--r--   0        0        0      210 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/gzip.py
+-rw-r--r--   0        0        0      662 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/json.py
+-rw-r--r--   0        0        0      525 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/png.py
+-rw-r--r--   0        0        0     1094 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/txt.py
+-rw-r--r--   0        0        0      552 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/validate_path.py
+-rw-r--r--   0        0        0     1289 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/xml.py
+-rw-r--r--   0        0        0     1153 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/yaml.py
+-rw-r--r--   0        0        0      281 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/archive/__init__.py
+-rw-r--r--   0        0        0    15193 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/archive/archive.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/archive/ddn/__init__.py
+-rw-r--r--   0        0        0     1727 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/archive/ddn/constants.py
+-rw-r--r--   0        0        0    10852 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/archive/ddn/ddn_data_flow_client.py
+-rw-r--r--   0        0        0     3704 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/archive/ddn/models.py
+-rw-r--r--   0        0        0     1250 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/archive/ddn/utils.py
+-rw-r--r--   0        0        0     2024 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/archive/models.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/backup/__init__.py
+-rw-r--r--   0        0        0    17426 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/backup/backup.py
+-rw-r--r--   0        0        0     5397 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/backup/pdc.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/clean/__init__.py
+-rw-r--r--   0        0        0     3901 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/clean/api.py
+-rw-r--r--   0        0        0     7738 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/clean/clean_flow_cells.py
+-rw-r--r--   0        0        0     1841 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/clean/clean_retrieved_spring_files.py
+-rw-r--r--   0        0        0       34 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/compress/__init__.py
+-rw-r--r--   0        0        0    14557 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/compress/compress.py
+-rw-r--r--   0        0        0     4947 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/compress/files.py
+-rw-r--r--   0        0        0       77 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/deliver/__init__.py
+-rw-r--r--   0        0        0    14672 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/deliver/deliver.py
+-rw-r--r--   0        0        0     4502 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/deliver/deliver_ticket.py
+-rw-r--r--   0        0        0      904 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/deliver/fastq_path_generator.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/delivery/__init__.py
+-rw-r--r--   0        0        0     8255 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/delivery/delivery.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/demultiplex/__init__.py
+-rw-r--r--   0        0        0     2592 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/demultiplex/combine_sequencing_metrics.py
+-rw-r--r--   0        0        0     5719 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/demultiplex/demux_post_processing.py
+-rw-r--r--   0        0        0     4135 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/demultiplex/files.py
+-rw-r--r--   0        0        0     7777 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/demultiplex/housekeeper_storage_functions.py
+-rw-r--r--   0        0        0     6126 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/demultiplex/status_db_storage_functions.py
+-rw-r--r--   0        0        0    10690 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/demultiplex/utils.py
+-rw-r--r--   0        0        0     2855 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/demultiplex/validation.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/encryption/__init__.py
+-rw-r--r--   0        0        0    20271 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/encryption/encryption.py
+-rw-r--r--   0        0        0      537 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/encryption/sbatch.py
+-rw-r--r--   0        0        0    10922 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/invoice.py
+-rw-r--r--   0        0        0     2360 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/meta.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/observations/__init__.py
+-rw-r--r--   0        0        0     6008 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/observations/balsamic_observations_api.py
+-rw-r--r--   0        0        0     5277 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/observations/mip_dna_observations_api.py
+-rw-r--r--   0        0        0     5364 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/observations/observations_api.py
+-rw-r--r--   0        0        0       27 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/__init__.py
+-rw-r--r--   0        0        0     3637 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/api.py
+-rw-r--r--   0        0        0      121 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/balsamic_qc_submitter.py
+-rw-r--r--   0        0        0      107 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/balsamic_submitter.py
+-rw-r--r--   0        0        0      122 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/balsamic_umi_submitter.py
+-rw-r--r--   0        0        0    15262 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/case_submitter.py
+-rw-r--r--   0        0        0     6102 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/fastq_submitter.py
+-rw-r--r--   0        0        0      105 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/fluffy_submitter.py
+-rw-r--r--   0        0        0     1254 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/lims.py
+-rw-r--r--   0        0        0     5782 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/metagenome_submitter.py
+-rw-r--r--   0        0        0     6337 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/microbial_submitter.py
+-rw-r--r--   0        0        0      123 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/microsalt_submitter.py
+-rw-r--r--   0        0        0      105 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/mip_dna_submitter.py
+-rw-r--r--   0        0        0      105 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/mip_rna_submitter.py
+-rw-r--r--   0        0        0     7761 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/pool_submitter.py
+-rw-r--r--   0        0        0      102 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/rml_submitter.py
+-rw-r--r--   0        0        0      718 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/rnafusion_submitter.py
+-rw-r--r--   0        0        0     1268 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/sars_cov_2_submitter.py
+-rw-r--r--   0        0        0     1754 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/submitter.py
+-rw-r--r--   0        0        0     7880 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/ticket_handler.py
+-rw-r--r--   0        0        0     4105 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/qc_metrics/collect_qc_metrics.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/__init__.py
+-rw-r--r--   0        0        0     8168 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/balsamic.py
+-rw-r--r--   0        0        0      562 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/balsamic_qc.py
+-rw-r--r--   0        0        0      717 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/balsamic_umi.py
+-rw-r--r--   0        0        0     4171 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/field_validators.py
+-rw-r--r--   0        0        0     6620 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/mip_dna.py
+-rw-r--r--   0        0        0    18606 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/report_api.py
+-rw-r--r--   0        0        0     5625 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/rnafusion.py
+-rw-r--r--   0        0        0     1911 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/delivery-report.html
+-rw-r--r--   0        0        0     4236 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/data_analysis/data_analysis.html
+-rw-r--r--   0        0        0     1049 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/data_analysis/limitations.html
+-rw-r--r--   0        0        0     3351 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html
+-rw-r--r--   0        0        0     1364 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html
+-rw-r--r--   0        0        0      753 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html
+-rw-r--r--   0        0        0     3284 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html
+-rw-r--r--   0        0        0     3670 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html
+-rw-r--r--   0        0        0     2332 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/header.html
+-rw-r--r--   0        0        0     2066 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/order.html
+-rw-r--r--   0        0        0     2243 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/sample_prep.html
+-rw-r--r--   0        0        0      472 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/ticket_system.html
+-rw-r--r--   0        0        0     1165 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html
+-rw-r--r--   0        0        0     1538 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html
+-rw-r--r--   0        0        0      428 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/uploaded_files/rnafusion_uploaded_files.html
+-rw-r--r--   0        0        0     4266 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html
+-rw-r--r--   0        0        0       80 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/partials/footer.html
+-rw-r--r--   0        0        0      172 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/partials/signature.html
+-rw-r--r--   0        0        0   232803 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0       33 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/static/css/custom.css
+-rw-r--r--   0        0        0    30068 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/static/images/SWEDAC_logo.png
+-rw-r--r--   0        0        0     3925 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/tomte.py
+-rw-r--r--   0        0        0       32 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/rsync/__init__.py
+-rw-r--r--   0        0        0    12291 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/rsync/rsync_api.py
+-rw-r--r--   0        0        0      387 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/rsync/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/tar/__init__.py
+-rw-r--r--   0        0        0     1694 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/tar/tar.py
+-rw-r--r--   0        0        0       71 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/transfer/__init__.py
+-rw-r--r--   0        0        0    10016 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/transfer/external_data.py
+-rw-r--r--   0        0        0     5814 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/transfer/lims.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/balsamic/__init__.py
+-rw-r--r--   0        0        0     3107 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/balsamic/balsamic.py
+-rw-r--r--   0        0        0     2224 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/coverage.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/fohm/__init__.py
+-rw-r--r--   0        0        0    12102 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/fohm/fohm.py
+-rw-r--r--   0        0        0       30 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/gisaid/__init__.py
+-rw-r--r--   0        0        0      928 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/gisaid/constants.py
+-rw-r--r--   0        0        0    13521 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/gisaid/gisaid.py
+-rw-r--r--   0        0        0     3312 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/gisaid/models.py
+-rw-r--r--   0        0        0     5310 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/gt.py
+-rw-r--r--   0        0        0      898 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/microsalt/microsalt_upload_api.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/mip/__init__.py
+-rw-r--r--   0        0        0     2546 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/mip/mip_dna.py
+-rw-r--r--   0        0        0     1400 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/mip/mip_rna.py
+-rw-r--r--   0        0        0     7294 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/mutacc.py
+-rw-r--r--   0        0        0     1853 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/nf_analysis.py
+-rw-r--r--   0        0        0       32 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/nipt/__init__.py
+-rw-r--r--   0        0        0      696 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/nipt/models.py
+-rw-r--r--   0        0        0     8106 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/nipt/nipt.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/scout/__init__.py
+-rw-r--r--   0        0        0     4009 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/scout/balsamic_config_builder.py
+-rw-r--r--   0        0        0     1491 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/scout/balsamic_umi_config_builder.py
+-rw-r--r--   0        0        0     3322 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/scout/hk_tags.py
+-rw-r--r--   0        0        0     9103 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/scout/mip_config_builder.py
+-rw-r--r--   0        0        0     3495 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/scout/rnafusion_config_builder.py
+-rw-r--r--   0        0        0     7231 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/scout/scout_config_builder.py
+-rw-r--r--   0        0        0    23146 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/scout/uploadscoutapi.py
+-rw-r--r--   0        0        0     3197 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/upload_api.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/__init__.py
+-rw-r--r--   0        0        0    28043 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/analysis.py
+-rw-r--r--   0        0        0    28188 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/balsamic.py
+-rw-r--r--   0        0        0     2700 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/balsamic_pon.py
+-rw-r--r--   0        0        0      553 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/balsamic_qc.py
+-rw-r--r--   0        0        0      556 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/balsamic_umi.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/downsample/__init__.py
+-rw-r--r--   0        0        0     3922 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/downsample/downsample.py
+-rw-r--r--   0        0        0      711 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/downsample/sbatch.py
+-rw-r--r--   0        0        0     8913 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/fastq.py
+-rw-r--r--   0        0        0    10687 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/fluffy.py
+-rw-r--r--   0        0        0      521 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/jasen.py
+-rw-r--r--   0        0        0       70 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/__init__.py
+-rw-r--r--   0        0        0      116 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/constants.py
+-rw-r--r--   0        0        0      174 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/metrics_parser/__init__.py
+-rw-r--r--   0        0        0      366 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/metrics_parser/metrics_parser.py
+-rw-r--r--   0        0        0      903 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/metrics_parser/models.py
+-rw-r--r--   0        0        0    13062 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/microsalt.py
+-rw-r--r--   0        0        0       95 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/quality_controller/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/quality_controller/models.py
+-rw-r--r--   0        0        0     5688 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/quality_controller/quality_controller.py
+-rw-r--r--   0        0        0     1217 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/quality_controller/report_generator.py
+-rw-r--r--   0        0        0     2373 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/quality_controller/result_logger.py
+-rw-r--r--   0        0        0     5641 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/quality_controller/utils.py
+-rw-r--r--   0        0        0     1220 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/utils.py
+-rw-r--r--   0        0        0    13924 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/mip.py
+-rw-r--r--   0        0        0     2991 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/mip_dna.py
+-rw-r--r--   0        0        0     2167 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/mip_rna.py
+-rw-r--r--   0        0        0    10587 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/mutant.py
+-rw-r--r--   0        0        0    35481 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/nf_analysis.py
+-rw-r--r--   0        0        0     6161 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/nf_handlers.py
+-rw-r--r--   0        0        0     6394 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/prepare_fastq.py
+-rw-r--r--   0        0        0     5988 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/raredisease.py
+-rw-r--r--   0        0        0     5214 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/rnafusion.py
+-rw-r--r--   0        0        0     4607 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/taxprofiler.py
+-rw-r--r--   0        0        0     3204 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/tomte.py
+-rw-r--r--   0        0        0      113 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/__init__.py
+-rw-r--r--   0        0        0      367 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/analysis.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/balsamic/__init__.py
+-rw-r--r--   0        0        0      459 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/balsamic/analysis.py
+-rw-r--r--   0        0        0     4550 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/balsamic/config.py
+-rw-r--r--   0        0        0     1986 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/balsamic/metrics.py
+-rw-r--r--   0        0        0    17539 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/cg_config.py
+-rw-r--r--   0        0        0     4302 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/compression_data.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/deliverables/__init__.py
+-rw-r--r--   0        0        0     5213 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/deliverables/metric_deliverables.py
+-rw-r--r--   0        0        0      243 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/delivery/delivery.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/demultiplex/__init__.py
+-rw-r--r--   0        0        0    12040 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/demultiplex/run_parameters.py
+-rw-r--r--   0        0        0      539 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/demultiplex/sbatch.py
+-rw-r--r--   0        0        0     7006 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/downsample/downsample_data.py
+-rw-r--r--   0        0        0      255 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/email.py
+-rw-r--r--   0        0        0     1046 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/fastq.py
+-rw-r--r--   0        0        0     2157 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/file_data.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/flow_cell/__init__.py
+-rw-r--r--   0        0        0    10373 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/flow_cell/flow_cell.py
+-rw-r--r--   0        0        0      317 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/flow_cell/utils.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/invoice/__init__.py
+-rw-r--r--   0        0        0     1254 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/invoice/invoice.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/lims/__init__.py
+-rw-r--r--   0        0        0     2019 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/lims/sample.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/mip/__init__.py
+-rw-r--r--   0        0        0      337 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/mip/mip_analysis.py
+-rw-r--r--   0        0        0     1564 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/mip/mip_config.py
+-rw-r--r--   0        0        0     4696 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/mip/mip_metrics_deliverables.py
+-rw-r--r--   0        0        0     2550 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/mip/mip_sample_info.py
+-rw-r--r--   0        0        0     2472 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/nf_analysis.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/observations/__init__.py
+-rw-r--r--   0        0        0      688 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/observations/input_files.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/__init__.py
+-rw-r--r--   0        0        0     2659 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/constants.py
+-rw-r--r--   0        0        0     5604 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/excel_sample.py
+-rw-r--r--   0        0        0      898 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/json_sample.py
+-rw-r--r--   0        0        0     1449 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/order.py
+-rw-r--r--   0        0        0      811 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/orderform_schema.py
+-rw-r--r--   0        0        0     4212 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/sample_base.py
+-rw-r--r--   0        0        0     9668 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/samples.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/validators/__init__.py
+-rw-r--r--   0        0        0     2300 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/validators/excel_sample_validators.py
+-rw-r--r--   0        0        0      576 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/validators/json_sample_validators.py
+-rw-r--r--   0        0        0       71 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/validators/sample_base_validators.py
+-rw-r--r--   0        0        0      101 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/qc_metrics.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/raredisease/__init__.py
+-rw-r--r--   0        0        0     1875 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/raredisease/raredisease.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/report/__init__.py
+-rw-r--r--   0        0        0     7461 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/report/metadata.py
+-rw-r--r--   0        0        0     6180 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/report/report.py
+-rw-r--r--   0        0        0     5221 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/report/sample.py
+-rw-r--r--   0        0        0     3004 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/report/validators.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/rnafusion/__init__.py
+-rw-r--r--   0        0        0     1865 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/rnafusion/rnafusion.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/scout/__init__.py
+-rw-r--r--   0        0        0     4783 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/scout/scout_load_config.py
+-rw-r--r--   0        0        0      116 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/scout/validators.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/slurm/__init__.py
+-rw-r--r--   0        0        0      617 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/slurm/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/taxprofiler/__init__.py
+-rw-r--r--   0        0        0     2443 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/taxprofiler/taxprofiler.py
+-rw-r--r--   0        0        0     1774 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/tomte/tomte.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/workflow/__init__.py
+-rw-r--r--   0        0        0      685 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/workflow/mutant.py
+-rw-r--r--   0        0        0       70 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/workflow/validators.py
+-rw-r--r--   0        0        0      842 2024-04-24 11:46:39.971723 cg-60.3.1/cg/resources/__init__.py
+-rw-r--r--   0        0        0     3493 2024-04-24 11:46:39.971723 cg-60.3.1/cg/resources/rnafusion_bundle_filenames.yaml
+-rw-r--r--   0        0        0     2434 2024-04-24 11:46:39.971723 cg-60.3.1/cg/resources/taxprofiler_bundle_filenames.yaml
+-rw-r--r--   0        0        0     3732 2024-04-24 11:46:39.971723 cg-60.3.1/cg/resources/tomte_bundle_filenames.yaml
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/__init__.py
+-rw-r--r--   0        0        0    20241 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/admin.py
+-rw-r--r--   0        0        0    22743 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/api.py
+-rw-r--r--   0        0        0     4887 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/app.py
+-rw-r--r--   0        0        0       48 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/auto.py
+-rw-r--r--   0        0        0     1184 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/config.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/dto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/dto/delivery_message/__init__.py
+-rw-r--r--   0        0        0      300 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/dto/delivery_message/delivery_message_request.py
+-rw-r--r--   0        0        0      183 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/dto/delivery_message/delivery_message_response.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/dto/orders/__init__.py
+-rw-r--r--   0        0        0      165 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/dto/orders/order_delivery_update_request.py
+-rw-r--r--   0        0        0       91 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/dto/orders/order_patch_request.py
+-rw-r--r--   0        0        0      662 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/dto/orders/orders_request.py
+-rw-r--r--   0        0        0      413 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/dto/orders/orders_response.py
+-rw-r--r--   0        0        0     2598 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/ext.py
+-rw-r--r--   0        0        0       29 2024-04-24 11:46:39.975723 cg-60.3.1/cg/server/invoices/__init__.py
+-rw-r--r--   0        0        0     4793 2024-04-24 11:46:39.975723 cg-60.3.1/cg/server/invoices/templates/invoices/index.html
+-rw-r--r--   0        0        0     8171 2024-04-24 11:46:39.975723 cg-60.3.1/cg/server/invoices/templates/invoices/invoice.html
+-rw-r--r--   0        0        0     2838 2024-04-24 11:46:39.975723 cg-60.3.1/cg/server/invoices/templates/invoices/layout.html
+-rw-r--r--   0        0        0     4956 2024-04-24 11:46:39.975723 cg-60.3.1/cg/server/invoices/templates/invoices/new.html
+-rw-r--r--   0        0        0     7708 2024-04-24 11:46:39.975723 cg-60.3.1/cg/server/invoices/views.py
+-rw-r--r--   0        0        0      354 2024-04-24 11:46:39.975723 cg-60.3.1/cg/server/templates/admin/index.html
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/analysis_service/__init__.py
+-rw-r--r--   0        0        0      482 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/analysis_service/analysis_service.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/__init__.py
+-rw-r--r--   0        0        0     2531 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/delivery_message_service.py
+-rw-r--r--   0        0        0      792 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/__init__.py
+-rw-r--r--   0        0        0     1366 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/analysis_scout_message.py
+-rw-r--r--   0        0        0      791 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/covid_message.py
+-rw-r--r--   0        0        0      189 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/delivery_message.py
+-rw-r--r--   0        0        0     1391 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/fastq_analysis_scout_message.py
+-rw-r--r--   0        0        0      535 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/fastq_message.py
+-rw-r--r--   0        0        0     1358 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/fastq_scout_message.py
+-rw-r--r--   0        0        0      604 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/microsalt_mwr_message.py
+-rw-r--r--   0        0        0      592 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/microsalt_mwx_message.py
+-rw-r--r--   0        0        0      903 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/scout_message.py
+-rw-r--r--   0        0        0      512 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/statina_message.py
+-rw-r--r--   0        0        0      779 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/utils.py
+-rw-r--r--   0        0        0     3300 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/utils.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/fastq_file_service/__init__.py
+-rw-r--r--   0        0        0      101 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/fastq_file_service/exceptions.py
+-rw-r--r--   0        0        0     1092 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/fastq_file_service/fastq_file_service.py
+-rw-r--r--   0        0        0     2991 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/fastq_file_service/utils.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/orders/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/orders/order_service/__init__.py
+-rw-r--r--   0        0        0     2684 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/orders/order_service/order_service.py
+-rw-r--r--   0        0        0     1214 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/orders/order_service/utils.py
+-rw-r--r--   0        0        0       94 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/orders/order_status_service/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/orders/order_status_service/dto/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/orders/order_status_service/dto/case_summary.py
+-rw-r--r--   0        0        0      289 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/orders/order_status_service/dto/order_summary.py
+-rw-r--r--   0        0        0     1768 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/orders/order_status_service/order_summary_service.py
+-rw-r--r--   0        0        0     1737 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/orders/order_status_service/utils.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/slurm_service/__init__.py
+-rw-r--r--   0        0        0      703 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/slurm_service/slurm_cli_service.py
+-rw-r--r--   0        0        0      242 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/slurm_service/slurm_service.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/slurm_upload_service/__init__.py
+-rw-r--r--   0        0        0      175 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/slurm_upload_service/slurm_upload_config.py
+-rw-r--r--   0        0        0     2074 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/slurm_upload_service/slurm_upload_service.py
+-rw-r--r--   0        0        0      203 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/slurm_upload_service/utils.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/__init__.py
+-rw-r--r--   0        0        0     4650 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/base.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/crud/__init__.py
+-rw-r--r--   0        0        0    13100 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/crud/create.py
+-rw-r--r--   0        0        0     2144 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/crud/delete.py
+-rw-r--r--   0        0        0    60188 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/crud/read.py
+-rw-r--r--   0        0        0     1121 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/crud/update.py
+-rw-r--r--   0        0        0     1662 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/database.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/__init__.py
+-rw-r--r--   0        0        0     5371 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_analysis_filters.py
+-rw-r--r--   0        0        0     1712 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_application_filters.py
+-rw-r--r--   0        0        0     1440 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_application_limitations_filters.py
+-rw-r--r--   0        0        0     2523 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_application_version_filters.py
+-rw-r--r--   0        0        0     1390 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_bed_filters.py
+-rw-r--r--   0        0        0     1317 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_bed_version_filters.py
+-rw-r--r--   0        0        0    10787 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_case_filters.py
+-rw-r--r--   0        0        0     3272 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_case_sample_filters.py
+-rw-r--r--   0        0        0      903 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_collaboration_filters.py
+-rw-r--r--   0        0        0     1412 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_customer_filters.py
+-rw-r--r--   0        0        0     1880 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_flow_cell_filters.py
+-rw-r--r--   0        0        0     1255 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_invoice_filters.py
+-rw-r--r--   0        0        0     2792 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_metrics_filters.py
+-rw-r--r--   0        0        0     3225 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_order_filters.py
+-rw-r--r--   0        0        0      851 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_organism_filters.py
+-rw-r--r--   0        0        0      783 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_panel_filters.py
+-rw-r--r--   0        0        0     3923 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_pool_filters.py
+-rw-r--r--   0        0        0     8660 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_sample_filters.py
+-rw-r--r--   0        0        0      731 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_user_filters.py
+-rw-r--r--   0        0        0    36844 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/models.py
+-rw-r--r--   0        0        0      593 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/store.py
+-rw-r--r--   0        0        0       30 2024-04-24 11:46:39.975723 cg-60.3.1/cg/utils/__init__.py
+-rw-r--r--   0        0        0      187 2024-04-24 11:46:39.975723 cg-60.3.1/cg/utils/calculations.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/utils/checksum/__init__.py
+-rw-r--r--   0        0        0     1579 2024-04-24 11:46:39.975723 cg-60.3.1/cg/utils/checksum/checksum.py
+-rw-r--r--   0        0        0     1655 2024-04-24 11:46:39.975723 cg-60.3.1/cg/utils/click/EnumChoice.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/utils/click/__init__.py
+-rw-r--r--   0        0        0     4910 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/commands.py
+-rw-r--r--   0        0        0     1811 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/date.py
+-rw-r--r--   0        0        0      635 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/dict.py
+-rw-r--r--   0        0        0     2111 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/dispatcher.py
+-rw-r--r--   0        0        0     1251 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/email.py
+-rw-r--r--   0        0        0      134 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/enums.py
+-rw-r--r--   0        0        0     3178 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/files.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/flask/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/flask/enum.py
+-rw-r--r--   0        0        0      233 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/flow_cell.py
+-rw-r--r--   0        0        0      834 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/time.py
+-rw-r--r--   0        0        0     1224 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/utils.py
+-rw-r--r--   0        0        0     1697 2024-04-24 11:46:39.979723 cg-60.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.979723 cg-60.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     1158 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/conftest.py
+-rw-r--r--   0        0        0      231 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/coverage/conftest.py
+-rw-r--r--   0        0        0     6188 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/coverage/test_coverage.py
+-rw-r--r--   0        0        0     1693 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/crunchy/conftest.py
+-rw-r--r--   0        0        0     5438 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/crunchy/test_compress_fastq.py
+-rw-r--r--   0        0        0     2283 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/crunchy/test_config.py
+-rw-r--r--   0        0        0    14032 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/crunchy/test_crunchy.py
+-rw-r--r--   0        0        0     9109 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/crunchy/test_spring_decompression.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/__init__.py
+-rw-r--r--   0        0        0    10079 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/conftest.py
+-rw-r--r--   0        0        0     4010 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0        0        0     7986 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/test_demultiplex_api.py
+-rw-r--r--   0        0        0     4782 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/test_index.py
+-rw-r--r--   0        0        0     9468 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/test_override_cycles_validator.py
+-rw-r--r--   0        0        0     3993 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/test_read_sample_sheet.py
+-rw-r--r--   0        0        0    12389 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/test_sample_models.py
+-rw-r--r--   0        0        0      951 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/test_sample_sheet_creator.py
+-rw-r--r--   0        0        0     3175 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/test_sample_sheet_models.py
+-rw-r--r--   0        0        0    10932 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/test_sample_sheet_validator.py
+-rw-r--r--   0        0        0     4940 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/test_translate_sample_sheet.py
+-rw-r--r--   0        0        0     1450 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/test_validate.py
+-rw-r--r--   0        0        0     5094 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/downsample/test_downsample.py
+-rw-r--r--   0        0        0     1419 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/downsample/test_downsample_utils.py
+-rw-r--r--   0        0        0     1716 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/gens/test_gens_api.py
+-rw-r--r--   0        0        0     1950 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/gt/conftest.py
+-rw-r--r--   0        0        0     4276 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/gt/test_gt_api.py
+-rw-r--r--   0        0        0     1453 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/hk/conftest.py
+-rw-r--r--   0        0        0      684 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/hk/test__getattr__.py
+-rw-r--r--   0        0        0     1593 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/hk/test_add_file.py
+-rw-r--r--   0        0        0     3523 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/hk/test_bundles.py
+-rw-r--r--   0        0        0      871 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/hk/test_core.py
+-rw-r--r--   0        0        0    31172 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/hk/test_file.py
+-rw-r--r--   0        0        0     5080 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/hk/test_version.py
+-rw-r--r--   0        0        0     1840 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/lims/conftest.py
+-rw-r--r--   0        0        0     3197 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/lims/test_api.py
+-rw-r--r--   0        0        0     1451 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/lims/test_sample_sheet.py
+-rw-r--r--   0        0        0     9223 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/loqus/conftest.py
+-rw-r--r--   0        0        0     8994 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/loqus/test_loqusdb_api.py
+-rw-r--r--   0        0        0     2439 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/madeline/conftest.py
+-rw-r--r--   0        0        0     4653 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/madeline/test_madeline.py
+-rw-r--r--   0        0        0     3328 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/mip/conftest.py
+-rw-r--r--   0        0        0     2487 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/mip/test_config_mip.py
+-rw-r--r--   0        0        0      883 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/mutacc_auto/conftest.py
+-rw-r--r--   0        0        0     2473 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/mutacc_auto/test_mutacc_auto.py
+-rw-r--r--   0        0        0    11930 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/orderform/conftest.py
+-rw-r--r--   0        0        0     9484 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/orderform/test_excel_orderform_parser.py
+-rw-r--r--   0        0        0     4351 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/orderform/test_excel_sample_schema.py
+-rw-r--r--   0        0        0     1032 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/orderform/test_json_orderform_parser.py
+-rw-r--r--   0        0        0     2474 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/orderform/test_orderform_parser.py
+-rw-r--r--   0        0        0    16002 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/orderform/validators/test_excel_sample_validators.py
+-rw-r--r--   0        0        0     3670 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/scout/conftest.py
+-rw-r--r--   0        0        0     2269 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/scout/test_get_causative_variants.py
+-rw-r--r--   0        0        0     1376 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/scout/test_get_scout_cases.py
+-rw-r--r--   0        0        0     1840 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/scout/test_scout_load_config.py
+-rw-r--r--   0        0        0     7047 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/scout/test_scout_models.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0        0        0     2639 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/sequencing_metrics_parser/conftest.py
+-rw-r--r--   0        0        0     2010 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/sequencing_metrics_parser/parsers/conftest.py
+-rw-r--r--   0        0        0     7105 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
+-rw-r--r--   0        0        0     3030 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/sequencing_metrics_parser/parsers/test_sequencing_metrics_parser_api.py
+-rw-r--r--   0        0        0     1131 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/slurm/conftest.py
+-rw-r--r--   0        0        0     4412 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/slurm/test_slurm_api.py
+-rw-r--r--   0        0        0      831 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/test_apps_environ.py
+-rw-r--r--   0        0        0      957 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/test_osticket.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/add/__init__.py
+-rw-r--r--   0        0        0     1174 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/add/test_cli_add.py
+-rw-r--r--   0        0        0     2471 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/add/test_cli_add_customer.py
+-rw-r--r--   0        0        0     6841 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/add/test_cli_add_family.py
+-rw-r--r--   0        0        0     7588 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/add/test_cli_add_relationship.py
+-rw-r--r--   0        0        0     8382 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/add/test_cli_add_sample.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/backup/__init__.py
+-rw-r--r--   0        0        0      705 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/backup/conftest.py
+-rw-r--r--   0        0        0    11101 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/backup/test_backup_command.py
+-rw-r--r--   0        0        0     6865 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/clean/conftest.py
+-rw-r--r--   0        0        0     5536 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/clean/test_balsamic_clean.py
+-rw-r--r--   0        0        0     2557 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/clean/test_clean_flow_cell.py
+-rw-r--r--   0        0        0     1830 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/clean/test_clean_hk_bundle_files.py
+-rw-r--r--   0        0        0     2098 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/clean/test_hk_bundle_files.py
+-rw-r--r--   0        0        0     4610 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/clean/test_hk_case_bundle_files.py
+-rw-r--r--   0        0        0     3585 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/clean/test_microbial_clean.py
+-rw-r--r--   0        0        0     1881 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/clean/test_rsync_past_run_dirs.py
+-rw-r--r--   0        0        0     9707 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/compress/conftest.py
+-rw-r--r--   0        0        0     7709 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/compress/test_cli_compress_fastq.py
+-rw-r--r--   0        0        0     1416 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/compress/test_cli_decompress_spring.py
+-rw-r--r--   0        0        0     5205 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/compress/test_compress_helpers.py
+-rw-r--r--   0        0        0     1239 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/compress/test_store_fastq.py
+-rw-r--r--   0        0        0     7558 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/conftest.py
+-rw-r--r--   0        0        0    12747 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/delete/test_cli_delete_case.py
+-rw-r--r--   0        0        0     1873 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/delete/test_cli_delete_cases.py
+-rw-r--r--   0        0        0     3794 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/deliver/conftest.py
+-rw-r--r--   0        0        0     4428 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/deliver/test_deliver_base.py
+-rw-r--r--   0        0        0     1166 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/deliver/test_rsync_base.py
+-rw-r--r--   0        0        0     8569 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/deliver/test_run_deliver_cmd.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/demultiplex/__init__.py
+-rw-r--r--   0        0        0     5109 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0        0        0     4773 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/demultiplex/test_demultiplex_flowcell.py
+-rw-r--r--   0        0        0     1607 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/demultiplex/test_finish_demux.py
+-rw-r--r--   0        0        0     2989 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/demultiplex/test_validate_sample_sheet.py
+-rw-r--r--   0        0        0     4423 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/demultiplex/test_verify_syncing.py
+-rw-r--r--   0        0        0     1585 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/downsample/test_cli_downsample.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/generate/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/generate/report/__init__.py
+-rw-r--r--   0        0        0     1622 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/generate/report/conftest.py
+-rw-r--r--   0        0        0     2477 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/generate/report/test_cli_delivery_report.py
+-rw-r--r--   0        0        0     2760 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/generate/report/test_utils.py
+-rw-r--r--   0        0        0      563 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/generate/test_cli_base.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/get/__init__.py
+-rw-r--r--   0        0        0      863 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/get/test_cli_get.py
+-rw-r--r--   0        0        0     1526 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/get/test_cli_get_analysis.py
+-rw-r--r--   0        0        0     1242 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/get/test_cli_get_case.py
+-rw-r--r--   0        0        0     6208 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/get/test_cli_get_flow_cell.py
+-rw-r--r--   0        0        0     8835 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/get/test_cli_get_sample.py
+-rw-r--r--   0        0        0     1364 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/set/conftest.py
+-rw-r--r--   0        0        0     7311 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/set/test_cli_set_case.py
+-rw-r--r--   0        0        0     1460 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/set/test_cli_set_cases.py
+-rw-r--r--   0        0        0     2016 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/set/test_cli_set_flowcell.py
+-rw-r--r--   0        0        0     1685 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/set/test_cli_set_list_keys.py
+-rw-r--r--   0        0        0    12450 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/set/test_cli_set_sample.py
+-rw-r--r--   0        0        0     6124 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/set/test_cli_set_samples.py
+-rw-r--r--   0        0        0     6934 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/store/test_store.py
+-rw-r--r--   0        0        0     2332 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/test_base.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/__init__.py
+-rw-r--r--   0        0        0    10057 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/conftest.py
+-rw-r--r--   0        0        0     2295 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/test_cli_scout.py
+-rw-r--r--   0        0        0     1789 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/test_cli_upload.py
+-rw-r--r--   0        0        0      971 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/test_cli_upload_auto.py
+-rw-r--r--   0        0        0     1669 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/test_cli_upload_delivery_report.py
+-rw-r--r--   0        0        0      895 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/test_cli_upload_fastq.py
+-rw-r--r--   0        0        0     1199 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/test_cli_upload_genotype.py
+-rw-r--r--   0        0        0      694 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/test_cli_upload_gens.py
+-rw-r--r--   0        0        0     9965 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/test_cli_upload_nipt.py
+-rw-r--r--   0        0        0     4684 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/test_cli_upload_nipt_ftp.py
+-rw-r--r--   0        0        0     1839 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/test_cli_upload_nipt_statina.py
+-rw-r--r--   0        0        0     6177 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/test_cli_upload_observations.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/__init__.py
+-rw-r--r--   0        0        0    30612 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/balsamic/conftest.py
+-rw-r--r--   0        0        0    13938 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
+-rw-r--r--   0        0        0     7957 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/balsamic/test_compound_commands.py
+-rw-r--r--   0        0        0     2336 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/balsamic/test_link.py
+-rw-r--r--   0        0        0     3554 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/balsamic/test_report_deliver.py
+-rw-r--r--   0        0        0     6209 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/balsamic/test_run.py
+-rw-r--r--   0        0        0     6934 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/balsamic/test_store_housekeeper.py
+-rw-r--r--   0        0        0     8458 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/fastq/__init__.py
+-rw-r--r--   0        0        0     2298 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/fastq/test_fastq_base.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0        0        0     5237 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/fluffy/conftest.py
+-rw-r--r--   0        0        0     5687 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
+-rw-r--r--   0        0        0     3302 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/fluffy/test_cli_link.py
+-rw-r--r--   0        0        0     1896 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/fluffy/test_cli_run.py
+-rw-r--r--   0        0        0     2968 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/fluffy/test_cli_start.py
+-rw-r--r--   0        0        0     7815 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/fluffy/test_cli_store.py
+-rw-r--r--   0        0        0     2775 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/microsalt/conftest.py
+-rw-r--r--   0        0        0     6926 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/microsalt/test_microsalt_case_config.py
+-rw-r--r--   0        0        0     1000 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/microsalt/test_microsalt_run.py
+-rw-r--r--   0        0        0     6544 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/conftest.py
+-rw-r--r--   0        0        0     7011 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_base.py
+-rw-r--r--   0        0        0     1542 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
+-rw-r--r--   0        0        0      431 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_dna_link.py
+-rw-r--r--   0        0        0     2108 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py
+-rw-r--r--   0        0        0     1273 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
+-rw-r--r--   0        0        0     3595 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_dna_run.py
+-rw-r--r--   0        0        0     3884 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_dna_start.py
+-rw-r--r--   0        0        0     1004 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
+-rw-r--r--   0        0        0      527 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_rna_link.py
+-rw-r--r--   0        0        0      716 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_rna_run.py
+-rw-r--r--   0        0        0     8559 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_store.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/nf_analysis/__init__.py
+-rw-r--r--   0        0        0     7365 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_config_case.py
+-rw-r--r--   0        0        0     3831 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py
+-rw-r--r--   0        0        0     5087 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py
+-rw-r--r--   0        0        0     9211 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_run.py
+-rw-r--r--   0        0        0     2994 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_start.py
+-rw-r--r--   0        0        0     9877 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_store.py
+-rw-r--r--   0        0        0    10373 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py
+-rw-r--r--   0        0        0      978 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/raredisease/__init__.py
+-rw-r--r--   0        0        0     3940 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py
+-rw-r--r--   0        0        0      921 2024-04-24 11:46:39.991723 cg-60.3.1/tests/cli/workflow/test_cli_workflow.py
+-rw-r--r--   0        0        0     4310 2024-04-24 11:46:39.991723 cg-60.3.1/tests/cli/workflow/test_cli_workflow_clean.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/clients/arnold/__init__.py
+-rw-r--r--   0        0        0     1080 2024-04-24 11:46:39.991723 cg-60.3.1/tests/clients/arnold/conftest.py
+-rw-r--r--   0        0        0     1503 2024-04-24 11:46:39.991723 cg-60.3.1/tests/clients/arnold/test_arnold_api_client.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/clients/janus/__init__.py
+-rw-r--r--   0        0        0     2381 2024-04-24 11:46:39.991723 cg-60.3.1/tests/clients/janus/conftest.py
+-rw-r--r--   0        0        0     1716 2024-04-24 11:46:39.991723 cg-60.3.1/tests/clients/janus/test_janus_api_client.py
+-rw-r--r--   0        0        0   133089 2024-04-24 11:46:39.991723 cg-60.3.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/delivery_fixtures/__init__.py
+-rw-r--r--   0        0        0     2653 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py
+-rw-r--r--   0        0        0     4972 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/delivery_fixtures/context_fixtures.py
+-rw-r--r--   0        0        0     1494 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/delivery_fixtures/path_fixtures.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/__init__.py
+-rw-r--r--   0        0        0     4702 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py
+-rw-r--r--   0        0        0     6152 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py
+-rw-r--r--   0        0        0    22442 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py
+-rw-r--r--   0        0        0     3699 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py
+-rw-r--r--   0        0        0     6000 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py
+-rw-r--r--   0        0        0     6514 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py
+-rw-r--r--   0        0        0     1304 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/timestamp_fixtures.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
+-rw-r--r--   0        0        0    14644 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
+-rw-r--r--   0        0        0    15921 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/ADM2.cram
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/ADM3.cram
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/adm1.cram
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/adm1.mt.bam
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/multiqc.html
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/report.pdf
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/smn.vcf
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/snv.vcf
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/snv_research.vcf
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/str.vcf
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/sv.vcf
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/sv_research.vcf
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
+-rw-r--r--   0        0        0       70 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/nf-analysis/pipeline_params.config
+-rw-r--r--   0        0        0      195 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/nf-analysis/pipeline_resource_optimisation.config
+-rw-r--r--   0        0        0      195 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/nf-analysis/platform.config
+-rw-r--r--   0        0        0     8173 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/raredisease/multiqc_data.json
+-rw-r--r--   0        0        0    20005 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml
+-rw-r--r--   0        0        0     5497 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/rnafusion/multiqc_data.json
+-rw-r--r--   0        0        0    12499 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml
+-rw-r--r--   0        0        0     2873 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/sample_coverage.bed
+-rw-r--r--   0        0        0     6506 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/taxprofiler/multiqc_data.json
+-rw-r--r--   0        0        0    10513 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0     5771 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/tomte/multiqc_data.json
+-rw-r--r--   0        0        0    14859 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml
+-rw-r--r--   0        0        0    10961 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/balsamic/case/config.json
+-rw-r--r--   0        0        0     3465 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/balsamic/case/metadata.yml
+-rw-r--r--   0        0        0       63 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/balsamic/case/metadata_directory.yml
+-rw-r--r--   0        0        0      165 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
+-rw-r--r--   0        0        0     2705 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
+-rw-r--r--   0        0        0      692 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/crunchy/spring_metadata.json
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0      412 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      484 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      658 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/demuxcomplete.txt
+-rw-r--r--   0        0        0     1757 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0        0        0        7 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0     6034 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0        0        0     1172 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0        0        0        7 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_1.fastq.gz
+-rw-r--r--   0        0        0        7 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_2.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0      345 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      650 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      896 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0      602 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/demuxcomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0      288 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      361 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      414 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/demuxcomplete.txt
+-rw-r--r--   0        0        0      315 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      434 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0     8624 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml
+-rw-r--r--   0        0        0      568 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0      220 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      463 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      622 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0      345 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      650 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      896 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0      619 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0      303 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      364 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      427 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/demuxcomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0     4439 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0        0        0     1172 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0     5127 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
+-rw-r--r--   0        0        0       43 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz
+-rw-r--r--   0        0        0       67 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz.md5
+-rw-r--r--   0        0        0   338370 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz
+-rw-r--r--   0        0        0       67 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz.md5
+-rw-r--r--   0        0        0   338349 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/CopyComplete.txt
+-rw-r--r--   0        0        0     2126 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json
+-rw-r--r--   0        0        0     1827 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json
+-rw-r--r--   0        0        0       90 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/README.txt
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAComplete.txt
+-rw-r--r--   0        0        0     6895 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml
+-rw-r--r--   0        0        0       37 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead1Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead2Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead3Complete.txt
+-rw-r--r--   0        0        0    24755 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml
+-rw-r--r--   0        0        0      692 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
+-rw-r--r--   0        0        0      724 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0       61 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SequencingComplete.txt
+-rw-r--r--   0        0        0     5775 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/CopyComplete.txt
+-rw-r--r--   0        0        0     2282 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json
+-rw-r--r--   0        0        0     1632 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json
+-rw-r--r--   0        0        0       75 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/README.txt
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAComplete.txt
+-rw-r--r--   0        0        0     6912 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml
+-rw-r--r--   0        0        0       36 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead1Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead2Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead3Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead4Complete.txt
+-rw-r--r--   0        0        0    24814 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml
+-rw-r--r--   0        0        0      814 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv
+-rw-r--r--   0        0        0      660 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0       61 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SequencingComplete.txt
+-rw-r--r--   0        0        0     5853 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/CopyComplete.txt
+-rw-r--r--   0        0        0    21848 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json
+-rw-r--r--   0        0        0    15512 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json
+-rw-r--r--   0        0        0       79 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/README.txt
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RTAComplete.txt
+-rw-r--r--   0        0        0      756 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml
+-rw-r--r--   0        0        0     4118 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv
+-rw-r--r--   0        0        0     1408 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0     5326 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/CopyComplete.txt
+-rw-r--r--   0        0        0    15041 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json
+-rw-r--r--   0        0        0    10649 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json
+-rw-r--r--   0        0        0       80 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/README.txt
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RTAComplete.txt
+-rw-r--r--   0        0        0      755 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml
+-rw-r--r--   0        0        0     2878 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv
+-rw-r--r--   0        0        0      928 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0     5359 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CopyComplete.txt
+-rw-r--r--   0        0        0    27887 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv
+-rw-r--r--   0        0        0   141870 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json
+-rwxr-xr-x   0        0        0   122682 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json
+-rw-r--r--   0        0        0      243 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/README.txt
+-rw-r--r--   0        0        0    28230 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTAComplete.txt
+-rw-r--r--   0        0        0    94426 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml
+-rw-r--r--   0        0        0     5819 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/SequenceComplete.txt
+-rw-r--r--   0        0        0     1757 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0        0        0     1757 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stdout
+-rw-r--r--   0        0        0       12 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/README.txt
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RTAComplete.txt
+-rw-r--r--   0        0        0     5945 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml
+-rw-r--r--   0        0        0      260 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/copycomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/demuxstarted.txt
+-rw-r--r--   0        0        0     1757 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0        0        0     1757 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout
+-rw-r--r--   0        0        0    47522 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json
+-rw-r--r--   0        0        0       12 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/README.txt
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0        0        0     6666 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0        0        0      254 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/copycomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/delivery.txt
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/demuxstarted.txt
+-rwxr-xr-x   0        0        0    47434 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CopyComplete.txt
+-rw-r--r--   0        0        0    10950 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv
+-rw-r--r--   0        0        0      225 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/Manifest.tsv
+-rw-r--r--   0        0        0       55 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/README.txt
+-rwxr-xr-x   0        0        0     2493 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg
+-rwxr-xr-x   0        0        0        1 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAComplete.txt
+-rwxr-xr-x   0        0        0        2 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAExited.txt
+-rwxr-xr-x   0        0        0      730 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml
+-rwxr-xr-x   0        0        0    79277 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml
+-rwxr-xr-x   0        0        0     2694 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
+-rw-r--r--   0        0        0    10950 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
+-rw-r--r--   0        0        0      619 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0        0        0       12 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/README.txt
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0        0        0      399 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CopyComplete.txt
+-rw-r--r--   0        0        0     4941 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv
+-rwxr-xr-x   0        0        0    20050 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stderr
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stdout
+-rw-r--r--   0        0        0      244 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/README.txt
+-rw-r--r--   0        0        0     6391 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTAComplete.txt
+-rw-r--r--   0        0        0    16428 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml
+-rw-r--r--   0        0        0     6728 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
+-rw-r--r--   0        0        0     5127 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SequenceComplete.txt
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/demuxstarted.txt
+-rw-r--r--   0        0        0      133 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/README.txt
+-rw-r--r--   0        0        0      724 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
+-rw-r--r--   0        0        0     5775 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
+-rw-r--r--   0        0        0      124 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/180509_D00450_0598_BHGYFNBCX2/README.txt
+-rw-r--r--   0        0        0      310 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/README.txt
+-rw-r--r--   0        0        0     5819 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
+-rw-r--r--   0        0        0      122 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/README.txt
+-rwxr-xr-x   0        0        0     2694 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
+-rw-r--r--   0        0        0      311 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/README.txt
+-rw-r--r--   0        0        0     6728 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0        0        0      399 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
+-rw-r--r--   0        0        0      399 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_0.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_1.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/final_summary_PAS86456_72d9fceb_8a4fd683.txt
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_0.pod5
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_1.pod5
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_0.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_1.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/final_summary_PAS97781_595b5663_efc7f02e.txt
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_0.pod5
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_1.pod5
+-rw-r--r--   0        0        0   111989 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
+-rw-r--r--   0        0        0     5319 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml
+-rw-r--r--   0        0        0     5944 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
+-rwxr-xr-x   0        0        0     2481 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
+-rwxr-xr-x   0        0        0     2474 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml
+-rw-r--r--   0        0        0     5899 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
+-rw-r--r--   0        0        0     4941 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv
+-rw-r--r--   0        0        0    10950 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/demultiplexing/spring/dummy_run_001.spring
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/demultiplexing/spring/dummy_run_002.spring
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/demultiplexing/spring/dummy_spring_meta_data.json
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
+-rw-r--r--   0        0        0     5554 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/fluffy/SampleSheet.csv
+-rw-r--r--   0        0        0      901 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/fluffy/deliverables.yaml
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/fluffy/multiqc_report.html
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/fluffy/summary.csv
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/gt/yellowhog.bcf
+-rw-r--r--   0        0        0     5114 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/madeline/madeline.xml
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/case_file.txt
+-rw-r--r--   0        0        0     3241 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0    21811 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/dna/store/case_config.yaml
+-rw-r--r--   0        0        0    23364 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
+-rw-r--r--   0        0        0    37367 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
+-rw-r--r--   0        0        0       16 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
+-rw-r--r--   0        0        0       16 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0       16 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
+-rw-r--r--   0        0        0      123 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
+-rw-r--r--   0        0        0    62741 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
+-rw-r--r--   0        0        0    11242 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/rna/case_config.yaml
+-rw-r--r--   0        0        0    12164 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
+-rw-r--r--   0        0        0     5231 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
+-rw-r--r--   0        0        0     9774 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/rna/store/case_config.yaml
+-rw-r--r--   0        0        0     4624 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
+-rw-r--r--   0        0        0    13666 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/sample_file.txt
+-rw-r--r--   0        0        0     1885 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/scout/643594.config.yaml
+-rw-r--r--   0        0        0     6027 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/scout/case_export.json
+-rw-r--r--   0        0        0     9349 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/scout/export_causatives.json
+-rw-r--r--   0        0        0     1315 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/scout/none_case_export.json
+-rw-r--r--   0        0        0     3518 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/scout/other_sex_case.json
+-rw-r--r--   0        0        0     8874 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/scout/panel_export.bed
+-rw-r--r--   0        0        0     4169 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/scout/panel_export.csv
+-rw-r--r--   0        0        0      619 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/SampleSheet.csv
+-rw-r--r--   0        0        0    63569 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0    42478 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0    69708 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0       42 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/shipping/scout-deploy.yaml
+-rw-r--r--   0        0        0     1036 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/cgweb_orders/balsamic.json
+-rw-r--r--   0        0        0     1104 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/cgweb_orders/fastq.json
+-rw-r--r--   0        0        0     1313 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/cgweb_orders/metagenome.json
+-rw-r--r--   0        0        0     3038 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/cgweb_orders/microsalt.json
+-rw-r--r--   0        0        0     3705 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/cgweb_orders/mip.json
+-rw-r--r--   0        0        0     1364 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/cgweb_orders/mip_rna.json
+-rw-r--r--   0        0        0     2125 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/cgweb_orders/rml.json
+-rw-r--r--   0        0        0     1368 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/cgweb_orders/rnafusion.json
+-rw-r--r--   0        0        0     4684 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/cgweb_orders/sarscov2.json
+-rw-r--r--   0        0        0     5609 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/data/SampleSheet.csv
+-rw-r--r--   0        0        0      511 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/data/bcl_convert_sample_sheet.csv
+-rw-r--r--   0        0        0   258048 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/data/cgfixture.db
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/data/fastq.fastq.gz
+-rw-r--r--   0        0        0    49152 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/data/hkstore.db
+-rw-r--r--   0        0        0       73 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/data/yellowhog/pedigree.yaml
+-rw-r--r--   0        0        0       76 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/io/casava_five_parts.fastq.gz
+-rw-r--r--   0        0        0       90 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/io/casava_seven_parts.fastq.gz
+-rw-r--r--   0        0        0       96 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/io/casava_ten_parts.fastq.gz
+-rw-r--r--   0        0        0      153 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/io/example.csv
+-rw-r--r--   0        0        0       46 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/io/example.gz
+-rw-r--r--   0        0        0      147 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/io/example.tsv
+-rw-r--r--   0        0        0       20 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/io/example.txt
+-rw-r--r--   0        0        0       20 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/io/example2.txt
+-rw-r--r--   0        0        0      582 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/io/example_json.json
+-rw-r--r--   0        0        0      103 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/io/example_xml.xml
+-rw-r--r--   0        0        0       20 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/meta/qc_metrics/file_with_right_tags.json
+-rw-r--r--   0        0        0       20 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/meta/qc_metrics/file_without_right_tags.json
+-rw-r--r--   0        0        0   156910 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/orderforms/1508.30.balsamic.xlsx
+-rw-r--r--   0        0        0   156770 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx
+-rw-r--r--   0        0        0   156737 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx
+-rw-r--r--   0        0        0   156582 2024-04-24 11:46:40.015723 cg-60.3.1/tests/fixtures/orderforms/1508.30.fastq.xlsx
+-rw-r--r--   0        0        0   155627 2024-04-24 11:46:40.015723 cg-60.3.1/tests/fixtures/orderforms/1508.30.metagenome.xlsx
+-rw-r--r--   0        0        0   156850 2024-04-24 11:46:40.015723 cg-60.3.1/tests/fixtures/orderforms/1508.30.mip.xlsx
+-rw-r--r--   0        0        0   258580 2024-04-24 11:46:40.015723 cg-60.3.1/tests/fixtures/orderforms/1508.30.mip_rna.xlsx
+-rw-r--r--   0        0        0   258342 2024-04-24 11:46:40.015723 cg-60.3.1/tests/fixtures/orderforms/1508.30.rnafusion.xlsx
+-rw-r--r--   0        0        0    82677 2024-04-24 11:46:40.015723 cg-60.3.1/tests/fixtures/orderforms/1603.11.microbial.xlsx
+-rw-r--r--   0        0        0   149394 2024-04-24 11:46:40.015723 cg-60.3.1/tests/fixtures/orderforms/1604.17.rml.xlsx
+-rw-r--r--   0        0        0   223184 2024-04-24 11:46:40.019723 cg-60.3.1/tests/fixtures/orderforms/2184.9.sarscov2.xlsx
+-rw-r--r--   0        0        0    18639 2024-04-24 11:46:40.019723 cg-60.3.1/tests/fixtures/orderforms/NIPT-json.json
+-rw-r--r--   0        0        0     6052 2024-04-24 11:46:40.019723 cg-60.3.1/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
+-rw-r--r--   0        0        0     6611 2024-04-24 11:46:40.019723 cg-60.3.1/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
+-rw-r--r--   0        0        0     1417 2024-04-24 11:46:40.019723 cg-60.3.1/tests/fixtures/report/case_data.json
+-rw-r--r--   0        0        0     1109 2024-04-24 11:46:40.019723 cg-60.3.1/tests/fixtures/report/lims_exported_samples.json
+-rw-r--r--   0        0        0     1562 2024-04-24 11:46:40.019723 cg-60.3.1/tests/fixtures/report/lims_family.json
+-rw-r--r--   0        0        0     3296 2024-04-24 11:46:40.019723 cg-60.3.1/tests/io/conftest.py
+-rw-r--r--   0        0        0      431 2024-04-24 11:46:40.019723 cg-60.3.1/tests/io/test_io_config.py
+-rw-r--r--   0        0        0     8639 2024-04-24 11:46:40.019723 cg-60.3.1/tests/io/test_io_controller.py
+-rw-r--r--   0        0        0     3877 2024-04-24 11:46:40.019723 cg-60.3.1/tests/io/test_io_csv.py
+-rw-r--r--   0        0        0      482 2024-04-24 11:46:40.019723 cg-60.3.1/tests/io/test_io_gzip.py
+-rw-r--r--   0        0        0     1779 2024-04-24 11:46:40.019723 cg-60.3.1/tests/io/test_io_json.py
+-rw-r--r--   0        0        0     2914 2024-04-24 11:46:40.019723 cg-60.3.1/tests/io/test_io_txt.py
+-rw-r--r--   0        0        0     1027 2024-04-24 11:46:40.019723 cg-60.3.1/tests/io/test_io_xml.py
+-rw-r--r--   0        0        0     2131 2024-04-24 11:46:40.019723 cg-60.3.1/tests/io/test_io_yaml.py
+-rw-r--r--   0        0        0     1233 2024-04-24 11:46:40.019723 cg-60.3.1/tests/io/test_validate_path.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/archive/__init__.py
+-rw-r--r--   0        0        0    13131 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/archive/conftest.py
+-rw-r--r--   0        0        0    16858 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/archive/test_archive_api.py
+-rw-r--r--   0        0        0    10246 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/archive/test_archive_cli.py
+-rw-r--r--   0        0        0    15766 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/archive/test_archiving.py
+-rw-r--r--   0        0        0     3807 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/backup/conftest.py
+-rw-r--r--   0        0        0    26368 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/backup/test_meta_backup.py
+-rw-r--r--   0        0        0    10055 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/backup/test_meta_pdc.py
+-rw-r--r--   0        0        0    12546 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/clean/conftest.py
+-rw-r--r--   0        0        0    16944 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/clean/test_clean_flow_cells_api.py
+-rw-r--r--   0        0        0     2286 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/clean/test_clean_retrieved_spring_files.py
+-rw-r--r--   0        0        0     7691 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/compress/conftest.py
+-rw-r--r--   0        0        0     7961 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/compress/test_clean_fastq.py
+-rw-r--r--   0        0        0     1778 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/compress/test_compress_files.py
+-rw-r--r--   0        0        0     3644 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/compress/test_compress_meta_fastq.py
+-rw-r--r--   0        0        0     1180 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/compress/test_decompress_spring_meta.py
+-rw-r--r--   0        0        0     6902 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/compress/test_meta_compress_update_hk.py
+-rw-r--r--   0        0        0     8207 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/deliver/__init__.py
+-rw-r--r--   0        0        0     3471 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/deliver/conftest.py
+-rw-r--r--   0        0        0     5533 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/deliver/test_deliver_ticket.py
+-rw-r--r--   0        0        0    10277 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/deliver/test_delivery_api.py
+-rw-r--r--   0        0        0     1057 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/deliver/test_fastq_path_generator.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/delivery/__init__.py
+-rw-r--r--   0        0        0    16660 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/delivery/test_delivery_api.py
+-rw-r--r--   0        0        0     8729 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/demultiplex/conftest.py
+-rw-r--r--   0        0        0     5382 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/demultiplex/test_combine_sequencing_metrics.py
+-rw-r--r--   0        0        0     8339 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/demultiplex/test_demux_post_processing.py
+-rw-r--r--   0        0        0    12330 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/demultiplex/test_housekeeper_storage_functions.py
+-rw-r--r--   0        0        0     4392 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/demultiplex/test_status_db_storage_functions.py
+-rw-r--r--   0        0        0    22705 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/demultiplex/test_utils.py
+-rw-r--r--   0        0        0     6193 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/demultiplex/test_validation.py
+-rw-r--r--   0        0        0     4943 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/encryption/conftest.py
+-rw-r--r--   0        0        0    18133 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/encryption/test_encryption.py
+-rw-r--r--   0        0        0     3122 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/observations/conftest.py
+-rw-r--r--   0        0        0    16164 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/observations/test_meta_upload_observations.py
+-rw-r--r--   0        0        0     4974 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/orders/conftest.py
+-rw-r--r--   0        0        0     1749 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/orders/test_PoolSubmitter_validate_order.py
+-rw-r--r--   0        0        0     1470 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
+-rw-r--r--   0        0        0     1768 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/orders/test_SarsCov2Submitter_store_order.py
+-rw-r--r--   0        0        0     2032 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
+-rw-r--r--   0        0        0    19783 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/orders/test_meta_orders_api.py
+-rw-r--r--   0        0        0     7086 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/orders/test_meta_orders_lims.py
+-rw-r--r--   0        0        0    29515 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/orders/test_meta_orders_status.py
+-rw-r--r--   0        0        0     1677 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/orders/test_rnafusion_submitter.py
+-rw-r--r--   0        0        0     1068 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/orders/test_ticket_handler.py
+-rw-r--r--   0        0        0     4336 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/qc_metrics/conftest.py
+-rw-r--r--   0        0        0     1972 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/qc_metrics/test_collect_qc_metrics.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/report/__init__.py
+-rw-r--r--   0        0        0     6512 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/report/conftest.py
+-rw-r--r--   0        0        0      434 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/report/helper.py
+-rw-r--r--   0        0        0     2604 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/report/test_balsamic_api.py
+-rw-r--r--   0        0        0     4056 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/report/test_field_validators.py
+-rw-r--r--   0        0        0     2858 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/report/test_mip_dna_api.py
+-rw-r--r--   0        0        0    16042 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/report/test_report_api.py
+-rw-r--r--   0        0        0     1365 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/report/test_rnafusion_api.py
+-rw-r--r--   0        0        0     1250 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/report/test_tomte_api.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/rsync/__init__.py
+-rw-r--r--   0        0        0      916 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/rsync/conftest.py
+-rw-r--r--   0        0        0     9442 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/rsync/test_rsync.py
+-rw-r--r--   0        0        0     3147 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/test_invoice.py
+-rw-r--r--   0        0        0     1220 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/transfer/conftest.py
+-rw-r--r--   0        0        0     9892 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/transfer/test_external_data.py
+-rw-r--r--   0        0        0     4395 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/transfer/test_meta_transfer_lims.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/__init__.py
+-rw-r--r--   0        0        0     2210 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/balsamic/test_balsamic.py
+-rw-r--r--   0        0        0     4002 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/gisaid/__init__.py
+-rw-r--r--   0        0        0     2557 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/gisaid/fixtures/four_samples.csv
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
+-rw-r--r--   0        0        0      211 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
+-rw-r--r--   0        0        0      371 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/mutacc/__init__.py
+-rw-r--r--   0        0        0     3684 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/mutacc/conftest.py
+-rw-r--r--   0        0        0     4188 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
+-rw-r--r--   0        0        0     1149 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/nipt/conftest.py
+-rw-r--r--   0        0        0     1683 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/nipt/test_models.py
+-rw-r--r--   0        0        0     1242 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/nipt/test_nipt_upload_api.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/scout/__init__.py
+-rw-r--r--   0        0        0    23954 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/scout/conftest.py
+-rw-r--r--   0        0        0     4734 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/scout/test_generate_load_config.py
+-rw-r--r--   0        0        0     4182 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/scout/test_meta_upload_scoutapi.py
+-rw-r--r--   0        0        0    33260 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
+-rw-r--r--   0        0        0     7372 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/scout/test_scout_config_builder.py
+-rw-r--r--   0        0        0     2511 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/test_meta_upload_coverage.py
+-rw-r--r--   0        0        0     1473 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/test_upload_api.py
+-rw-r--r--   0        0        0     2547 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/test_upload_genotypes_api.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/__init__.py
+-rw-r--r--   0        0        0    10262 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/conftest.py
+-rw-r--r--   0        0        0     3652 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/microsalt/conftest.py
+-rw-r--r--   0        0        0      318 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/microsalt/test_parsing_metrics.py
+-rw-r--r--   0        0        0     3714 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/microsalt/test_quality_controller.py
+-rw-r--r--   0        0        0    14367 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/microsalt/test_quality_controller_utils.py
+-rw-r--r--   0        0        0      825 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/microsalt/test_report_generation.py
+-rw-r--r--   0        0        0    20848 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/test_analysis.py
+-rw-r--r--   0        0        0     7934 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/test_balsamic.py
+-rw-r--r--   0        0        0     3034 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/test_fastq.py
+-rw-r--r--   0        0        0     1532 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/test_microsalt.py
+-rw-r--r--   0        0        0     2721 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/test_nf_analysis.py
+-rw-r--r--   0        0        0     7741 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/test_prepare_fastq_api.py
+-rw-r--r--   0        0        0     1920 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/test_raredisease.py
+-rw-r--r--   0        0        0     1674 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/test_rnafusion.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/__init__.py
+-rw-r--r--   0        0        0     1168 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/balsamic_analysis_mock.py
+-rw-r--r--   0        0        0     3500 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/crunchy.py
+-rw-r--r--   0        0        0    21778 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/hk_mock.py
+-rw-r--r--   0        0        0     4106 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/limsmock.py
+-rw-r--r--   0        0        0      572 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/madeline.py
+-rw-r--r--   0        0        0     1297 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/mip_analysis_mock.py
+-rw-r--r--   0        0        0     1525 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/osticket.py
+-rw-r--r--   0        0        0     3239 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/process_mock.py
+-rw-r--r--   0        0        0     4713 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/report.py
+-rw-r--r--   0        0        0     3915 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/scout.py
+-rw-r--r--   0        0        0      750 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/store_model.py
+-rw-r--r--   0        0        0     1532 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/tb_mock.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.023723 cg-60.3.1/tests/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.023723 cg-60.3.1/tests/models/balsamic/__init__.py
+-rw-r--r--   0        0        0     1194 2024-04-24 11:46:40.023723 cg-60.3.1/tests/models/balsamic/conftest.py
+-rw-r--r--   0        0        0     1030 2024-04-24 11:46:40.023723 cg-60.3.1/tests/models/balsamic/test_balsamic_analysis.py
+-rw-r--r--   0        0        0     1050 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/demultiplexing/__init__.py
+-rw-r--r--   0        0        0      284 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/demultiplexing/conftest.py
+-rw-r--r--   0        0        0    11446 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/demultiplexing/test_run_parameters.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/downsample/__init__.py
+-rw-r--r--   0        0        0     2096 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/downsample/test_down_sample_meta_data.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/flow_cell/__init__.py
+-rw-r--r--   0        0        0     6659 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/flow_cell/test_flowcell_model.py
+-rw-r--r--   0        0        0     6637 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/mip/conftest.py
+-rw-r--r--   0        0        0     1239 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/mip/test_mip_analysis.py
+-rw-r--r--   0        0        0     2348 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/mip/test_mip_config.py
+-rw-r--r--   0        0        0     6392 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/mip/test_mip_metrics_deliverables.py
+-rw-r--r--   0        0        0     3959 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/mip/test_mip_sample_info.py
+-rw-r--r--   0        0        0     3314 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/nextflow/test_nextflow_deliver.py
+-rw-r--r--   0        0        0     1602 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/observations/conftest.py
+-rw-r--r--   0        0        0     2579 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/observations/test_observations_input_files.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/report/__init__.py
+-rw-r--r--   0        0        0     7327 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/report/test_validators.py
+-rw-r--r--   0        0        0     3855 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/rnafusion/test_rnafusion_sample.py
+-rw-r--r--   0        0        0     1374 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/test_cg_models.py
+-rw-r--r--   0        0        0      990 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/test_compression_data.py
+-rw-r--r--   0        0        0      729 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/test_fastq.py
+-rw-r--r--   0        0        0     2860 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/test_file_data.py
+-rw-r--r--   0        0        0     4539 2024-04-24 11:46:40.027723 cg-60.3.1/tests/server/conftest.py
+-rw-r--r--   0        0        0     3135 2024-04-24 11:46:40.027723 cg-60.3.1/tests/server/endpoints/test_delivery_message_endpoint.py
+-rw-r--r--   0        0        0     3239 2024-04-24 11:46:40.027723 cg-60.3.1/tests/server/endpoints/test_orders_endpoint.py
+-rw-r--r--   0        0        0      271 2024-04-24 11:46:40.027723 cg-60.3.1/tests/server/test_server_auto.py
+-rw-r--r--   0        0        0     1047 2024-04-24 11:46:40.027723 cg-60.3.1/tests/services/fastq_file_service/conftest.py
+-rw-r--r--   0        0        0     3634 2024-04-24 11:46:40.027723 cg-60.3.1/tests/services/fastq_file_service/test_fastq_file_service.py
+-rw-r--r--   0        0        0     4861 2024-04-24 11:46:40.027723 cg-60.3.1/tests/services/orders/order_status_service/conftest.py
+-rw-r--r--   0        0        0     2865 2024-04-24 11:46:40.027723 cg-60.3.1/tests/services/orders/order_status_service/test_order_summary_service.py
+-rw-r--r--   0        0        0      318 2024-04-24 11:46:40.027723 cg-60.3.1/tests/small_helpers.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/api/__init__.py
+-rw-r--r--   0        0        0     2984 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/api/conftest.py
+-rw-r--r--   0        0        0     1557 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/api/test_base.py
+-rw-r--r--   0        0        0    20096 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/add/__init__.py
+-rw-r--r--   0        0        0     1497 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/add/test_store_add_application_version.py
+-rw-r--r--   0        0        0     3958 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/add/test_store_add_base.py
+-rw-r--r--   0        0        0     2502 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/add/test_store_add_customer.py
+-rw-r--r--   0        0        0     1640 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/add/test_store_add_flow_celll.py
+-rw-r--r--   0        0        0    12212 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/delete/__init__.py
+-rw-r--r--   0        0        0     5541 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/delete/test_delete.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/read/__init__.py
+-rw-r--r--   0        0        0    57211 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/read/test_read.py
+-rw-r--r--   0        0        0     5461 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/read/test_read_analyses_to_clean.py
+-rw-r--r--   0        0        0     3553 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/read/test_read_analyses_to_delivery_report.py
+-rw-r--r--   0        0        0    18463 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/read/test_read_analysis.py
+-rw-r--r--   0        0        0     2743 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/read/test_read_application_version.py
+-rw-r--r--   0        0        0     1105 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/read/test_read_customer.py
+-rw-r--r--   0        0        0     1530 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/read/test_read_pool.py
+-rw-r--r--   0        0        0    21503 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/read/test_read_sample.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/update/__init__.py
+-rw-r--r--   0        0        0      737 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/update/test_update.py
+-rw-r--r--   0        0        0    11693 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_analyses_filters.py
+-rw-r--r--   0        0        0     3397 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_application_filters.py
+-rw-r--r--   0        0        0     2073 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_application_limitations_filters.py
+-rw-r--r--   0        0        0    10452 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_application_version_filters.py
+-rw-r--r--   0        0        0     2804 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_bed_filters.py
+-rw-r--r--   0        0        0     2362 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_bed_version_filters.py
+-rw-r--r--   0        0        0     3495 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_case_sample_filters.py
+-rw-r--r--   0        0        0    39100 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_cases_filters.py
+-rw-r--r--   0        0        0     1345 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_collaboration_filters.py
+-rw-r--r--   0        0        0     2482 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_customer_filters.py
+-rw-r--r--   0        0        0     4907 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_flow_cell_filters.py
+-rw-r--r--   0        0        0     2226 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_invoice_filters.py
+-rw-r--r--   0        0        0     5871 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_metrics_filters.py
+-rw-r--r--   0        0        0     2404 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_organism_filters.py
+-rw-r--r--   0        0        0     1804 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_panel_filters.py
+-rw-r--r--   0        0        0     8720 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_pool_filters.py
+-rw-r--r--   0        0        0    22875 2024-04-24 11:46:40.031723 cg-60.3.1/tests/store/filters/test_status_samples_filters.py
+-rw-r--r--   0        0        0     1576 2024-04-24 11:46:40.031723 cg-60.3.1/tests/store/filters/test_status_user_filters.py
+-rw-r--r--   0        0        0     2147 2024-04-24 11:46:40.031723 cg-60.3.1/tests/store/test_delivery.py
+-rw-r--r--   0        0        0     4127 2024-04-24 11:46:40.031723 cg-60.3.1/tests/store/test_store_models.py
+-rw-r--r--   0        0        0    37040 2024-04-24 11:46:40.031723 cg-60.3.1/tests/store_helpers.py
+-rw-r--r--   0        0        0     4930 2024-04-24 11:46:40.031723 cg-60.3.1/tests/test_copy_novaseqx_flow_cell.py
+-rw-r--r--   0        0        0      911 2024-04-24 11:46:40.031723 cg-60.3.1/tests/test_store_helpers.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:46:40.031723 cg-60.3.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1754 2024-04-24 11:46:40.031723 cg-60.3.1/tests/utils/conftest.py
+-rw-r--r--   0        0        0      371 2024-04-24 11:46:40.031723 cg-60.3.1/tests/utils/test_calculations.py
+-rw-r--r--   0        0        0     2920 2024-04-24 11:46:40.031723 cg-60.3.1/tests/utils/test_commands.py
+-rw-r--r--   0        0        0      953 2024-04-24 11:46:40.031723 cg-60.3.1/tests/utils/test_date.py
+-rw-r--r--   0        0        0     1508 2024-04-24 11:46:40.031723 cg-60.3.1/tests/utils/test_dict.py
+-rw-r--r--   0        0        0     7154 2024-04-24 11:46:40.031723 cg-60.3.1/tests/utils/test_dispatcher.py
+-rw-r--r--   0        0        0     4100 2024-04-24 11:46:40.031723 cg-60.3.1/tests/utils/test_files.py
+-rw-r--r--   0        0        0     1170 2024-04-24 11:46:40.031723 cg-60.3.1/tests/utils/test_time.py
+-rw-r--r--   0        0        0     2366 2024-04-24 11:46:40.031723 cg-60.3.1/tests/utils/test_utils.py
+-rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 cg-60.3.1/PKG-INFO
```

### Comparing `cg-60.3.0/README.md` & `cg-60.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/coverage/api.py` & `cg-60.3.1/cg/apps/coverage/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/crunchy/crunchy.py` & `cg-60.3.1/cg/apps/crunchy/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/crunchy/files.py` & `cg-60.3.1/cg/apps/crunchy/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/crunchy/sbatch.py` & `cg-60.3.1/cg/apps/crunchy/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/demultiplex/demultiplex_api.py` & `cg-60.3.1/cg/apps/demultiplex/demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/demultiplex/sample_sheet/api.py` & `cg-60.3.1/cg/apps/demultiplex/sample_sheet/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 import logging
 from pathlib import Path
 
 import click
 
-from cg.apps.demultiplex.sample_sheet.read_sample_sheet import (
-    get_flow_cell_samples_from_content,
-    get_sample_type_from_content,
-)
-from cg.apps.demultiplex.sample_sheet.sample_models import (
-    FlowCellSampleBcl2Fastq,
-    FlowCellSampleBCLConvert,
-)
+from cg.apps.demultiplex.sample_sheet.read_sample_sheet import get_flow_cell_samples_from_content
+from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample
 from cg.apps.demultiplex.sample_sheet.sample_sheet_creator import SampleSheetCreator
 from cg.apps.demultiplex.sample_sheet.sample_sheet_validator import SampleSheetValidator
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.apps.lims import LimsAPI
 from cg.apps.lims.sample_sheet import get_flow_cell_samples
 from cg.constants.constants import FileFormat
 from cg.constants.demultiplexing import SampleSheetBcl2FastqSections, SampleSheetBCLConvertSections
@@ -92,65 +86,42 @@
             return False
         if not flow_cell.sample_sheet_path.exists():
             LOG.error(f"Sample sheet for flow cell {flow_cell.full_name} does not exist")
             return False
         return True
 
     @staticmethod
-    def _is_sample_sheet_bcl2fastq(flow_cell: FlowCellDirectoryData) -> bool:
-        """Determine if the sample sheet from the flow cell directory is in BCL2FASTQ format."""
-        sample_sheet_content: list[list[str]] = ReadFile.get_content_from_file(
-            file_format=FileFormat.CSV, file_path=flow_cell.sample_sheet_path
-        )
-        if get_sample_type_from_content(sample_sheet_content) is not FlowCellSampleBcl2Fastq:
-            LOG.error(
-                f"Sample sheet for flow cell {flow_cell.full_name} is not a Bcl2Fastq sample sheet"
-            )
-            return False
-        return True
-
-    def _is_sample_sheet_from_flow_cell_translatable(
-        self, flow_cell: FlowCellDirectoryData
-    ) -> bool:
-        """
-        Determine if the sample sheet from the flow cell directory is translatable to BCLConvert.
-        """
-        return self._are_necessary_files_in_flow_cell(
-            flow_cell
-        ) and self._is_sample_sheet_bcl2fastq(flow_cell)
-
-    @staticmethod
     def _replace_sample_header(sample_sheet_content: list[list[str]]) -> list[list[str]]:
         """
         Replace the old sample ID header in the Bcl2Fastq sample sheet content with the BCLConvert
         formatted one.
         Raises:
             SampleSheetError: If the data header is not found in the sample sheet.
         """
         for line in sample_sheet_content:
             if SampleSheetBcl2FastqSections.Data.SAMPLE_INTERNAL_ID_BCL2FASTQ.value in line:
                 idx = line.index(
                     SampleSheetBcl2FastqSections.Data.SAMPLE_INTERNAL_ID_BCL2FASTQ.value
                 )
                 line[idx] = SampleSheetBCLConvertSections.Data.SAMPLE_INTERNAL_ID.value
                 return sample_sheet_content
-        raise SampleSheetError("Could not find data header in sample sheet")
+        raise SampleSheetError("Could not find BCL2FASTQ data header in sample sheet")
 
     def translate_sample_sheet(self, flow_cell_name: str) -> None:
         """Translate a Bcl2Fastq sample sheet to a BCLConvert sample sheet."""
         flow_cell: FlowCellDirectoryData = self._get_flow_cell(flow_cell_name)
-        if not self._is_sample_sheet_from_flow_cell_translatable(flow_cell):
+        if not self._are_necessary_files_in_flow_cell(flow_cell):
             raise SampleSheetError("Could not translate sample sheet")
         original_content: list[list[str]] = ReadFile.get_content_from_file(
             file_format=FileFormat.CSV, file_path=flow_cell.sample_sheet_path
         )
         content_with_fixed_header: list[list[str]] = self._replace_sample_header(original_content)
 
-        flow_cell_samples: list[FlowCellSampleBCLConvert] = get_flow_cell_samples_from_content(
-            sample_sheet_content=content_with_fixed_header, sample_type=FlowCellSampleBCLConvert
+        flow_cell_samples: list[FlowCellSample] = get_flow_cell_samples_from_content(
+            sample_sheet_content=content_with_fixed_header
         )
         bcl_convert_creator = SampleSheetCreator(
             flow_cell=flow_cell, lims_samples=flow_cell_samples
         )
         new_content = bcl_convert_creator.construct_sample_sheet()
         self.validator.validate_sample_sheet_from_content(new_content)
         if self.dry_run:
@@ -194,15 +165,15 @@
                 flow_cell_directory=flow_cell.path,
                 flow_cell_name=flow_cell.id,
                 hk_api=self.hk_api,
             )
 
     def _get_sample_sheet_content(self, flow_cell: FlowCellDirectoryData) -> list[list[str]]:
         """Return the sample sheet content for a flow cell."""
-        lims_samples: list[FlowCellSampleBCLConvert] = list(
+        lims_samples: list[FlowCellSample] = list(
             get_flow_cell_samples(
                 lims=self.lims_api,
                 flow_cell_id=flow_cell.id,
             )
         )
         if not lims_samples:
             message: str = f"Could not find any samples in LIMS for {flow_cell.id}"
```

### Comparing `cg-60.3.0/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py` & `cg-60.3.1/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py` & `cg-60.3.1/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 import logging
-from typing import Type
 
 from pydantic import TypeAdapter
 
-from cg.apps.demultiplex.sample_sheet.sample_models import (
-    FlowCellSample,
-    FlowCellSampleBcl2Fastq,
-    FlowCellSampleBCLConvert,
-)
+from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample
 from cg.constants.demultiplexing import SampleSheetBcl2FastqSections, SampleSheetBCLConvertSections
 from cg.exc import SampleSheetError
 
 LOG = logging.getLogger(__name__)
 
 
 def validate_samples_are_unique(samples: list[FlowCellSample]) -> None:
@@ -30,32 +25,14 @@
     """Validate that each sample only exists once per lane in a sample sheet."""
     sample_by_lane: dict[int, list[FlowCellSample]] = get_samples_by_lane(samples)
     for lane, lane_samples in sample_by_lane.items():
         LOG.debug(f"Validate that samples are unique in lane: {lane}")
         validate_samples_are_unique(samples=lane_samples)
 
 
-def get_sample_type_from_content(
-    sample_sheet_content: list[list[str]],
-) -> Type[FlowCellSampleBcl2Fastq | FlowCellSampleBCLConvert]:
-    """Returns the sample type identified from the sample sheet content."""
-    for row in sample_sheet_content:
-        if not row:
-            continue
-        if SampleSheetBCLConvertSections.Data.HEADER in row[0]:
-            LOG.info("Sample sheet was generated for BCL Convert")
-            return FlowCellSampleBCLConvert
-        if SampleSheetBcl2FastqSections.Data.HEADER in row[0]:
-            LOG.info("Sample sheet was generated for BCL2FASTQ")
-            return FlowCellSampleBcl2Fastq
-    message: str = "Could not determine sample sheet type"
-    LOG.error(message)
-    raise SampleSheetError(message)
-
-
 def get_raw_samples_from_content(sample_sheet_content: list[list[str]]) -> list[dict[str, str]]:
     """Return the samples in a sample sheet as a list of dictionaries."""
     header: list[str] = []
     raw_samples: list[dict[str, str]] = []
 
     for line in sample_sheet_content:
         # Skip lines that are too short to contain samples
@@ -92,23 +69,18 @@
             sample_by_lane[sample.lane] = []
         sample_by_lane[sample.lane].append(sample)
     return sample_by_lane
 
 
 def get_flow_cell_samples_from_content(
     sample_sheet_content: list[list[str]],
-    sample_type: Type[FlowCellSample] | None = None,
-) -> list[FlowCellSampleBcl2Fastq | FlowCellSampleBCLConvert]:
+) -> list[FlowCellSample]:
     """
     Return the samples in a sample sheet as a list of FlowCellSample objects.
     Raises:
         ValidationError: if the samples do not have the correct attributes based on their model.
     """
-    if not sample_type:
-        sample_type: Type[FlowCellSampleBcl2Fastq | FlowCellSampleBCLConvert] = (
-            get_sample_type_from_content(sample_sheet_content)
-        )
     raw_samples: list[dict[str, str]] = get_raw_samples_from_content(
         sample_sheet_content=sample_sheet_content
     )
-    adapter = TypeAdapter(list[sample_type])
+    adapter = TypeAdapter(list[FlowCellSample])
     return adapter.validate_python(raw_samples)
```

### Comparing `cg-60.3.0/cg/apps/demultiplex/sample_sheet/sample_models.py` & `cg-60.3.1/cg/apps/demultiplex/sample_sheet/sample_models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,132 +1,51 @@
 import logging
-from abc import abstractmethod
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from cg.apps.demultiplex.sample_sheet.index import (
     MINIMUM_HAMMING_DISTANCE,
     get_hamming_distance_index_1,
     get_hamming_distance_index_2,
     get_reverse_complement_dna_seq,
     is_dual_index,
-    is_padding_needed,
-    pad_index_one,
-    pad_index_two,
 )
 from cg.apps.demultiplex.sample_sheet.validators import SampleId
-from cg.constants.constants import GenomeVersion
-from cg.constants.demultiplexing import (
-    CUSTOM_INDEX_TAIL,
-    SampleSheetBcl2FastqSections,
-    SampleSheetBCLConvertSections,
-)
+from cg.constants.demultiplexing import CUSTOM_INDEX_TAIL, SampleSheetBCLConvertSections
 from cg.constants.symbols import EMPTY_STRING
 from cg.exc import SampleSheetError
 from cg.models.demultiplex.run_parameters import RunParameters
 
 LOG = logging.getLogger(__name__)
 
 
 class FlowCellSample(BaseModel):
-    """Base class for flow cell samples."""
-
-    lane: int
-    sample_id: SampleId
-    index: str
-    index2: str = EMPTY_STRING
-    model_config = ConfigDict(populate_by_name=True)
-
-    def separate_indexes(self, is_run_single_index: bool) -> None:
-        """Update values for index and index2 splitting the original LIMS dual index."""
-        if is_dual_index(self.index):
-            index1, index2 = self.index.split("-")
-            self.index = index1.strip().replace(CUSTOM_INDEX_TAIL, EMPTY_STRING)
-            self.index2 = index2.strip() if not is_run_single_index else EMPTY_STRING
-
-    @abstractmethod
-    def process_indexes(self, run_parameters: RunParameters):
-        """Update index attributes with the final values for the sample sheet."""
-        pass
-
-    @abstractmethod
-    def update_barcode_mismatches(
-        self, samples_to_compare: list, is_run_single_index: bool, is_reverse_complement: bool
-    ) -> None:
-        """Update the barcode_mismatches_1 and barcode_mismatches_2 attributes."""
-        pass
-
-
-class FlowCellSampleBcl2Fastq(FlowCellSample):
-    """Class that represents a Bcl2Fastq sample."""
-
-    flowcell_id: str = Field("", alias=SampleSheetBcl2FastqSections.Data.FLOW_CELL_ID)
-    lane: int = Field(..., alias=SampleSheetBcl2FastqSections.Data.LANE)
-    sample_ref: str = Field(
-        GenomeVersion.hg19, alias=SampleSheetBcl2FastqSections.Data.SAMPLE_REFERENCE
-    )
-    index: str = Field(..., alias=SampleSheetBcl2FastqSections.Data.INDEX_1)
-    index2: str = Field("", alias=SampleSheetBcl2FastqSections.Data.INDEX_2)
-    sample_name: str = Field(..., alias=SampleSheetBcl2FastqSections.Data.SAMPLE_NAME)
-    control: str = Field("N", alias=SampleSheetBcl2FastqSections.Data.CONTROL)
-    recipe: str = Field("R1", alias=SampleSheetBcl2FastqSections.Data.RECIPE)
-    operator: str = Field("script", alias=SampleSheetBcl2FastqSections.Data.OPERATOR)
-
-    sample_id: SampleId = Field(
-        ..., alias=SampleSheetBcl2FastqSections.Data.SAMPLE_INTERNAL_ID_BCL2FASTQ
-    )
-    project: str = Field(..., alias=SampleSheetBcl2FastqSections.Data.SAMPLE_PROJECT_BCL2FASTQ)
-
-    def _pad_indexes_if_necessary(self, run_parameters: RunParameters) -> None:
-        index_length: int = len(self.index)
-        if is_padding_needed(
-            index1_cycles=run_parameters.get_index_1_cycles(),
-            index2_cycles=run_parameters.get_index_2_cycles(),
-            sample_index_length=index_length,
-        ):
-            LOG.debug("Padding indexes")
-            self.index = pad_index_one(index_string=self.index)
-            self.index2 = pad_index_two(
-                index_string=self.index2,
-                reverse_complement=run_parameters.index_settings.should_i5_be_reverse_complemented,
-            )
-            return
-        LOG.debug(f"Padding not necessary for sample {self.sample_id}")
-
-    def process_indexes(self, run_parameters: RunParameters):
-        """Parses, pads and reverse complement the indexes if necessary."""
-        reverse_index2: bool = run_parameters.index_settings.should_i5_be_reverse_complemented
-        self.separate_indexes(is_run_single_index=run_parameters.is_single_index)
-        self._pad_indexes_if_necessary(run_parameters=run_parameters)
-        if reverse_index2:
-            self.index2 = get_reverse_complement_dna_seq(self.index2)
-
-    def update_barcode_mismatches(
-        self, samples_to_compare: list, is_run_single_index: bool, is_reverse_complement: bool
-    ) -> None:
-        """No updating of barcode mismatch values for Bcl2Fastq samples."""
-        LOG.debug(f"No updating of barcode mismatch values for Bcl2Fastq sample {self.sample_id}")
-
-
-class FlowCellSampleBCLConvert(FlowCellSample):
-    """Class that represents a BCLConvert sample."""
+    """Class that represents a flow cell sample."""
 
     lane: int = Field(..., alias=SampleSheetBCLConvertSections.Data.LANE)
     sample_id: SampleId = Field(..., alias=SampleSheetBCLConvertSections.Data.SAMPLE_INTERNAL_ID)
     index: str = Field(..., alias=SampleSheetBCLConvertSections.Data.INDEX_1)
     index2: str = Field(EMPTY_STRING, alias=SampleSheetBCLConvertSections.Data.INDEX_2)
     override_cycles: str = Field(
         EMPTY_STRING, alias=SampleSheetBCLConvertSections.Data.OVERRIDE_CYCLES
     )
     barcode_mismatches_1: int = Field(
         1, alias=SampleSheetBCLConvertSections.Data.BARCODE_MISMATCHES_1
     )
     barcode_mismatches_2: int | str = Field(
         1, alias=SampleSheetBCLConvertSections.Data.BARCODE_MISMATCHES_2
     )
+    model_config = ConfigDict(populate_by_name=True)
+
+    def separate_indexes(self, is_run_single_index: bool) -> None:
+        """Update values for index and index2 splitting the original LIMS dual index."""
+        if is_dual_index(self.index):
+            index1, index2 = self.index.split("-")
+            self.index = index1.strip().replace(CUSTOM_INDEX_TAIL, EMPTY_STRING)
+            self.index2 = index2.strip() if not is_run_single_index else EMPTY_STRING
 
     def _get_index1_override_cycles(self, len_index1_cycles: int) -> str:
         """Create the index 1 sub-string for the override cycles attribute."""
         len_index_1_sample: int = len(self.index)
         cycles_format: str = f"I{len_index1_cycles};"
         if len_index_1_sample < len_index1_cycles:
             cycles_format = f"I{len_index_1_sample}N{len_index1_cycles - len_index_1_sample};"
@@ -158,17 +77,15 @@
         index1_cycles: str = self._get_index1_override_cycles(run_parameters.get_index_1_cycles())
         index2_cycles: str = self._get_index2_override_cycles(
             len_index2_cycles=run_parameters.get_index_2_cycles(),
             reverse_cycle=reverse_index2_cycles,
         )
         self.override_cycles = read1_cycles + index1_cycles + index2_cycles + read2_cycles
 
-    def _update_barcode_mismatches_1(
-        self, samples_to_compare: list["FlowCellSampleBCLConvert"]
-    ) -> None:
+    def _update_barcode_mismatches_1(self, samples_to_compare: list["FlowCellSample"]) -> None:
         """Assign zero to barcode_mismatches_1 if the hamming distance between self.index
         and the index1 of any sample in the lane is below the minimum threshold."""
         for sample in samples_to_compare:
             if self.sample_id == sample.sample_id:
                 continue
             if (
                 get_hamming_distance_index_1(sequence_1=self.index, sequence_2=sample.index)
@@ -176,15 +93,15 @@
             ):
                 LOG.debug(f"Turning barcode mismatch for index 1 to 0 for sample {self.sample_id}")
                 self.barcode_mismatches_1 = 0
                 break
 
     def _update_barcode_mismatches_2(
         self,
-        samples_to_compare: list["FlowCellSampleBCLConvert"],
+        samples_to_compare: list["FlowCellSample"],
         is_reverse_complement: bool,
     ) -> None:
         """Assign zero to barcode_mismatches_2 if the hamming distance between self.index2
         and the index2 of any sample in the lane is below the minimum threshold.
         If the sample is single-indexed, assign 'na'."""
         if self.index2 == EMPTY_STRING and "-" not in self.index:
             LOG.debug(f"Turning barcode mismatch for index 2 to 'na' for sample {self.sample_id}")
@@ -210,15 +127,15 @@
         self.separate_indexes(is_run_single_index=run_parameters.is_single_index)
         if run_parameters.index_settings.should_i5_be_reverse_complemented:
             self.index2 = get_reverse_complement_dna_seq(self.index2)
         self.update_override_cycles(run_parameters=run_parameters)
 
     def update_barcode_mismatches(
         self,
-        samples_to_compare: list["FlowCellSampleBCLConvert"],
+        samples_to_compare: list["FlowCellSample"],
         is_run_single_index: bool,
         is_reverse_complement: bool,
     ) -> None:
         """Update barcode mismatch attributes comparing to the rest of the samples in the lane."""
         if not samples_to_compare:
             raise SampleSheetError("No samples to compare with to update barcode mismatch values")
         self._update_barcode_mismatches_1(samples_to_compare=samples_to_compare)
```

### Comparing `cg-60.3.0/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py` & `cg-60.3.1/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 """ Create a sample sheet for NovaSeq flow cells."""
 
 import logging
 
 from cg.apps.demultiplex.sample_sheet.read_sample_sheet import get_samples_by_lane
-from cg.apps.demultiplex.sample_sheet.sample_models import (
-    FlowCellSampleBcl2Fastq,
-    FlowCellSampleBCLConvert,
-)
+from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample
 from cg.constants.demultiplexing import IndexSettings, SampleSheetBCLConvertSections
 from cg.models.demultiplex.run_parameters import RunParameters
 from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
 
 LOG = logging.getLogger(__name__)
 
 
 class SampleSheetCreator:
     """Base class for sample sheet creation."""
 
     def __init__(
         self,
         flow_cell: FlowCellDirectoryData,
-        lims_samples: list[FlowCellSampleBCLConvert],
+        lims_samples: list[FlowCellSample],
     ):
         self.flow_cell: FlowCellDirectoryData = flow_cell
         self.flow_cell_id: str = flow_cell.id
-        self.lims_samples: list[FlowCellSampleBCLConvert] = lims_samples
+        self.lims_samples: list[FlowCellSample] = lims_samples
         self.run_parameters: RunParameters = flow_cell.run_parameters
         self.index_settings: IndexSettings = self.run_parameters.index_settings
 
     def convert_sample_to_header_dict(
         self,
-        sample: FlowCellSampleBCLConvert | FlowCellSampleBcl2Fastq,
+        sample: FlowCellSample,
         data_column_names: list[str],
     ) -> list[str]:
         """Convert a lims sample object to a list that corresponds to the sample sheet headers."""
         if self.run_parameters.is_single_index:
             sample_serialisation: dict = sample.model_dump(
                 by_alias=True, exclude={"index2", "barcode_mismatches_2"}
             )
```

### Comparing `cg-60.3.0/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py` & `cg-60.3.1/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import logging
 from collections import defaultdict
 
 from pydantic import BaseModel
 
-from cg.apps.demultiplex.sample_sheet.sample_models import (
-    FlowCellSample,
-    FlowCellSampleBcl2Fastq,
-    FlowCellSampleBCLConvert,
-)
+from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample
 
 LOG = logging.getLogger(__name__)
 
 
 class SampleSheet(BaseModel):
     samples: list[FlowCellSample]
 
@@ -32,15 +28,7 @@
 
     def get_sample_ids(self) -> list[str]:
         """Return ids for samples in sheet."""
         sample_internal_ids: list[str] = []
         for sample in self.samples:
             sample_internal_ids.append(sample.sample_id)
         return list(set(sample_internal_ids))
-
-
-class SampleSheetBcl2Fastq(SampleSheet):
-    samples: list[FlowCellSampleBcl2Fastq]
-
-
-class SampleSheetBCLConvert(SampleSheet):
-    samples: list[FlowCellSampleBCLConvert]
```

### Comparing `cg-60.3.0/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py` & `cg-60.3.1/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Module with validator classes for the sample sheet."""
 
 import logging
 from pathlib import Path
-from typing import Type
 
 from pydantic import ValidationError
 
 from cg.apps.demultiplex.sample_sheet.override_cycles_validator import OverrideCyclesValidator
 from cg.apps.demultiplex.sample_sheet.read_sample_sheet import (
     get_flow_cell_samples_from_content,
     get_raw_samples_from_content,
     validate_samples_unique_per_lane,
 )
-from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample, FlowCellSampleBCLConvert
+from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample
 from cg.apps.demultiplex.sample_sheet.sample_sheet_models import SampleSheet
 from cg.constants.constants import FileFormat
 from cg.constants.demultiplexing import NAME_TO_INDEX_SETTINGS, SampleSheetBCLConvertSections
 from cg.exc import OverrideCyclesError, SampleSheetError
 from cg.io.controller import ReadFile
 
 LOG = logging.getLogger(__name__)
@@ -101,25 +100,25 @@
         self.read1_cycles = self._get_cycle(SampleSheetBCLConvertSections.Reads.READ_CYCLES_1)
         self.read2_cycles = self._get_cycle(SampleSheetBCLConvertSections.Reads.READ_CYCLES_2)
         self.index1_cycles = self._get_cycle(SampleSheetBCLConvertSections.Reads.INDEX_CYCLES_1)
         self.index2_cycles = self._get_cycle(
             cycle_name=SampleSheetBCLConvertSections.Reads.INDEX_CYCLES_2, nullable=True
         )
 
-    def _validate_samples(self, sample_type: Type[FlowCellSample] | None = None) -> None:
+    def _validate_samples(self) -> None:
         """
         Determine if the samples have the correct attributes and are unique per lane.
         Raises:
             SampleSheetError if the samples do not have the correct attributes based on their model
             or are not unique per lane.
         """
         LOG.debug("Validating samples")
         try:
             validated_samples: list[FlowCellSample] = get_flow_cell_samples_from_content(
-                sample_sheet_content=self.content, sample_type=sample_type
+                sample_sheet_content=self.content
             )
         except ValidationError as error:
             LOG.error("Sample sheet failed validation: samples are not in the correct format")
             raise SampleSheetError from error
         validate_samples_unique_per_lane(validated_samples)
 
     def _validate_override_cycles(self) -> None:
@@ -154,15 +153,15 @@
             SampleSheetError: If the sample sheet is not valid.
         """
         self.set_sample_sheet_content(content)
         LOG.debug("Validating sample sheet")
         self._validate_all_sections_present()
         self._set_is_index2_reverse_complement()
         self._set_cycles()
-        self._validate_samples(sample_type=FlowCellSampleBCLConvert)
+        self._validate_samples()
         self._validate_override_cycles()
         LOG.info("Samplesheet passed validation")
 
     def validate_sample_sheet_from_file(self, file_path: Path) -> None:
         """
         Validate a sample sheet given the path to the file.
         Raises:
@@ -175,12 +174,9 @@
 
     def get_sample_sheet_object_from_file(self, file_path: Path) -> SampleSheet:
         """Return a sample sheet object given the path to the file.
         Raises:
             SampleSheetError: If the sample sheet is not valid.
         """
         self.validate_sample_sheet_from_file(file_path)
-        samples: list[FlowCellSample] = get_flow_cell_samples_from_content(
-            sample_sheet_content=self.content,
-            sample_type=FlowCellSampleBCLConvert,
-        )
+        samples: list[FlowCellSample] = get_flow_cell_samples_from_content(self.content)
         return SampleSheet(samples=samples)
```

### Comparing `cg-60.3.0/cg/apps/demultiplex/sample_sheet/validators.py` & `cg-60.3.1/cg/apps/demultiplex/sample_sheet/validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/demultiplex/sbatch.py` & `cg-60.3.1/cg/apps/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/downsample/downsample.py` & `cg-60.3.1/cg/apps/downsample/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/downsample/utils.py` & `cg-60.3.1/cg/apps/downsample/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/gens.py` & `cg-60.3.1/cg/apps/gens.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/gt.py` & `cg-60.3.1/cg/apps/gt.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/hermes/hermes_api.py` & `cg-60.3.1/cg/apps/hermes/hermes_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/hermes/models.py` & `cg-60.3.1/cg/apps/hermes/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/housekeeper/hk.py` & `cg-60.3.1/cg/apps/housekeeper/hk.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/invoice/render.py` & `cg-60.3.1/cg/apps/invoice/render.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/invoice/templates/KI_pool_invoice.xlsx` & `cg-60.3.1/cg/apps/invoice/templates/KI_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/invoice/templates/KI_sample_invoice.xlsx` & `cg-60.3.1/cg/apps/invoice/templates/KI_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/invoice/templates/KTH_pool_invoice.xlsx` & `cg-60.3.1/cg/apps/invoice/templates/KTH_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/invoice/templates/KTH_sample_invoice.xlsx` & `cg-60.3.1/cg/apps/invoice/templates/KTH_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/lims/api.py` & `cg-60.3.1/cg/apps/lims/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/lims/batch.py` & `cg-60.3.1/cg/apps/lims/batch.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/lims/order.py` & `cg-60.3.1/cg/apps/lims/order.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/lims/sample_sheet.py` & `cg-60.3.1/cg/apps/lims/sample_sheet.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import re
 from typing import Iterable, Type
 
 from genologics.entities import Artifact, Container, Sample
 from genologics.lims import Lims
 
-from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSampleBCLConvert
+from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample
 
 LOG = logging.getLogger(__name__)
 
 
 def get_placement_lane(lane: str) -> int:
     """Parse out the lane information from an artifact.placement."""
     return int(lane.split(":")[0])
@@ -65,15 +65,15 @@
 
     return sequence
 
 
 def get_flow_cell_samples(
     lims: Lims,
     flow_cell_id: str,
-) -> Iterable[FlowCellSampleBCLConvert]:
+) -> Iterable[FlowCellSample]:
     """Return samples from LIMS for a given flow cell."""
     LOG.info(f"Fetching samples from lims for flowcell {flow_cell_id}")
     containers: list[Container] = lims.get_containers(name=flow_cell_id)
     if not containers:
         return []
     container: Container = containers[-1]  # only take the last one. See ÖA#217.
     raw_lanes: list[str] = sorted(container.placements.keys())
@@ -81,12 +81,12 @@
         lane: int = get_placement_lane(raw_lane)
         placement_artifact: Artifact = container.placements[raw_lane]
         non_pooled_artifacts: list[Artifact] = get_non_pooled_artifacts(placement_artifact)
         for artifact in non_pooled_artifacts:
             sample: Sample = artifact.samples[0]  # we are assured it only has one sample
             label: str | None = get_reagent_label(artifact)
             index = get_index(lims=lims, label=label)
-            yield FlowCellSampleBCLConvert(
+            yield FlowCellSample(
                 lane=lane,
                 sample_id=sample.id,
                 index=index,
             )
```

### Comparing `cg-60.3.0/cg/apps/loqus.py` & `cg-60.3.1/cg/apps/loqus.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/madeline/api.py` & `cg-60.3.1/cg/apps/madeline/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/mip/confighandler.py` & `cg-60.3.1/cg/apps/mip/confighandler.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/mutacc_auto.py` & `cg-60.3.1/cg/apps/mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/orderform/excel_orderform_parser.py` & `cg-60.3.1/cg/apps/orderform/excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/orderform/json_orderform_parser.py` & `cg-60.3.1/cg/apps/orderform/json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/orderform/orderform_parser.py` & `cg-60.3.1/cg/apps/orderform/orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/osticket.py` & `cg-60.3.1/cg/apps/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/scout/scout_export.py` & `cg-60.3.1/cg/apps/scout/scout_export.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/scout/scoutapi.py` & `cg-60.3.1/cg/apps/scout/scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/sequencing_metrics_parser/api.py` & `cg-60.3.1/cg/apps/sequencing_metrics_parser/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/sequencing_metrics_parser/models.py` & `cg-60.3.1/cg/apps/sequencing_metrics_parser/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/sequencing_metrics_parser/parser.py` & `cg-60.3.1/cg/apps/sequencing_metrics_parser/parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/slurm/sbatch.py` & `cg-60.3.1/cg/apps/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/slurm/slurm_api.py` & `cg-60.3.1/cg/apps/slurm/slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/tb/api.py` & `cg-60.3.1/cg/apps/tb/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/apps/tb/models.py` & `cg-60.3.1/cg/apps/tb/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/add.py` & `cg-60.3.1/cg/cli/add.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/archive.py` & `cg-60.3.1/cg/cli/archive.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/backup.py` & `cg-60.3.1/cg/cli/backup.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/base.py` & `cg-60.3.1/cg/cli/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/clean.py` & `cg-60.3.1/cg/cli/clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/compress/base.py` & `cg-60.3.1/cg/cli/compress/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/compress/fastq.py` & `cg-60.3.1/cg/cli/compress/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/compress/helpers.py` & `cg-60.3.1/cg/cli/compress/helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/delete/base.py` & `cg-60.3.1/cg/cli/delete/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/delete/case.py` & `cg-60.3.1/cg/cli/delete/case.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/delete/cases.py` & `cg-60.3.1/cg/cli/delete/cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/delete/observations.py` & `cg-60.3.1/cg/cli/delete/observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/deliver/base.py` & `cg-60.3.1/cg/cli/deliver/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/demultiplex/base.py` & `cg-60.3.1/cg/cli/demultiplex/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py` & `cg-60.3.1/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/demultiplex/demux.py` & `cg-60.3.1/cg/cli/demultiplex/demux.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/demultiplex/finish.py` & `cg-60.3.1/cg/cli/demultiplex/finish.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/demultiplex/sample_sheet.py` & `cg-60.3.1/cg/cli/demultiplex/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/downsample.py` & `cg-60.3.1/cg/cli/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/generate/report/base.py` & `cg-60.3.1/cg/cli/generate/report/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/generate/report/options.py` & `cg-60.3.1/cg/cli/generate/report/options.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/generate/report/utils.py` & `cg-60.3.1/cg/cli/generate/report/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/get.py` & `cg-60.3.1/cg/cli/get.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/set/base.py` & `cg-60.3.1/cg/cli/set/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/set/case.py` & `cg-60.3.1/cg/cli/set/case.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/set/cases.py` & `cg-60.3.1/cg/cli/set/cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/store/base.py` & `cg-60.3.1/cg/cli/store/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/store/store.py` & `cg-60.3.1/cg/cli/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/transfer.py` & `cg-60.3.1/cg/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/upload/base.py` & `cg-60.3.1/cg/cli/upload/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/upload/clinical_delivery.py` & `cg-60.3.1/cg/cli/upload/clinical_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/upload/coverage.py` & `cg-60.3.1/cg/cli/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/upload/delivery_report.py` & `cg-60.3.1/cg/cli/upload/delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/upload/fohm.py` & `cg-60.3.1/cg/cli/upload/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/upload/genotype.py` & `cg-60.3.1/cg/cli/upload/genotype.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/upload/gens.py` & `cg-60.3.1/cg/cli/upload/gens.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/upload/gisaid.py` & `cg-60.3.1/cg/cli/upload/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/upload/mutacc.py` & `cg-60.3.1/cg/cli/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/upload/nipt/base.py` & `cg-60.3.1/cg/cli/upload/nipt/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/upload/nipt/ftp.py` & `cg-60.3.1/cg/cli/upload/nipt/ftp.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/upload/nipt/statina.py` & `cg-60.3.1/cg/cli/upload/nipt/statina.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/upload/observations/observations.py` & `cg-60.3.1/cg/cli/upload/observations/observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/upload/observations/utils.py` & `cg-60.3.1/cg/cli/upload/observations/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/upload/scout.py` & `cg-60.3.1/cg/cli/upload/scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/upload/utils.py` & `cg-60.3.1/cg/cli/upload/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/upload/validate.py` & `cg-60.3.1/cg/cli/upload/validate.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/workflow/balsamic/base.py` & `cg-60.3.1/cg/cli/workflow/balsamic/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/workflow/balsamic/options.py` & `cg-60.3.1/cg/cli/workflow/balsamic/options.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/workflow/balsamic/pon.py` & `cg-60.3.1/cg/cli/workflow/balsamic/pon.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/workflow/balsamic/qc.py` & `cg-60.3.1/cg/cli/workflow/balsamic/qc.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/workflow/balsamic/umi.py` & `cg-60.3.1/cg/cli/workflow/balsamic/umi.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/workflow/base.py` & `cg-60.3.1/cg/cli/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/workflow/commands.py` & `cg-60.3.1/cg/cli/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/workflow/fastq/base.py` & `cg-60.3.1/cg/cli/workflow/fastq/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/workflow/fastq/fastq_service.py` & `cg-60.3.1/cg/cli/workflow/fastq/fastq_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/workflow/fluffy/base.py` & `cg-60.3.1/cg/cli/workflow/fluffy/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/workflow/jasen/base.py` & `cg-60.3.1/cg/cli/workflow/jasen/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/workflow/microsalt/base.py` & `cg-60.3.1/cg/cli/workflow/microsalt/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/workflow/mip/base.py` & `cg-60.3.1/cg/cli/workflow/mip/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/workflow/mip/options.py` & `cg-60.3.1/cg/cli/workflow/mip/options.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/workflow/mip_dna/base.py` & `cg-60.3.1/cg/cli/workflow/mip_dna/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/workflow/mip_rna/base.py` & `cg-60.3.1/cg/cli/workflow/mip_rna/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/workflow/mutant/base.py` & `cg-60.3.1/cg/cli/workflow/mutant/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/workflow/nf_analysis.py` & `cg-60.3.1/cg/cli/workflow/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/workflow/raredisease/base.py` & `cg-60.3.1/cg/cli/workflow/raredisease/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/workflow/rnafusion/base.py` & `cg-60.3.1/cg/cli/workflow/rnafusion/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/workflow/taxprofiler/base.py` & `cg-60.3.1/cg/cli/workflow/taxprofiler/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/cli/workflow/tomte/base.py` & `cg-60.3.1/cg/cli/workflow/tomte/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/clients/arnold/api.py` & `cg-60.3.1/cg/clients/arnold/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/clients/janus/api.py` & `cg-60.3.1/cg/clients/janus/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/constants/__init__.py` & `cg-60.3.1/cg/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/constants/bcl_convert_metrics.py` & `cg-60.3.1/cg/constants/bcl_convert_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/constants/constants.py` & `cg-60.3.1/cg/constants/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/constants/delivery.py` & `cg-60.3.1/cg/constants/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/constants/demultiplexing.py` & `cg-60.3.1/cg/constants/demultiplexing.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/constants/encryption.py` & `cg-60.3.1/cg/constants/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/constants/gene_panel.py` & `cg-60.3.1/cg/constants/gene_panel.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/constants/housekeeper_tags.py` & `cg-60.3.1/cg/constants/housekeeper_tags.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/constants/lims.py` & `cg-60.3.1/cg/constants/lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/constants/metrics.py` & `cg-60.3.1/cg/constants/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/constants/nextflow.py` & `cg-60.3.1/cg/constants/nextflow.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/constants/nf_analysis.py` & `cg-60.3.1/cg/constants/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/constants/observations.py` & `cg-60.3.1/cg/constants/observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/constants/orderforms.py` & `cg-60.3.1/cg/constants/orderforms.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/constants/priority.py` & `cg-60.3.1/cg/constants/priority.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/constants/report.py` & `cg-60.3.1/cg/constants/report.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/constants/scout.py` & `cg-60.3.1/cg/constants/scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/constants/sequencing.py` & `cg-60.3.1/cg/constants/sequencing.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/constants/subject.py` & `cg-60.3.1/cg/constants/subject.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/exc.py` & `cg-60.3.1/cg/exc.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/io/api.py` & `cg-60.3.1/cg/io/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/io/config.py` & `cg-60.3.1/cg/io/config.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/io/controller.py` & `cg-60.3.1/cg/io/controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/io/csv.py` & `cg-60.3.1/cg/io/csv.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/io/json.py` & `cg-60.3.1/cg/io/json.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/io/png.py` & `cg-60.3.1/cg/io/png.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/io/txt.py` & `cg-60.3.1/cg/io/txt.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/io/validate_path.py` & `cg-60.3.1/cg/io/validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/io/xml.py` & `cg-60.3.1/cg/io/xml.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/io/yaml.py` & `cg-60.3.1/cg/io/yaml.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/archive/archive.py` & `cg-60.3.1/cg/meta/archive/archive.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/archive/ddn/constants.py` & `cg-60.3.1/cg/meta/archive/ddn/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/archive/ddn/ddn_data_flow_client.py` & `cg-60.3.1/cg/meta/archive/ddn/ddn_data_flow_client.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/archive/ddn/models.py` & `cg-60.3.1/cg/meta/archive/ddn/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/archive/ddn/utils.py` & `cg-60.3.1/cg/meta/archive/ddn/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/archive/models.py` & `cg-60.3.1/cg/meta/archive/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/backup/backup.py` & `cg-60.3.1/cg/meta/backup/backup.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/backup/pdc.py` & `cg-60.3.1/cg/meta/backup/pdc.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/clean/api.py` & `cg-60.3.1/cg/meta/clean/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/clean/clean_flow_cells.py` & `cg-60.3.1/cg/meta/clean/clean_flow_cells.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/clean/clean_retrieved_spring_files.py` & `cg-60.3.1/cg/meta/clean/clean_retrieved_spring_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/compress/compress.py` & `cg-60.3.1/cg/meta/compress/compress.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/compress/files.py` & `cg-60.3.1/cg/meta/compress/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/deliver/deliver.py` & `cg-60.3.1/cg/meta/deliver/deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/deliver/deliver_ticket.py` & `cg-60.3.1/cg/meta/deliver/deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/deliver/fastq_path_generator.py` & `cg-60.3.1/cg/meta/deliver/fastq_path_generator.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/delivery/delivery.py` & `cg-60.3.1/cg/meta/delivery/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/demultiplex/combine_sequencing_metrics.py` & `cg-60.3.1/cg/meta/demultiplex/combine_sequencing_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/demultiplex/demux_post_processing.py` & `cg-60.3.1/cg/meta/demultiplex/demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/demultiplex/files.py` & `cg-60.3.1/cg/meta/demultiplex/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/demultiplex/housekeeper_storage_functions.py` & `cg-60.3.1/cg/meta/demultiplex/housekeeper_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/demultiplex/status_db_storage_functions.py` & `cg-60.3.1/cg/meta/demultiplex/status_db_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/demultiplex/utils.py` & `cg-60.3.1/cg/meta/demultiplex/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/demultiplex/validation.py` & `cg-60.3.1/cg/meta/demultiplex/validation.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/encryption/encryption.py` & `cg-60.3.1/cg/meta/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/encryption/sbatch.py` & `cg-60.3.1/cg/meta/encryption/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/invoice.py` & `cg-60.3.1/cg/meta/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/meta.py` & `cg-60.3.1/cg/meta/meta.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/observations/balsamic_observations_api.py` & `cg-60.3.1/cg/meta/observations/balsamic_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/observations/mip_dna_observations_api.py` & `cg-60.3.1/cg/meta/observations/mip_dna_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/observations/observations_api.py` & `cg-60.3.1/cg/meta/observations/observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/orders/api.py` & `cg-60.3.1/cg/meta/orders/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/orders/case_submitter.py` & `cg-60.3.1/cg/meta/orders/case_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/orders/fastq_submitter.py` & `cg-60.3.1/cg/meta/orders/fastq_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/orders/lims.py` & `cg-60.3.1/cg/meta/orders/lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/orders/metagenome_submitter.py` & `cg-60.3.1/cg/meta/orders/metagenome_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/orders/microbial_submitter.py` & `cg-60.3.1/cg/meta/orders/microbial_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/orders/pool_submitter.py` & `cg-60.3.1/cg/meta/orders/pool_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/orders/rnafusion_submitter.py` & `cg-60.3.1/cg/meta/orders/rnafusion_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/orders/sars_cov_2_submitter.py` & `cg-60.3.1/cg/meta/orders/sars_cov_2_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/orders/submitter.py` & `cg-60.3.1/cg/meta/orders/submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/orders/ticket_handler.py` & `cg-60.3.1/cg/meta/orders/ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/qc_metrics/collect_qc_metrics.py` & `cg-60.3.1/cg/meta/qc_metrics/collect_qc_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/balsamic.py` & `cg-60.3.1/cg/meta/report/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/balsamic_qc.py` & `cg-60.3.1/cg/meta/report/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/balsamic_umi.py` & `cg-60.3.1/cg/meta/report/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/field_validators.py` & `cg-60.3.1/cg/meta/report/field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/mip_dna.py` & `cg-60.3.1/cg/meta/report/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/report_api.py` & `cg-60.3.1/cg/meta/report/report_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/rnafusion.py` & `cg-60.3.1/cg/meta/report/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/templates/delivery-report.html` & `cg-60.3.1/cg/meta/report/templates/delivery-report.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/templates/macros/data_analysis/data_analysis.html` & `cg-60.3.1/cg/meta/report/templates/macros/data_analysis/data_analysis.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/templates/macros/data_analysis/limitations.html` & `cg-60.3.1/cg/meta/report/templates/macros/data_analysis/limitations.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html` & `cg-60.3.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html` & `cg-60.3.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html` & `cg-60.3.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html` & `cg-60.3.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html` & `cg-60.3.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/templates/macros/header.html` & `cg-60.3.1/cg/meta/report/templates/macros/header.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/templates/macros/order.html` & `cg-60.3.1/cg/meta/report/templates/macros/order.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/templates/macros/sample_prep.html` & `cg-60.3.1/cg/meta/report/templates/macros/sample_prep.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html` & `cg-60.3.1/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html` & `cg-60.3.1/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html` & `cg-60.3.1/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/templates/static/css/bootstrap.min.css` & `cg-60.3.1/cg/meta/report/templates/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/templates/static/images/SWEDAC_logo.png` & `cg-60.3.1/cg/meta/report/templates/static/images/SWEDAC_logo.png`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/report/tomte.py` & `cg-60.3.1/cg/meta/report/tomte.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/rsync/rsync_api.py` & `cg-60.3.1/cg/meta/rsync/rsync_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/tar/tar.py` & `cg-60.3.1/cg/meta/tar/tar.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/transfer/external_data.py` & `cg-60.3.1/cg/meta/transfer/external_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/transfer/lims.py` & `cg-60.3.1/cg/meta/transfer/lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/upload/balsamic/balsamic.py` & `cg-60.3.1/cg/meta/upload/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/upload/coverage.py` & `cg-60.3.1/cg/meta/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/upload/fohm/fohm.py` & `cg-60.3.1/cg/meta/upload/fohm/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/upload/gisaid/constants.py` & `cg-60.3.1/cg/meta/upload/gisaid/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/upload/gisaid/gisaid.py` & `cg-60.3.1/cg/meta/upload/gisaid/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/upload/gisaid/models.py` & `cg-60.3.1/cg/meta/upload/gisaid/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/upload/gt.py` & `cg-60.3.1/cg/meta/upload/gt.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/upload/microsalt/microsalt_upload_api.py` & `cg-60.3.1/cg/meta/upload/microsalt/microsalt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/upload/mip/mip_dna.py` & `cg-60.3.1/cg/meta/upload/mip/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/upload/mip/mip_rna.py` & `cg-60.3.1/cg/meta/upload/mip/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/upload/mutacc.py` & `cg-60.3.1/cg/meta/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/upload/nf_analysis.py` & `cg-60.3.1/cg/meta/upload/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/upload/nipt/models.py` & `cg-60.3.1/cg/meta/upload/nipt/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/upload/nipt/nipt.py` & `cg-60.3.1/cg/meta/upload/nipt/nipt.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/upload/scout/balsamic_config_builder.py` & `cg-60.3.1/cg/meta/upload/scout/balsamic_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/upload/scout/balsamic_umi_config_builder.py` & `cg-60.3.1/cg/meta/upload/scout/balsamic_umi_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/upload/scout/hk_tags.py` & `cg-60.3.1/cg/meta/upload/scout/hk_tags.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/upload/scout/mip_config_builder.py` & `cg-60.3.1/cg/meta/upload/scout/mip_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/upload/scout/rnafusion_config_builder.py` & `cg-60.3.1/cg/meta/upload/scout/rnafusion_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/upload/scout/scout_config_builder.py` & `cg-60.3.1/cg/meta/upload/scout/scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/upload/scout/uploadscoutapi.py` & `cg-60.3.1/cg/meta/upload/scout/uploadscoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/upload/upload_api.py` & `cg-60.3.1/cg/meta/upload/upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/analysis.py` & `cg-60.3.1/cg/meta/workflow/analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/balsamic.py` & `cg-60.3.1/cg/meta/workflow/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/balsamic_pon.py` & `cg-60.3.1/cg/meta/workflow/balsamic_pon.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/balsamic_qc.py` & `cg-60.3.1/cg/meta/workflow/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/balsamic_umi.py` & `cg-60.3.1/cg/meta/workflow/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/downsample/downsample.py` & `cg-60.3.1/cg/meta/workflow/downsample/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/downsample/sbatch.py` & `cg-60.3.1/cg/meta/workflow/downsample/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/fastq.py` & `cg-60.3.1/cg/meta/workflow/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/fluffy.py` & `cg-60.3.1/cg/meta/workflow/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/jasen.py` & `cg-60.3.1/cg/meta/workflow/jasen.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/microsalt/metrics_parser/models.py` & `cg-60.3.1/cg/meta/workflow/microsalt/metrics_parser/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/microsalt/microsalt.py` & `cg-60.3.1/cg/meta/workflow/microsalt/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/microsalt/quality_controller/models.py` & `cg-60.3.1/cg/meta/workflow/microsalt/quality_controller/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/microsalt/quality_controller/quality_controller.py` & `cg-60.3.1/cg/meta/workflow/microsalt/quality_controller/quality_controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/microsalt/quality_controller/report_generator.py` & `cg-60.3.1/cg/meta/workflow/microsalt/quality_controller/report_generator.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/microsalt/quality_controller/result_logger.py` & `cg-60.3.1/cg/meta/workflow/microsalt/quality_controller/result_logger.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/microsalt/quality_controller/utils.py` & `cg-60.3.1/cg/meta/workflow/microsalt/quality_controller/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/microsalt/utils.py` & `cg-60.3.1/cg/meta/workflow/microsalt/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/mip.py` & `cg-60.3.1/cg/meta/workflow/mip.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/mip_dna.py` & `cg-60.3.1/cg/meta/workflow/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/mip_rna.py` & `cg-60.3.1/cg/meta/workflow/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/mutant.py` & `cg-60.3.1/cg/meta/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/nf_analysis.py` & `cg-60.3.1/cg/meta/workflow/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/nf_handlers.py` & `cg-60.3.1/cg/meta/workflow/nf_handlers.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/prepare_fastq.py` & `cg-60.3.1/cg/meta/workflow/prepare_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/raredisease.py` & `cg-60.3.1/cg/meta/workflow/raredisease.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/rnafusion.py` & `cg-60.3.1/cg/meta/workflow/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/taxprofiler.py` & `cg-60.3.1/cg/meta/workflow/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/meta/workflow/tomte.py` & `cg-60.3.1/cg/meta/workflow/tomte.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/balsamic/config.py` & `cg-60.3.1/cg/models/balsamic/config.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/balsamic/metrics.py` & `cg-60.3.1/cg/models/balsamic/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/cg_config.py` & `cg-60.3.1/cg/models/cg_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/compression_data.py` & `cg-60.3.1/cg/models/compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/deliverables/metric_deliverables.py` & `cg-60.3.1/cg/models/deliverables/metric_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/demultiplex/run_parameters.py` & `cg-60.3.1/cg/models/demultiplex/run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/demultiplex/sbatch.py` & `cg-60.3.1/cg/models/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/downsample/downsample_data.py` & `cg-60.3.1/cg/models/downsample/downsample_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/fastq.py` & `cg-60.3.1/cg/models/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/file_data.py` & `cg-60.3.1/cg/models/file_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/flow_cell/flow_cell.py` & `cg-60.3.1/cg/models/flow_cell/flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/invoice/invoice.py` & `cg-60.3.1/cg/models/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/lims/sample.py` & `cg-60.3.1/cg/models/lims/sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/mip/mip_config.py` & `cg-60.3.1/cg/models/mip/mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/mip/mip_metrics_deliverables.py` & `cg-60.3.1/cg/models/mip/mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/mip/mip_sample_info.py` & `cg-60.3.1/cg/models/mip/mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/nf_analysis.py` & `cg-60.3.1/cg/models/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/observations/input_files.py` & `cg-60.3.1/cg/models/observations/input_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/orders/constants.py` & `cg-60.3.1/cg/models/orders/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/orders/excel_sample.py` & `cg-60.3.1/cg/models/orders/excel_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/orders/json_sample.py` & `cg-60.3.1/cg/models/orders/json_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/orders/order.py` & `cg-60.3.1/cg/models/orders/order.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/orders/orderform_schema.py` & `cg-60.3.1/cg/models/orders/orderform_schema.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/orders/sample_base.py` & `cg-60.3.1/cg/models/orders/sample_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/orders/samples.py` & `cg-60.3.1/cg/models/orders/samples.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/orders/validators/excel_sample_validators.py` & `cg-60.3.1/cg/models/orders/validators/excel_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/orders/validators/json_sample_validators.py` & `cg-60.3.1/cg/models/orders/validators/json_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/raredisease/raredisease.py` & `cg-60.3.1/cg/models/raredisease/raredisease.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/report/metadata.py` & `cg-60.3.1/cg/models/report/metadata.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/report/report.py` & `cg-60.3.1/cg/models/report/report.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/report/sample.py` & `cg-60.3.1/cg/models/report/sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/report/validators.py` & `cg-60.3.1/cg/models/report/validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/rnafusion/rnafusion.py` & `cg-60.3.1/cg/models/rnafusion/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/scout/scout_load_config.py` & `cg-60.3.1/cg/models/scout/scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/slurm/sbatch.py` & `cg-60.3.1/cg/models/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/taxprofiler/taxprofiler.py` & `cg-60.3.1/cg/models/taxprofiler/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/tomte/tomte.py` & `cg-60.3.1/cg/models/tomte/tomte.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/models/workflow/mutant.py` & `cg-60.3.1/cg/models/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/resources/__init__.py` & `cg-60.3.1/cg/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/resources/rnafusion_bundle_filenames.yaml` & `cg-60.3.1/cg/resources/rnafusion_bundle_filenames.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/resources/taxprofiler_bundle_filenames.yaml` & `cg-60.3.1/cg/resources/taxprofiler_bundle_filenames.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/resources/tomte_bundle_filenames.yaml` & `cg-60.3.1/cg/resources/tomte_bundle_filenames.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/server/admin.py` & `cg-60.3.1/cg/server/admin.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/server/api.py` & `cg-60.3.1/cg/server/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/server/app.py` & `cg-60.3.1/cg/server/app.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/server/config.py` & `cg-60.3.1/cg/server/config.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/server/dto/orders/orders_request.py` & `cg-60.3.1/cg/server/dto/orders/orders_request.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/server/ext.py` & `cg-60.3.1/cg/server/ext.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/server/invoices/templates/invoices/index.html` & `cg-60.3.1/cg/server/invoices/templates/invoices/index.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/server/invoices/templates/invoices/invoice.html` & `cg-60.3.1/cg/server/invoices/templates/invoices/invoice.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/server/invoices/templates/invoices/layout.html` & `cg-60.3.1/cg/server/invoices/templates/invoices/layout.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/server/invoices/templates/invoices/new.html` & `cg-60.3.1/cg/server/invoices/templates/invoices/new.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/server/invoices/views.py` & `cg-60.3.1/cg/server/invoices/views.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/services/delivery_message/delivery_message_service.py` & `cg-60.3.1/cg/services/delivery_message/delivery_message_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/services/delivery_message/messages/__init__.py` & `cg-60.3.1/cg/services/delivery_message/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/services/delivery_message/messages/analysis_scout_message.py` & `cg-60.3.1/cg/services/delivery_message/messages/analysis_scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/services/delivery_message/messages/covid_message.py` & `cg-60.3.1/cg/services/delivery_message/messages/covid_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/services/delivery_message/messages/fastq_analysis_scout_message.py` & `cg-60.3.1/cg/services/delivery_message/messages/fastq_analysis_scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/services/delivery_message/messages/fastq_message.py` & `cg-60.3.1/cg/services/delivery_message/messages/fastq_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/services/delivery_message/messages/fastq_scout_message.py` & `cg-60.3.1/cg/services/delivery_message/messages/fastq_scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/services/delivery_message/messages/microsalt_mwr_message.py` & `cg-60.3.1/cg/services/delivery_message/messages/microsalt_mwr_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/services/delivery_message/messages/microsalt_mwx_message.py` & `cg-60.3.1/cg/services/delivery_message/messages/microsalt_mwx_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/services/delivery_message/messages/scout_message.py` & `cg-60.3.1/cg/services/delivery_message/messages/scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/services/delivery_message/messages/statina_message.py` & `cg-60.3.1/cg/services/delivery_message/messages/statina_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/services/delivery_message/messages/utils.py` & `cg-60.3.1/cg/services/delivery_message/messages/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/services/delivery_message/utils.py` & `cg-60.3.1/cg/services/delivery_message/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/services/fastq_file_service/fastq_file_service.py` & `cg-60.3.1/cg/services/fastq_file_service/fastq_file_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/services/fastq_file_service/utils.py` & `cg-60.3.1/cg/services/fastq_file_service/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/services/orders/order_service/order_service.py` & `cg-60.3.1/cg/services/orders/order_service/order_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/services/orders/order_service/utils.py` & `cg-60.3.1/cg/services/orders/order_service/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/services/orders/order_status_service/order_summary_service.py` & `cg-60.3.1/cg/services/orders/order_status_service/order_summary_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/services/orders/order_status_service/utils.py` & `cg-60.3.1/cg/services/orders/order_status_service/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/services/slurm_service/slurm_cli_service.py` & `cg-60.3.1/cg/services/slurm_service/slurm_cli_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/services/slurm_upload_service/slurm_upload_service.py` & `cg-60.3.1/cg/services/slurm_upload_service/slurm_upload_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/base.py` & `cg-60.3.1/cg/store/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/crud/create.py` & `cg-60.3.1/cg/store/crud/create.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/crud/delete.py` & `cg-60.3.1/cg/store/crud/delete.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/crud/read.py` & `cg-60.3.1/cg/store/crud/read.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/crud/update.py` & `cg-60.3.1/cg/store/crud/update.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/database.py` & `cg-60.3.1/cg/store/database.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/filters/status_analysis_filters.py` & `cg-60.3.1/cg/store/filters/status_analysis_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/filters/status_application_filters.py` & `cg-60.3.1/cg/store/filters/status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/filters/status_application_limitations_filters.py` & `cg-60.3.1/cg/store/filters/status_application_limitations_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/filters/status_application_version_filters.py` & `cg-60.3.1/cg/store/filters/status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/filters/status_bed_filters.py` & `cg-60.3.1/cg/store/filters/status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/filters/status_bed_version_filters.py` & `cg-60.3.1/cg/store/filters/status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/filters/status_case_filters.py` & `cg-60.3.1/cg/store/filters/status_case_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/filters/status_case_sample_filters.py` & `cg-60.3.1/cg/store/filters/status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/filters/status_collaboration_filters.py` & `cg-60.3.1/cg/store/filters/status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/filters/status_customer_filters.py` & `cg-60.3.1/cg/store/filters/status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/filters/status_flow_cell_filters.py` & `cg-60.3.1/cg/store/filters/status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/filters/status_invoice_filters.py` & `cg-60.3.1/cg/store/filters/status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/filters/status_metrics_filters.py` & `cg-60.3.1/cg/store/filters/status_metrics_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/filters/status_order_filters.py` & `cg-60.3.1/cg/store/filters/status_order_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/filters/status_organism_filters.py` & `cg-60.3.1/cg/store/filters/status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/filters/status_panel_filters.py` & `cg-60.3.1/cg/store/filters/status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/filters/status_pool_filters.py` & `cg-60.3.1/cg/store/filters/status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/filters/status_sample_filters.py` & `cg-60.3.1/cg/store/filters/status_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/filters/status_user_filters.py` & `cg-60.3.1/cg/store/filters/status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/models.py` & `cg-60.3.1/cg/store/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/store/store.py` & `cg-60.3.1/cg/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/utils/checksum/checksum.py` & `cg-60.3.1/cg/utils/checksum/checksum.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/utils/click/EnumChoice.py` & `cg-60.3.1/cg/utils/click/EnumChoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/utils/commands.py` & `cg-60.3.1/cg/utils/commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/utils/date.py` & `cg-60.3.1/cg/utils/date.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/utils/dict.py` & `cg-60.3.1/cg/utils/dict.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/utils/dispatcher.py` & `cg-60.3.1/cg/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/utils/email.py` & `cg-60.3.1/cg/utils/email.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/utils/files.py` & `cg-60.3.1/cg/utils/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/utils/flask/enum.py` & `cg-60.3.1/cg/utils/flask/enum.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/utils/time.py` & `cg-60.3.1/cg/utils/time.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/cg/utils/utils.py` & `cg-60.3.1/cg/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/pyproject.toml` & `cg-60.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cg"
-version = "60.3.0"
+version = "60.3.1"
 description = "Clinical Genomics command center"
 authors = ["Clinical Genomics <support@clinicalgenomics.se>"]
 readme = "README.md"
 homepage = "https://github.com/Clinical-Genomics/cg"
 repository = "https://github.com/Clinical-Genomics/cg"
 classifiers = [
   "Programming Language :: Python",
```

### Comparing `cg-60.3.0/tests/apps/conftest.py` & `cg-60.3.1/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/coverage/test_coverage.py` & `cg-60.3.1/tests/apps/coverage/test_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/crunchy/conftest.py` & `cg-60.3.1/tests/apps/crunchy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/crunchy/test_compress_fastq.py` & `cg-60.3.1/tests/apps/crunchy/test_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/crunchy/test_config.py` & `cg-60.3.1/tests/apps/crunchy/test_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/crunchy/test_crunchy.py` & `cg-60.3.1/tests/apps/crunchy/test_crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/crunchy/test_spring_decompression.py` & `cg-60.3.1/tests/apps/crunchy/test_spring_decompression.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/demultiplex/conftest.py` & `cg-60.3.1/tests/apps/demultiplex/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,31 @@
 from pathlib import Path
 
 import pytest
 
 from cg.apps.demultiplex.sample_sheet.override_cycles_validator import OverrideCyclesValidator
-from cg.apps.demultiplex.sample_sheet.sample_models import (
-    FlowCellSampleBcl2Fastq,
-    FlowCellSampleBCLConvert,
-)
+from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample
 from cg.constants.demultiplexing import SampleSheetBcl2FastqSections, SampleSheetBCLConvertSections
 
 
 @pytest.fixture
-def bcl_convert_samples_similar_index1() -> list[FlowCellSampleBCLConvert]:
+def bcl_convert_samples_similar_index1() -> list[FlowCellSample]:
     """Return a list of three FlowCellSampleBCLConvert with updated indexes."""
-    sample_1 = FlowCellSampleBCLConvert(
-        lane=1, sample_id="ACC123", index="CAGAAGAT", index2="GCGCAAGC"
-    )
-    sample_2 = FlowCellSampleBCLConvert(
-        lane=1, sample_id="ACC456", index="CAGAAGAG", index2="CAATGTAT"
-    )
-    sample_3 = FlowCellSampleBCLConvert(
-        lane=2, sample_id="ACC789", index="AAGCGATA", index2="AACCGCAA"
-    )
+    sample_1 = FlowCellSample(lane=1, sample_id="ACC123", index="CAGAAGAT", index2="GCGCAAGC")
+    sample_2 = FlowCellSample(lane=1, sample_id="ACC456", index="CAGAAGAG", index2="CAATGTAT")
+    sample_3 = FlowCellSample(lane=2, sample_id="ACC789", index="AAGCGATA", index2="AACCGCAA")
     return [sample_1, sample_2, sample_3]
 
 
 @pytest.fixture
-def bcl_convert_samples_similar_index2() -> list[FlowCellSampleBCLConvert]:
+def bcl_convert_samples_similar_index2() -> list[FlowCellSample]:
     """Return a list of three FlowCellSampleBCLConvert with updated indexes."""
-    sample_1 = FlowCellSampleBCLConvert(
-        lane=1, sample_id="ACC123", index="GCGCAAGC", index2="CAATGTAC"
-    )
-    sample_2 = FlowCellSampleBCLConvert(
-        lane=1, sample_id="ACC456", index="CAATGTAT", index2="CAATGTAT"
-    )
-    sample_3 = FlowCellSampleBCLConvert(
-        lane=2, sample_id="ACC789", index="AAGCGATA", index2="AACCGCAA"
-    )
+    sample_1 = FlowCellSample(lane=1, sample_id="ACC123", index="GCGCAAGC", index2="CAATGTAC")
+    sample_2 = FlowCellSample(lane=1, sample_id="ACC456", index="CAATGTAT", index2="CAATGTAT")
+    sample_3 = FlowCellSample(lane=2, sample_id="ACC789", index="AAGCGATA", index2="AACCGCAA")
     return [sample_1, sample_2, sample_3]
 
 
 # Sample sheet validation
 
 
 @pytest.fixture
@@ -175,72 +160,52 @@
             "814206",
         ]
     )
     return valid_sample_sheet_bcl2fastq
 
 
 @pytest.fixture
-def novaseq6000_flow_cell_sample_1() -> FlowCellSampleBcl2Fastq:
+def novaseq6000_flow_cell_sample_1() -> FlowCellSample:
     """Return a NovaSeq sample."""
-    return FlowCellSampleBcl2Fastq(
-        FCID="HWHMWDMXX",
-        Lane=1,
-        SampleID="ACC7628A68",
-        SampleRef="hg19",
+    return FlowCellSample(
+        lane=1,
+        sample_id="ACC7628A68",
         index="ATTCCACACT",
         index2="TGGTCTTGTT",
-        SampleName="814206",
-        Control="N",
-        Recipe="R1",
-        Operator="script",
-        Project="814206",
     )
 
 
 @pytest.fixture
-def novaseq6000_flow_cell_sample_2() -> FlowCellSampleBcl2Fastq:
+def novaseq6000_flow_cell_sample_2() -> FlowCellSample:
     """Return a NovaSeq sample."""
-    return FlowCellSampleBcl2Fastq(
-        FCID="HWHMWDMXX",
-        Lane=2,
-        SampleID="ACC7628A1",
-        SampleRef="hg19",
+    return FlowCellSample(
+        lane=2,
+        sample_id="ACC7628A1",
         index="ATTCCACACT",
         index2="TGGTCTTGTT",
-        SampleName="814206",
-        Control="N",
-        Recipe="R1",
-        Operator="script",
-        Project="814206",
     )
 
 
 @pytest.fixture
-def novaseq6000_flow_cell_sample_no_dual_index() -> FlowCellSampleBcl2Fastq:
+def novaseq6000_flow_cell_sample_no_dual_index() -> FlowCellSample:
     """Return a NovaSeq sample without dual indexes."""
-    return FlowCellSampleBcl2Fastq(
-        FCID="HWHMWDMXX",
-        Lane=2,
-        SampleID="ACC7628A1",
+    return FlowCellSample(
+        lane=2,
+        sample_id="ACC7628A1",
         index="ATTCCACACT",
-        SampleName="814206",
-        Project="814206",
     )
 
 
 @pytest.fixture
-def novaseq6000_flow_cell_sample_before_adapt_indexes() -> FlowCellSampleBcl2Fastq:
+def novaseq6000_flow_cell_sample_before_adapt_indexes() -> FlowCellSample:
     """Return a NovaSeq sample without dual indexes."""
-    return FlowCellSampleBcl2Fastq(
-        FCID="HWHMWDMXX",
-        Lane=2,
-        SampleID="ACC7628A1",
+    return FlowCellSample(
+        lane=2,
+        sample_id="ACC7628A1",
         index="ATTCCACACT-TGGTCTTGTT",
-        SampleName="814206",
-        Project="814206",
     )
 
 
 @pytest.fixture
 def index1_8_nt_sequence_from_lims() -> str:
     """Return an index 1 sequence."""
     return "GTCTACAC"
@@ -269,17 +234,17 @@
     index1_8_nt_sequence_from_lims: str, index2_8_nt_sequence_from_lims: str
 ) -> str:
     """Return a raw index."""
     return f"{index1_8_nt_sequence_from_lims}-{index2_8_nt_sequence_from_lims}"
 
 
 @pytest.fixture
-def bcl_convert_flow_cell_sample(raw_index_sequence: str) -> FlowCellSampleBCLConvert:
+def bcl_convert_flow_cell_sample(raw_index_sequence: str) -> FlowCellSample:
     """Return a BCL Convert sample."""
-    return FlowCellSampleBCLConvert(lane=1, index=raw_index_sequence, sample_id="ACC123")
+    return FlowCellSample(lane=1, index=raw_index_sequence, sample_id="ACC123")
 
 
 @pytest.fixture
 def bcl_convert_sample_sheet_path(illumina_demultiplexed_runs_directory):
     return Path(
         illumina_demultiplexed_runs_directory,
         "230504_A00689_0804_BHY7FFDRX2",
```

### Comparing `cg-60.3.0/tests/apps/demultiplex/test_create_sample_sheet.py` & `cg-60.3.1/tests/apps/demultiplex/test_create_sample_sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from pathlib import Path
 from typing import Any
 
 import pytest
 from _pytest.logging import LogCaptureFixture
 from pytest_mock import MockFixture
 
-from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSampleBCLConvert
+from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample
 from cg.exc import HousekeeperFileMissingError
 from cg.models.cg_config import CGConfig
 from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
 from tests.store_helpers import StoreHelpers
 
 GET_FLOW_CELL_SAMPLES: str = "cg.apps.demultiplex.sample_sheet.api.get_flow_cell_samples"
 
 
 def test_get_create_sample_sheet_hk_has_bcl2fastq_sample_sheet(
     sample_sheet_context_broken_flow_cells: CGConfig,
     tmp_flow_cell_with_bcl2fastq_sample_sheet: Path,
     sample_sheet_bcl2fastq_bundle_data: dict[str, Any],
-    hiseq_x_single_index_bcl_convert_lims_samples: list[FlowCellSampleBCLConvert],
+    hiseq_x_single_index_bcl_convert_lims_samples: list[FlowCellSample],
     helpers: StoreHelpers,
     mocker: MockFixture,
 ):
     """Test that a BCL2FASTQ sample sheet in Housekeeper is updated to BCLConvert."""
     # GIVEN a sample sheet context with a sample sheet API and a Housekeeper API
     sample_sheet_api = sample_sheet_context_broken_flow_cells.sample_sheet_api
     hk_api = sample_sheet_context_broken_flow_cells.housekeeper_api
@@ -49,15 +49,15 @@
     # THEN the sample sheet in the flow cell is replaced with the BCLConvert sample sheet
     sample_sheet_api.validate_sample_sheet(flow_cell.sample_sheet_path)
 
 
 def test_get_create_sample_sheet_flow_cell_has_bcl2fastq_sample_sheet(
     sample_sheet_context_broken_flow_cells: CGConfig,
     tmp_flow_cell_with_bcl2fastq_sample_sheet: Path,
-    hiseq_x_single_index_bcl_convert_lims_samples: list[FlowCellSampleBCLConvert],
+    hiseq_x_single_index_bcl_convert_lims_samples: list[FlowCellSample],
     mocker: MockFixture,
     caplog: LogCaptureFixture,
 ):
     """
     Test that a BCL2FASTQ sample sheet in the flow cell directory is updated to BCLConvert
     and added to Housekeeeper.
     """
```

### Comparing `cg-60.3.0/tests/apps/demultiplex/test_demultiplex_api.py` & `cg-60.3.1/tests/apps/demultiplex/test_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/demultiplex/test_index.py` & `cg-60.3.1/tests/apps/demultiplex/test_index.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,48 +2,17 @@
 
 import pytest
 
 from cg.apps.demultiplex.sample_sheet.index import (
     get_hamming_distance_index_1,
     get_hamming_distance_index_2,
     get_reverse_complement_dna_seq,
-    is_padding_needed,
 )
 
 
-@pytest.mark.parametrize(
-    "index1_cycles, index2_cycles, sample_index_length, expected_is_padding_needed",
-    [
-        (10, 10, 8, True),
-        (10, 10, 10, False),
-        (17, 8, 17, False),
-        (8, 8, 10, False),
-        (8, 8, 8, False),
-    ],
-)
-def test_is_padding_needed(
-    index1_cycles: int,
-    index2_cycles: int,
-    sample_index_length: int,
-    expected_is_padding_needed: bool,
-):
-    """Test that evaluating if a situation needs padding returns the expected value."""
-    # GIVEN a sample index length and the number of index cycles reads stated in the run parameters
-
-    # WHEN checking if padding is needed
-    padding_needed: bool = is_padding_needed(
-        index1_cycles=index1_cycles,
-        index2_cycles=index2_cycles,
-        sample_index_length=sample_index_length,
-    )
-
-    # THEN assert that the result is the expected
-    assert padding_needed == expected_is_padding_needed
-
-
 def test_get_reverse_complement():
     """Test that getting the reverse complement of a DNA strain returns the correct sequence."""
     # GIVEN a DNA strain and its reverse complement
     dna_strain: str = "ACCTCTGT"
     reversed_complement: str = "ACAGAGGT"
 
     # WHEN getting the reverse complement of the DNA strain
```

### Comparing `cg-60.3.0/tests/apps/demultiplex/test_override_cycles_validator.py` & `cg-60.3.1/tests/apps/demultiplex/test_override_cycles_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/demultiplex/test_read_sample_sheet.py` & `cg-60.3.1/tests/apps/demultiplex/test_read_sample_sheet.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,38 @@
 import logging
-from pathlib import Path
-from typing import Type
 
 import pytest
 
 from cg.apps.demultiplex.sample_sheet.read_sample_sheet import (
     get_raw_samples_from_content,
-    get_sample_type_from_content,
     get_samples_by_lane,
     validate_samples_are_unique,
 )
-from cg.apps.demultiplex.sample_sheet.sample_models import (
-    FlowCellSample,
-    FlowCellSampleBcl2Fastq,
-    FlowCellSampleBCLConvert,
-)
-from cg.constants.constants import FileFormat
+from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample
 from cg.exc import SampleSheetError
-from cg.io.controller import ReadFile
 
 
 def test_validate_samples_are_unique(
-    novaseq6000_flow_cell_sample_1: FlowCellSampleBcl2Fastq,
-    novaseq6000_flow_cell_sample_2: FlowCellSampleBcl2Fastq,
+    novaseq6000_flow_cell_sample_1: FlowCellSample,
+    novaseq6000_flow_cell_sample_2: FlowCellSample,
 ):
     """Test that validating two different samples finishes successfully."""
     # GIVEN two different NovaSeq samples
     assert novaseq6000_flow_cell_sample_1 != novaseq6000_flow_cell_sample_2
 
     # WHEN validating the samples
     validate_samples_are_unique(
         samples=[novaseq6000_flow_cell_sample_1, novaseq6000_flow_cell_sample_2]
     )
 
     # THEN no error is raised
 
 
 def test_validate_samples_are_unique_when_not_unique(
-    novaseq6000_flow_cell_sample_1: FlowCellSampleBcl2Fastq, caplog
+    novaseq6000_flow_cell_sample_1: FlowCellSample, caplog
 ):
     """Test that validating two identical samples fails."""
     # GIVEN two identical NovaSeq samples
     caplog.set_level(logging.INFO)
 
     # WHEN validating the samples
     with pytest.raises(SampleSheetError):
@@ -53,16 +44,16 @@
     assert (
         f"Sample {novaseq6000_flow_cell_sample_1.sample_id} exists multiple times in sample sheet"
         in caplog.text
     )
 
 
 def test_get_samples_by_lane(
-    novaseq6000_flow_cell_sample_1: FlowCellSampleBcl2Fastq,
-    novaseq6000_flow_cell_sample_2: FlowCellSampleBcl2Fastq,
+    novaseq6000_flow_cell_sample_1: FlowCellSample,
+    novaseq6000_flow_cell_sample_2: FlowCellSample,
 ):
     """Test that grouping two samples with different lanes returns two groups."""
     # GIVEN two samples on two different lanes
 
     # WHEN getting the samples per lane
     samples_per_lane: dict[int, list[FlowCellSample]] = get_samples_by_lane(
         samples=[novaseq6000_flow_cell_sample_1, novaseq6000_flow_cell_sample_2]
@@ -111,33 +102,7 @@
 
     # WHEN trying to get the samples from the sample sheet
     with pytest.raises(SampleSheetError):
         get_raw_samples_from_content(sample_sheet_content=sample_sheet_bcl2fastq_data_header)
 
     # THEN an exception is raised because of the missing samples
     assert "Could not find any samples in sample sheet" in caplog.text
-
-
-def test_get_sample_type_for_bcl_convert(bcl_convert_sample_sheet_path: Path):
-    # GIVEN a bcl convert sample sheet path
-
-    # WHEN getting the sample type
-    content: list[list[str]] = ReadFile.get_content_from_file(
-        file_format=FileFormat.CSV, file_path=bcl_convert_sample_sheet_path
-    )
-    sample_type: Type[FlowCellSample] = get_sample_type_from_content(content)
-
-    # THEN the sample type is FlowCellSampleBCLConvert
-    assert sample_type is FlowCellSampleBCLConvert
-
-
-def test_get_sample_type_for_bcl2fastq(hiseq_x_single_index_bcl2fastq_sample_sheet_path: Path):
-    # GIVEN a bcl convert sample sheet path
-
-    # WHEN getting the sample type
-    content: list[list[str]] = ReadFile.get_content_from_file(
-        file_format=FileFormat.CSV, file_path=hiseq_x_single_index_bcl2fastq_sample_sheet_path
-    )
-    sample_type: Type[FlowCellSample] = get_sample_type_from_content(content)
-
-    # THEN the sample type is FlowCellSampleBCLConvert
-    assert sample_type is FlowCellSampleBcl2Fastq
```

### Comparing `cg-60.3.0/tests/apps/demultiplex/test_sample_models.py` & `cg-60.3.1/tests/apps/demultiplex/test_sample_models.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,12 @@
-from unittest.mock import Mock
-
 import pytest
 
-from cg.apps.demultiplex.sample_sheet.index import (
-    INDEX_ONE_PAD_SEQUENCE,
-    INDEX_TWO_PAD_SEQUENCE,
-    LONG_INDEX_CYCLE_NR,
-    SHORT_SAMPLE_INDEX_LENGTH,
-    get_reverse_complement_dna_seq,
-)
-from cg.apps.demultiplex.sample_sheet.sample_models import (
-    FlowCellSampleBcl2Fastq,
-    FlowCellSampleBCLConvert,
-)
-from cg.constants.demultiplexing import (
-    NO_REVERSE_COMPLEMENTS_INDEX_SETTINGS,
-    NOVASEQ_6000_POST_1_5_KITS_INDEX_SETTINGS,
-    IndexOverrideCycles,
-    IndexSettings,
-)
+from cg.apps.demultiplex.sample_sheet.index import get_reverse_complement_dna_seq
+from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample
+from cg.constants.demultiplexing import IndexOverrideCycles
 from cg.constants.symbols import EMPTY_STRING
 from cg.models.demultiplex.run_parameters import RunParameters
 
 
 @pytest.mark.parametrize(
     "lims_sample",
     [
@@ -34,15 +18,15 @@
 )
 def test_validate_inputs_bcl_convert_sample_missing_attribute(lims_sample: dict):
     """Test that validating a BCLConvert sample with a missing attribute fails."""
     # GIVEN a raw LIMS sample without a mandatory attribute
 
     # WHEN validating the sample
     with pytest.raises(AttributeError) as exc_info:
-        FlowCellSampleBCLConvert.validate_inputs(lims_sample=lims_sample)
+        FlowCellSample.validate_inputs(lims_sample=lims_sample)
 
     # THEN a pydantic validation error is raised
     assert "validate_inputs" in str(exc_info.value)
 
 
 @pytest.mark.parametrize(
     "lims_index, expected_index_1, expected_index2",
@@ -60,121 +44,39 @@
         "single index with dash",
         "index with newline",
     ],
 )
 def test_separate_indexes_dual_run(lims_index: str, expected_index_1: str, expected_index2: str):
     """Test that parsing different kinds of dual-run raw indexes as index and index2 works."""
     # GIVEN a sample sheet with a single sample on one lane
-    sample = FlowCellSampleBCLConvert(lane=1, index=lims_index, sample_id="ACC123")
+    sample = FlowCellSample(lane=1, index=lims_index, sample_id="ACC123")
 
     # WHEN separating the index
     sample.separate_indexes(is_run_single_index=False)
 
     # THEN the index should be separated
     assert sample.index == expected_index_1
     assert sample.index2 == expected_index2
 
 
 def test_separate_indexes_single_run(
-    index1_8_nt_sequence_from_lims: str, bcl_convert_flow_cell_sample: FlowCellSampleBCLConvert
+    index1_8_nt_sequence_from_lims: str, bcl_convert_flow_cell_sample: FlowCellSample
 ):
     """Test index2 is ignored when parsing a double index in a single index run."""
     # GIVEN a sample with a double index
 
     # WHEN separating the index
     bcl_convert_flow_cell_sample.separate_indexes(is_run_single_index=True)
 
     # THEN the index should be separated
     assert bcl_convert_flow_cell_sample.index == index1_8_nt_sequence_from_lims
     assert bcl_convert_flow_cell_sample.index2 == EMPTY_STRING
 
 
 @pytest.mark.parametrize(
-    "index_settings, expected_index2",
-    [
-        (NOVASEQ_6000_POST_1_5_KITS_INDEX_SETTINGS, f"{INDEX_TWO_PAD_SEQUENCE}GCCAAGGT"),
-        (NO_REVERSE_COMPLEMENTS_INDEX_SETTINGS, f"GCCAAGGT{INDEX_TWO_PAD_SEQUENCE}"),
-    ],
-    ids=["reverse complement", "no reverse complement"],
-)
-def test_pad_indexes_needs_padding(index_settings: IndexSettings, expected_index2: str):
-    """Test that indexes that need to be padded are padded with and without reverse complement."""
-    # GIVEN an IndexSettings object
-
-    # GIVEN a run parameters file with 10-nt indexes and the index settings
-    mock_run_parameters = Mock(
-        spec=RunParameters,
-        get_index_1_cycles=Mock(return_value=10),
-        get_index_2_cycles=Mock(return_value=10),
-        index_settings=index_settings,
-    )
-
-    # GIVEN a FlowCellSampleBcl2Fastq with 8-nt indexes
-    sample = FlowCellSampleBcl2Fastq(
-        lane=1, index="GTCTACAC-GCCAAGGT", sample_id="ACC123", project="project", sample_name="name"
-    )
-    sample.separate_indexes(is_run_single_index=False)
-
-    # WHEN padding the indexes
-    sample._pad_indexes_if_necessary(run_parameters=mock_run_parameters)
-
-    # THEN the indexes were correctly padded
-    assert_correct_padding(
-        sample=sample,
-        index_length=LONG_INDEX_CYCLE_NR,
-        index1_value=f"GTCTACAC{INDEX_ONE_PAD_SEQUENCE}",
-        index2_value=expected_index2,
-    )
-
-
-def assert_correct_padding(
-    sample: FlowCellSampleBcl2Fastq, index_length: int, index1_value: str, index2_value: str
-):
-    """Assert that the indexes have the correct length and are correctly padded."""
-    assert len(sample.index) == index_length
-    assert sample.index == index1_value
-    # THEN the second index was correctly padded
-    assert len(sample.index2) == index_length
-    assert sample.index2 == index2_value
-
-
-def test_pad_indexes_no_padding():
-    """Test that indexes that do not need to be padded are not padded."""
-    # GIVEN a RunParameters with 8-nt indexes
-    mock_run_parameters = Mock(
-        spec=RunParameters,
-        get_index_1_cycles=Mock(return_value=8),
-        get_index_2_cycles=Mock(return_value=8),
-    )
-
-    # GIVEN a FlowCellSampleBcl2Fastq with 8-nt indexes
-    initial_index1: str = "GTCTACAC"
-    initial_index2: str = "GCCAAGGT"
-    sample = FlowCellSampleBcl2Fastq(
-        lane=1,
-        index=f"{initial_index1}-{initial_index2}",
-        sample_id="ACC123",
-        project="project",
-        sample_name="name",
-    )
-    sample.separate_indexes(is_run_single_index=False)
-
-    # WHEN trying to pad the indexes
-    sample._pad_indexes_if_necessary(run_parameters=mock_run_parameters)
-
-    # THEN the indexes were not padded
-    assert_correct_padding(
-        sample=sample,
-        index_length=SHORT_SAMPLE_INDEX_LENGTH,
-        index1_value=initial_index1,
-        index2_value=initial_index2,
-    )
-
-
-@pytest.mark.parametrize(
     "lims_index, index1_cycles, expected_parsed_cycles",
     [
         ("CGATAGCAGG", 10, IndexOverrideCycles.FULL_10_INDEX),
         ("CCATTCGANNNNNNNNN-GTTGTCCG", 8, IndexOverrideCycles.FULL_8_INDEX),
         ("GTTCCAAT", 8, IndexOverrideCycles.FULL_8_INDEX),
         ("GTTCCAAT", 10, IndexOverrideCycles.INDEX_8_IGNORED_2),
     ],
@@ -186,15 +88,15 @@
     ],
 )
 def test_get_index1_override_cycles(
     lims_index: str, index1_cycles: int, expected_parsed_cycles: str
 ):
     """Test that the returned index 1 cycles is the expected for different index configurations."""
     # GIVEN a FlowCellSampleBCLConvert with an index
-    sample = FlowCellSampleBCLConvert(lane=1, index=lims_index, sample_id="ACC123")
+    sample = FlowCellSample(lane=1, index=lims_index, sample_id="ACC123")
 
     # WHEN getting the index1 override cycles
     index1_cycles: str = sample._get_index1_override_cycles(len_index1_cycles=index1_cycles)
 
     # THEN the index1 override cycles value is the expected one
     assert index1_cycles == expected_parsed_cycles
 
@@ -221,15 +123,15 @@
     ],
 )
 def test_get_index2_override_cycles(
     lims_index: str, index2_cycles: int, reverse_cycle: bool, expected_parsed_cycles: str
 ):
     """Test that the returned index 2 cycles is the expected for different index configurations."""
     # GIVEN a FlowCellSampleBCLConvert with separated indexes
-    sample = FlowCellSampleBCLConvert(lane=1, index=lims_index, sample_id="ACC123")
+    sample = FlowCellSample(lane=1, index=lims_index, sample_id="ACC123")
     is_run_single_index: bool = not bool(index2_cycles)
     sample.separate_indexes(is_run_single_index=is_run_single_index)
 
     # WHEN getting the index2 override cycles
     index2_cycles: str = sample._get_index2_override_cycles(
         len_index2_cycles=index2_cycles, reverse_cycle=reverse_cycle
     )
@@ -247,15 +149,15 @@
         "hiseq_2500_custom_index_run_parameters",
         "novaseq_6000_run_parameters_pre_1_5_kits",
         "novaseq_6000_run_parameters_post_1_5_kits",
         "novaseq_x_run_parameters",
     ],
 )
 def test_update_override_cycles(
-    bcl_convert_flow_cell_sample: FlowCellSampleBCLConvert,
+    bcl_convert_flow_cell_sample: FlowCellSample,
     run_parameters_fixture: str,
     request: pytest.FixtureRequest,
 ):
     """Test that updating a sample's override cycles works for different run parameters objects."""
     # GIVEN a run parameters object
     run_parameters: RunParameters = request.getfixturevalue(run_parameters_fixture)
 
@@ -279,18 +181,18 @@
     ids=["barcode1_0", "barcode1_1"],
 )
 def test_update_barcode_mismatches_1(
     sample_list_fixture: str, expected_barcode_mismatch: int, request: pytest.FixtureRequest
 ):
     """Test that index 1 barcode mismatches values are as expected for different sets of samples."""
     # GIVEN a list of FlowCellSampleBCLConvert
-    sample_list: list[FlowCellSampleBCLConvert] = request.getfixturevalue(sample_list_fixture)
+    sample_list: list[FlowCellSample] = request.getfixturevalue(sample_list_fixture)
 
     # GIVEN a FlowCellSampleBCLConvert
-    sample_to_update: FlowCellSampleBCLConvert = sample_list[0]
+    sample_to_update: FlowCellSample = sample_list[0]
 
     # WHEN updating the value for index 1 barcode mismatches
     sample_to_update._update_barcode_mismatches_1(samples_to_compare=sample_list)
 
     # THEN the value for index 1 barcode mismatches is updated with the expected value
     assert sample_to_update.barcode_mismatches_1 == expected_barcode_mismatch
 
@@ -301,18 +203,18 @@
     ids=["barcode2_0", "barcode2_1"],
 )
 def test_update_barcode_mismatches_2(
     sample_list_fixture: str, expected_barcode_mismatch: int, request: pytest.FixtureRequest
 ):
     """Test that index 2 barcode mismatches values are as expected for different sets of samples."""
     # GIVEN a list of FlowCellSampleBCLConvert
-    sample_list: list[FlowCellSampleBCLConvert] = request.getfixturevalue(sample_list_fixture)
+    sample_list: list[FlowCellSample] = request.getfixturevalue(sample_list_fixture)
 
     # GIVEN a FlowCellSampleBCLConvert
-    sample_to_update: FlowCellSampleBCLConvert = sample_list[0]
+    sample_to_update: FlowCellSample = sample_list[0]
 
     # WHEN updating the value for index 2 barcode mismatches
     sample_to_update._update_barcode_mismatches_2(
         samples_to_compare=sample_list, is_reverse_complement=False
     )
 
     # THEN the value for index 2 barcode mismatches is updated with the expected value
@@ -351,20 +253,18 @@
 )
 def test_process_indexes_for_sample_sheet_bcl_convert(
     run_parameters_fixture: str, raw_lims_samples_fixture: str, request: pytest.FixtureRequest
 ):
     """Test that indexes are processed correctly for a BCLConvert sample."""
     # GIVEN a run parameters object and a list of BCLConvert samples from a flow cell
     run_parameters: RunParameters = request.getfixturevalue(run_parameters_fixture)
-    raw_lims_samples: list[FlowCellSampleBCLConvert] = request.getfixturevalue(
-        raw_lims_samples_fixture
-    )
+    raw_lims_samples: list[FlowCellSample] = request.getfixturevalue(raw_lims_samples_fixture)
 
     # GIVEN a FlowCellSampleBCLConvert
-    sample: FlowCellSampleBCLConvert = raw_lims_samples[0]
+    sample: FlowCellSample = raw_lims_samples[0]
 
     # WHEN processing the sample for a sample sheet
     sample.process_indexes(run_parameters=run_parameters)
 
     # THEN the sample is processed correctly
     assert "-" not in sample.index
     assert sample.override_cycles != EMPTY_STRING
@@ -388,24 +288,24 @@
         "HiSeq2500 custom index",
         "NovaSeq6000 pre1.5",
         "NovaSeq6000 post1.5",
         "NovaSeqX",
     ],
 )
 def test_process_indexes_bcl_convert(
-    bcl_convert_flow_cell_sample: FlowCellSampleBCLConvert,
+    bcl_convert_flow_cell_sample: FlowCellSample,
     run_parameters_fixture: str,
     expected_index2: str,
     request: pytest.FixtureRequest,
 ):
     """Test that processing indexes of a BCLConvert sample from different sequencers work."""
     # GIVEN a run parameters object
     run_parameters: RunParameters = request.getfixturevalue(run_parameters_fixture)
 
-    # GIVEN a FlowCellSampleBcl2Fastq with 8-nt indexes
+    # GIVEN a FlowCellSampleBclConvert with 8-nt indexes
 
     # WHEN processing the sample for a sample sheet
     bcl_convert_flow_cell_sample.process_indexes(run_parameters=run_parameters)
 
     # THEN the sample indexes and override cycles are processed
     assert bcl_convert_flow_cell_sample.index2 == expected_index2
     assert bcl_convert_flow_cell_sample.override_cycles != EMPTY_STRING
```

### Comparing `cg-60.3.0/tests/apps/demultiplex/test_sample_sheet_creator.py` & `cg-60.3.1/tests/apps/demultiplex/test_sample_sheet_creator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """Tests for the SampleSheetCreator classes."""
 
 from pathlib import Path
 
 from cg.apps.demultiplex.sample_sheet.read_sample_sheet import get_flow_cell_samples_from_content
-from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample, FlowCellSampleBCLConvert
+from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample
 from cg.apps.demultiplex.sample_sheet.sample_sheet_creator import SampleSheetCreator
 
 
 def test_construct_bcl_convert_sheet(
     bcl_convert_sample_sheet_creator: SampleSheetCreator, project_dir: Path
 ):
     """Test that a created BCL Convert sample sheet has samples."""
     # GIVEN a BCL convert sample sheet creator populated with BCL convert samples
     assert bcl_convert_sample_sheet_creator.lims_samples
 
     # WHEN building the sample sheet content
     content: list[list[str]] = bcl_convert_sample_sheet_creator.construct_sample_sheet()
 
     # THEN a correctly formatted sample sheet was created
-    samples: list[FlowCellSample] = get_flow_cell_samples_from_content(
-        sample_sheet_content=content, sample_type=FlowCellSampleBCLConvert
-    )
+    samples: list[FlowCellSample] = get_flow_cell_samples_from_content(content)
     assert samples
```

### Comparing `cg-60.3.0/tests/apps/demultiplex/test_sample_sheet_models.py` & `cg-60.3.1/tests/apps/demultiplex/test_sample_sheet_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSampleBCLConvert
+from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample
 from cg.apps.demultiplex.sample_sheet.sample_sheet_models import SampleSheet
 from cg.apps.demultiplex.sample_sheet.sample_sheet_validator import SampleSheetValidator
 from cg.apps.demultiplex.sample_sheet.validators import is_valid_sample_internal_id
 
 
 def test_get_non_pooled_samples_when_no_samples():
     # GIVEN a sample sheet with no samples
@@ -13,42 +13,42 @@
 
     # THEN no samples should be returned
     assert not samples
 
 
 def test_get_non_pooled_samples_when_multiple_samples_same_lane():
     # GIVEN a sample sheet with multiple samples on the same lane
-    sample1 = FlowCellSampleBCLConvert(lane=1, sample_id="ACC123", index="A")
-    sample2 = FlowCellSampleBCLConvert(lane=1, sample_id="ACC456", index="A")
+    sample1 = FlowCellSample(lane=1, sample_id="ACC123", index="A")
+    sample2 = FlowCellSample(lane=1, sample_id="ACC456", index="A")
     sample_sheet = SampleSheet(samples=[sample1, sample2])
 
     # WHEN retrieving any non pooled samples
     samples = sample_sheet.get_non_pooled_samples()
 
     # THEN no samples should be returned
     assert not samples
 
 
 def test_get_non_pooled_samples_when_single_sample_one_lane():
     # GIVEN a sample sheet with a single sample on one lane
-    non_pooled_sample = FlowCellSampleBCLConvert(lane=1, sample_id="ACC123", index="A")
+    non_pooled_sample = FlowCellSample(lane=1, sample_id="ACC123", index="A")
     sample_sheet = SampleSheet(samples=[non_pooled_sample])
 
     # WHEN retrieving any non pooled samples
     samples = sample_sheet.get_non_pooled_samples()
 
     # THEN the non pooled sample should be returned
     assert samples == [non_pooled_sample]
 
 
 def test_get_non_pooled_samples_when_multiple_lanes_one_single():
     # GIVEN a sample sheet with multiple lanes and a single sample in one lane
-    sample1 = FlowCellSampleBCLConvert(lane=1, sample_id="ACC123", index="A")
-    sample2 = FlowCellSampleBCLConvert(lane=1, sample_id="ACC456", index="A")
-    non_pooled_sample = FlowCellSampleBCLConvert(lane=2, sample_id="ACC789", index="A")
+    sample1 = FlowCellSample(lane=1, sample_id="ACC123", index="A")
+    sample2 = FlowCellSample(lane=1, sample_id="ACC456", index="A")
+    non_pooled_sample = FlowCellSample(lane=2, sample_id="ACC789", index="A")
     sample_sheet = SampleSheet(samples=[sample1, sample2, non_pooled_sample])
 
     # WHEN retrieving any non pooled samples
     samples = sample_sheet.get_non_pooled_samples()
 
     # THEN the non pooled sample should be returned
     assert samples == [non_pooled_sample]
```

### Comparing `cg-60.3.0/tests/apps/demultiplex/test_sample_sheet_validator.py` & `cg-60.3.1/tests/apps/demultiplex/test_sample_sheet_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/demultiplex/test_validate.py` & `cg-60.3.1/tests/apps/demultiplex/test_validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSampleBcl2Fastq
+from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample
 from cg.apps.demultiplex.sample_sheet.validators import is_valid_sample_internal_id
 
 
 def test_is_valid_sample_internal_id(
-    novaseq6000_flow_cell_sample_1: FlowCellSampleBcl2Fastq,
-    novaseq6000_flow_cell_sample_2: FlowCellSampleBcl2Fastq,
+    novaseq6000_flow_cell_sample_1: FlowCellSample,
+    novaseq6000_flow_cell_sample_2: FlowCellSample,
 ):
     """Test that validating two different samples finishes successfully."""
     # GIVEN two different NovaSeq samples with valid internal IDs
 
     # WHEN validating the sample internal ids
     for sample in [novaseq6000_flow_cell_sample_1, novaseq6000_flow_cell_sample_2]:
         # THEN no error is raised
         assert is_valid_sample_internal_id(sample_internal_id=sample.sample_id)
 
 
 def test_is_valid_sample_internal_id_invalid_sample_internal_ids(
-    novaseq6000_flow_cell_sample_1: FlowCellSampleBcl2Fastq,
-    novaseq6000_flow_cell_sample_2: FlowCellSampleBcl2Fastq,
+    novaseq6000_flow_cell_sample_1: FlowCellSample,
+    novaseq6000_flow_cell_sample_2: FlowCellSample,
 ):
     """Test that validating two different samples finishes successfully."""
     # GIVEN two different NovaSeq samples with valid internal IDs
 
     # WHEN setting the sample internal ids to invalid values
     novaseq6000_flow_cell_sample_1.sample_id = "invalid_sample_id"
     novaseq6000_flow_cell_sample_2.sample_id = "invalid_sample_id"
```

### Comparing `cg-60.3.0/tests/apps/downsample/test_downsample.py` & `cg-60.3.1/tests/apps/downsample/test_downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/downsample/test_downsample_utils.py` & `cg-60.3.1/tests/apps/downsample/test_downsample_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/gens/test_gens_api.py` & `cg-60.3.1/tests/apps/gens/test_gens_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/gt/conftest.py` & `cg-60.3.1/tests/apps/gt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/gt/test_gt_api.py` & `cg-60.3.1/tests/apps/gt/test_gt_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/hk/conftest.py` & `cg-60.3.1/tests/apps/hk/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/hk/test__getattr__.py` & `cg-60.3.1/tests/apps/hk/test__getattr__.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/hk/test_add_file.py` & `cg-60.3.1/tests/apps/hk/test_add_file.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/hk/test_bundles.py` & `cg-60.3.1/tests/apps/hk/test_bundles.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/hk/test_core.py` & `cg-60.3.1/tests/apps/hk/test_core.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/hk/test_file.py` & `cg-60.3.1/tests/apps/hk/test_file.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/hk/test_version.py` & `cg-60.3.1/tests/apps/hk/test_version.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/lims/conftest.py` & `cg-60.3.1/tests/apps/lims/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/lims/test_api.py` & `cg-60.3.1/tests/apps/lims/test_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/lims/test_sample_sheet.py` & `cg-60.3.1/tests/apps/lims/test_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/loqus/conftest.py` & `cg-60.3.1/tests/apps/loqus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/loqus/test_loqusdb_api.py` & `cg-60.3.1/tests/apps/loqus/test_loqusdb_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/madeline/conftest.py` & `cg-60.3.1/tests/apps/madeline/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/madeline/test_madeline.py` & `cg-60.3.1/tests/apps/madeline/test_madeline.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/mip/conftest.py` & `cg-60.3.1/tests/apps/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/mip/test_config_mip.py` & `cg-60.3.1/tests/apps/mip/test_config_mip.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/mutacc_auto/conftest.py` & `cg-60.3.1/tests/apps/mutacc_auto/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/mutacc_auto/test_mutacc_auto.py` & `cg-60.3.1/tests/apps/mutacc_auto/test_mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/orderform/conftest.py` & `cg-60.3.1/tests/apps/orderform/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/orderform/test_excel_orderform_parser.py` & `cg-60.3.1/tests/apps/orderform/test_excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/orderform/test_excel_sample_schema.py` & `cg-60.3.1/tests/apps/orderform/test_excel_sample_schema.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/orderform/test_json_orderform_parser.py` & `cg-60.3.1/tests/apps/orderform/test_json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/orderform/test_orderform_parser.py` & `cg-60.3.1/tests/apps/orderform/test_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/orderform/validators/test_excel_sample_validators.py` & `cg-60.3.1/tests/apps/orderform/validators/test_excel_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/scout/conftest.py` & `cg-60.3.1/tests/apps/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/scout/test_get_causative_variants.py` & `cg-60.3.1/tests/apps/scout/test_get_causative_variants.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/scout/test_get_scout_cases.py` & `cg-60.3.1/tests/apps/scout/test_get_scout_cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/scout/test_scout_load_config.py` & `cg-60.3.1/tests/apps/scout/test_scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/scout/test_scout_models.py` & `cg-60.3.1/tests/apps/scout/test_scout_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/sequencing_metrics_parser/conftest.py` & `cg-60.3.1/tests/apps/sequencing_metrics_parser/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/sequencing_metrics_parser/parsers/conftest.py` & `cg-60.3.1/tests/apps/sequencing_metrics_parser/parsers/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py` & `cg-60.3.1/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/sequencing_metrics_parser/parsers/test_sequencing_metrics_parser_api.py` & `cg-60.3.1/tests/apps/sequencing_metrics_parser/parsers/test_sequencing_metrics_parser_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/slurm/conftest.py` & `cg-60.3.1/tests/apps/slurm/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/slurm/test_slurm_api.py` & `cg-60.3.1/tests/apps/slurm/test_slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/test_apps_environ.py` & `cg-60.3.1/tests/apps/test_apps_environ.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/apps/test_osticket.py` & `cg-60.3.1/tests/apps/test_osticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/add/test_cli_add.py` & `cg-60.3.1/tests/cli/add/test_cli_add.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/add/test_cli_add_customer.py` & `cg-60.3.1/tests/cli/add/test_cli_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/add/test_cli_add_family.py` & `cg-60.3.1/tests/cli/add/test_cli_add_family.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/add/test_cli_add_relationship.py` & `cg-60.3.1/tests/cli/add/test_cli_add_relationship.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/add/test_cli_add_sample.py` & `cg-60.3.1/tests/cli/add/test_cli_add_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/backup/conftest.py` & `cg-60.3.1/tests/cli/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/backup/test_backup_command.py` & `cg-60.3.1/tests/cli/backup/test_backup_command.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/clean/conftest.py` & `cg-60.3.1/tests/cli/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/clean/test_balsamic_clean.py` & `cg-60.3.1/tests/cli/clean/test_balsamic_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/clean/test_clean_flow_cell.py` & `cg-60.3.1/tests/cli/clean/test_clean_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/clean/test_clean_hk_bundle_files.py` & `cg-60.3.1/tests/cli/clean/test_clean_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/clean/test_hk_bundle_files.py` & `cg-60.3.1/tests/cli/clean/test_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/clean/test_hk_case_bundle_files.py` & `cg-60.3.1/tests/cli/clean/test_hk_case_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/clean/test_microbial_clean.py` & `cg-60.3.1/tests/cli/clean/test_microbial_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/clean/test_rsync_past_run_dirs.py` & `cg-60.3.1/tests/cli/clean/test_rsync_past_run_dirs.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/compress/conftest.py` & `cg-60.3.1/tests/cli/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/compress/test_cli_compress_fastq.py` & `cg-60.3.1/tests/cli/compress/test_cli_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/compress/test_cli_decompress_spring.py` & `cg-60.3.1/tests/cli/compress/test_cli_decompress_spring.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/compress/test_compress_helpers.py` & `cg-60.3.1/tests/cli/compress/test_compress_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/compress/test_store_fastq.py` & `cg-60.3.1/tests/cli/compress/test_store_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/conftest.py` & `cg-60.3.1/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/delete/test_cli_delete_case.py` & `cg-60.3.1/tests/cli/delete/test_cli_delete_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/delete/test_cli_delete_cases.py` & `cg-60.3.1/tests/cli/delete/test_cli_delete_cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/deliver/conftest.py` & `cg-60.3.1/tests/cli/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/deliver/test_deliver_base.py` & `cg-60.3.1/tests/cli/deliver/test_deliver_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/deliver/test_rsync_base.py` & `cg-60.3.1/tests/cli/deliver/test_rsync_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/deliver/test_run_deliver_cmd.py` & `cg-60.3.1/tests/cli/deliver/test_run_deliver_cmd.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/demultiplex/test_create_sample_sheet.py` & `cg-60.3.1/tests/cli/demultiplex/test_create_sample_sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 import pytest
 from _pytest.fixtures import FixtureRequest
 from click.testing import CliRunner, Result
 from pydantic import BaseModel
 
 from cg.apps.demultiplex.sample_sheet.api import SampleSheetAPI
-from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSampleBCLConvert
+from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample
 from cg.cli.demultiplex.sample_sheet import create_sheet
 from cg.constants.process import EXIT_SUCCESS
 from cg.io.txt import read_txt
 from cg.models.cg_config import CGConfig
 from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
 
 GET_FLOW_CELL_SAMPLES: str = "cg.apps.demultiplex.sample_sheet.api.get_flow_cell_samples"
 
 
 def test_create_sample_sheet_no_run_parameters_fails(
     cli_runner: CliRunner,
     tmp_flow_cell_without_run_parameters_path: Path,
     sample_sheet_context_broken_flow_cells: CGConfig,
-    hiseq_2500_custom_index_bcl_convert_lims_samples: list[FlowCellSampleBCLConvert],
+    hiseq_2500_custom_index_bcl_convert_lims_samples: list[FlowCellSample],
     caplog,
     mocker,
 ):
     """Test that creating a flow cell sample sheet fails if there is no run parameters file."""
     # GIVEN a flow cell directory with a non-existing sample sheet nor RunParameters file
     flow_cell = FlowCellDirectoryData(tmp_flow_cell_without_run_parameters_path)
```

### Comparing `cg-60.3.0/tests/cli/demultiplex/test_demultiplex_flowcell.py` & `cg-60.3.1/tests/cli/demultiplex/test_demultiplex_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/demultiplex/test_finish_demux.py` & `cg-60.3.1/tests/cli/demultiplex/test_finish_demux.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/demultiplex/test_validate_sample_sheet.py` & `cg-60.3.1/tests/cli/demultiplex/test_validate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/demultiplex/test_verify_syncing.py` & `cg-60.3.1/tests/cli/demultiplex/test_verify_syncing.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/downsample/test_cli_downsample.py` & `cg-60.3.1/tests/cli/downsample/test_cli_downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/generate/report/conftest.py` & `cg-60.3.1/tests/cli/generate/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/generate/report/test_cli_delivery_report.py` & `cg-60.3.1/tests/cli/generate/report/test_cli_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/generate/report/test_utils.py` & `cg-60.3.1/tests/cli/generate/report/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/generate/test_cli_base.py` & `cg-60.3.1/tests/cli/generate/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/get/test_cli_get.py` & `cg-60.3.1/tests/cli/get/test_cli_get.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/get/test_cli_get_analysis.py` & `cg-60.3.1/tests/cli/get/test_cli_get_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/get/test_cli_get_case.py` & `cg-60.3.1/tests/cli/get/test_cli_get_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/get/test_cli_get_flow_cell.py` & `cg-60.3.1/tests/cli/get/test_cli_get_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/get/test_cli_get_sample.py` & `cg-60.3.1/tests/cli/get/test_cli_get_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/set/conftest.py` & `cg-60.3.1/tests/cli/set/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/set/test_cli_set_case.py` & `cg-60.3.1/tests/cli/set/test_cli_set_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/set/test_cli_set_cases.py` & `cg-60.3.1/tests/cli/set/test_cli_set_cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/set/test_cli_set_flowcell.py` & `cg-60.3.1/tests/cli/set/test_cli_set_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/set/test_cli_set_list_keys.py` & `cg-60.3.1/tests/cli/set/test_cli_set_list_keys.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/set/test_cli_set_sample.py` & `cg-60.3.1/tests/cli/set/test_cli_set_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/set/test_cli_set_samples.py` & `cg-60.3.1/tests/cli/set/test_cli_set_samples.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/store/test_store.py` & `cg-60.3.1/tests/cli/store/test_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/test_base.py` & `cg-60.3.1/tests/cli/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/upload/conftest.py` & `cg-60.3.1/tests/cli/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/upload/test_cli_scout.py` & `cg-60.3.1/tests/cli/upload/test_cli_scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/upload/test_cli_upload.py` & `cg-60.3.1/tests/cli/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/upload/test_cli_upload_auto.py` & `cg-60.3.1/tests/cli/upload/test_cli_upload_auto.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/upload/test_cli_upload_delivery_report.py` & `cg-60.3.1/tests/cli/upload/test_cli_upload_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/upload/test_cli_upload_fastq.py` & `cg-60.3.1/tests/cli/upload/test_cli_upload_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/upload/test_cli_upload_genotype.py` & `cg-60.3.1/tests/cli/upload/test_cli_upload_genotype.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/upload/test_cli_upload_gens.py` & `cg-60.3.1/tests/cli/upload/test_cli_upload_gens.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/upload/test_cli_upload_nipt.py` & `cg-60.3.1/tests/cli/upload/test_cli_upload_nipt.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/upload/test_cli_upload_nipt_ftp.py` & `cg-60.3.1/tests/cli/upload/test_cli_upload_nipt_ftp.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/upload/test_cli_upload_nipt_statina.py` & `cg-60.3.1/tests/cli/upload/test_cli_upload_nipt_statina.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/upload/test_cli_upload_observations.py` & `cg-60.3.1/tests/cli/upload/test_cli_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/balsamic/conftest.py` & `cg-60.3.1/tests/cli/workflow/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py` & `cg-60.3.1/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/balsamic/test_compound_commands.py` & `cg-60.3.1/tests/cli/workflow/balsamic/test_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/balsamic/test_link.py` & `cg-60.3.1/tests/cli/workflow/balsamic/test_link.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/balsamic/test_report_deliver.py` & `cg-60.3.1/tests/cli/workflow/balsamic/test_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/balsamic/test_run.py` & `cg-60.3.1/tests/cli/workflow/balsamic/test_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/balsamic/test_store_housekeeper.py` & `cg-60.3.1/tests/cli/workflow/balsamic/test_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/conftest.py` & `cg-60.3.1/tests/cli/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/fastq/test_fastq_base.py` & `cg-60.3.1/tests/cli/workflow/fastq/test_fastq_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/fluffy/conftest.py` & `cg-60.3.1/tests/cli/workflow/fluffy/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,19 +55,14 @@
         order="sample_project",
         control="positive",
         last_sequenced_at=dt.datetime.now(),
     )
 
 
 @pytest.fixture(scope="function")
-def samplesheet_path():
-    return Path("tests/fixtures/data/SampleSheet.csv").absolute()
-
-
-@pytest.fixture(scope="function")
 def fluffy_fastq_file_path(config_root_dir):
     path = Path(config_root_dir)
     path.mkdir(parents=True, exist_ok=True)
     fastq_path = Path(path, "fastq.fastq.gz")
     fastq_path.touch(exist_ok=True)
     return fastq_path
 
@@ -121,22 +116,22 @@
                 "archive": False,
             }
         ],
     }
 
 
 @pytest.fixture(scope="function")
-def fluffy_samplesheet_bundle_data(samplesheet_path) -> dict:
+def fluffy_samplesheet_bundle_data(novaseq_6000_post_1_5_kits_correct_sample_sheet_path) -> dict:
     return {
         "name": "flowcell",
         "created": dt.datetime.now(),
         "version": "1.0",
         "files": [
             {
-                "path": str(samplesheet_path),
+                "path": str(novaseq_6000_post_1_5_kits_correct_sample_sheet_path),
                 "tags": ["flowcell", "samplesheet"],
                 "archive": False,
             }
         ],
     }
```

### Comparing `cg-60.3.0/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py` & `cg-60.3.1/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/fluffy/test_cli_link.py` & `cg-60.3.1/tests/cli/workflow/fluffy/test_cli_link.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/fluffy/test_cli_run.py` & `cg-60.3.1/tests/cli/workflow/fluffy/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/fluffy/test_cli_start.py` & `cg-60.3.1/tests/cli/workflow/fluffy/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/fluffy/test_cli_store.py` & `cg-60.3.1/tests/cli/workflow/fluffy/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/microsalt/conftest.py` & `cg-60.3.1/tests/cli/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/microsalt/test_microsalt_case_config.py` & `cg-60.3.1/tests/cli/workflow/microsalt/test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/microsalt/test_microsalt_run.py` & `cg-60.3.1/tests/cli/workflow/microsalt/test_microsalt_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/mip/conftest.py` & `cg-60.3.1/tests/cli/workflow/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/mip/test_cli_mip_base.py` & `cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py` & `cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py` & `cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/mip/test_cli_mip_dna_panel.py` & `cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_dna_panel.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/mip/test_cli_mip_dna_run.py` & `cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_dna_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/mip/test_cli_mip_dna_start.py` & `cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_dna_start.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py` & `cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/mip/test_cli_mip_rna_link.py` & `cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_rna_link.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/mip/test_cli_mip_rna_run.py` & `cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_rna_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/mip/test_cli_mip_store.py` & `cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/nf_analysis/test_cli_config_case.py` & `cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py` & `cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py` & `cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/nf_analysis/test_cli_run.py` & `cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/nf_analysis/test_cli_start.py` & `cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/nf_analysis/test_cli_store.py` & `cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py` & `cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py` & `cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py` & `cg-60.3.1/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/test_cli_workflow.py` & `cg-60.3.1/tests/cli/workflow/test_cli_workflow.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/cli/workflow/test_cli_workflow_clean.py` & `cg-60.3.1/tests/cli/workflow/test_cli_workflow_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/clients/arnold/conftest.py` & `cg-60.3.1/tests/clients/arnold/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/clients/arnold/test_arnold_api_client.py` & `cg-60.3.1/tests/clients/arnold/test_arnold_api_client.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/clients/janus/conftest.py` & `cg-60.3.1/tests/clients/janus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/clients/janus/test_janus_api_client.py` & `cg-60.3.1/tests/clients/janus/test_janus_api_client.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/conftest.py` & `cg-60.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py` & `cg-60.3.1/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixture_plugins/delivery_fixtures/context_fixtures.py` & `cg-60.3.1/tests/fixture_plugins/delivery_fixtures/context_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixture_plugins/delivery_fixtures/path_fixtures.py` & `cg-60.3.1/tests/fixture_plugins/delivery_fixtures/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py` & `cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py` & `cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py` & `cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py` & `cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py` & `cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,117 +1,117 @@
 """Fixtures for parsed raw LIMS samples for demultiplexing and sample sheet creation."""
 
 from pathlib import Path
 
 import pytest
 
-from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSampleBCLConvert
+from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample
 from cg.apps.demultiplex.sample_sheet.sample_sheet_creator import SampleSheetCreator
 from cg.constants import FileExtensions
 from cg.io.json import read_json
 from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
 
 
 @pytest.fixture
 def hiseq_x_single_index_bcl_convert_lims_samples(
     hiseq_x_single_index_flow_cell_dir: Path,
-) -> list[FlowCellSampleBCLConvert]:
+) -> list[FlowCellSample]:
     """Return a list of BCLConvert samples parsed from LIMS for a HiSeqX single index flow cell."""
     path = Path(
         hiseq_x_single_index_flow_cell_dir, f"HJCFFALXX_bcl_convert_raw{FileExtensions.JSON}"
     )
-    return [FlowCellSampleBCLConvert.model_validate(sample) for sample in read_json(path)]
+    return [FlowCellSample.model_validate(sample) for sample in read_json(path)]
 
 
 @pytest.fixture
 def selected_hiseq_x_single_index_sample_ids() -> list[str]:
     """Return a list of sample ids for a HiSeqX single index flow cell."""
     return ["SVE2648A1", "ACC2655A1"]
 
 
 @pytest.fixture
 def hiseq_x_dual_index_bcl_convert_lims_samples(
     hiseq_x_dual_index_flow_cell_dir: Path,
-) -> list[FlowCellSampleBCLConvert]:
+) -> list[FlowCellSample]:
     """Return a list of BCLConvert samples parsed from LIMS for a HiSeqX dual index flow cell."""
     path = Path(hiseq_x_dual_index_flow_cell_dir, f"HL32LCCXY_bcl_convert_raw{FileExtensions.JSON}")
-    return [FlowCellSampleBCLConvert.model_validate(sample) for sample in read_json(path)]
+    return [FlowCellSample.model_validate(sample) for sample in read_json(path)]
 
 
 @pytest.fixture
 def selected_hiseq_x_dual_index_sample_ids() -> list[str]:
     """Return a list of sample ids for a HiSeqX single index flow cell."""
     return ["ACC4519A1", "ACC4519A2"]
 
 
 @pytest.fixture
 def hiseq_2500_dual_index_bcl_convert_lims_samples(
     hiseq_2500_dual_index_flow_cell_dir: Path,
-) -> list[FlowCellSampleBCLConvert]:
+) -> list[FlowCellSample]:
     """Return a list of BCLConvert samples parsed from LIMS for a HiSeq2500 dual index flow cell."""
     path = Path(hiseq_2500_dual_index_flow_cell_dir, "HM2LNBCX2_bcl_convert_raw.json")
-    return [FlowCellSampleBCLConvert.model_validate(sample) for sample in read_json(path)]
+    return [FlowCellSample.model_validate(sample) for sample in read_json(path)]
 
 
 @pytest.fixture
 def selected_hiseq_2500_dual_index_sample_ids() -> list[str]:
     """Return a list of sample ids for a HiSeqX single index flow cell."""
     return ["MIC4464A1", "ACC4551A1"]
 
 
 @pytest.fixture
 def hiseq_2500_custom_index_bcl_convert_lims_samples(
     hiseq_2500_custom_index_flow_cell_dir: Path,
-) -> list[FlowCellSampleBCLConvert]:
+) -> list[FlowCellSample]:
     """Return a list of BCLConvert samples parsed from LIMS for a HiSeq2500 custom index flow cell."""
     path = Path(hiseq_2500_custom_index_flow_cell_dir, "HGYFNBCX2_bcl_convert_raw.json")
-    return [FlowCellSampleBCLConvert.model_validate(sample) for sample in read_json(path)]
+    return [FlowCellSample.model_validate(sample) for sample in read_json(path)]
 
 
 @pytest.fixture
 def selected_hiseq_2500_custom_index_sample_ids() -> list[str]:
     """Return a list of sample ids for a HiSeqX single index flow cell."""
     return ["ACC4842A47", "ACC4551A1"]
 
 
 @pytest.fixture
 def novaseq_6000_pre_1_5_kits_bcl_convert_lims_samples(
     novaseq_6000_pre_1_5_kits_flow_cell_path: Path,
-) -> list[FlowCellSampleBCLConvert]:
+) -> list[FlowCellSample]:
     """Return a list of BCLConvert samples parsed from LIMS for a NovaSeq6000 pre 1.5 flow cell."""
     path = Path(novaseq_6000_pre_1_5_kits_flow_cell_path, "HLYWYDSXX_bcl_convert_raw.json")
-    return [FlowCellSampleBCLConvert.model_validate(sample) for sample in read_json(path)]
+    return [FlowCellSample.model_validate(sample) for sample in read_json(path)]
 
 
 @pytest.fixture
 def selected_novaseq_6000_pre_1_5_kits_sample_ids() -> list[str]:
     """Return a list of sample ids for a HiSeqX single index flow cell."""
     return ["ACC6217A7", "ACC6217A12"]
 
 
 @pytest.fixture
 def novaseq_6000_post_1_5_kits_bcl_convert_lims_samples(
     novaseq_6000_post_1_5_kits_flow_cell_path: Path,
-) -> list[FlowCellSampleBCLConvert]:
+) -> list[FlowCellSample]:
     """Return a list of BCLConvert samples parsed from LIMS for a NovaSeq6000 post 1.5 flow cell."""
     path = Path(novaseq_6000_post_1_5_kits_flow_cell_path, "HK33MDRX3_bcl_convert_raw.json")
-    return [FlowCellSampleBCLConvert.model_validate(sample) for sample in read_json(path)]
+    return [FlowCellSample.model_validate(sample) for sample in read_json(path)]
 
 
 @pytest.fixture
 def selected_novaseq_6000_post_1_5_kits_sample_ids() -> list[str]:
     """Return a list of sample ids for a HiSeqX single index flow cell."""
     return ["ACC12642A4", "ACC12642A7"]
 
 
 @pytest.fixture
-def novaseq_x_lims_samples(novaseq_x_flow_cell_directory: Path) -> list[FlowCellSampleBCLConvert]:
+def novaseq_x_lims_samples(novaseq_x_flow_cell_directory: Path) -> list[FlowCellSample]:
     """Return a list of BCLConvert samples parsed from LIMS for a NovaSeqX flow cell."""
     path = Path(novaseq_x_flow_cell_directory, "22F52TLT3_raw.json")
-    return [FlowCellSampleBCLConvert.model_validate(sample) for sample in read_json(path)]
+    return [FlowCellSample.model_validate(sample) for sample in read_json(path)]
 
 
 @pytest.fixture
 def selected_novaseq_x_sample_ids() -> list[str]:
     """Return a list of sample ids for a HiSeqX single index flow cell."""
     return ["ACC13169A1", "ACC13170A6"]
 
@@ -140,14 +140,14 @@
 
 # Sample sheet creators
 
 
 @pytest.fixture
 def bcl_convert_sample_sheet_creator(
     novaseq_x_flow_cell: FlowCellDirectoryData,
-    novaseq_x_lims_samples: list[FlowCellSampleBCLConvert],
+    novaseq_x_lims_samples: list[FlowCellSample],
 ) -> SampleSheetCreator:
     """Returns a sample sheet creator for sample sheet v2."""
     return SampleSheetCreator(
         flow_cell=novaseq_x_flow_cell,
         lims_samples=novaseq_x_lims_samples,
     )
```

### Comparing `cg-60.3.0/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py` & `cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixture_plugins/timestamp_fixtures.py` & `cg-60.3.1/tests/fixture_plugins/timestamp_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json` & `cg-60.3.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json` & `cg-60.3.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/analysis/raredisease/multiqc_data.json` & `cg-60.3.1/tests/fixtures/analysis/raredisease/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml` & `cg-60.3.1/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/analysis/rnafusion/multiqc_data.json` & `cg-60.3.1/tests/fixtures/analysis/rnafusion/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml` & `cg-60.3.1/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/analysis/sample_coverage.bed` & `cg-60.3.1/tests/fixtures/analysis/sample_coverage.bed`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/analysis/taxprofiler/multiqc_data.json` & `cg-60.3.1/tests/fixtures/analysis/taxprofiler/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml` & `cg-60.3.1/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/analysis/tomte/multiqc_data.json` & `cg-60.3.1/tests/fixtures/analysis/tomte/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml` & `cg-60.3.1/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/balsamic/case/config.json` & `cg-60.3.1/tests/fixtures/apps/balsamic/case/config.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/balsamic/case/metadata.yml` & `cg-60.3.1/tests/fixtures/apps/balsamic/case/metadata.yml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml` & `cg-60.3.1/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/crunchy/spring_metadata.json` & `cg-60.3.1/tests/fixtures/apps/crunchy/spring_metadata.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Demultiplex_Stats.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Quality_Metrics.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stderr` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stdout` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RunParameters.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv` & `cg-60.3.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/fluffy/SampleSheet.csv` & `cg-60.3.1/tests/fixtures/apps/fluffy/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/fluffy/deliverables.yaml` & `cg-60.3.1/tests/fixtures/apps/fluffy/deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/madeline/madeline.xml` & `cg-60.3.1/tests/fixtures/apps/madeline/madeline.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/mip/case_metrics_deliverables.yaml` & `cg-60.3.1/tests/fixtures/apps/mip/case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/mip/dna/store/case_config.yaml` & `cg-60.3.1/tests/fixtures/apps/mip/dna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml` & `cg-60.3.1/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml` & `cg-60.3.1/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf` & `cg-60.3.1/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/mip/rna/case_config.yaml` & `cg-60.3.1/tests/fixtures/apps/mip/rna/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml` & `cg-60.3.1/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/mip/rna/store/bundle_data.yaml` & `cg-60.3.1/tests/fixtures/apps/mip/rna/store/bundle_data.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/mip/rna/store/case_config.yaml` & `cg-60.3.1/tests/fixtures/apps/mip/rna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml` & `cg-60.3.1/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml` & `cg-60.3.1/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/scout/643594.config.yaml` & `cg-60.3.1/tests/fixtures/apps/scout/643594.config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/scout/case_export.json` & `cg-60.3.1/tests/fixtures/apps/scout/case_export.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/scout/export_causatives.json` & `cg-60.3.1/tests/fixtures/apps/scout/export_causatives.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/scout/none_case_export.json` & `cg-60.3.1/tests/fixtures/apps/scout/none_case_export.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/scout/other_sex_case.json` & `cg-60.3.1/tests/fixtures/apps/scout/other_sex_case.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/scout/panel_export.bed` & `cg-60.3.1/tests/fixtures/apps/scout/panel_export.bed`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/scout/panel_export.csv` & `cg-60.3.1/tests/fixtures/apps/scout/panel_export.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/SampleSheet.csv` & `cg-60.3.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv` & `cg-60.3.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv` & `cg-60.3.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv` & `cg-60.3.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/cgweb_orders/balsamic.json` & `cg-60.3.1/tests/fixtures/cgweb_orders/balsamic.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/cgweb_orders/fastq.json` & `cg-60.3.1/tests/fixtures/cgweb_orders/fastq.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/cgweb_orders/metagenome.json` & `cg-60.3.1/tests/fixtures/cgweb_orders/metagenome.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/cgweb_orders/microsalt.json` & `cg-60.3.1/tests/fixtures/cgweb_orders/microsalt.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/cgweb_orders/mip.json` & `cg-60.3.1/tests/fixtures/cgweb_orders/mip.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/cgweb_orders/mip_rna.json` & `cg-60.3.1/tests/fixtures/cgweb_orders/mip_rna.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/cgweb_orders/rml.json` & `cg-60.3.1/tests/fixtures/cgweb_orders/rml.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/cgweb_orders/rnafusion.json` & `cg-60.3.1/tests/fixtures/cgweb_orders/rnafusion.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/cgweb_orders/sarscov2.json` & `cg-60.3.1/tests/fixtures/cgweb_orders/sarscov2.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/data/SampleSheet.csv` & `cg-60.3.1/tests/fixtures/data/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/data/cgfixture.db` & `cg-60.3.1/tests/fixtures/data/cgfixture.db`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/data/hkstore.db` & `cg-60.3.1/tests/fixtures/data/hkstore.db`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/io/example_json.json` & `cg-60.3.1/tests/fixtures/io/example_json.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/orderforms/1508.30.balsamic.xlsx` & `cg-60.3.1/tests/fixtures/orderforms/1508.30.balsamic.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx` & `cg-60.3.1/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx` & `cg-60.3.1/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/orderforms/1508.30.fastq.xlsx` & `cg-60.3.1/tests/fixtures/orderforms/1508.30.fastq.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/orderforms/1508.30.metagenome.xlsx` & `cg-60.3.1/tests/fixtures/orderforms/1508.30.metagenome.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/orderforms/1508.30.mip.xlsx` & `cg-60.3.1/tests/fixtures/orderforms/1508.30.mip.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/orderforms/1508.30.mip_rna.xlsx` & `cg-60.3.1/tests/fixtures/orderforms/1508.30.mip_rna.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/orderforms/1508.30.rnafusion.xlsx` & `cg-60.3.1/tests/fixtures/orderforms/1508.30.rnafusion.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/orderforms/1603.11.microbial.xlsx` & `cg-60.3.1/tests/fixtures/orderforms/1603.11.microbial.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/orderforms/1604.17.rml.xlsx` & `cg-60.3.1/tests/fixtures/orderforms/1604.17.rml.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/orderforms/2184.9.sarscov2.xlsx` & `cg-60.3.1/tests/fixtures/orderforms/2184.9.sarscov2.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/orderforms/NIPT-json.json` & `cg-60.3.1/tests/fixtures/orderforms/NIPT-json.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json` & `cg-60.3.1/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/orderforms/mip_uploaded_json_orderform.json` & `cg-60.3.1/tests/fixtures/orderforms/mip_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/report/case_data.json` & `cg-60.3.1/tests/fixtures/report/case_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/report/lims_exported_samples.json` & `cg-60.3.1/tests/fixtures/report/lims_exported_samples.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/fixtures/report/lims_family.json` & `cg-60.3.1/tests/fixtures/report/lims_family.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/io/conftest.py` & `cg-60.3.1/tests/io/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/io/test_io_controller.py` & `cg-60.3.1/tests/io/test_io_controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/io/test_io_csv.py` & `cg-60.3.1/tests/io/test_io_csv.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/io/test_io_json.py` & `cg-60.3.1/tests/io/test_io_json.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/io/test_io_txt.py` & `cg-60.3.1/tests/io/test_io_txt.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/io/test_io_xml.py` & `cg-60.3.1/tests/io/test_io_xml.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/io/test_io_yaml.py` & `cg-60.3.1/tests/io/test_io_yaml.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/io/test_validate_path.py` & `cg-60.3.1/tests/io/test_validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/archive/conftest.py` & `cg-60.3.1/tests/meta/archive/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/archive/test_archive_api.py` & `cg-60.3.1/tests/meta/archive/test_archive_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/archive/test_archive_cli.py` & `cg-60.3.1/tests/meta/archive/test_archive_cli.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/archive/test_archiving.py` & `cg-60.3.1/tests/meta/archive/test_archiving.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/backup/conftest.py` & `cg-60.3.1/tests/meta/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/backup/test_meta_backup.py` & `cg-60.3.1/tests/meta/backup/test_meta_backup.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/backup/test_meta_pdc.py` & `cg-60.3.1/tests/meta/backup/test_meta_pdc.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/clean/conftest.py` & `cg-60.3.1/tests/meta/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/clean/test_clean_flow_cells_api.py` & `cg-60.3.1/tests/meta/clean/test_clean_flow_cells_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/clean/test_clean_retrieved_spring_files.py` & `cg-60.3.1/tests/meta/clean/test_clean_retrieved_spring_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/compress/conftest.py` & `cg-60.3.1/tests/meta/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/compress/test_clean_fastq.py` & `cg-60.3.1/tests/meta/compress/test_clean_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/compress/test_compress_files.py` & `cg-60.3.1/tests/meta/compress/test_compress_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/compress/test_compress_meta_fastq.py` & `cg-60.3.1/tests/meta/compress/test_compress_meta_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/compress/test_decompress_spring_meta.py` & `cg-60.3.1/tests/meta/compress/test_decompress_spring_meta.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/compress/test_meta_compress_update_hk.py` & `cg-60.3.1/tests/meta/compress/test_meta_compress_update_hk.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/conftest.py` & `cg-60.3.1/tests/meta/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/deliver/conftest.py` & `cg-60.3.1/tests/meta/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/deliver/test_deliver_ticket.py` & `cg-60.3.1/tests/meta/deliver/test_deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/deliver/test_delivery_api.py` & `cg-60.3.1/tests/meta/deliver/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/deliver/test_fastq_path_generator.py` & `cg-60.3.1/tests/meta/deliver/test_fastq_path_generator.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/delivery/test_delivery_api.py` & `cg-60.3.1/tests/meta/delivery/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/demultiplex/conftest.py` & `cg-60.3.1/tests/meta/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/demultiplex/test_combine_sequencing_metrics.py` & `cg-60.3.1/tests/meta/demultiplex/test_combine_sequencing_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/demultiplex/test_demux_post_processing.py` & `cg-60.3.1/tests/meta/demultiplex/test_demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/demultiplex/test_housekeeper_storage_functions.py` & `cg-60.3.1/tests/meta/demultiplex/test_housekeeper_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/demultiplex/test_status_db_storage_functions.py` & `cg-60.3.1/tests/meta/demultiplex/test_status_db_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/demultiplex/test_utils.py` & `cg-60.3.1/tests/meta/demultiplex/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/demultiplex/test_validation.py` & `cg-60.3.1/tests/meta/demultiplex/test_validation.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/encryption/conftest.py` & `cg-60.3.1/tests/meta/encryption/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/encryption/test_encryption.py` & `cg-60.3.1/tests/meta/encryption/test_encryption.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/observations/conftest.py` & `cg-60.3.1/tests/meta/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/observations/test_meta_upload_observations.py` & `cg-60.3.1/tests/meta/observations/test_meta_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/orders/conftest.py` & `cg-60.3.1/tests/meta/orders/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/orders/test_PoolSubmitter_validate_order.py` & `cg-60.3.1/tests/meta/orders/test_PoolSubmitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py` & `cg-60.3.1/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/orders/test_SarsCov2Submitter_store_order.py` & `cg-60.3.1/tests/meta/orders/test_SarsCov2Submitter_store_order.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/orders/test_SarsCov2Submitter_validate_order.py` & `cg-60.3.1/tests/meta/orders/test_SarsCov2Submitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/orders/test_meta_orders_api.py` & `cg-60.3.1/tests/meta/orders/test_meta_orders_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/orders/test_meta_orders_lims.py` & `cg-60.3.1/tests/meta/orders/test_meta_orders_lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/orders/test_meta_orders_status.py` & `cg-60.3.1/tests/meta/orders/test_meta_orders_status.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/orders/test_rnafusion_submitter.py` & `cg-60.3.1/tests/meta/orders/test_rnafusion_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/orders/test_ticket_handler.py` & `cg-60.3.1/tests/meta/orders/test_ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/qc_metrics/conftest.py` & `cg-60.3.1/tests/meta/qc_metrics/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/qc_metrics/test_collect_qc_metrics.py` & `cg-60.3.1/tests/meta/qc_metrics/test_collect_qc_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/report/conftest.py` & `cg-60.3.1/tests/meta/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/report/test_balsamic_api.py` & `cg-60.3.1/tests/meta/report/test_balsamic_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/report/test_field_validators.py` & `cg-60.3.1/tests/meta/report/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/report/test_mip_dna_api.py` & `cg-60.3.1/tests/meta/report/test_mip_dna_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/report/test_report_api.py` & `cg-60.3.1/tests/meta/report/test_report_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/report/test_rnafusion_api.py` & `cg-60.3.1/tests/meta/report/test_rnafusion_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/report/test_tomte_api.py` & `cg-60.3.1/tests/meta/report/test_tomte_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/rsync/conftest.py` & `cg-60.3.1/tests/meta/rsync/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/rsync/test_rsync.py` & `cg-60.3.1/tests/meta/rsync/test_rsync.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/test_invoice.py` & `cg-60.3.1/tests/meta/test_invoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/transfer/conftest.py` & `cg-60.3.1/tests/meta/transfer/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/transfer/test_external_data.py` & `cg-60.3.1/tests/meta/transfer/test_external_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/transfer/test_meta_transfer_lims.py` & `cg-60.3.1/tests/meta/transfer/test_meta_transfer_lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/upload/balsamic/test_balsamic.py` & `cg-60.3.1/tests/meta/upload/balsamic/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/upload/conftest.py` & `cg-60.3.1/tests/meta/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/upload/gisaid/fixtures/four_samples.csv` & `cg-60.3.1/tests/meta/upload/gisaid/fixtures/four_samples.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/upload/mutacc/conftest.py` & `cg-60.3.1/tests/meta/upload/mutacc/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/upload/mutacc/test_meta_upload_mutacc.py` & `cg-60.3.1/tests/meta/upload/mutacc/test_meta_upload_mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/upload/nipt/conftest.py` & `cg-60.3.1/tests/meta/upload/nipt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/upload/nipt/test_models.py` & `cg-60.3.1/tests/meta/upload/nipt/test_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/upload/nipt/test_nipt_upload_api.py` & `cg-60.3.1/tests/meta/upload/nipt/test_nipt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/upload/scout/conftest.py` & `cg-60.3.1/tests/meta/upload/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/upload/scout/test_generate_load_config.py` & `cg-60.3.1/tests/meta/upload/scout/test_generate_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/upload/scout/test_meta_upload_scoutapi.py` & `cg-60.3.1/tests/meta/upload/scout/test_meta_upload_scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py` & `cg-60.3.1/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/upload/scout/test_scout_config_builder.py` & `cg-60.3.1/tests/meta/upload/scout/test_scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/upload/test_meta_upload_coverage.py` & `cg-60.3.1/tests/meta/upload/test_meta_upload_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/upload/test_upload_api.py` & `cg-60.3.1/tests/meta/upload/test_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/upload/test_upload_genotypes_api.py` & `cg-60.3.1/tests/meta/upload/test_upload_genotypes_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/workflow/conftest.py` & `cg-60.3.1/tests/meta/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/workflow/microsalt/conftest.py` & `cg-60.3.1/tests/meta/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/workflow/microsalt/test_quality_controller.py` & `cg-60.3.1/tests/meta/workflow/microsalt/test_quality_controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/workflow/microsalt/test_quality_controller_utils.py` & `cg-60.3.1/tests/meta/workflow/microsalt/test_quality_controller_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/workflow/microsalt/test_report_generation.py` & `cg-60.3.1/tests/meta/workflow/microsalt/test_report_generation.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/workflow/test_analysis.py` & `cg-60.3.1/tests/meta/workflow/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/workflow/test_balsamic.py` & `cg-60.3.1/tests/meta/workflow/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/workflow/test_fastq.py` & `cg-60.3.1/tests/meta/workflow/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/workflow/test_microsalt.py` & `cg-60.3.1/tests/meta/workflow/test_microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/workflow/test_nf_analysis.py` & `cg-60.3.1/tests/meta/workflow/test_nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/workflow/test_prepare_fastq_api.py` & `cg-60.3.1/tests/meta/workflow/test_prepare_fastq_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/workflow/test_raredisease.py` & `cg-60.3.1/tests/meta/workflow/test_raredisease.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/meta/workflow/test_rnafusion.py` & `cg-60.3.1/tests/meta/workflow/test_rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/mocks/balsamic_analysis_mock.py` & `cg-60.3.1/tests/mocks/balsamic_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/mocks/crunchy.py` & `cg-60.3.1/tests/mocks/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/mocks/hk_mock.py` & `cg-60.3.1/tests/mocks/hk_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/mocks/limsmock.py` & `cg-60.3.1/tests/mocks/limsmock.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/mocks/madeline.py` & `cg-60.3.1/tests/mocks/madeline.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/mocks/mip_analysis_mock.py` & `cg-60.3.1/tests/mocks/mip_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/mocks/osticket.py` & `cg-60.3.1/tests/mocks/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/mocks/process_mock.py` & `cg-60.3.1/tests/mocks/process_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/mocks/report.py` & `cg-60.3.1/tests/mocks/report.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/mocks/scout.py` & `cg-60.3.1/tests/mocks/scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/mocks/store_model.py` & `cg-60.3.1/tests/mocks/store_model.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/mocks/tb_mock.py` & `cg-60.3.1/tests/mocks/tb_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/models/balsamic/conftest.py` & `cg-60.3.1/tests/models/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/models/balsamic/test_balsamic_analysis.py` & `cg-60.3.1/tests/models/balsamic/test_balsamic_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/models/conftest.py` & `cg-60.3.1/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/models/demultiplexing/test_run_parameters.py` & `cg-60.3.1/tests/models/demultiplexing/test_run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/models/downsample/test_down_sample_meta_data.py` & `cg-60.3.1/tests/models/downsample/test_down_sample_meta_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/models/flow_cell/test_flowcell_model.py` & `cg-60.3.1/tests/models/flow_cell/test_flowcell_model.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/models/mip/conftest.py` & `cg-60.3.1/tests/models/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/models/mip/test_mip_analysis.py` & `cg-60.3.1/tests/models/mip/test_mip_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/models/mip/test_mip_config.py` & `cg-60.3.1/tests/models/mip/test_mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/models/mip/test_mip_metrics_deliverables.py` & `cg-60.3.1/tests/models/mip/test_mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/models/mip/test_mip_sample_info.py` & `cg-60.3.1/tests/models/mip/test_mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/models/nextflow/test_nextflow_deliver.py` & `cg-60.3.1/tests/models/nextflow/test_nextflow_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/models/observations/conftest.py` & `cg-60.3.1/tests/models/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/models/observations/test_observations_input_files.py` & `cg-60.3.1/tests/models/observations/test_observations_input_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/models/report/test_validators.py` & `cg-60.3.1/tests/models/report/test_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/models/rnafusion/test_rnafusion_sample.py` & `cg-60.3.1/tests/models/rnafusion/test_rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/models/test_cg_models.py` & `cg-60.3.1/tests/models/test_cg_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/models/test_compression_data.py` & `cg-60.3.1/tests/models/test_compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/models/test_fastq.py` & `cg-60.3.1/tests/models/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/models/test_file_data.py` & `cg-60.3.1/tests/models/test_file_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/server/conftest.py` & `cg-60.3.1/tests/server/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/server/endpoints/test_delivery_message_endpoint.py` & `cg-60.3.1/tests/server/endpoints/test_delivery_message_endpoint.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/server/endpoints/test_orders_endpoint.py` & `cg-60.3.1/tests/server/endpoints/test_orders_endpoint.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/services/fastq_file_service/conftest.py` & `cg-60.3.1/tests/services/fastq_file_service/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/services/fastq_file_service/test_fastq_file_service.py` & `cg-60.3.1/tests/services/fastq_file_service/test_fastq_file_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/services/orders/order_status_service/conftest.py` & `cg-60.3.1/tests/services/orders/order_status_service/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/services/orders/order_status_service/test_order_summary_service.py` & `cg-60.3.1/tests/services/orders/order_status_service/test_order_summary_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/api/conftest.py` & `cg-60.3.1/tests/store/api/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/api/test_base.py` & `cg-60.3.1/tests/store/api/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/conftest.py` & `cg-60.3.1/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/crud/add/test_store_add_application_version.py` & `cg-60.3.1/tests/store/crud/add/test_store_add_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/crud/add/test_store_add_base.py` & `cg-60.3.1/tests/store/crud/add/test_store_add_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/crud/add/test_store_add_customer.py` & `cg-60.3.1/tests/store/crud/add/test_store_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/crud/add/test_store_add_flow_celll.py` & `cg-60.3.1/tests/store/crud/add/test_store_add_flow_celll.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/crud/conftest.py` & `cg-60.3.1/tests/store/crud/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/crud/delete/test_delete.py` & `cg-60.3.1/tests/store/crud/delete/test_delete.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/crud/read/test_read.py` & `cg-60.3.1/tests/store/crud/read/test_read.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/crud/read/test_read_analyses_to_clean.py` & `cg-60.3.1/tests/store/crud/read/test_read_analyses_to_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/crud/read/test_read_analyses_to_delivery_report.py` & `cg-60.3.1/tests/store/crud/read/test_read_analyses_to_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/crud/read/test_read_analysis.py` & `cg-60.3.1/tests/store/crud/read/test_read_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/crud/read/test_read_application_version.py` & `cg-60.3.1/tests/store/crud/read/test_read_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/crud/read/test_read_customer.py` & `cg-60.3.1/tests/store/crud/read/test_read_customer.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/crud/read/test_read_pool.py` & `cg-60.3.1/tests/store/crud/read/test_read_pool.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/crud/read/test_read_sample.py` & `cg-60.3.1/tests/store/crud/read/test_read_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/crud/update/test_update.py` & `cg-60.3.1/tests/store/crud/update/test_update.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/filters/test_status_analyses_filters.py` & `cg-60.3.1/tests/store/filters/test_status_analyses_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/filters/test_status_application_filters.py` & `cg-60.3.1/tests/store/filters/test_status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/filters/test_status_application_limitations_filters.py` & `cg-60.3.1/tests/store/filters/test_status_application_limitations_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/filters/test_status_application_version_filters.py` & `cg-60.3.1/tests/store/filters/test_status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/filters/test_status_bed_filters.py` & `cg-60.3.1/tests/store/filters/test_status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/filters/test_status_bed_version_filters.py` & `cg-60.3.1/tests/store/filters/test_status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/filters/test_status_case_sample_filters.py` & `cg-60.3.1/tests/store/filters/test_status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/filters/test_status_cases_filters.py` & `cg-60.3.1/tests/store/filters/test_status_cases_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/filters/test_status_collaboration_filters.py` & `cg-60.3.1/tests/store/filters/test_status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/filters/test_status_customer_filters.py` & `cg-60.3.1/tests/store/filters/test_status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/filters/test_status_flow_cell_filters.py` & `cg-60.3.1/tests/store/filters/test_status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/filters/test_status_invoice_filters.py` & `cg-60.3.1/tests/store/filters/test_status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/filters/test_status_metrics_filters.py` & `cg-60.3.1/tests/store/filters/test_status_metrics_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/filters/test_status_organism_filters.py` & `cg-60.3.1/tests/store/filters/test_status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/filters/test_status_panel_filters.py` & `cg-60.3.1/tests/store/filters/test_status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/filters/test_status_pool_filters.py` & `cg-60.3.1/tests/store/filters/test_status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/filters/test_status_samples_filters.py` & `cg-60.3.1/tests/store/filters/test_status_samples_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/filters/test_status_user_filters.py` & `cg-60.3.1/tests/store/filters/test_status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/test_delivery.py` & `cg-60.3.1/tests/store/test_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store/test_store_models.py` & `cg-60.3.1/tests/store/test_store_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/store_helpers.py` & `cg-60.3.1/tests/store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/test_copy_novaseqx_flow_cell.py` & `cg-60.3.1/tests/test_copy_novaseqx_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/test_store_helpers.py` & `cg-60.3.1/tests/test_store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/utils/conftest.py` & `cg-60.3.1/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/utils/test_commands.py` & `cg-60.3.1/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/utils/test_date.py` & `cg-60.3.1/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/utils/test_dict.py` & `cg-60.3.1/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/utils/test_dispatcher.py` & `cg-60.3.1/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/utils/test_files.py` & `cg-60.3.1/tests/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/utils/test_time.py` & `cg-60.3.1/tests/utils/test_time.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/tests/utils/test_utils.py` & `cg-60.3.1/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.0/PKG-INFO` & `cg-60.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 60.3.0
+Version: 60.3.1
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

