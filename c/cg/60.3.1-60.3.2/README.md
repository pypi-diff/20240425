# Comparing `tmp/cg-60.3.1.tar.gz` & `tmp/cg-60.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cg-60.3.1.tar", max compression
+gzip compressed data, was "cg-60.3.2.tar", max compression
```

## Comparing `cg-60.3.1.tar` & `cg-60.3.2.tar`

### file list

```diff
@@ -1,1369 +1,1354 @@
--rw-r--r--   0        0        0     2686 2024-04-24 11:46:39.943723 cg-60.3.1/README.md
--rw-r--r--   0        0        0       40 2024-04-24 11:46:39.947723 cg-60.3.1/cg/__init__.py
--rw-r--r--   0        0        0      315 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/__init__.py
--rw-r--r--   0        0        0       27 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/coverage/__init__.py
--rw-r--r--   0        0        0     2940 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/coverage/api.py
--rw-r--r--   0        0        0       56 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/crunchy/__init__.py
--rw-r--r--   0        0        0    12783 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/crunchy/crunchy.py
--rw-r--r--   0        0        0     4502 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/crunchy/files.py
--rw-r--r--   0        0        0      430 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/crunchy/models.py
--rw-r--r--   0        0        0      910 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/crunchy/sbatch.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/__init__.py
--rw-r--r--   0        0        0    11299 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/demultiplex_api.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/sample_sheet/__init__.py
--rw-r--r--   0        0        0    11249 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/sample_sheet/api.py
--rw-r--r--   0        0        0     2183 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/sample_sheet/index.py
--rw-r--r--   0        0        0     7341 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py
--rw-r--r--   0        0        0     3188 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py
--rw-r--r--   0        0        0     7071 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/sample_sheet/sample_models.py
--rw-r--r--   0        0        0     6076 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py
--rw-r--r--   0        0        0     1372 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py
--rw-r--r--   0        0        0     8092 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py
--rw-r--r--   0        0        0      824 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/sample_sheet/validators.py
--rw-r--r--   0        0        0      677 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/demultiplex/sbatch.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/downsample/__init__.py
--rw-r--r--   0        0        0     6160 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/downsample/downsample.py
--rw-r--r--   0        0        0     2125 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/downsample/utils.py
--rw-r--r--   0        0        0      298 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/environ.py
--rw-r--r--   0        0        0     1741 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/gens.py
--rw-r--r--   0        0        0     3419 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/gt.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/hermes/__init__.py
--rw-r--r--   0        0        0     2249 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/hermes/hermes_api.py
--rw-r--r--   0        0        0     1298 2024-04-24 11:46:39.947723 cg-60.3.1/cg/apps/hermes/models.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/housekeeper/__init__.py
--rw-r--r--   0        0        0    30395 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/housekeeper/hk.py
--rw-r--r--   0        0        0      326 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/housekeeper/models.py
--rw-r--r--   0        0        0       32 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/invoice/__init__.py
--rw-r--r--   0        0        0     4804 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/invoice/render.py
--rw-r--r--   0        0        0   113467 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/invoice/templates/KI_pool_invoice.xlsx
--rw-r--r--   0        0        0    75562 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/invoice/templates/KI_sample_invoice.xlsx
--rw-r--r--   0        0        0   113512 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
--rw-r--r--   0        0        0    75459 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
--rw-r--r--   0        0        0       25 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/lims/__init__.py
--rw-r--r--   0        0        0    18546 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/lims/api.py
--rw-r--r--   0        0        0     2652 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/lims/batch.py
--rw-r--r--   0        0        0     8129 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/lims/order.py
--rw-r--r--   0        0        0     3118 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/lims/sample_sheet.py
--rw-r--r--   0        0        0     4866 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/loqus.py
--rw-r--r--   0        0        0       35 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/madeline/__init__.py
--rw-r--r--   0        0        0     3213 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/madeline/api.py
--rw-r--r--   0        0        0       23 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/mip/__init__.py
--rw-r--r--   0        0        0     3564 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/mip/confighandler.py
--rw-r--r--   0        0        0     2207 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/mutacc_auto.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/orderform/__init__.py
--rw-r--r--   0        0        0     9498 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/orderform/excel_orderform_parser.py
--rw-r--r--   0        0        0     3051 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/orderform/json_orderform_parser.py
--rw-r--r--   0        0        0     6419 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/orderform/orderform_parser.py
--rw-r--r--   0        0        0      252 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/orderform/utils.py
--rw-r--r--   0        0        0     2537 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/osticket.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/scout/__init__.py
--rw-r--r--   0        0        0     3177 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/scout/scout_export.py
--rw-r--r--   0        0        0    11054 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/scout/scoutapi.py
--rw-r--r--   0        0        0      444 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/scout/validators.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0        0        0     3457 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/sequencing_metrics_parser/api.py
--rw-r--r--   0        0        0      923 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/sequencing_metrics_parser/models.py
--rw-r--r--   0        0        0     6670 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/sequencing_metrics_parser/parser.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/slurm/__init__.py
--rw-r--r--   0        0        0     1277 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/slurm/sbatch.py
--rw-r--r--   0        0        0     3559 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/slurm/slurm_api.py
--rw-r--r--   0        0        0       32 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/tb/__init__.py
--rw-r--r--   0        0        0     7995 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/tb/api.py
--rw-r--r--   0        0        0      152 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/tb/dto/create_job_request.py
--rw-r--r--   0        0        0      250 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/tb/dto/summary_response.py
--rw-r--r--   0        0        0     1305 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/tb/models.py
--rw-r--r--   0        0        0      305 2024-04-24 11:46:39.951723 cg-60.3.1/cg/apps/tb/validators.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.951723 cg-60.3.1/cg/cli/__init__.py
--rw-r--r--   0        0        0    11558 2024-04-24 11:46:39.951723 cg-60.3.1/cg/cli/add.py
--rw-r--r--   0        0        0     2653 2024-04-24 11:46:39.951723 cg-60.3.1/cg/cli/archive.py
--rw-r--r--   0        0        0    10118 2024-04-24 11:46:39.951723 cg-60.3.1/cg/cli/backup.py
--rw-r--r--   0        0        0     3852 2024-04-24 11:46:39.951723 cg-60.3.1/cg/cli/base.py
--rw-r--r--   0        0        0    10506 2024-04-24 11:46:39.951723 cg-60.3.1/cg/cli/clean.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.951723 cg-60.3.1/cg/cli/compress/__init__.py
--rw-r--r--   0        0        0     2135 2024-04-24 11:46:39.951723 cg-60.3.1/cg/cli/compress/base.py
--rw-r--r--   0        0        0     6706 2024-04-24 11:46:39.951723 cg-60.3.1/cg/cli/compress/fastq.py
--rw-r--r--   0        0        0     8163 2024-04-24 11:46:39.951723 cg-60.3.1/cg/cli/compress/helpers.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/delete/__init__.py
--rw-r--r--   0        0        0      564 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/delete/base.py
--rw-r--r--   0        0        0     4603 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/delete/case.py
--rw-r--r--   0        0        0     1884 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/delete/cases.py
--rw-r--r--   0        0        0     2633 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/delete/observations.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/deliver/__init__.py
--rw-r--r--   0        0        0     6030 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/deliver/base.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/demultiplex/__init__.py
--rw-r--r--   0        0        0      829 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/demultiplex/base.py
--rw-r--r--   0        0        0     4905 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py
--rw-r--r--   0        0        0     7726 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/demultiplex/demux.py
--rw-r--r--   0        0        0     1473 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/demultiplex/finish.py
--rw-r--r--   0        0        0     3119 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/demultiplex/sample_sheet.py
--rw-r--r--   0        0        0     2995 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/downsample.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/generate/__init__.py
--rw-r--r--   0        0        0      356 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/generate/base.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/generate/report/__init__.py
--rw-r--r--   0        0        0     4636 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/generate/report/base.py
--rw-r--r--   0        0        0      854 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/generate/report/options.py
--rw-r--r--   0        0        0     5340 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/generate/report/utils.py
--rw-r--r--   0        0        0     8327 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/get.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/set/__init__.py
--rw-r--r--   0        0        0     9856 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/set/base.py
--rw-r--r--   0        0        0     4384 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/set/case.py
--rw-r--r--   0        0        0     2595 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/set/cases.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/store/__init__.py
--rw-r--r--   0        0        0     1093 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/store/base.py
--rw-r--r--   0        0        0     6191 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/store/store.py
--rw-r--r--   0        0        0     1761 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/transfer.py
--rw-r--r--   0        0        0        1 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/__init__.py
--rw-r--r--   0        0        0     5706 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/base.py
--rw-r--r--   0        0        0     5503 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/clinical_delivery.py
--rw-r--r--   0        0        0     1175 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/coverage.py
--rw-r--r--   0        0        0     1528 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/delivery_report.py
--rw-r--r--   0        0        0     4022 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/fohm.py
--rw-r--r--   0        0        0     1463 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/genotype.py
--rw-r--r--   0        0        0     1885 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/gens.py
--rw-r--r--   0        0        0      584 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/gisaid.py
--rw-r--r--   0        0        0     2645 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/mutacc.py
--rw-r--r--   0        0        0       23 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/nipt/__init__.py
--rw-r--r--   0        0        0     3006 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/nipt/base.py
--rw-r--r--   0        0        0     2275 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/nipt/ftp.py
--rw-r--r--   0        0        0     1596 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/nipt/statina.py
--rw-r--r--   0        0        0      112 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/observations/__init__.py
--rw-r--r--   0        0        0     2672 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/observations/observations.py
--rw-r--r--   0        0        0     2904 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/observations/utils.py
--rw-r--r--   0        0        0     9970 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/scout.py
--rw-r--r--   0        0        0      650 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/utils.py
--rw-r--r--   0        0        0     1667 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/upload/validate.py
--rw-r--r--   0        0        0      105 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/utils.py
--rw-r--r--   0        0        0       18 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/__init__.py
--rw-r--r--   0        0        0       22 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/balsamic/__init__.py
--rw-r--r--   0        0        0     8925 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/balsamic/base.py
--rw-r--r--   0        0        0     1980 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/balsamic/options.py
--rw-r--r--   0        0        0      881 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/balsamic/pon.py
--rw-r--r--   0        0        0     1162 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/balsamic/qc.py
--rw-r--r--   0        0        0     1177 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/balsamic/umi.py
--rw-r--r--   0        0        0     1342 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/base.py
--rw-r--r--   0        0        0    12379 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/commands.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/fastq/__init__.py
--rw-r--r--   0        0        0     1367 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/fastq/base.py
--rw-r--r--   0        0        0     1787 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/fastq/fastq_service.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/fluffy/__init__.py
--rw-r--r--   0        0        0     4177 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/fluffy/base.py
--rw-r--r--   0        0        0       22 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/jasen/__init__.py
--rw-r--r--   0        0        0      535 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/jasen/base.py
--rw-r--r--   0        0        0       22 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/microsalt/__init__.py
--rw-r--r--   0        0        0     7810 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/microsalt/base.py
--rw-r--r--   0        0        0       22 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/mip/__init__.py
--rw-r--r--   0        0        0     6596 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/mip/base.py
--rw-r--r--   0        0        0     1268 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/mip/options.py
--rw-r--r--   0        0        0       22 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/mip_dna/__init__.py
--rw-r--r--   0        0        0     1013 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/mip_dna/base.py
--rw-r--r--   0        0        0       22 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/mip_rna/__init__.py
--rw-r--r--   0        0        0      916 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/mip_rna/base.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/mutant/__init__.py
--rw-r--r--   0        0        0     3413 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/mutant/base.py
--rw-r--r--   0        0        0     9002 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/nf_analysis.py
--rw-r--r--   0        0        0       22 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/raredisease/__init__.py
--rw-r--r--   0        0        0     2210 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/raredisease/base.py
--rw-r--r--   0        0        0       22 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/rnafusion/__init__.py
--rw-r--r--   0        0        0     1179 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/rnafusion/base.py
--rw-r--r--   0        0        0       22 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/taxprofiler/__init__.py
--rw-r--r--   0        0        0     1211 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/taxprofiler/base.py
--rw-r--r--   0        0        0     1111 2024-04-24 11:46:39.955723 cg-60.3.1/cg/cli/workflow/tomte/base.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.959723 cg-60.3.1/cg/clients/__init__.py
--rw-r--r--   0        0        0     1363 2024-04-24 11:46:39.959723 cg-60.3.1/cg/clients/arnold/api.py
--rw-r--r--   0        0        0      160 2024-04-24 11:46:39.959723 cg-60.3.1/cg/clients/arnold/dto/create_case_request.py
--rw-r--r--   0        0        0      384 2024-04-24 11:46:39.959723 cg-60.3.1/cg/clients/arnold/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.959723 cg-60.3.1/cg/clients/janus/__init__.py
--rw-r--r--   0        0        0     1246 2024-04-24 11:46:39.959723 cg-60.3.1/cg/clients/janus/api.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.959723 cg-60.3.1/cg/clients/janus/dto/__init__.py
--rw-r--r--   0        0        0      503 2024-04-24 11:46:39.959723 cg-60.3.1/cg/clients/janus/dto/create_qc_metrics_request.py
--rw-r--r--   0        0        0      420 2024-04-24 11:46:39.959723 cg-60.3.1/cg/clients/janus/exceptions.py
--rw-r--r--   0        0        0      937 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/__init__.py
--rw-r--r--   0        0        0      253 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/archiving.py
--rw-r--r--   0        0        0       35 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/backup.py
--rw-r--r--   0        0        0      769 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/bcl_convert_metrics.py
--rw-r--r--   0        0        0      469 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/compression.py
--rw-r--r--   0        0        0     6613 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/constants.py
--rw-r--r--   0        0        0     6033 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/delivery.py
--rw-r--r--   0        0        0     8120 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/demultiplexing.py
--rw-r--r--   0        0        0     1422 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/encryption.py
--rw-r--r--   0        0        0      372 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/extraction.py
--rw-r--r--   0        0        0     2054 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/gene_panel.py
--rw-r--r--   0        0        0     6704 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/housekeeper_tags.py
--rw-r--r--   0        0        0       95 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/invoice.py
--rw-r--r--   0        0        0     5815 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/lims.py
--rw-r--r--   0        0        0      743 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/metrics.py
--rw-r--r--   0        0        0      231 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/nanopore_files.py
--rw-r--r--   0        0        0      650 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/nextflow.py
--rw-r--r--   0        0        0     1529 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/nf_analysis.py
--rw-r--r--   0        0        0       19 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/nipt.py
--rw-r--r--   0        0        0     2257 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/observations.py
--rw-r--r--   0        0        0     1216 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/orderforms.py
--rw-r--r--   0        0        0       96 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/paths.py
--rw-r--r--   0        0        0      266 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/pdc.py
--rw-r--r--   0        0        0      160 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/pedigree.py
--rw-r--r--   0        0        0     1044 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/priority.py
--rw-r--r--   0        0        0       79 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/process.py
--rw-r--r--   0        0        0     5474 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/report.py
--rw-r--r--   0        0        0      485 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/sample_sources.py
--rw-r--r--   0        0        0     3111 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/scout.py
--rw-r--r--   0        0        0     1669 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/sequencing.py
--rw-r--r--   0        0        0      313 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/slurm.py
--rw-r--r--   0        0        0      529 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/subject.py
--rw-r--r--   0        0        0       55 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/symbols.py
--rw-r--r--   0        0        0      435 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/tb.py
--rw-r--r--   0        0        0      161 2024-04-24 11:46:39.959723 cg-60.3.1/cg/constants/time.py
--rw-r--r--   0        0        0     6639 2024-04-24 11:46:39.959723 cg-60.3.1/cg/exc.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/__init__.py
--rw-r--r--   0        0        0     1037 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/api.py
--rw-r--r--   0        0        0      621 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/config.py
--rw-r--r--   0        0        0     2978 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/controller.py
--rw-r--r--   0        0        0     1763 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/csv.py
--rw-r--r--   0        0        0      210 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/gzip.py
--rw-r--r--   0        0        0      662 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/json.py
--rw-r--r--   0        0        0      525 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/png.py
--rw-r--r--   0        0        0     1094 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/txt.py
--rw-r--r--   0        0        0      552 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/validate_path.py
--rw-r--r--   0        0        0     1289 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/xml.py
--rw-r--r--   0        0        0     1153 2024-04-24 11:46:39.959723 cg-60.3.1/cg/io/yaml.py
--rw-r--r--   0        0        0      281 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/archive/__init__.py
--rw-r--r--   0        0        0    15193 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/archive/archive.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/archive/ddn/__init__.py
--rw-r--r--   0        0        0     1727 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/archive/ddn/constants.py
--rw-r--r--   0        0        0    10852 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/archive/ddn/ddn_data_flow_client.py
--rw-r--r--   0        0        0     3704 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/archive/ddn/models.py
--rw-r--r--   0        0        0     1250 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/archive/ddn/utils.py
--rw-r--r--   0        0        0     2024 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/archive/models.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/backup/__init__.py
--rw-r--r--   0        0        0    17426 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/backup/backup.py
--rw-r--r--   0        0        0     5397 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/backup/pdc.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/clean/__init__.py
--rw-r--r--   0        0        0     3901 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/clean/api.py
--rw-r--r--   0        0        0     7738 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/clean/clean_flow_cells.py
--rw-r--r--   0        0        0     1841 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/clean/clean_retrieved_spring_files.py
--rw-r--r--   0        0        0       34 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/compress/__init__.py
--rw-r--r--   0        0        0    14557 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/compress/compress.py
--rw-r--r--   0        0        0     4947 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/compress/files.py
--rw-r--r--   0        0        0       77 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/deliver/__init__.py
--rw-r--r--   0        0        0    14672 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/deliver/deliver.py
--rw-r--r--   0        0        0     4502 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/deliver/deliver_ticket.py
--rw-r--r--   0        0        0      904 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/deliver/fastq_path_generator.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/delivery/__init__.py
--rw-r--r--   0        0        0     8255 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/delivery/delivery.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/demultiplex/__init__.py
--rw-r--r--   0        0        0     2592 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/demultiplex/combine_sequencing_metrics.py
--rw-r--r--   0        0        0     5719 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/demultiplex/demux_post_processing.py
--rw-r--r--   0        0        0     4135 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/demultiplex/files.py
--rw-r--r--   0        0        0     7777 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/demultiplex/housekeeper_storage_functions.py
--rw-r--r--   0        0        0     6126 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/demultiplex/status_db_storage_functions.py
--rw-r--r--   0        0        0    10690 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/demultiplex/utils.py
--rw-r--r--   0        0        0     2855 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/demultiplex/validation.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.959723 cg-60.3.1/cg/meta/encryption/__init__.py
--rw-r--r--   0        0        0    20271 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/encryption/encryption.py
--rw-r--r--   0        0        0      537 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/encryption/sbatch.py
--rw-r--r--   0        0        0    10922 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/invoice.py
--rw-r--r--   0        0        0     2360 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/meta.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/observations/__init__.py
--rw-r--r--   0        0        0     6008 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/observations/balsamic_observations_api.py
--rw-r--r--   0        0        0     5277 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/observations/mip_dna_observations_api.py
--rw-r--r--   0        0        0     5364 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/observations/observations_api.py
--rw-r--r--   0        0        0       27 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/__init__.py
--rw-r--r--   0        0        0     3637 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/api.py
--rw-r--r--   0        0        0      121 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/balsamic_qc_submitter.py
--rw-r--r--   0        0        0      107 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/balsamic_submitter.py
--rw-r--r--   0        0        0      122 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/balsamic_umi_submitter.py
--rw-r--r--   0        0        0    15262 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/case_submitter.py
--rw-r--r--   0        0        0     6102 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/fastq_submitter.py
--rw-r--r--   0        0        0      105 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/fluffy_submitter.py
--rw-r--r--   0        0        0     1254 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/lims.py
--rw-r--r--   0        0        0     5782 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/metagenome_submitter.py
--rw-r--r--   0        0        0     6337 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/microbial_submitter.py
--rw-r--r--   0        0        0      123 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/microsalt_submitter.py
--rw-r--r--   0        0        0      105 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/mip_dna_submitter.py
--rw-r--r--   0        0        0      105 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/mip_rna_submitter.py
--rw-r--r--   0        0        0     7761 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/pool_submitter.py
--rw-r--r--   0        0        0      102 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/rml_submitter.py
--rw-r--r--   0        0        0      718 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/rnafusion_submitter.py
--rw-r--r--   0        0        0     1268 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/sars_cov_2_submitter.py
--rw-r--r--   0        0        0     1754 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/submitter.py
--rw-r--r--   0        0        0     7880 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/orders/ticket_handler.py
--rw-r--r--   0        0        0     4105 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/qc_metrics/collect_qc_metrics.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/__init__.py
--rw-r--r--   0        0        0     8168 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/balsamic.py
--rw-r--r--   0        0        0      562 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/balsamic_qc.py
--rw-r--r--   0        0        0      717 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/balsamic_umi.py
--rw-r--r--   0        0        0     4171 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/field_validators.py
--rw-r--r--   0        0        0     6620 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/mip_dna.py
--rw-r--r--   0        0        0    18606 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/report_api.py
--rw-r--r--   0        0        0     5625 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/rnafusion.py
--rw-r--r--   0        0        0     1911 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/delivery-report.html
--rw-r--r--   0        0        0     4236 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/data_analysis/data_analysis.html
--rw-r--r--   0        0        0     1049 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/data_analysis/limitations.html
--rw-r--r--   0        0        0     3351 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html
--rw-r--r--   0        0        0     1364 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html
--rw-r--r--   0        0        0      753 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html
--rw-r--r--   0        0        0     3284 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html
--rw-r--r--   0        0        0     3670 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html
--rw-r--r--   0        0        0     2332 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/header.html
--rw-r--r--   0        0        0     2066 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/order.html
--rw-r--r--   0        0        0     2243 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/sample_prep.html
--rw-r--r--   0        0        0      472 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/ticket_system.html
--rw-r--r--   0        0        0     1165 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html
--rw-r--r--   0        0        0     1538 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html
--rw-r--r--   0        0        0      428 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/uploaded_files/rnafusion_uploaded_files.html
--rw-r--r--   0        0        0     4266 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html
--rw-r--r--   0        0        0       80 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/partials/footer.html
--rw-r--r--   0        0        0      172 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/partials/signature.html
--rw-r--r--   0        0        0   232803 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/static/css/bootstrap.min.css
--rw-r--r--   0        0        0       33 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/static/css/custom.css
--rw-r--r--   0        0        0    30068 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/templates/static/images/SWEDAC_logo.png
--rw-r--r--   0        0        0     3925 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/report/tomte.py
--rw-r--r--   0        0        0       32 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/rsync/__init__.py
--rw-r--r--   0        0        0    12291 2024-04-24 11:46:39.963723 cg-60.3.1/cg/meta/rsync/rsync_api.py
--rw-r--r--   0        0        0      387 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/rsync/sbatch.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/tar/__init__.py
--rw-r--r--   0        0        0     1694 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/tar/tar.py
--rw-r--r--   0        0        0       71 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/transfer/__init__.py
--rw-r--r--   0        0        0    10016 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/transfer/external_data.py
--rw-r--r--   0        0        0     5814 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/transfer/lims.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/balsamic/__init__.py
--rw-r--r--   0        0        0     3107 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/balsamic/balsamic.py
--rw-r--r--   0        0        0     2224 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/coverage.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/fohm/__init__.py
--rw-r--r--   0        0        0    12102 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/fohm/fohm.py
--rw-r--r--   0        0        0       30 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/gisaid/__init__.py
--rw-r--r--   0        0        0      928 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/gisaid/constants.py
--rw-r--r--   0        0        0    13521 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/gisaid/gisaid.py
--rw-r--r--   0        0        0     3312 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/gisaid/models.py
--rw-r--r--   0        0        0     5310 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/gt.py
--rw-r--r--   0        0        0      898 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/microsalt/microsalt_upload_api.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/mip/__init__.py
--rw-r--r--   0        0        0     2546 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/mip/mip_dna.py
--rw-r--r--   0        0        0     1400 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/mip/mip_rna.py
--rw-r--r--   0        0        0     7294 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/mutacc.py
--rw-r--r--   0        0        0     1853 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/nf_analysis.py
--rw-r--r--   0        0        0       32 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/nipt/__init__.py
--rw-r--r--   0        0        0      696 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/nipt/models.py
--rw-r--r--   0        0        0     8106 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/nipt/nipt.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/scout/__init__.py
--rw-r--r--   0        0        0     4009 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/scout/balsamic_config_builder.py
--rw-r--r--   0        0        0     1491 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/scout/balsamic_umi_config_builder.py
--rw-r--r--   0        0        0     3322 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/scout/hk_tags.py
--rw-r--r--   0        0        0     9103 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/scout/mip_config_builder.py
--rw-r--r--   0        0        0     3495 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/scout/rnafusion_config_builder.py
--rw-r--r--   0        0        0     7231 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/scout/scout_config_builder.py
--rw-r--r--   0        0        0    23146 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/scout/uploadscoutapi.py
--rw-r--r--   0        0        0     3197 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/upload/upload_api.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/__init__.py
--rw-r--r--   0        0        0    28043 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/analysis.py
--rw-r--r--   0        0        0    28188 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/balsamic.py
--rw-r--r--   0        0        0     2700 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/balsamic_pon.py
--rw-r--r--   0        0        0      553 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/balsamic_qc.py
--rw-r--r--   0        0        0      556 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/balsamic_umi.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/downsample/__init__.py
--rw-r--r--   0        0        0     3922 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/downsample/downsample.py
--rw-r--r--   0        0        0      711 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/downsample/sbatch.py
--rw-r--r--   0        0        0     8913 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/fastq.py
--rw-r--r--   0        0        0    10687 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/fluffy.py
--rw-r--r--   0        0        0      521 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/jasen.py
--rw-r--r--   0        0        0       70 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/__init__.py
--rw-r--r--   0        0        0      116 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/constants.py
--rw-r--r--   0        0        0      174 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/metrics_parser/__init__.py
--rw-r--r--   0        0        0      366 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/metrics_parser/metrics_parser.py
--rw-r--r--   0        0        0      903 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/metrics_parser/models.py
--rw-r--r--   0        0        0    13062 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/microsalt.py
--rw-r--r--   0        0        0       95 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/quality_controller/__init__.py
--rw-r--r--   0        0        0      712 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/quality_controller/models.py
--rw-r--r--   0        0        0     5688 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/quality_controller/quality_controller.py
--rw-r--r--   0        0        0     1217 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/quality_controller/report_generator.py
--rw-r--r--   0        0        0     2373 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/quality_controller/result_logger.py
--rw-r--r--   0        0        0     5641 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/quality_controller/utils.py
--rw-r--r--   0        0        0     1220 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/microsalt/utils.py
--rw-r--r--   0        0        0    13924 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/mip.py
--rw-r--r--   0        0        0     2991 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/mip_dna.py
--rw-r--r--   0        0        0     2167 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/mip_rna.py
--rw-r--r--   0        0        0    10587 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/mutant.py
--rw-r--r--   0        0        0    35481 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/nf_analysis.py
--rw-r--r--   0        0        0     6161 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/nf_handlers.py
--rw-r--r--   0        0        0     6394 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/prepare_fastq.py
--rw-r--r--   0        0        0     5988 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/raredisease.py
--rw-r--r--   0        0        0     5214 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/rnafusion.py
--rw-r--r--   0        0        0     4607 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/taxprofiler.py
--rw-r--r--   0        0        0     3204 2024-04-24 11:46:39.967723 cg-60.3.1/cg/meta/workflow/tomte.py
--rw-r--r--   0        0        0      113 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/__init__.py
--rw-r--r--   0        0        0      367 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/analysis.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/balsamic/__init__.py
--rw-r--r--   0        0        0      459 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/balsamic/analysis.py
--rw-r--r--   0        0        0     4550 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/balsamic/config.py
--rw-r--r--   0        0        0     1986 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/balsamic/metrics.py
--rw-r--r--   0        0        0    17539 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/cg_config.py
--rw-r--r--   0        0        0     4302 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/compression_data.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/deliverables/__init__.py
--rw-r--r--   0        0        0     5213 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/deliverables/metric_deliverables.py
--rw-r--r--   0        0        0      243 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/delivery/delivery.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/demultiplex/__init__.py
--rw-r--r--   0        0        0    12040 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/demultiplex/run_parameters.py
--rw-r--r--   0        0        0      539 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/demultiplex/sbatch.py
--rw-r--r--   0        0        0     7006 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/downsample/downsample_data.py
--rw-r--r--   0        0        0      255 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/email.py
--rw-r--r--   0        0        0     1046 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/fastq.py
--rw-r--r--   0        0        0     2157 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/file_data.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/flow_cell/__init__.py
--rw-r--r--   0        0        0    10373 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/flow_cell/flow_cell.py
--rw-r--r--   0        0        0      317 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/flow_cell/utils.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/invoice/__init__.py
--rw-r--r--   0        0        0     1254 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/invoice/invoice.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/lims/__init__.py
--rw-r--r--   0        0        0     2019 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/lims/sample.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/mip/__init__.py
--rw-r--r--   0        0        0      337 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/mip/mip_analysis.py
--rw-r--r--   0        0        0     1564 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/mip/mip_config.py
--rw-r--r--   0        0        0     4696 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/mip/mip_metrics_deliverables.py
--rw-r--r--   0        0        0     2550 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/mip/mip_sample_info.py
--rw-r--r--   0        0        0     2472 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/nf_analysis.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/observations/__init__.py
--rw-r--r--   0        0        0      688 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/observations/input_files.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/__init__.py
--rw-r--r--   0        0        0     2659 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/constants.py
--rw-r--r--   0        0        0     5604 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/excel_sample.py
--rw-r--r--   0        0        0      898 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/json_sample.py
--rw-r--r--   0        0        0     1449 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/order.py
--rw-r--r--   0        0        0      811 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/orderform_schema.py
--rw-r--r--   0        0        0     4212 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/sample_base.py
--rw-r--r--   0        0        0     9668 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/samples.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/validators/__init__.py
--rw-r--r--   0        0        0     2300 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/validators/excel_sample_validators.py
--rw-r--r--   0        0        0      576 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/validators/json_sample_validators.py
--rw-r--r--   0        0        0       71 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/orders/validators/sample_base_validators.py
--rw-r--r--   0        0        0      101 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/qc_metrics.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/raredisease/__init__.py
--rw-r--r--   0        0        0     1875 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/raredisease/raredisease.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/report/__init__.py
--rw-r--r--   0        0        0     7461 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/report/metadata.py
--rw-r--r--   0        0        0     6180 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/report/report.py
--rw-r--r--   0        0        0     5221 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/report/sample.py
--rw-r--r--   0        0        0     3004 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/report/validators.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/rnafusion/__init__.py
--rw-r--r--   0        0        0     1865 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/rnafusion/rnafusion.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/scout/__init__.py
--rw-r--r--   0        0        0     4783 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/scout/scout_load_config.py
--rw-r--r--   0        0        0      116 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/scout/validators.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/slurm/__init__.py
--rw-r--r--   0        0        0      617 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/slurm/sbatch.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/taxprofiler/__init__.py
--rw-r--r--   0        0        0     2443 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/taxprofiler/taxprofiler.py
--rw-r--r--   0        0        0     1774 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/tomte/tomte.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/workflow/__init__.py
--rw-r--r--   0        0        0      685 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/workflow/mutant.py
--rw-r--r--   0        0        0       70 2024-04-24 11:46:39.971723 cg-60.3.1/cg/models/workflow/validators.py
--rw-r--r--   0        0        0      842 2024-04-24 11:46:39.971723 cg-60.3.1/cg/resources/__init__.py
--rw-r--r--   0        0        0     3493 2024-04-24 11:46:39.971723 cg-60.3.1/cg/resources/rnafusion_bundle_filenames.yaml
--rw-r--r--   0        0        0     2434 2024-04-24 11:46:39.971723 cg-60.3.1/cg/resources/taxprofiler_bundle_filenames.yaml
--rw-r--r--   0        0        0     3732 2024-04-24 11:46:39.971723 cg-60.3.1/cg/resources/tomte_bundle_filenames.yaml
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/__init__.py
--rw-r--r--   0        0        0    20241 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/admin.py
--rw-r--r--   0        0        0    22743 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/api.py
--rw-r--r--   0        0        0     4887 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/app.py
--rw-r--r--   0        0        0       48 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/auto.py
--rw-r--r--   0        0        0     1184 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/config.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/dto/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/dto/delivery_message/__init__.py
--rw-r--r--   0        0        0      300 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/dto/delivery_message/delivery_message_request.py
--rw-r--r--   0        0        0      183 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/dto/delivery_message/delivery_message_response.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/dto/orders/__init__.py
--rw-r--r--   0        0        0      165 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/dto/orders/order_delivery_update_request.py
--rw-r--r--   0        0        0       91 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/dto/orders/order_patch_request.py
--rw-r--r--   0        0        0      662 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/dto/orders/orders_request.py
--rw-r--r--   0        0        0      413 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/dto/orders/orders_response.py
--rw-r--r--   0        0        0     2598 2024-04-24 11:46:39.971723 cg-60.3.1/cg/server/ext.py
--rw-r--r--   0        0        0       29 2024-04-24 11:46:39.975723 cg-60.3.1/cg/server/invoices/__init__.py
--rw-r--r--   0        0        0     4793 2024-04-24 11:46:39.975723 cg-60.3.1/cg/server/invoices/templates/invoices/index.html
--rw-r--r--   0        0        0     8171 2024-04-24 11:46:39.975723 cg-60.3.1/cg/server/invoices/templates/invoices/invoice.html
--rw-r--r--   0        0        0     2838 2024-04-24 11:46:39.975723 cg-60.3.1/cg/server/invoices/templates/invoices/layout.html
--rw-r--r--   0        0        0     4956 2024-04-24 11:46:39.975723 cg-60.3.1/cg/server/invoices/templates/invoices/new.html
--rw-r--r--   0        0        0     7708 2024-04-24 11:46:39.975723 cg-60.3.1/cg/server/invoices/views.py
--rw-r--r--   0        0        0      354 2024-04-24 11:46:39.975723 cg-60.3.1/cg/server/templates/admin/index.html
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/analysis_service/__init__.py
--rw-r--r--   0        0        0      482 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/analysis_service/analysis_service.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/__init__.py
--rw-r--r--   0        0        0     2531 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/delivery_message_service.py
--rw-r--r--   0        0        0      792 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/__init__.py
--rw-r--r--   0        0        0     1366 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/analysis_scout_message.py
--rw-r--r--   0        0        0      791 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/covid_message.py
--rw-r--r--   0        0        0      189 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/delivery_message.py
--rw-r--r--   0        0        0     1391 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/fastq_analysis_scout_message.py
--rw-r--r--   0        0        0      535 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/fastq_message.py
--rw-r--r--   0        0        0     1358 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/fastq_scout_message.py
--rw-r--r--   0        0        0      604 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/microsalt_mwr_message.py
--rw-r--r--   0        0        0      592 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/microsalt_mwx_message.py
--rw-r--r--   0        0        0      903 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/scout_message.py
--rw-r--r--   0        0        0      512 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/statina_message.py
--rw-r--r--   0        0        0      779 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/messages/utils.py
--rw-r--r--   0        0        0     3300 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/delivery_message/utils.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/fastq_file_service/__init__.py
--rw-r--r--   0        0        0      101 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/fastq_file_service/exceptions.py
--rw-r--r--   0        0        0     1092 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/fastq_file_service/fastq_file_service.py
--rw-r--r--   0        0        0     2991 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/fastq_file_service/utils.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/orders/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/orders/order_service/__init__.py
--rw-r--r--   0        0        0     2684 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/orders/order_service/order_service.py
--rw-r--r--   0        0        0     1214 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/orders/order_service/utils.py
--rw-r--r--   0        0        0       94 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/orders/order_status_service/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/orders/order_status_service/dto/__init__.py
--rw-r--r--   0        0        0      192 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/orders/order_status_service/dto/case_summary.py
--rw-r--r--   0        0        0      289 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/orders/order_status_service/dto/order_summary.py
--rw-r--r--   0        0        0     1768 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/orders/order_status_service/order_summary_service.py
--rw-r--r--   0        0        0     1737 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/orders/order_status_service/utils.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/slurm_service/__init__.py
--rw-r--r--   0        0        0      703 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/slurm_service/slurm_cli_service.py
--rw-r--r--   0        0        0      242 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/slurm_service/slurm_service.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/slurm_upload_service/__init__.py
--rw-r--r--   0        0        0      175 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/slurm_upload_service/slurm_upload_config.py
--rw-r--r--   0        0        0     2074 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/slurm_upload_service/slurm_upload_service.py
--rw-r--r--   0        0        0      203 2024-04-24 11:46:39.975723 cg-60.3.1/cg/services/slurm_upload_service/utils.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/__init__.py
--rw-r--r--   0        0        0     4650 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/base.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/crud/__init__.py
--rw-r--r--   0        0        0    13100 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/crud/create.py
--rw-r--r--   0        0        0     2144 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/crud/delete.py
--rw-r--r--   0        0        0    60188 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/crud/read.py
--rw-r--r--   0        0        0     1121 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/crud/update.py
--rw-r--r--   0        0        0     1662 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/database.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/__init__.py
--rw-r--r--   0        0        0     5371 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_analysis_filters.py
--rw-r--r--   0        0        0     1712 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_application_filters.py
--rw-r--r--   0        0        0     1440 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_application_limitations_filters.py
--rw-r--r--   0        0        0     2523 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_application_version_filters.py
--rw-r--r--   0        0        0     1390 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_bed_filters.py
--rw-r--r--   0        0        0     1317 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_bed_version_filters.py
--rw-r--r--   0        0        0    10787 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_case_filters.py
--rw-r--r--   0        0        0     3272 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_case_sample_filters.py
--rw-r--r--   0        0        0      903 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_collaboration_filters.py
--rw-r--r--   0        0        0     1412 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_customer_filters.py
--rw-r--r--   0        0        0     1880 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_flow_cell_filters.py
--rw-r--r--   0        0        0     1255 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_invoice_filters.py
--rw-r--r--   0        0        0     2792 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_metrics_filters.py
--rw-r--r--   0        0        0     3225 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_order_filters.py
--rw-r--r--   0        0        0      851 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_organism_filters.py
--rw-r--r--   0        0        0      783 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_panel_filters.py
--rw-r--r--   0        0        0     3923 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_pool_filters.py
--rw-r--r--   0        0        0     8660 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_sample_filters.py
--rw-r--r--   0        0        0      731 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/filters/status_user_filters.py
--rw-r--r--   0        0        0    36844 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/models.py
--rw-r--r--   0        0        0      593 2024-04-24 11:46:39.975723 cg-60.3.1/cg/store/store.py
--rw-r--r--   0        0        0       30 2024-04-24 11:46:39.975723 cg-60.3.1/cg/utils/__init__.py
--rw-r--r--   0        0        0      187 2024-04-24 11:46:39.975723 cg-60.3.1/cg/utils/calculations.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/utils/checksum/__init__.py
--rw-r--r--   0        0        0     1579 2024-04-24 11:46:39.975723 cg-60.3.1/cg/utils/checksum/checksum.py
--rw-r--r--   0        0        0     1655 2024-04-24 11:46:39.975723 cg-60.3.1/cg/utils/click/EnumChoice.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.975723 cg-60.3.1/cg/utils/click/__init__.py
--rw-r--r--   0        0        0     4910 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/commands.py
--rw-r--r--   0        0        0     1811 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/date.py
--rw-r--r--   0        0        0      635 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/dict.py
--rw-r--r--   0        0        0     2111 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/dispatcher.py
--rw-r--r--   0        0        0     1251 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/email.py
--rw-r--r--   0        0        0      134 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/enums.py
--rw-r--r--   0        0        0     3178 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/files.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/flask/__init__.py
--rw-r--r--   0        0        0     1052 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/flask/enum.py
--rw-r--r--   0        0        0      233 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/flow_cell.py
--rw-r--r--   0        0        0      834 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/time.py
--rw-r--r--   0        0        0     1224 2024-04-24 11:46:39.979723 cg-60.3.1/cg/utils/utils.py
--rw-r--r--   0        0        0     1697 2024-04-24 11:46:39.979723 cg-60.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.979723 cg-60.3.1/tests/__init__.py
--rw-r--r--   0        0        0     1158 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/conftest.py
--rw-r--r--   0        0        0      231 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/coverage/conftest.py
--rw-r--r--   0        0        0     6188 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/coverage/test_coverage.py
--rw-r--r--   0        0        0     1693 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/crunchy/conftest.py
--rw-r--r--   0        0        0     5438 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/crunchy/test_compress_fastq.py
--rw-r--r--   0        0        0     2283 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/crunchy/test_config.py
--rw-r--r--   0        0        0    14032 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/crunchy/test_crunchy.py
--rw-r--r--   0        0        0     9109 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/crunchy/test_spring_decompression.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/__init__.py
--rw-r--r--   0        0        0    10079 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/conftest.py
--rw-r--r--   0        0        0     4010 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0        0        0     7986 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/test_demultiplex_api.py
--rw-r--r--   0        0        0     4782 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/test_index.py
--rw-r--r--   0        0        0     9468 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/test_override_cycles_validator.py
--rw-r--r--   0        0        0     3993 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/test_read_sample_sheet.py
--rw-r--r--   0        0        0    12389 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/test_sample_models.py
--rw-r--r--   0        0        0      951 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/test_sample_sheet_creator.py
--rw-r--r--   0        0        0     3175 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/test_sample_sheet_models.py
--rw-r--r--   0        0        0    10932 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/test_sample_sheet_validator.py
--rw-r--r--   0        0        0     4940 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/test_translate_sample_sheet.py
--rw-r--r--   0        0        0     1450 2024-04-24 11:46:39.979723 cg-60.3.1/tests/apps/demultiplex/test_validate.py
--rw-r--r--   0        0        0     5094 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/downsample/test_downsample.py
--rw-r--r--   0        0        0     1419 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/downsample/test_downsample_utils.py
--rw-r--r--   0        0        0     1716 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/gens/test_gens_api.py
--rw-r--r--   0        0        0     1950 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/gt/conftest.py
--rw-r--r--   0        0        0     4276 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/gt/test_gt_api.py
--rw-r--r--   0        0        0     1453 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/hk/conftest.py
--rw-r--r--   0        0        0      684 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/hk/test__getattr__.py
--rw-r--r--   0        0        0     1593 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/hk/test_add_file.py
--rw-r--r--   0        0        0     3523 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/hk/test_bundles.py
--rw-r--r--   0        0        0      871 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/hk/test_core.py
--rw-r--r--   0        0        0    31172 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/hk/test_file.py
--rw-r--r--   0        0        0     5080 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/hk/test_version.py
--rw-r--r--   0        0        0     1840 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/lims/conftest.py
--rw-r--r--   0        0        0     3197 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/lims/test_api.py
--rw-r--r--   0        0        0     1451 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/lims/test_sample_sheet.py
--rw-r--r--   0        0        0     9223 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/loqus/conftest.py
--rw-r--r--   0        0        0     8994 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/loqus/test_loqusdb_api.py
--rw-r--r--   0        0        0     2439 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/madeline/conftest.py
--rw-r--r--   0        0        0     4653 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/madeline/test_madeline.py
--rw-r--r--   0        0        0     3328 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/mip/conftest.py
--rw-r--r--   0        0        0     2487 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/mip/test_config_mip.py
--rw-r--r--   0        0        0      883 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/mutacc_auto/conftest.py
--rw-r--r--   0        0        0     2473 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/mutacc_auto/test_mutacc_auto.py
--rw-r--r--   0        0        0    11930 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/orderform/conftest.py
--rw-r--r--   0        0        0     9484 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/orderform/test_excel_orderform_parser.py
--rw-r--r--   0        0        0     4351 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/orderform/test_excel_sample_schema.py
--rw-r--r--   0        0        0     1032 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/orderform/test_json_orderform_parser.py
--rw-r--r--   0        0        0     2474 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/orderform/test_orderform_parser.py
--rw-r--r--   0        0        0    16002 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/orderform/validators/test_excel_sample_validators.py
--rw-r--r--   0        0        0     3670 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/scout/conftest.py
--rw-r--r--   0        0        0     2269 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/scout/test_get_causative_variants.py
--rw-r--r--   0        0        0     1376 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/scout/test_get_scout_cases.py
--rw-r--r--   0        0        0     1840 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/scout/test_scout_load_config.py
--rw-r--r--   0        0        0     7047 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/scout/test_scout_models.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0        0        0     2639 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/sequencing_metrics_parser/conftest.py
--rw-r--r--   0        0        0     2010 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/sequencing_metrics_parser/parsers/conftest.py
--rw-r--r--   0        0        0     7105 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
--rw-r--r--   0        0        0     3030 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/sequencing_metrics_parser/parsers/test_sequencing_metrics_parser_api.py
--rw-r--r--   0        0        0     1131 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/slurm/conftest.py
--rw-r--r--   0        0        0     4412 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/slurm/test_slurm_api.py
--rw-r--r--   0        0        0      831 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/test_apps_environ.py
--rw-r--r--   0        0        0      957 2024-04-24 11:46:39.983723 cg-60.3.1/tests/apps/test_osticket.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/add/__init__.py
--rw-r--r--   0        0        0     1174 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/add/test_cli_add.py
--rw-r--r--   0        0        0     2471 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/add/test_cli_add_customer.py
--rw-r--r--   0        0        0     6841 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/add/test_cli_add_family.py
--rw-r--r--   0        0        0     7588 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/add/test_cli_add_relationship.py
--rw-r--r--   0        0        0     8382 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/add/test_cli_add_sample.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/backup/__init__.py
--rw-r--r--   0        0        0      705 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/backup/conftest.py
--rw-r--r--   0        0        0    11101 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/backup/test_backup_command.py
--rw-r--r--   0        0        0     6865 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/clean/conftest.py
--rw-r--r--   0        0        0     5536 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/clean/test_balsamic_clean.py
--rw-r--r--   0        0        0     2557 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/clean/test_clean_flow_cell.py
--rw-r--r--   0        0        0     1830 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/clean/test_clean_hk_bundle_files.py
--rw-r--r--   0        0        0     2098 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/clean/test_hk_bundle_files.py
--rw-r--r--   0        0        0     4610 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/clean/test_hk_case_bundle_files.py
--rw-r--r--   0        0        0     3585 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/clean/test_microbial_clean.py
--rw-r--r--   0        0        0     1881 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/clean/test_rsync_past_run_dirs.py
--rw-r--r--   0        0        0     9707 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/compress/conftest.py
--rw-r--r--   0        0        0     7709 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/compress/test_cli_compress_fastq.py
--rw-r--r--   0        0        0     1416 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/compress/test_cli_decompress_spring.py
--rw-r--r--   0        0        0     5205 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/compress/test_compress_helpers.py
--rw-r--r--   0        0        0     1239 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/compress/test_store_fastq.py
--rw-r--r--   0        0        0     7558 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/conftest.py
--rw-r--r--   0        0        0    12747 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/delete/test_cli_delete_case.py
--rw-r--r--   0        0        0     1873 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/delete/test_cli_delete_cases.py
--rw-r--r--   0        0        0     3794 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/deliver/conftest.py
--rw-r--r--   0        0        0     4428 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/deliver/test_deliver_base.py
--rw-r--r--   0        0        0     1166 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/deliver/test_rsync_base.py
--rw-r--r--   0        0        0     8569 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/deliver/test_run_deliver_cmd.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/demultiplex/__init__.py
--rw-r--r--   0        0        0     5109 2024-04-24 11:46:39.983723 cg-60.3.1/tests/cli/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0        0        0     4773 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/demultiplex/test_demultiplex_flowcell.py
--rw-r--r--   0        0        0     1607 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/demultiplex/test_finish_demux.py
--rw-r--r--   0        0        0     2989 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/demultiplex/test_validate_sample_sheet.py
--rw-r--r--   0        0        0     4423 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/demultiplex/test_verify_syncing.py
--rw-r--r--   0        0        0     1585 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/downsample/test_cli_downsample.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/generate/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/generate/report/__init__.py
--rw-r--r--   0        0        0     1622 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/generate/report/conftest.py
--rw-r--r--   0        0        0     2477 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/generate/report/test_cli_delivery_report.py
--rw-r--r--   0        0        0     2760 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/generate/report/test_utils.py
--rw-r--r--   0        0        0      563 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/generate/test_cli_base.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/get/__init__.py
--rw-r--r--   0        0        0      863 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/get/test_cli_get.py
--rw-r--r--   0        0        0     1526 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/get/test_cli_get_analysis.py
--rw-r--r--   0        0        0     1242 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/get/test_cli_get_case.py
--rw-r--r--   0        0        0     6208 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/get/test_cli_get_flow_cell.py
--rw-r--r--   0        0        0     8835 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/get/test_cli_get_sample.py
--rw-r--r--   0        0        0     1364 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/set/conftest.py
--rw-r--r--   0        0        0     7311 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/set/test_cli_set_case.py
--rw-r--r--   0        0        0     1460 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/set/test_cli_set_cases.py
--rw-r--r--   0        0        0     2016 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/set/test_cli_set_flowcell.py
--rw-r--r--   0        0        0     1685 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/set/test_cli_set_list_keys.py
--rw-r--r--   0        0        0    12450 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/set/test_cli_set_sample.py
--rw-r--r--   0        0        0     6124 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/set/test_cli_set_samples.py
--rw-r--r--   0        0        0     6934 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/store/test_store.py
--rw-r--r--   0        0        0     2332 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/test_base.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/__init__.py
--rw-r--r--   0        0        0    10057 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/conftest.py
--rw-r--r--   0        0        0     2295 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/test_cli_scout.py
--rw-r--r--   0        0        0     1789 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/test_cli_upload.py
--rw-r--r--   0        0        0      971 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/test_cli_upload_auto.py
--rw-r--r--   0        0        0     1669 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/test_cli_upload_delivery_report.py
--rw-r--r--   0        0        0      895 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/test_cli_upload_fastq.py
--rw-r--r--   0        0        0     1199 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/test_cli_upload_genotype.py
--rw-r--r--   0        0        0      694 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/test_cli_upload_gens.py
--rw-r--r--   0        0        0     9965 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/test_cli_upload_nipt.py
--rw-r--r--   0        0        0     4684 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/test_cli_upload_nipt_ftp.py
--rw-r--r--   0        0        0     1839 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/test_cli_upload_nipt_statina.py
--rw-r--r--   0        0        0     6177 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/upload/test_cli_upload_observations.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/__init__.py
--rw-r--r--   0        0        0    30612 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/balsamic/conftest.py
--rw-r--r--   0        0        0    13938 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
--rw-r--r--   0        0        0     7957 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/balsamic/test_compound_commands.py
--rw-r--r--   0        0        0     2336 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/balsamic/test_link.py
--rw-r--r--   0        0        0     3554 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/balsamic/test_report_deliver.py
--rw-r--r--   0        0        0     6209 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/balsamic/test_run.py
--rw-r--r--   0        0        0     6934 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/balsamic/test_store_housekeeper.py
--rw-r--r--   0        0        0     8458 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/conftest.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/fastq/__init__.py
--rw-r--r--   0        0        0     2298 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/fastq/test_fastq_base.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/fluffy/__init__.py
--rw-r--r--   0        0        0     5237 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/fluffy/conftest.py
--rw-r--r--   0        0        0     5687 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
--rw-r--r--   0        0        0     3302 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/fluffy/test_cli_link.py
--rw-r--r--   0        0        0     1896 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/fluffy/test_cli_run.py
--rw-r--r--   0        0        0     2968 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/fluffy/test_cli_start.py
--rw-r--r--   0        0        0     7815 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/fluffy/test_cli_store.py
--rw-r--r--   0        0        0     2775 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/microsalt/conftest.py
--rw-r--r--   0        0        0     6926 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/microsalt/test_microsalt_case_config.py
--rw-r--r--   0        0        0     1000 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/microsalt/test_microsalt_run.py
--rw-r--r--   0        0        0     6544 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/conftest.py
--rw-r--r--   0        0        0     7011 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_base.py
--rw-r--r--   0        0        0     1542 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
--rw-r--r--   0        0        0      431 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_dna_link.py
--rw-r--r--   0        0        0     2108 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py
--rw-r--r--   0        0        0     1273 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
--rw-r--r--   0        0        0     3595 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_dna_run.py
--rw-r--r--   0        0        0     3884 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_dna_start.py
--rw-r--r--   0        0        0     1004 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
--rw-r--r--   0        0        0      527 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_rna_link.py
--rw-r--r--   0        0        0      716 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_rna_run.py
--rw-r--r--   0        0        0     8559 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_store.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/nf_analysis/__init__.py
--rw-r--r--   0        0        0     7365 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_config_case.py
--rw-r--r--   0        0        0     3831 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py
--rw-r--r--   0        0        0     5087 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py
--rw-r--r--   0        0        0     9211 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_run.py
--rw-r--r--   0        0        0     2994 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_start.py
--rw-r--r--   0        0        0     9877 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_store.py
--rw-r--r--   0        0        0    10373 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py
--rw-r--r--   0        0        0      978 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/raredisease/__init__.py
--rw-r--r--   0        0        0     3940 2024-04-24 11:46:39.987723 cg-60.3.1/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py
--rw-r--r--   0        0        0      921 2024-04-24 11:46:39.991723 cg-60.3.1/tests/cli/workflow/test_cli_workflow.py
--rw-r--r--   0        0        0     4310 2024-04-24 11:46:39.991723 cg-60.3.1/tests/cli/workflow/test_cli_workflow_clean.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/clients/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/clients/arnold/__init__.py
--rw-r--r--   0        0        0     1080 2024-04-24 11:46:39.991723 cg-60.3.1/tests/clients/arnold/conftest.py
--rw-r--r--   0        0        0     1503 2024-04-24 11:46:39.991723 cg-60.3.1/tests/clients/arnold/test_arnold_api_client.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/clients/janus/__init__.py
--rw-r--r--   0        0        0     2381 2024-04-24 11:46:39.991723 cg-60.3.1/tests/clients/janus/conftest.py
--rw-r--r--   0        0        0     1716 2024-04-24 11:46:39.991723 cg-60.3.1/tests/clients/janus/test_janus_api_client.py
--rw-r--r--   0        0        0   133089 2024-04-24 11:46:39.991723 cg-60.3.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/delivery_fixtures/__init__.py
--rw-r--r--   0        0        0     2653 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py
--rw-r--r--   0        0        0     4972 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/delivery_fixtures/context_fixtures.py
--rw-r--r--   0        0        0     1494 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/delivery_fixtures/path_fixtures.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/__init__.py
--rw-r--r--   0        0        0     4702 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py
--rw-r--r--   0        0        0     6152 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py
--rw-r--r--   0        0        0    22442 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py
--rw-r--r--   0        0        0     3699 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py
--rw-r--r--   0        0        0     6000 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py
--rw-r--r--   0        0        0     6514 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py
--rw-r--r--   0        0        0     1304 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixture_plugins/timestamp_fixtures.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
--rw-r--r--   0        0        0    14644 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
--rw-r--r--   0        0        0    15921 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/ADM2.cram
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/ADM3.cram
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/adm1.cram
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/adm1.mt.bam
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/multiqc.html
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/report.pdf
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/smn.vcf
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/snv.vcf
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/snv_research.vcf
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/str.vcf
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/sv.vcf
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/sv_research.vcf
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
--rw-r--r--   0        0        0       70 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/nf-analysis/pipeline_params.config
--rw-r--r--   0        0        0      195 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/nf-analysis/pipeline_resource_optimisation.config
--rw-r--r--   0        0        0      195 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/nf-analysis/platform.config
--rw-r--r--   0        0        0     8173 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/raredisease/multiqc_data.json
--rw-r--r--   0        0        0    20005 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml
--rw-r--r--   0        0        0     5497 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/rnafusion/multiqc_data.json
--rw-r--r--   0        0        0    12499 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml
--rw-r--r--   0        0        0     2873 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/sample_coverage.bed
--rw-r--r--   0        0        0     6506 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/taxprofiler/multiqc_data.json
--rw-r--r--   0        0        0    10513 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml
--rw-r--r--   0        0        0     5771 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/tomte/multiqc_data.json
--rw-r--r--   0        0        0    14859 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml
--rw-r--r--   0        0        0    10961 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/balsamic/case/config.json
--rw-r--r--   0        0        0     3465 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/balsamic/case/metadata.yml
--rw-r--r--   0        0        0       63 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/balsamic/case/metadata_directory.yml
--rw-r--r--   0        0        0      165 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
--rw-r--r--   0        0        0     2705 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
--rw-r--r--   0        0        0      692 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/crunchy/spring_metadata.json
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0      412 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      484 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      658 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/demuxcomplete.txt
--rw-r--r--   0        0        0     1757 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0        0        0        7 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0     6034 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0        0        0     1172 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0        0        0        7 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_1.fastq.gz
--rw-r--r--   0        0        0        7 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_2.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0      345 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      650 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      896 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0      602 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/demuxcomplete.txt
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0      288 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      361 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      414 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/demuxcomplete.txt
--rw-r--r--   0        0        0      315 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      434 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0     8624 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml
--rw-r--r--   0        0        0      568 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0      220 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      463 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      622 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0      345 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      650 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      896 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0      619 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0      303 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      364 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      427 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/demuxcomplete.txt
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0     4439 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0        0        0     1172 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0     5127 2024-04-24 11:46:39.991723 cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
--rw-r--r--   0        0        0       43 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz
--rw-r--r--   0        0        0       67 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz.md5
--rw-r--r--   0        0        0   338370 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz
--rw-r--r--   0        0        0       67 2024-04-24 11:46:39.995723 cg-60.3.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz.md5
--rw-r--r--   0        0        0   338349 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/CopyComplete.txt
--rw-r--r--   0        0        0     2126 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json
--rw-r--r--   0        0        0     1827 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json
--rw-r--r--   0        0        0       90 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/README.txt
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAComplete.txt
--rw-r--r--   0        0        0     6895 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml
--rw-r--r--   0        0        0       37 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead1Complete.txt
--rw-r--r--   0        0        0       36 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead2Complete.txt
--rw-r--r--   0        0        0       36 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead3Complete.txt
--rw-r--r--   0        0        0    24755 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml
--rw-r--r--   0        0        0      692 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
--rw-r--r--   0        0        0      724 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0       61 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SequencingComplete.txt
--rw-r--r--   0        0        0     5775 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/CopyComplete.txt
--rw-r--r--   0        0        0     2282 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json
--rw-r--r--   0        0        0     1632 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json
--rw-r--r--   0        0        0       75 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/README.txt
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAComplete.txt
--rw-r--r--   0        0        0     6912 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml
--rw-r--r--   0        0        0       36 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead1Complete.txt
--rw-r--r--   0        0        0       36 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead2Complete.txt
--rw-r--r--   0        0        0       36 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead3Complete.txt
--rw-r--r--   0        0        0       36 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead4Complete.txt
--rw-r--r--   0        0        0    24814 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml
--rw-r--r--   0        0        0      814 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv
--rw-r--r--   0        0        0      660 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0       61 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SequencingComplete.txt
--rw-r--r--   0        0        0     5853 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/CopyComplete.txt
--rw-r--r--   0        0        0    21848 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json
--rw-r--r--   0        0        0    15512 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json
--rw-r--r--   0        0        0       79 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/README.txt
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RTAComplete.txt
--rw-r--r--   0        0        0      756 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml
--rw-r--r--   0        0        0     4118 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv
--rw-r--r--   0        0        0     1408 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0     5326 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/CopyComplete.txt
--rw-r--r--   0        0        0    15041 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json
--rw-r--r--   0        0        0    10649 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json
--rw-r--r--   0        0        0       80 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/README.txt
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RTAComplete.txt
--rw-r--r--   0        0        0      755 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml
--rw-r--r--   0        0        0     2878 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv
--rw-r--r--   0        0        0      928 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0     5359 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CopyComplete.txt
--rw-r--r--   0        0        0    27887 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv
--rw-r--r--   0        0        0   141870 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json
--rwxr-xr-x   0        0        0   122682 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json
--rw-r--r--   0        0        0      243 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/README.txt
--rw-r--r--   0        0        0    28230 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTAComplete.txt
--rw-r--r--   0        0        0    94426 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml
--rw-r--r--   0        0        0     5819 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/SequenceComplete.txt
--rw-r--r--   0        0        0     1757 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0        0        0     1757 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stdout
--rw-r--r--   0        0        0       12 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/README.txt
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RTAComplete.txt
--rw-r--r--   0        0        0     5945 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml
--rw-r--r--   0        0        0      260 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/copycomplete.txt
--rw-r--r--   0        0        0        0 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/demuxstarted.txt
--rw-r--r--   0        0        0     1757 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0        0        0     1757 2024-04-24 11:46:39.999723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout
--rw-r--r--   0        0        0    47522 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json
--rw-r--r--   0        0        0       12 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/README.txt
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0        0        0     6666 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0        0        0      254 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/copycomplete.txt
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/delivery.txt
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/demuxstarted.txt
--rwxr-xr-x   0        0        0    47434 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CopyComplete.txt
--rw-r--r--   0        0        0    10950 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv
--rw-r--r--   0        0        0      225 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/Manifest.tsv
--rw-r--r--   0        0        0       55 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/README.txt
--rwxr-xr-x   0        0        0     2493 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg
--rwxr-xr-x   0        0        0        1 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAComplete.txt
--rwxr-xr-x   0        0        0        2 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAExited.txt
--rwxr-xr-x   0        0        0      730 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml
--rwxr-xr-x   0        0        0    79277 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml
--rwxr-xr-x   0        0        0     2694 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
--rw-r--r--   0        0        0    10950 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
--rw-r--r--   0        0        0      619 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0        0        0       12 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/README.txt
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0        0        0      399 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CopyComplete.txt
--rw-r--r--   0        0        0     4941 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv
--rwxr-xr-x   0        0        0    20050 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stderr
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stdout
--rw-r--r--   0        0        0      244 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/README.txt
--rw-r--r--   0        0        0     6391 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTAComplete.txt
--rw-r--r--   0        0        0    16428 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml
--rw-r--r--   0        0        0     6728 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
--rw-r--r--   0        0        0     5127 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SequenceComplete.txt
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/demuxstarted.txt
--rw-r--r--   0        0        0      133 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/README.txt
--rw-r--r--   0        0        0      724 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
--rw-r--r--   0        0        0     5775 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
--rw-r--r--   0        0        0      124 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/180509_D00450_0598_BHGYFNBCX2/README.txt
--rw-r--r--   0        0        0      310 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/README.txt
--rw-r--r--   0        0        0     5819 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
--rw-r--r--   0        0        0      122 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/README.txt
--rwxr-xr-x   0        0        0     2694 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
--rw-r--r--   0        0        0      311 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/README.txt
--rw-r--r--   0        0        0     6728 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0        0        0      399 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
--rw-r--r--   0        0        0      399 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_0.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_1.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/final_summary_PAS86456_72d9fceb_8a4fd683.txt
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_0.pod5
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_1.pod5
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_0.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_1.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/final_summary_PAS97781_595b5663_efc7f02e.txt
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_0.pod5
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_1.pod5
--rw-r--r--   0        0        0   111989 2024-04-24 11:46:40.003723 cg-60.3.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
--rw-r--r--   0        0        0     5319 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml
--rw-r--r--   0        0        0     5944 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
--rwxr-xr-x   0        0        0     2481 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
--rwxr-xr-x   0        0        0     2474 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml
--rw-r--r--   0        0        0     5899 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
--rw-r--r--   0        0        0     4941 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv
--rw-r--r--   0        0        0    10950 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/demultiplexing/spring/dummy_run_001.spring
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/demultiplexing/spring/dummy_run_002.spring
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/demultiplexing/spring/dummy_spring_meta_data.json
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
--rw-r--r--   0        0        0     5554 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/fluffy/SampleSheet.csv
--rw-r--r--   0        0        0      901 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/fluffy/deliverables.yaml
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/fluffy/multiqc_report.html
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/fluffy/summary.csv
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/gt/yellowhog.bcf
--rw-r--r--   0        0        0     5114 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/madeline/madeline.xml
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/case_file.txt
--rw-r--r--   0        0        0     3241 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
--rw-r--r--   0        0        0    21811 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/dna/store/case_config.yaml
--rw-r--r--   0        0        0    23364 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
--rw-r--r--   0        0        0    37367 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
--rw-r--r--   0        0        0       16 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
--rw-r--r--   0        0        0       16 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
--rw-r--r--   0        0        0       16 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
--rw-r--r--   0        0        0      123 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
--rw-r--r--   0        0        0    62741 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
--rw-r--r--   0        0        0    11242 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/rna/case_config.yaml
--rw-r--r--   0        0        0    12164 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
--rw-r--r--   0        0        0     5231 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
--rw-r--r--   0        0        0     9774 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/rna/store/case_config.yaml
--rw-r--r--   0        0        0     4624 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
--rw-r--r--   0        0        0    13666 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/mip/sample_file.txt
--rw-r--r--   0        0        0     1885 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/scout/643594.config.yaml
--rw-r--r--   0        0        0     6027 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/scout/case_export.json
--rw-r--r--   0        0        0     9349 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/scout/export_causatives.json
--rw-r--r--   0        0        0     1315 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/scout/none_case_export.json
--rw-r--r--   0        0        0     3518 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/scout/other_sex_case.json
--rw-r--r--   0        0        0     8874 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/scout/panel_export.bed
--rw-r--r--   0        0        0     4169 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/scout/panel_export.csv
--rw-r--r--   0        0        0      619 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/SampleSheet.csv
--rw-r--r--   0        0        0    63569 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0    42478 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0    69708 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0       42 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/apps/shipping/scout-deploy.yaml
--rw-r--r--   0        0        0     1036 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/cgweb_orders/balsamic.json
--rw-r--r--   0        0        0     1104 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/cgweb_orders/fastq.json
--rw-r--r--   0        0        0     1313 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/cgweb_orders/metagenome.json
--rw-r--r--   0        0        0     3038 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/cgweb_orders/microsalt.json
--rw-r--r--   0        0        0     3705 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/cgweb_orders/mip.json
--rw-r--r--   0        0        0     1364 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/cgweb_orders/mip_rna.json
--rw-r--r--   0        0        0     2125 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/cgweb_orders/rml.json
--rw-r--r--   0        0        0     1368 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/cgweb_orders/rnafusion.json
--rw-r--r--   0        0        0     4684 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/cgweb_orders/sarscov2.json
--rw-r--r--   0        0        0     5609 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/data/SampleSheet.csv
--rw-r--r--   0        0        0      511 2024-04-24 11:46:40.007723 cg-60.3.1/tests/fixtures/data/bcl_convert_sample_sheet.csv
--rw-r--r--   0        0        0   258048 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/data/cgfixture.db
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/data/fastq.fastq.gz
--rw-r--r--   0        0        0    49152 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/data/hkstore.db
--rw-r--r--   0        0        0       73 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/data/yellowhog/pedigree.yaml
--rw-r--r--   0        0        0       76 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/io/casava_five_parts.fastq.gz
--rw-r--r--   0        0        0       90 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/io/casava_seven_parts.fastq.gz
--rw-r--r--   0        0        0       96 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/io/casava_ten_parts.fastq.gz
--rw-r--r--   0        0        0      153 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/io/example.csv
--rw-r--r--   0        0        0       46 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/io/example.gz
--rw-r--r--   0        0        0      147 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/io/example.tsv
--rw-r--r--   0        0        0       20 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/io/example.txt
--rw-r--r--   0        0        0       20 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/io/example2.txt
--rw-r--r--   0        0        0      582 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/io/example_json.json
--rw-r--r--   0        0        0      103 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/io/example_xml.xml
--rw-r--r--   0        0        0       20 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/meta/qc_metrics/file_with_right_tags.json
--rw-r--r--   0        0        0       20 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/meta/qc_metrics/file_without_right_tags.json
--rw-r--r--   0        0        0   156910 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/orderforms/1508.30.balsamic.xlsx
--rw-r--r--   0        0        0   156770 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx
--rw-r--r--   0        0        0   156737 2024-04-24 11:46:40.011723 cg-60.3.1/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx
--rw-r--r--   0        0        0   156582 2024-04-24 11:46:40.015723 cg-60.3.1/tests/fixtures/orderforms/1508.30.fastq.xlsx
--rw-r--r--   0        0        0   155627 2024-04-24 11:46:40.015723 cg-60.3.1/tests/fixtures/orderforms/1508.30.metagenome.xlsx
--rw-r--r--   0        0        0   156850 2024-04-24 11:46:40.015723 cg-60.3.1/tests/fixtures/orderforms/1508.30.mip.xlsx
--rw-r--r--   0        0        0   258580 2024-04-24 11:46:40.015723 cg-60.3.1/tests/fixtures/orderforms/1508.30.mip_rna.xlsx
--rw-r--r--   0        0        0   258342 2024-04-24 11:46:40.015723 cg-60.3.1/tests/fixtures/orderforms/1508.30.rnafusion.xlsx
--rw-r--r--   0        0        0    82677 2024-04-24 11:46:40.015723 cg-60.3.1/tests/fixtures/orderforms/1603.11.microbial.xlsx
--rw-r--r--   0        0        0   149394 2024-04-24 11:46:40.015723 cg-60.3.1/tests/fixtures/orderforms/1604.17.rml.xlsx
--rw-r--r--   0        0        0   223184 2024-04-24 11:46:40.019723 cg-60.3.1/tests/fixtures/orderforms/2184.9.sarscov2.xlsx
--rw-r--r--   0        0        0    18639 2024-04-24 11:46:40.019723 cg-60.3.1/tests/fixtures/orderforms/NIPT-json.json
--rw-r--r--   0        0        0     6052 2024-04-24 11:46:40.019723 cg-60.3.1/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
--rw-r--r--   0        0        0     6611 2024-04-24 11:46:40.019723 cg-60.3.1/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
--rw-r--r--   0        0        0     1417 2024-04-24 11:46:40.019723 cg-60.3.1/tests/fixtures/report/case_data.json
--rw-r--r--   0        0        0     1109 2024-04-24 11:46:40.019723 cg-60.3.1/tests/fixtures/report/lims_exported_samples.json
--rw-r--r--   0        0        0     1562 2024-04-24 11:46:40.019723 cg-60.3.1/tests/fixtures/report/lims_family.json
--rw-r--r--   0        0        0     3296 2024-04-24 11:46:40.019723 cg-60.3.1/tests/io/conftest.py
--rw-r--r--   0        0        0      431 2024-04-24 11:46:40.019723 cg-60.3.1/tests/io/test_io_config.py
--rw-r--r--   0        0        0     8639 2024-04-24 11:46:40.019723 cg-60.3.1/tests/io/test_io_controller.py
--rw-r--r--   0        0        0     3877 2024-04-24 11:46:40.019723 cg-60.3.1/tests/io/test_io_csv.py
--rw-r--r--   0        0        0      482 2024-04-24 11:46:40.019723 cg-60.3.1/tests/io/test_io_gzip.py
--rw-r--r--   0        0        0     1779 2024-04-24 11:46:40.019723 cg-60.3.1/tests/io/test_io_json.py
--rw-r--r--   0        0        0     2914 2024-04-24 11:46:40.019723 cg-60.3.1/tests/io/test_io_txt.py
--rw-r--r--   0        0        0     1027 2024-04-24 11:46:40.019723 cg-60.3.1/tests/io/test_io_xml.py
--rw-r--r--   0        0        0     2131 2024-04-24 11:46:40.019723 cg-60.3.1/tests/io/test_io_yaml.py
--rw-r--r--   0        0        0     1233 2024-04-24 11:46:40.019723 cg-60.3.1/tests/io/test_validate_path.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/archive/__init__.py
--rw-r--r--   0        0        0    13131 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/archive/conftest.py
--rw-r--r--   0        0        0    16858 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/archive/test_archive_api.py
--rw-r--r--   0        0        0    10246 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/archive/test_archive_cli.py
--rw-r--r--   0        0        0    15766 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/archive/test_archiving.py
--rw-r--r--   0        0        0     3807 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/backup/conftest.py
--rw-r--r--   0        0        0    26368 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/backup/test_meta_backup.py
--rw-r--r--   0        0        0    10055 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/backup/test_meta_pdc.py
--rw-r--r--   0        0        0    12546 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/clean/conftest.py
--rw-r--r--   0        0        0    16944 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/clean/test_clean_flow_cells_api.py
--rw-r--r--   0        0        0     2286 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/clean/test_clean_retrieved_spring_files.py
--rw-r--r--   0        0        0     7691 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/compress/conftest.py
--rw-r--r--   0        0        0     7961 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/compress/test_clean_fastq.py
--rw-r--r--   0        0        0     1778 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/compress/test_compress_files.py
--rw-r--r--   0        0        0     3644 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/compress/test_compress_meta_fastq.py
--rw-r--r--   0        0        0     1180 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/compress/test_decompress_spring_meta.py
--rw-r--r--   0        0        0     6902 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/compress/test_meta_compress_update_hk.py
--rw-r--r--   0        0        0     8207 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/conftest.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/deliver/__init__.py
--rw-r--r--   0        0        0     3471 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/deliver/conftest.py
--rw-r--r--   0        0        0     5533 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/deliver/test_deliver_ticket.py
--rw-r--r--   0        0        0    10277 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/deliver/test_delivery_api.py
--rw-r--r--   0        0        0     1057 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/deliver/test_fastq_path_generator.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/delivery/__init__.py
--rw-r--r--   0        0        0    16660 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/delivery/test_delivery_api.py
--rw-r--r--   0        0        0     8729 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/demultiplex/conftest.py
--rw-r--r--   0        0        0     5382 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/demultiplex/test_combine_sequencing_metrics.py
--rw-r--r--   0        0        0     8339 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/demultiplex/test_demux_post_processing.py
--rw-r--r--   0        0        0    12330 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/demultiplex/test_housekeeper_storage_functions.py
--rw-r--r--   0        0        0     4392 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/demultiplex/test_status_db_storage_functions.py
--rw-r--r--   0        0        0    22705 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/demultiplex/test_utils.py
--rw-r--r--   0        0        0     6193 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/demultiplex/test_validation.py
--rw-r--r--   0        0        0     4943 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/encryption/conftest.py
--rw-r--r--   0        0        0    18133 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/encryption/test_encryption.py
--rw-r--r--   0        0        0     3122 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/observations/conftest.py
--rw-r--r--   0        0        0    16164 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/observations/test_meta_upload_observations.py
--rw-r--r--   0        0        0     4974 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/orders/conftest.py
--rw-r--r--   0        0        0     1749 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/orders/test_PoolSubmitter_validate_order.py
--rw-r--r--   0        0        0     1470 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
--rw-r--r--   0        0        0     1768 2024-04-24 11:46:40.019723 cg-60.3.1/tests/meta/orders/test_SarsCov2Submitter_store_order.py
--rw-r--r--   0        0        0     2032 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
--rw-r--r--   0        0        0    19783 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/orders/test_meta_orders_api.py
--rw-r--r--   0        0        0     7086 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/orders/test_meta_orders_lims.py
--rw-r--r--   0        0        0    29515 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/orders/test_meta_orders_status.py
--rw-r--r--   0        0        0     1677 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/orders/test_rnafusion_submitter.py
--rw-r--r--   0        0        0     1068 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/orders/test_ticket_handler.py
--rw-r--r--   0        0        0     4336 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/qc_metrics/conftest.py
--rw-r--r--   0        0        0     1972 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/qc_metrics/test_collect_qc_metrics.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/report/__init__.py
--rw-r--r--   0        0        0     6512 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/report/conftest.py
--rw-r--r--   0        0        0      434 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/report/helper.py
--rw-r--r--   0        0        0     2604 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/report/test_balsamic_api.py
--rw-r--r--   0        0        0     4056 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/report/test_field_validators.py
--rw-r--r--   0        0        0     2858 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/report/test_mip_dna_api.py
--rw-r--r--   0        0        0    16042 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/report/test_report_api.py
--rw-r--r--   0        0        0     1365 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/report/test_rnafusion_api.py
--rw-r--r--   0        0        0     1250 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/report/test_tomte_api.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/rsync/__init__.py
--rw-r--r--   0        0        0      916 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/rsync/conftest.py
--rw-r--r--   0        0        0     9442 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/rsync/test_rsync.py
--rw-r--r--   0        0        0     3147 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/test_invoice.py
--rw-r--r--   0        0        0     1220 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/transfer/conftest.py
--rw-r--r--   0        0        0     9892 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/transfer/test_external_data.py
--rw-r--r--   0        0        0     4395 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/transfer/test_meta_transfer_lims.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/__init__.py
--rw-r--r--   0        0        0     2210 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/balsamic/test_balsamic.py
--rw-r--r--   0        0        0     4002 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/conftest.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/gisaid/__init__.py
--rw-r--r--   0        0        0     2557 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/gisaid/fixtures/four_samples.csv
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
--rw-r--r--   0        0        0      211 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
--rw-r--r--   0        0        0      371 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/mutacc/__init__.py
--rw-r--r--   0        0        0     3684 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/mutacc/conftest.py
--rw-r--r--   0        0        0     4188 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
--rw-r--r--   0        0        0     1149 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/nipt/conftest.py
--rw-r--r--   0        0        0     1683 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/nipt/test_models.py
--rw-r--r--   0        0        0     1242 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/nipt/test_nipt_upload_api.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/scout/__init__.py
--rw-r--r--   0        0        0    23954 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/scout/conftest.py
--rw-r--r--   0        0        0     4734 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/scout/test_generate_load_config.py
--rw-r--r--   0        0        0     4182 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/scout/test_meta_upload_scoutapi.py
--rw-r--r--   0        0        0    33260 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
--rw-r--r--   0        0        0     7372 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/scout/test_scout_config_builder.py
--rw-r--r--   0        0        0     2511 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/test_meta_upload_coverage.py
--rw-r--r--   0        0        0     1473 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/test_upload_api.py
--rw-r--r--   0        0        0     2547 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/upload/test_upload_genotypes_api.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/__init__.py
--rw-r--r--   0        0        0    10262 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/conftest.py
--rw-r--r--   0        0        0     3652 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/microsalt/conftest.py
--rw-r--r--   0        0        0      318 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/microsalt/test_parsing_metrics.py
--rw-r--r--   0        0        0     3714 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/microsalt/test_quality_controller.py
--rw-r--r--   0        0        0    14367 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/microsalt/test_quality_controller_utils.py
--rw-r--r--   0        0        0      825 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/microsalt/test_report_generation.py
--rw-r--r--   0        0        0    20848 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/test_analysis.py
--rw-r--r--   0        0        0     7934 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/test_balsamic.py
--rw-r--r--   0        0        0     3034 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/test_fastq.py
--rw-r--r--   0        0        0     1532 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/test_microsalt.py
--rw-r--r--   0        0        0     2721 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/test_nf_analysis.py
--rw-r--r--   0        0        0     7741 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/test_prepare_fastq_api.py
--rw-r--r--   0        0        0     1920 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/test_raredisease.py
--rw-r--r--   0        0        0     1674 2024-04-24 11:46:40.023723 cg-60.3.1/tests/meta/workflow/test_rnafusion.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/__init__.py
--rw-r--r--   0        0        0     1168 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/balsamic_analysis_mock.py
--rw-r--r--   0        0        0     3500 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/crunchy.py
--rw-r--r--   0        0        0    21778 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/hk_mock.py
--rw-r--r--   0        0        0     4106 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/limsmock.py
--rw-r--r--   0        0        0      572 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/madeline.py
--rw-r--r--   0        0        0     1297 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/mip_analysis_mock.py
--rw-r--r--   0        0        0     1525 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/osticket.py
--rw-r--r--   0        0        0     3239 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/process_mock.py
--rw-r--r--   0        0        0     4713 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/report.py
--rw-r--r--   0        0        0     3915 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/scout.py
--rw-r--r--   0        0        0      750 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/store_model.py
--rw-r--r--   0        0        0     1532 2024-04-24 11:46:40.023723 cg-60.3.1/tests/mocks/tb_mock.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.023723 cg-60.3.1/tests/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.023723 cg-60.3.1/tests/models/balsamic/__init__.py
--rw-r--r--   0        0        0     1194 2024-04-24 11:46:40.023723 cg-60.3.1/tests/models/balsamic/conftest.py
--rw-r--r--   0        0        0     1030 2024-04-24 11:46:40.023723 cg-60.3.1/tests/models/balsamic/test_balsamic_analysis.py
--rw-r--r--   0        0        0     1050 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/conftest.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/demultiplexing/__init__.py
--rw-r--r--   0        0        0      284 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/demultiplexing/conftest.py
--rw-r--r--   0        0        0    11446 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/demultiplexing/test_run_parameters.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/downsample/__init__.py
--rw-r--r--   0        0        0     2096 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/downsample/test_down_sample_meta_data.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/flow_cell/__init__.py
--rw-r--r--   0        0        0     6659 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/flow_cell/test_flowcell_model.py
--rw-r--r--   0        0        0     6637 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/mip/conftest.py
--rw-r--r--   0        0        0     1239 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/mip/test_mip_analysis.py
--rw-r--r--   0        0        0     2348 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/mip/test_mip_config.py
--rw-r--r--   0        0        0     6392 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/mip/test_mip_metrics_deliverables.py
--rw-r--r--   0        0        0     3959 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/mip/test_mip_sample_info.py
--rw-r--r--   0        0        0     3314 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/nextflow/test_nextflow_deliver.py
--rw-r--r--   0        0        0     1602 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/observations/conftest.py
--rw-r--r--   0        0        0     2579 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/observations/test_observations_input_files.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/report/__init__.py
--rw-r--r--   0        0        0     7327 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/report/test_validators.py
--rw-r--r--   0        0        0     3855 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/rnafusion/test_rnafusion_sample.py
--rw-r--r--   0        0        0     1374 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/test_cg_models.py
--rw-r--r--   0        0        0      990 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/test_compression_data.py
--rw-r--r--   0        0        0      729 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/test_fastq.py
--rw-r--r--   0        0        0     2860 2024-04-24 11:46:40.027723 cg-60.3.1/tests/models/test_file_data.py
--rw-r--r--   0        0        0     4539 2024-04-24 11:46:40.027723 cg-60.3.1/tests/server/conftest.py
--rw-r--r--   0        0        0     3135 2024-04-24 11:46:40.027723 cg-60.3.1/tests/server/endpoints/test_delivery_message_endpoint.py
--rw-r--r--   0        0        0     3239 2024-04-24 11:46:40.027723 cg-60.3.1/tests/server/endpoints/test_orders_endpoint.py
--rw-r--r--   0        0        0      271 2024-04-24 11:46:40.027723 cg-60.3.1/tests/server/test_server_auto.py
--rw-r--r--   0        0        0     1047 2024-04-24 11:46:40.027723 cg-60.3.1/tests/services/fastq_file_service/conftest.py
--rw-r--r--   0        0        0     3634 2024-04-24 11:46:40.027723 cg-60.3.1/tests/services/fastq_file_service/test_fastq_file_service.py
--rw-r--r--   0        0        0     4861 2024-04-24 11:46:40.027723 cg-60.3.1/tests/services/orders/order_status_service/conftest.py
--rw-r--r--   0        0        0     2865 2024-04-24 11:46:40.027723 cg-60.3.1/tests/services/orders/order_status_service/test_order_summary_service.py
--rw-r--r--   0        0        0      318 2024-04-24 11:46:40.027723 cg-60.3.1/tests/small_helpers.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/api/__init__.py
--rw-r--r--   0        0        0     2984 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/api/conftest.py
--rw-r--r--   0        0        0     1557 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/api/test_base.py
--rw-r--r--   0        0        0    20096 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/conftest.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/add/__init__.py
--rw-r--r--   0        0        0     1497 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/add/test_store_add_application_version.py
--rw-r--r--   0        0        0     3958 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/add/test_store_add_base.py
--rw-r--r--   0        0        0     2502 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/add/test_store_add_customer.py
--rw-r--r--   0        0        0     1640 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/add/test_store_add_flow_celll.py
--rw-r--r--   0        0        0    12212 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/conftest.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/delete/__init__.py
--rw-r--r--   0        0        0     5541 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/delete/test_delete.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/read/__init__.py
--rw-r--r--   0        0        0    57211 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/read/test_read.py
--rw-r--r--   0        0        0     5461 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/read/test_read_analyses_to_clean.py
--rw-r--r--   0        0        0     3553 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/read/test_read_analyses_to_delivery_report.py
--rw-r--r--   0        0        0    18463 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/read/test_read_analysis.py
--rw-r--r--   0        0        0     2743 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/read/test_read_application_version.py
--rw-r--r--   0        0        0     1105 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/read/test_read_customer.py
--rw-r--r--   0        0        0     1530 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/read/test_read_pool.py
--rw-r--r--   0        0        0    21503 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/read/test_read_sample.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/update/__init__.py
--rw-r--r--   0        0        0      737 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/crud/update/test_update.py
--rw-r--r--   0        0        0    11693 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_analyses_filters.py
--rw-r--r--   0        0        0     3397 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_application_filters.py
--rw-r--r--   0        0        0     2073 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_application_limitations_filters.py
--rw-r--r--   0        0        0    10452 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_application_version_filters.py
--rw-r--r--   0        0        0     2804 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_bed_filters.py
--rw-r--r--   0        0        0     2362 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_bed_version_filters.py
--rw-r--r--   0        0        0     3495 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_case_sample_filters.py
--rw-r--r--   0        0        0    39100 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_cases_filters.py
--rw-r--r--   0        0        0     1345 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_collaboration_filters.py
--rw-r--r--   0        0        0     2482 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_customer_filters.py
--rw-r--r--   0        0        0     4907 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_flow_cell_filters.py
--rw-r--r--   0        0        0     2226 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_invoice_filters.py
--rw-r--r--   0        0        0     5871 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_metrics_filters.py
--rw-r--r--   0        0        0     2404 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_organism_filters.py
--rw-r--r--   0        0        0     1804 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_panel_filters.py
--rw-r--r--   0        0        0     8720 2024-04-24 11:46:40.027723 cg-60.3.1/tests/store/filters/test_status_pool_filters.py
--rw-r--r--   0        0        0    22875 2024-04-24 11:46:40.031723 cg-60.3.1/tests/store/filters/test_status_samples_filters.py
--rw-r--r--   0        0        0     1576 2024-04-24 11:46:40.031723 cg-60.3.1/tests/store/filters/test_status_user_filters.py
--rw-r--r--   0        0        0     2147 2024-04-24 11:46:40.031723 cg-60.3.1/tests/store/test_delivery.py
--rw-r--r--   0        0        0     4127 2024-04-24 11:46:40.031723 cg-60.3.1/tests/store/test_store_models.py
--rw-r--r--   0        0        0    37040 2024-04-24 11:46:40.031723 cg-60.3.1/tests/store_helpers.py
--rw-r--r--   0        0        0     4930 2024-04-24 11:46:40.031723 cg-60.3.1/tests/test_copy_novaseqx_flow_cell.py
--rw-r--r--   0        0        0      911 2024-04-24 11:46:40.031723 cg-60.3.1/tests/test_store_helpers.py
--rw-r--r--   0        0        0        0 2024-04-24 11:46:40.031723 cg-60.3.1/tests/utils/__init__.py
--rw-r--r--   0        0        0     1754 2024-04-24 11:46:40.031723 cg-60.3.1/tests/utils/conftest.py
--rw-r--r--   0        0        0      371 2024-04-24 11:46:40.031723 cg-60.3.1/tests/utils/test_calculations.py
--rw-r--r--   0        0        0     2920 2024-04-24 11:46:40.031723 cg-60.3.1/tests/utils/test_commands.py
--rw-r--r--   0        0        0      953 2024-04-24 11:46:40.031723 cg-60.3.1/tests/utils/test_date.py
--rw-r--r--   0        0        0     1508 2024-04-24 11:46:40.031723 cg-60.3.1/tests/utils/test_dict.py
--rw-r--r--   0        0        0     7154 2024-04-24 11:46:40.031723 cg-60.3.1/tests/utils/test_dispatcher.py
--rw-r--r--   0        0        0     4100 2024-04-24 11:46:40.031723 cg-60.3.1/tests/utils/test_files.py
--rw-r--r--   0        0        0     1170 2024-04-24 11:46:40.031723 cg-60.3.1/tests/utils/test_time.py
--rw-r--r--   0        0        0     2366 2024-04-24 11:46:40.031723 cg-60.3.1/tests/utils/test_utils.py
--rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 cg-60.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2686 2024-04-25 07:10:48.501212 cg-60.3.2/README.md
+-rw-r--r--   0        0        0       40 2024-04-25 07:10:48.505212 cg-60.3.2/cg/__init__.py
+-rw-r--r--   0        0        0      315 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/coverage/__init__.py
+-rw-r--r--   0        0        0     2940 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/coverage/api.py
+-rw-r--r--   0        0        0       56 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/crunchy/__init__.py
+-rw-r--r--   0        0        0    12783 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/crunchy/crunchy.py
+-rw-r--r--   0        0        0     4502 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/crunchy/files.py
+-rw-r--r--   0        0        0      430 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/crunchy/models.py
+-rw-r--r--   0        0        0      910 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/crunchy/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/demultiplex/__init__.py
+-rw-r--r--   0        0        0    11299 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/demultiplex/demultiplex_api.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/demultiplex/sample_sheet/__init__.py
+-rw-r--r--   0        0        0    11227 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/demultiplex/sample_sheet/api.py
+-rw-r--r--   0        0        0     2183 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/demultiplex/sample_sheet/index.py
+-rw-r--r--   0        0        0     7341 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py
+-rw-r--r--   0        0        0     3188 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py
+-rw-r--r--   0        0        0     7071 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/demultiplex/sample_sheet/sample_models.py
+-rw-r--r--   0        0        0     6076 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py
+-rw-r--r--   0        0        0     1372 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py
+-rw-r--r--   0        0        0     8092 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py
+-rw-r--r--   0        0        0      824 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/demultiplex/sample_sheet/validators.py
+-rw-r--r--   0        0        0      677 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/demultiplex/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/downsample/__init__.py
+-rw-r--r--   0        0        0     6160 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/downsample/downsample.py
+-rw-r--r--   0        0        0     2125 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/downsample/utils.py
+-rw-r--r--   0        0        0      298 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/environ.py
+-rw-r--r--   0        0        0     1741 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/gens.py
+-rw-r--r--   0        0        0     3419 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/gt.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/hermes/__init__.py
+-rw-r--r--   0        0        0     2249 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/hermes/hermes_api.py
+-rw-r--r--   0        0        0     1298 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/hermes/models.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/housekeeper/__init__.py
+-rw-r--r--   0        0        0    30395 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/housekeeper/hk.py
+-rw-r--r--   0        0        0      326 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/housekeeper/models.py
+-rw-r--r--   0        0        0       32 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/invoice/__init__.py
+-rw-r--r--   0        0        0     4804 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/invoice/render.py
+-rw-r--r--   0        0        0   113467 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/invoice/templates/KI_pool_invoice.xlsx
+-rw-r--r--   0        0        0    75562 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/invoice/templates/KI_sample_invoice.xlsx
+-rw-r--r--   0        0        0   113512 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
+-rw-r--r--   0        0        0    75459 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
+-rw-r--r--   0        0        0       25 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/lims/__init__.py
+-rw-r--r--   0        0        0    18546 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/lims/api.py
+-rw-r--r--   0        0        0     2652 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/lims/batch.py
+-rw-r--r--   0        0        0     8129 2024-04-25 07:10:48.505212 cg-60.3.2/cg/apps/lims/order.py
+-rw-r--r--   0        0        0     3118 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/lims/sample_sheet.py
+-rw-r--r--   0        0        0     4866 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/loqus.py
+-rw-r--r--   0        0        0       35 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/madeline/__init__.py
+-rw-r--r--   0        0        0     3213 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/madeline/api.py
+-rw-r--r--   0        0        0       23 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/mip/__init__.py
+-rw-r--r--   0        0        0     3564 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/mip/confighandler.py
+-rw-r--r--   0        0        0     2207 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/mutacc_auto.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/orderform/__init__.py
+-rw-r--r--   0        0        0     9498 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/orderform/excel_orderform_parser.py
+-rw-r--r--   0        0        0     3051 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/orderform/json_orderform_parser.py
+-rw-r--r--   0        0        0     6419 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/orderform/orderform_parser.py
+-rw-r--r--   0        0        0      252 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/orderform/utils.py
+-rw-r--r--   0        0        0     2537 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/osticket.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/scout/__init__.py
+-rw-r--r--   0        0        0     3177 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/scout/scout_export.py
+-rw-r--r--   0        0        0    11054 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/scout/scoutapi.py
+-rw-r--r--   0        0        0      444 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/scout/validators.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0        0        0     3457 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/sequencing_metrics_parser/api.py
+-rw-r--r--   0        0        0      923 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/sequencing_metrics_parser/models.py
+-rw-r--r--   0        0        0     6658 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/sequencing_metrics_parser/parser.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/slurm/__init__.py
+-rw-r--r--   0        0        0     1277 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/slurm/sbatch.py
+-rw-r--r--   0        0        0     3559 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/slurm/slurm_api.py
+-rw-r--r--   0        0        0       32 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/tb/__init__.py
+-rw-r--r--   0        0        0     7995 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/tb/api.py
+-rw-r--r--   0        0        0      152 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/tb/dto/create_job_request.py
+-rw-r--r--   0        0        0      250 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/tb/dto/summary_response.py
+-rw-r--r--   0        0        0     1305 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/tb/models.py
+-rw-r--r--   0        0        0      305 2024-04-25 07:10:48.509212 cg-60.3.2/cg/apps/tb/validators.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/__init__.py
+-rw-r--r--   0        0        0    11558 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/add.py
+-rw-r--r--   0        0        0     2653 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/archive.py
+-rw-r--r--   0        0        0    10118 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/backup.py
+-rw-r--r--   0        0        0     3852 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/base.py
+-rw-r--r--   0        0        0    10506 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/clean.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/compress/__init__.py
+-rw-r--r--   0        0        0     2135 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/compress/base.py
+-rw-r--r--   0        0        0     6706 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/compress/fastq.py
+-rw-r--r--   0        0        0     8163 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/compress/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/delete/__init__.py
+-rw-r--r--   0        0        0      564 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/delete/base.py
+-rw-r--r--   0        0        0     4603 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/delete/case.py
+-rw-r--r--   0        0        0     1884 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/delete/cases.py
+-rw-r--r--   0        0        0     2633 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/delete/observations.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/deliver/__init__.py
+-rw-r--r--   0        0        0     6030 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/deliver/base.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/demultiplex/__init__.py
+-rw-r--r--   0        0        0      829 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/demultiplex/base.py
+-rw-r--r--   0        0        0     4905 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py
+-rw-r--r--   0        0        0     7726 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/demultiplex/demux.py
+-rw-r--r--   0        0        0     1473 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/demultiplex/finish.py
+-rw-r--r--   0        0        0     3119 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/demultiplex/sample_sheet.py
+-rw-r--r--   0        0        0     2995 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/downsample.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/generate/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/generate/base.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/generate/report/__init__.py
+-rw-r--r--   0        0        0     4636 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/generate/report/base.py
+-rw-r--r--   0        0        0      854 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/generate/report/options.py
+-rw-r--r--   0        0        0     5340 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/generate/report/utils.py
+-rw-r--r--   0        0        0     8327 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/get.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/set/__init__.py
+-rw-r--r--   0        0        0     9856 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/set/base.py
+-rw-r--r--   0        0        0     4384 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/set/case.py
+-rw-r--r--   0        0        0     2595 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/set/cases.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/store/__init__.py
+-rw-r--r--   0        0        0     1093 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/store/base.py
+-rw-r--r--   0        0        0     6191 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/store/store.py
+-rw-r--r--   0        0        0     1761 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/transfer.py
+-rw-r--r--   0        0        0        1 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/upload/__init__.py
+-rw-r--r--   0        0        0     5706 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/upload/base.py
+-rw-r--r--   0        0        0     5503 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/upload/clinical_delivery.py
+-rw-r--r--   0        0        0     1175 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/upload/coverage.py
+-rw-r--r--   0        0        0     1528 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/upload/delivery_report.py
+-rw-r--r--   0        0        0     4022 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/upload/fohm.py
+-rw-r--r--   0        0        0     1463 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/upload/genotype.py
+-rw-r--r--   0        0        0     1885 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/upload/gens.py
+-rw-r--r--   0        0        0      584 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/upload/gisaid.py
+-rw-r--r--   0        0        0     2645 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/upload/mutacc.py
+-rw-r--r--   0        0        0       23 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/upload/nipt/__init__.py
+-rw-r--r--   0        0        0     3006 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/upload/nipt/base.py
+-rw-r--r--   0        0        0     2275 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/upload/nipt/ftp.py
+-rw-r--r--   0        0        0     1596 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/upload/nipt/statina.py
+-rw-r--r--   0        0        0      112 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/upload/observations/__init__.py
+-rw-r--r--   0        0        0     2672 2024-04-25 07:10:48.509212 cg-60.3.2/cg/cli/upload/observations/observations.py
+-rw-r--r--   0        0        0     2904 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/upload/observations/utils.py
+-rw-r--r--   0        0        0     9970 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/upload/scout.py
+-rw-r--r--   0        0        0      650 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/upload/utils.py
+-rw-r--r--   0        0        0     1667 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/upload/validate.py
+-rw-r--r--   0        0        0      105 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/utils.py
+-rw-r--r--   0        0        0       18 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/balsamic/__init__.py
+-rw-r--r--   0        0        0     8925 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/balsamic/base.py
+-rw-r--r--   0        0        0     1980 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/balsamic/options.py
+-rw-r--r--   0        0        0      881 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/balsamic/pon.py
+-rw-r--r--   0        0        0     1162 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/balsamic/qc.py
+-rw-r--r--   0        0        0     1177 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/balsamic/umi.py
+-rw-r--r--   0        0        0     1342 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/base.py
+-rw-r--r--   0        0        0    12379 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/commands.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/fastq/__init__.py
+-rw-r--r--   0        0        0     1367 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/fastq/base.py
+-rw-r--r--   0        0        0     1787 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/fastq/fastq_service.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0        0        0     4177 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/fluffy/base.py
+-rw-r--r--   0        0        0       22 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/jasen/__init__.py
+-rw-r--r--   0        0        0      535 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/jasen/base.py
+-rw-r--r--   0        0        0       22 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/microsalt/__init__.py
+-rw-r--r--   0        0        0     7810 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/microsalt/base.py
+-rw-r--r--   0        0        0       22 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/mip/__init__.py
+-rw-r--r--   0        0        0     6596 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/mip/base.py
+-rw-r--r--   0        0        0     1268 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/mip/options.py
+-rw-r--r--   0        0        0       22 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/mip_dna/__init__.py
+-rw-r--r--   0        0        0     1013 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/mip_dna/base.py
+-rw-r--r--   0        0        0       22 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/mip_rna/__init__.py
+-rw-r--r--   0        0        0      916 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/mip_rna/base.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/mutant/__init__.py
+-rw-r--r--   0        0        0     3413 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/mutant/base.py
+-rw-r--r--   0        0        0     9002 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/nf_analysis.py
+-rw-r--r--   0        0        0       22 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/raredisease/__init__.py
+-rw-r--r--   0        0        0     2210 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/raredisease/base.py
+-rw-r--r--   0        0        0       22 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/rnafusion/__init__.py
+-rw-r--r--   0        0        0     1179 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/rnafusion/base.py
+-rw-r--r--   0        0        0       22 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/taxprofiler/__init__.py
+-rw-r--r--   0        0        0     1211 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/taxprofiler/base.py
+-rw-r--r--   0        0        0     1111 2024-04-25 07:10:48.513212 cg-60.3.2/cg/cli/workflow/tomte/base.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.513212 cg-60.3.2/cg/clients/__init__.py
+-rw-r--r--   0        0        0     1363 2024-04-25 07:10:48.513212 cg-60.3.2/cg/clients/arnold/api.py
+-rw-r--r--   0        0        0      160 2024-04-25 07:10:48.513212 cg-60.3.2/cg/clients/arnold/dto/create_case_request.py
+-rw-r--r--   0        0        0      384 2024-04-25 07:10:48.513212 cg-60.3.2/cg/clients/arnold/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.513212 cg-60.3.2/cg/clients/janus/__init__.py
+-rw-r--r--   0        0        0     1246 2024-04-25 07:10:48.513212 cg-60.3.2/cg/clients/janus/api.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.513212 cg-60.3.2/cg/clients/janus/dto/__init__.py
+-rw-r--r--   0        0        0      503 2024-04-25 07:10:48.513212 cg-60.3.2/cg/clients/janus/dto/create_qc_metrics_request.py
+-rw-r--r--   0        0        0      420 2024-04-25 07:10:48.513212 cg-60.3.2/cg/clients/janus/exceptions.py
+-rw-r--r--   0        0        0      937 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/__init__.py
+-rw-r--r--   0        0        0      253 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/archiving.py
+-rw-r--r--   0        0        0       35 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/backup.py
+-rw-r--r--   0        0        0      769 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/bcl_convert_metrics.py
+-rw-r--r--   0        0        0      469 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/compression.py
+-rw-r--r--   0        0        0     6613 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/constants.py
+-rw-r--r--   0        0        0     6033 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/delivery.py
+-rw-r--r--   0        0        0     7387 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/demultiplexing.py
+-rw-r--r--   0        0        0     1422 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/encryption.py
+-rw-r--r--   0        0        0      372 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/extraction.py
+-rw-r--r--   0        0        0     2054 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/gene_panel.py
+-rw-r--r--   0        0        0     6704 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/housekeeper_tags.py
+-rw-r--r--   0        0        0       95 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/invoice.py
+-rw-r--r--   0        0        0     5815 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/lims.py
+-rw-r--r--   0        0        0      743 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/metrics.py
+-rw-r--r--   0        0        0      231 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/nanopore_files.py
+-rw-r--r--   0        0        0      650 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/nextflow.py
+-rw-r--r--   0        0        0     1529 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/nf_analysis.py
+-rw-r--r--   0        0        0       19 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/nipt.py
+-rw-r--r--   0        0        0     2257 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/observations.py
+-rw-r--r--   0        0        0     1216 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/orderforms.py
+-rw-r--r--   0        0        0       96 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/paths.py
+-rw-r--r--   0        0        0      266 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/pdc.py
+-rw-r--r--   0        0        0      160 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/pedigree.py
+-rw-r--r--   0        0        0     1044 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/priority.py
+-rw-r--r--   0        0        0       79 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/process.py
+-rw-r--r--   0        0        0     5474 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/report.py
+-rw-r--r--   0        0        0      485 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/sample_sources.py
+-rw-r--r--   0        0        0     3111 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/scout.py
+-rw-r--r--   0        0        0     1669 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/sequencing.py
+-rw-r--r--   0        0        0      313 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/slurm.py
+-rw-r--r--   0        0        0      529 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/subject.py
+-rw-r--r--   0        0        0       55 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/symbols.py
+-rw-r--r--   0        0        0      435 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/tb.py
+-rw-r--r--   0        0        0      161 2024-04-25 07:10:48.513212 cg-60.3.2/cg/constants/time.py
+-rw-r--r--   0        0        0     6639 2024-04-25 07:10:48.513212 cg-60.3.2/cg/exc.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.513212 cg-60.3.2/cg/io/__init__.py
+-rw-r--r--   0        0        0     1037 2024-04-25 07:10:48.513212 cg-60.3.2/cg/io/api.py
+-rw-r--r--   0        0        0      621 2024-04-25 07:10:48.513212 cg-60.3.2/cg/io/config.py
+-rw-r--r--   0        0        0     2978 2024-04-25 07:10:48.513212 cg-60.3.2/cg/io/controller.py
+-rw-r--r--   0        0        0     1763 2024-04-25 07:10:48.513212 cg-60.3.2/cg/io/csv.py
+-rw-r--r--   0        0        0      210 2024-04-25 07:10:48.513212 cg-60.3.2/cg/io/gzip.py
+-rw-r--r--   0        0        0      662 2024-04-25 07:10:48.513212 cg-60.3.2/cg/io/json.py
+-rw-r--r--   0        0        0      525 2024-04-25 07:10:48.513212 cg-60.3.2/cg/io/png.py
+-rw-r--r--   0        0        0     1094 2024-04-25 07:10:48.517212 cg-60.3.2/cg/io/txt.py
+-rw-r--r--   0        0        0      552 2024-04-25 07:10:48.517212 cg-60.3.2/cg/io/validate_path.py
+-rw-r--r--   0        0        0     1289 2024-04-25 07:10:48.517212 cg-60.3.2/cg/io/xml.py
+-rw-r--r--   0        0        0     1153 2024-04-25 07:10:48.517212 cg-60.3.2/cg/io/yaml.py
+-rw-r--r--   0        0        0      281 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/archive/__init__.py
+-rw-r--r--   0        0        0    15193 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/archive/archive.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/archive/ddn/__init__.py
+-rw-r--r--   0        0        0     1727 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/archive/ddn/constants.py
+-rw-r--r--   0        0        0    10852 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/archive/ddn/ddn_data_flow_client.py
+-rw-r--r--   0        0        0     3704 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/archive/ddn/models.py
+-rw-r--r--   0        0        0     1250 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/archive/ddn/utils.py
+-rw-r--r--   0        0        0     2024 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/archive/models.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/backup/__init__.py
+-rw-r--r--   0        0        0    17426 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/backup/backup.py
+-rw-r--r--   0        0        0     5397 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/backup/pdc.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/clean/__init__.py
+-rw-r--r--   0        0        0     3901 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/clean/api.py
+-rw-r--r--   0        0        0     7738 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/clean/clean_flow_cells.py
+-rw-r--r--   0        0        0     1841 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/clean/clean_retrieved_spring_files.py
+-rw-r--r--   0        0        0       34 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/compress/__init__.py
+-rw-r--r--   0        0        0    14557 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/compress/compress.py
+-rw-r--r--   0        0        0     4947 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/compress/files.py
+-rw-r--r--   0        0        0       77 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/deliver/__init__.py
+-rw-r--r--   0        0        0    14672 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/deliver/deliver.py
+-rw-r--r--   0        0        0     4502 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/deliver/deliver_ticket.py
+-rw-r--r--   0        0        0      904 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/deliver/fastq_path_generator.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/delivery/__init__.py
+-rw-r--r--   0        0        0     8255 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/delivery/delivery.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/demultiplex/__init__.py
+-rw-r--r--   0        0        0     2592 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/demultiplex/combine_sequencing_metrics.py
+-rw-r--r--   0        0        0     5719 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/demultiplex/demux_post_processing.py
+-rw-r--r--   0        0        0     4135 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/demultiplex/files.py
+-rw-r--r--   0        0        0     7777 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/demultiplex/housekeeper_storage_functions.py
+-rw-r--r--   0        0        0     6126 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/demultiplex/status_db_storage_functions.py
+-rw-r--r--   0        0        0    10690 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/demultiplex/utils.py
+-rw-r--r--   0        0        0     2855 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/demultiplex/validation.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/encryption/__init__.py
+-rw-r--r--   0        0        0    20271 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/encryption/encryption.py
+-rw-r--r--   0        0        0      537 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/encryption/sbatch.py
+-rw-r--r--   0        0        0    10922 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/invoice.py
+-rw-r--r--   0        0        0     2360 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/meta.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/observations/__init__.py
+-rw-r--r--   0        0        0     6008 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/observations/balsamic_observations_api.py
+-rw-r--r--   0        0        0     5277 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/observations/mip_dna_observations_api.py
+-rw-r--r--   0        0        0     5364 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/observations/observations_api.py
+-rw-r--r--   0        0        0       27 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/orders/__init__.py
+-rw-r--r--   0        0        0     3637 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/orders/api.py
+-rw-r--r--   0        0        0      121 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/orders/balsamic_qc_submitter.py
+-rw-r--r--   0        0        0      107 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/orders/balsamic_submitter.py
+-rw-r--r--   0        0        0      122 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/orders/balsamic_umi_submitter.py
+-rw-r--r--   0        0        0    15262 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/orders/case_submitter.py
+-rw-r--r--   0        0        0     6102 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/orders/fastq_submitter.py
+-rw-r--r--   0        0        0      105 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/orders/fluffy_submitter.py
+-rw-r--r--   0        0        0     1254 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/orders/lims.py
+-rw-r--r--   0        0        0     5782 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/orders/metagenome_submitter.py
+-rw-r--r--   0        0        0     6337 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/orders/microbial_submitter.py
+-rw-r--r--   0        0        0      123 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/orders/microsalt_submitter.py
+-rw-r--r--   0        0        0      105 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/orders/mip_dna_submitter.py
+-rw-r--r--   0        0        0      105 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/orders/mip_rna_submitter.py
+-rw-r--r--   0        0        0     7761 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/orders/pool_submitter.py
+-rw-r--r--   0        0        0      102 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/orders/rml_submitter.py
+-rw-r--r--   0        0        0      718 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/orders/rnafusion_submitter.py
+-rw-r--r--   0        0        0     1268 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/orders/sars_cov_2_submitter.py
+-rw-r--r--   0        0        0     1754 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/orders/submitter.py
+-rw-r--r--   0        0        0     7880 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/orders/ticket_handler.py
+-rw-r--r--   0        0        0     4105 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/qc_metrics/collect_qc_metrics.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/report/__init__.py
+-rw-r--r--   0        0        0     8168 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/report/balsamic.py
+-rw-r--r--   0        0        0      562 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/report/balsamic_qc.py
+-rw-r--r--   0        0        0      717 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/report/balsamic_umi.py
+-rw-r--r--   0        0        0     4171 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/report/field_validators.py
+-rw-r--r--   0        0        0     6620 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/report/mip_dna.py
+-rw-r--r--   0        0        0    18606 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/report/report_api.py
+-rw-r--r--   0        0        0     5625 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/report/rnafusion.py
+-rw-r--r--   0        0        0     1911 2024-04-25 07:10:48.517212 cg-60.3.2/cg/meta/report/templates/delivery-report.html
+-rw-r--r--   0        0        0     4236 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/report/templates/macros/data_analysis/data_analysis.html
+-rw-r--r--   0        0        0     1049 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/report/templates/macros/data_analysis/limitations.html
+-rw-r--r--   0        0        0     3351 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html
+-rw-r--r--   0        0        0     1364 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html
+-rw-r--r--   0        0        0      753 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html
+-rw-r--r--   0        0        0     3284 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html
+-rw-r--r--   0        0        0     3670 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html
+-rw-r--r--   0        0        0     2332 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/report/templates/macros/header.html
+-rw-r--r--   0        0        0     2066 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/report/templates/macros/order.html
+-rw-r--r--   0        0        0     2243 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/report/templates/macros/sample_prep.html
+-rw-r--r--   0        0        0      472 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/report/templates/macros/ticket_system.html
+-rw-r--r--   0        0        0     1165 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html
+-rw-r--r--   0        0        0     1538 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html
+-rw-r--r--   0        0        0      428 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/report/templates/macros/uploaded_files/rnafusion_uploaded_files.html
+-rw-r--r--   0        0        0     4266 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html
+-rw-r--r--   0        0        0       80 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/report/templates/partials/footer.html
+-rw-r--r--   0        0        0      172 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/report/templates/partials/signature.html
+-rw-r--r--   0        0        0   232803 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/report/templates/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0       33 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/report/templates/static/css/custom.css
+-rw-r--r--   0        0        0    30068 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/report/templates/static/images/SWEDAC_logo.png
+-rw-r--r--   0        0        0     3925 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/report/tomte.py
+-rw-r--r--   0        0        0       32 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/rsync/__init__.py
+-rw-r--r--   0        0        0    12291 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/rsync/rsync_api.py
+-rw-r--r--   0        0        0      387 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/rsync/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/tar/__init__.py
+-rw-r--r--   0        0        0     1694 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/tar/tar.py
+-rw-r--r--   0        0        0       71 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/transfer/__init__.py
+-rw-r--r--   0        0        0    10016 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/transfer/external_data.py
+-rw-r--r--   0        0        0     5814 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/transfer/lims.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/balsamic/__init__.py
+-rw-r--r--   0        0        0     3107 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/balsamic/balsamic.py
+-rw-r--r--   0        0        0     2224 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/coverage.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/fohm/__init__.py
+-rw-r--r--   0        0        0    12102 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/fohm/fohm.py
+-rw-r--r--   0        0        0       30 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/gisaid/__init__.py
+-rw-r--r--   0        0        0      928 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/gisaid/constants.py
+-rw-r--r--   0        0        0    13521 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/gisaid/gisaid.py
+-rw-r--r--   0        0        0     3312 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/gisaid/models.py
+-rw-r--r--   0        0        0     5310 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/gt.py
+-rw-r--r--   0        0        0      898 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/microsalt/microsalt_upload_api.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/mip/__init__.py
+-rw-r--r--   0        0        0     2546 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/mip/mip_dna.py
+-rw-r--r--   0        0        0     1400 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/mip/mip_rna.py
+-rw-r--r--   0        0        0     7294 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/mutacc.py
+-rw-r--r--   0        0        0     1853 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/nf_analysis.py
+-rw-r--r--   0        0        0       32 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/nipt/__init__.py
+-rw-r--r--   0        0        0      696 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/nipt/models.py
+-rw-r--r--   0        0        0     8106 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/nipt/nipt.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/scout/__init__.py
+-rw-r--r--   0        0        0     4009 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/scout/balsamic_config_builder.py
+-rw-r--r--   0        0        0     1491 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/scout/balsamic_umi_config_builder.py
+-rw-r--r--   0        0        0     3322 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/scout/hk_tags.py
+-rw-r--r--   0        0        0     9103 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/scout/mip_config_builder.py
+-rw-r--r--   0        0        0     3495 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/scout/rnafusion_config_builder.py
+-rw-r--r--   0        0        0     7231 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/scout/scout_config_builder.py
+-rw-r--r--   0        0        0    23146 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/scout/uploadscoutapi.py
+-rw-r--r--   0        0        0     3197 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/upload/upload_api.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.521211 cg-60.3.2/cg/meta/workflow/__init__.py
+-rw-r--r--   0        0        0    28043 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/analysis.py
+-rw-r--r--   0        0        0    28188 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/balsamic.py
+-rw-r--r--   0        0        0     2700 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/balsamic_pon.py
+-rw-r--r--   0        0        0      553 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/balsamic_qc.py
+-rw-r--r--   0        0        0      556 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/balsamic_umi.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/downsample/__init__.py
+-rw-r--r--   0        0        0     3922 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/downsample/downsample.py
+-rw-r--r--   0        0        0      711 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/downsample/sbatch.py
+-rw-r--r--   0        0        0     8913 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/fastq.py
+-rw-r--r--   0        0        0    10687 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/fluffy.py
+-rw-r--r--   0        0        0      521 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/jasen.py
+-rw-r--r--   0        0        0       70 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/microsalt/__init__.py
+-rw-r--r--   0        0        0      116 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/microsalt/constants.py
+-rw-r--r--   0        0        0      174 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/microsalt/metrics_parser/__init__.py
+-rw-r--r--   0        0        0      366 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/microsalt/metrics_parser/metrics_parser.py
+-rw-r--r--   0        0        0      903 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/microsalt/metrics_parser/models.py
+-rw-r--r--   0        0        0    13062 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/microsalt/microsalt.py
+-rw-r--r--   0        0        0       95 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/microsalt/quality_controller/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/microsalt/quality_controller/models.py
+-rw-r--r--   0        0        0     5688 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/microsalt/quality_controller/quality_controller.py
+-rw-r--r--   0        0        0     1217 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/microsalt/quality_controller/report_generator.py
+-rw-r--r--   0        0        0     2373 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/microsalt/quality_controller/result_logger.py
+-rw-r--r--   0        0        0     5641 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/microsalt/quality_controller/utils.py
+-rw-r--r--   0        0        0     1220 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/microsalt/utils.py
+-rw-r--r--   0        0        0    13924 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/mip.py
+-rw-r--r--   0        0        0     2991 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/mip_dna.py
+-rw-r--r--   0        0        0     2167 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/mip_rna.py
+-rw-r--r--   0        0        0    10587 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/mutant.py
+-rw-r--r--   0        0        0    35481 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/nf_analysis.py
+-rw-r--r--   0        0        0     6161 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/nf_handlers.py
+-rw-r--r--   0        0        0     6394 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/prepare_fastq.py
+-rw-r--r--   0        0        0     5988 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/raredisease.py
+-rw-r--r--   0        0        0     5214 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/rnafusion.py
+-rw-r--r--   0        0        0     4607 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/taxprofiler.py
+-rw-r--r--   0        0        0     3204 2024-04-25 07:10:48.525211 cg-60.3.2/cg/meta/workflow/tomte.py
+-rw-r--r--   0        0        0      113 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/__init__.py
+-rw-r--r--   0        0        0      367 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/analysis.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/balsamic/__init__.py
+-rw-r--r--   0        0        0      459 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/balsamic/analysis.py
+-rw-r--r--   0        0        0     4550 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/balsamic/config.py
+-rw-r--r--   0        0        0     1986 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/balsamic/metrics.py
+-rw-r--r--   0        0        0    17539 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/cg_config.py
+-rw-r--r--   0        0        0     4302 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/compression_data.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/deliverables/__init__.py
+-rw-r--r--   0        0        0     5213 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/deliverables/metric_deliverables.py
+-rw-r--r--   0        0        0      243 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/delivery/delivery.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/demultiplex/__init__.py
+-rw-r--r--   0        0        0    12040 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/demultiplex/run_parameters.py
+-rw-r--r--   0        0        0      539 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/demultiplex/sbatch.py
+-rw-r--r--   0        0        0     7006 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/downsample/downsample_data.py
+-rw-r--r--   0        0        0      255 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/email.py
+-rw-r--r--   0        0        0     1046 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/fastq.py
+-rw-r--r--   0        0        0     2157 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/file_data.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/flow_cell/__init__.py
+-rw-r--r--   0        0        0     9984 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/flow_cell/flow_cell.py
+-rw-r--r--   0        0        0      317 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/flow_cell/utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/invoice/__init__.py
+-rw-r--r--   0        0        0     1254 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/invoice/invoice.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/lims/__init__.py
+-rw-r--r--   0        0        0     2019 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/lims/sample.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/mip/__init__.py
+-rw-r--r--   0        0        0      337 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/mip/mip_analysis.py
+-rw-r--r--   0        0        0     1564 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/mip/mip_config.py
+-rw-r--r--   0        0        0     4696 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/mip/mip_metrics_deliverables.py
+-rw-r--r--   0        0        0     2550 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/mip/mip_sample_info.py
+-rw-r--r--   0        0        0     2472 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/nf_analysis.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/observations/__init__.py
+-rw-r--r--   0        0        0      688 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/observations/input_files.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/orders/__init__.py
+-rw-r--r--   0        0        0     2659 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/orders/constants.py
+-rw-r--r--   0        0        0     5604 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/orders/excel_sample.py
+-rw-r--r--   0        0        0      898 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/orders/json_sample.py
+-rw-r--r--   0        0        0     1449 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/orders/order.py
+-rw-r--r--   0        0        0      811 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/orders/orderform_schema.py
+-rw-r--r--   0        0        0     4212 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/orders/sample_base.py
+-rw-r--r--   0        0        0     9668 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/orders/samples.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/orders/validators/__init__.py
+-rw-r--r--   0        0        0     2300 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/orders/validators/excel_sample_validators.py
+-rw-r--r--   0        0        0      576 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/orders/validators/json_sample_validators.py
+-rw-r--r--   0        0        0       71 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/orders/validators/sample_base_validators.py
+-rw-r--r--   0        0        0      101 2024-04-25 07:10:48.525211 cg-60.3.2/cg/models/qc_metrics.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.529212 cg-60.3.2/cg/models/raredisease/__init__.py
+-rw-r--r--   0        0        0     1875 2024-04-25 07:10:48.529212 cg-60.3.2/cg/models/raredisease/raredisease.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.529212 cg-60.3.2/cg/models/report/__init__.py
+-rw-r--r--   0        0        0     7461 2024-04-25 07:10:48.529212 cg-60.3.2/cg/models/report/metadata.py
+-rw-r--r--   0        0        0     6180 2024-04-25 07:10:48.529212 cg-60.3.2/cg/models/report/report.py
+-rw-r--r--   0        0        0     5221 2024-04-25 07:10:48.529212 cg-60.3.2/cg/models/report/sample.py
+-rw-r--r--   0        0        0     3004 2024-04-25 07:10:48.529212 cg-60.3.2/cg/models/report/validators.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.529212 cg-60.3.2/cg/models/rnafusion/__init__.py
+-rw-r--r--   0        0        0     1865 2024-04-25 07:10:48.529212 cg-60.3.2/cg/models/rnafusion/rnafusion.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.529212 cg-60.3.2/cg/models/scout/__init__.py
+-rw-r--r--   0        0        0     4783 2024-04-25 07:10:48.529212 cg-60.3.2/cg/models/scout/scout_load_config.py
+-rw-r--r--   0        0        0      116 2024-04-25 07:10:48.529212 cg-60.3.2/cg/models/scout/validators.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.529212 cg-60.3.2/cg/models/slurm/__init__.py
+-rw-r--r--   0        0        0      617 2024-04-25 07:10:48.529212 cg-60.3.2/cg/models/slurm/sbatch.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.529212 cg-60.3.2/cg/models/taxprofiler/__init__.py
+-rw-r--r--   0        0        0     2443 2024-04-25 07:10:48.529212 cg-60.3.2/cg/models/taxprofiler/taxprofiler.py
+-rw-r--r--   0        0        0     1774 2024-04-25 07:10:48.529212 cg-60.3.2/cg/models/tomte/tomte.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.529212 cg-60.3.2/cg/models/workflow/__init__.py
+-rw-r--r--   0        0        0      685 2024-04-25 07:10:48.529212 cg-60.3.2/cg/models/workflow/mutant.py
+-rw-r--r--   0        0        0       70 2024-04-25 07:10:48.529212 cg-60.3.2/cg/models/workflow/validators.py
+-rw-r--r--   0        0        0      842 2024-04-25 07:10:48.529212 cg-60.3.2/cg/resources/__init__.py
+-rw-r--r--   0        0        0     3493 2024-04-25 07:10:48.529212 cg-60.3.2/cg/resources/rnafusion_bundle_filenames.yaml
+-rw-r--r--   0        0        0     2434 2024-04-25 07:10:48.529212 cg-60.3.2/cg/resources/taxprofiler_bundle_filenames.yaml
+-rw-r--r--   0        0        0     3732 2024-04-25 07:10:48.529212 cg-60.3.2/cg/resources/tomte_bundle_filenames.yaml
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/__init__.py
+-rw-r--r--   0        0        0    20241 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/admin.py
+-rw-r--r--   0        0        0    22743 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/api.py
+-rw-r--r--   0        0        0     4887 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/app.py
+-rw-r--r--   0        0        0       48 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/auto.py
+-rw-r--r--   0        0        0     1184 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/config.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/dto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/dto/delivery_message/__init__.py
+-rw-r--r--   0        0        0      300 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/dto/delivery_message/delivery_message_request.py
+-rw-r--r--   0        0        0      183 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/dto/delivery_message/delivery_message_response.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/dto/orders/__init__.py
+-rw-r--r--   0        0        0      165 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/dto/orders/order_delivery_update_request.py
+-rw-r--r--   0        0        0       91 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/dto/orders/order_patch_request.py
+-rw-r--r--   0        0        0      662 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/dto/orders/orders_request.py
+-rw-r--r--   0        0        0      413 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/dto/orders/orders_response.py
+-rw-r--r--   0        0        0     2598 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/ext.py
+-rw-r--r--   0        0        0       29 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/invoices/__init__.py
+-rw-r--r--   0        0        0     4793 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/invoices/templates/invoices/index.html
+-rw-r--r--   0        0        0     8171 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/invoices/templates/invoices/invoice.html
+-rw-r--r--   0        0        0     2838 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/invoices/templates/invoices/layout.html
+-rw-r--r--   0        0        0     4956 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/invoices/templates/invoices/new.html
+-rw-r--r--   0        0        0     7708 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/invoices/views.py
+-rw-r--r--   0        0        0      354 2024-04-25 07:10:48.529212 cg-60.3.2/cg/server/templates/admin/index.html
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/analysis_service/__init__.py
+-rw-r--r--   0        0        0      482 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/analysis_service/analysis_service.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/delivery_message/__init__.py
+-rw-r--r--   0        0        0     2531 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/delivery_message/delivery_message_service.py
+-rw-r--r--   0        0        0      792 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/delivery_message/messages/__init__.py
+-rw-r--r--   0        0        0     1366 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/delivery_message/messages/analysis_scout_message.py
+-rw-r--r--   0        0        0      791 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/delivery_message/messages/covid_message.py
+-rw-r--r--   0        0        0      189 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/delivery_message/messages/delivery_message.py
+-rw-r--r--   0        0        0     1391 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/delivery_message/messages/fastq_analysis_scout_message.py
+-rw-r--r--   0        0        0      535 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/delivery_message/messages/fastq_message.py
+-rw-r--r--   0        0        0     1358 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/delivery_message/messages/fastq_scout_message.py
+-rw-r--r--   0        0        0      604 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/delivery_message/messages/microsalt_mwr_message.py
+-rw-r--r--   0        0        0      592 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/delivery_message/messages/microsalt_mwx_message.py
+-rw-r--r--   0        0        0      903 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/delivery_message/messages/scout_message.py
+-rw-r--r--   0        0        0      512 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/delivery_message/messages/statina_message.py
+-rw-r--r--   0        0        0      779 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/delivery_message/messages/utils.py
+-rw-r--r--   0        0        0     3300 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/delivery_message/utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/fastq_file_service/__init__.py
+-rw-r--r--   0        0        0      101 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/fastq_file_service/exceptions.py
+-rw-r--r--   0        0        0     1092 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/fastq_file_service/fastq_file_service.py
+-rw-r--r--   0        0        0     2991 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/fastq_file_service/utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/orders/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/orders/order_service/__init__.py
+-rw-r--r--   0        0        0     2684 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/orders/order_service/order_service.py
+-rw-r--r--   0        0        0     1214 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/orders/order_service/utils.py
+-rw-r--r--   0        0        0       94 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/orders/order_status_service/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/orders/order_status_service/dto/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/orders/order_status_service/dto/case_summary.py
+-rw-r--r--   0        0        0      289 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/orders/order_status_service/dto/order_summary.py
+-rw-r--r--   0        0        0     1768 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/orders/order_status_service/order_summary_service.py
+-rw-r--r--   0        0        0     1737 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/orders/order_status_service/utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/slurm_service/__init__.py
+-rw-r--r--   0        0        0      703 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/slurm_service/slurm_cli_service.py
+-rw-r--r--   0        0        0      242 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/slurm_service/slurm_service.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/slurm_upload_service/__init__.py
+-rw-r--r--   0        0        0      175 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/slurm_upload_service/slurm_upload_config.py
+-rw-r--r--   0        0        0     2074 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/slurm_upload_service/slurm_upload_service.py
+-rw-r--r--   0        0        0      203 2024-04-25 07:10:48.529212 cg-60.3.2/cg/services/slurm_upload_service/utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.529212 cg-60.3.2/cg/store/__init__.py
+-rw-r--r--   0        0        0     4650 2024-04-25 07:10:48.529212 cg-60.3.2/cg/store/base.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.529212 cg-60.3.2/cg/store/crud/__init__.py
+-rw-r--r--   0        0        0    13100 2024-04-25 07:10:48.529212 cg-60.3.2/cg/store/crud/create.py
+-rw-r--r--   0        0        0     2144 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/crud/delete.py
+-rw-r--r--   0        0        0    60188 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/crud/read.py
+-rw-r--r--   0        0        0     1121 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/crud/update.py
+-rw-r--r--   0        0        0     1662 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/database.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/filters/__init__.py
+-rw-r--r--   0        0        0     5371 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/filters/status_analysis_filters.py
+-rw-r--r--   0        0        0     1712 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/filters/status_application_filters.py
+-rw-r--r--   0        0        0     1440 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/filters/status_application_limitations_filters.py
+-rw-r--r--   0        0        0     2523 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/filters/status_application_version_filters.py
+-rw-r--r--   0        0        0     1390 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/filters/status_bed_filters.py
+-rw-r--r--   0        0        0     1317 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/filters/status_bed_version_filters.py
+-rw-r--r--   0        0        0    10787 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/filters/status_case_filters.py
+-rw-r--r--   0        0        0     3272 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/filters/status_case_sample_filters.py
+-rw-r--r--   0        0        0      903 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/filters/status_collaboration_filters.py
+-rw-r--r--   0        0        0     1412 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/filters/status_customer_filters.py
+-rw-r--r--   0        0        0     1880 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/filters/status_flow_cell_filters.py
+-rw-r--r--   0        0        0     1255 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/filters/status_invoice_filters.py
+-rw-r--r--   0        0        0     2792 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/filters/status_metrics_filters.py
+-rw-r--r--   0        0        0     3225 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/filters/status_order_filters.py
+-rw-r--r--   0        0        0      851 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/filters/status_organism_filters.py
+-rw-r--r--   0        0        0      783 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/filters/status_panel_filters.py
+-rw-r--r--   0        0        0     3923 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/filters/status_pool_filters.py
+-rw-r--r--   0        0        0     8660 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/filters/status_sample_filters.py
+-rw-r--r--   0        0        0      731 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/filters/status_user_filters.py
+-rw-r--r--   0        0        0    36844 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/models.py
+-rw-r--r--   0        0        0      593 2024-04-25 07:10:48.533212 cg-60.3.2/cg/store/store.py
+-rw-r--r--   0        0        0       30 2024-04-25 07:10:48.533212 cg-60.3.2/cg/utils/__init__.py
+-rw-r--r--   0        0        0      187 2024-04-25 07:10:48.533212 cg-60.3.2/cg/utils/calculations.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.533212 cg-60.3.2/cg/utils/checksum/__init__.py
+-rw-r--r--   0        0        0     1579 2024-04-25 07:10:48.533212 cg-60.3.2/cg/utils/checksum/checksum.py
+-rw-r--r--   0        0        0     1655 2024-04-25 07:10:48.533212 cg-60.3.2/cg/utils/click/EnumChoice.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.533212 cg-60.3.2/cg/utils/click/__init__.py
+-rw-r--r--   0        0        0     4910 2024-04-25 07:10:48.533212 cg-60.3.2/cg/utils/commands.py
+-rw-r--r--   0        0        0     1811 2024-04-25 07:10:48.533212 cg-60.3.2/cg/utils/date.py
+-rw-r--r--   0        0        0      635 2024-04-25 07:10:48.533212 cg-60.3.2/cg/utils/dict.py
+-rw-r--r--   0        0        0     2111 2024-04-25 07:10:48.533212 cg-60.3.2/cg/utils/dispatcher.py
+-rw-r--r--   0        0        0     1251 2024-04-25 07:10:48.533212 cg-60.3.2/cg/utils/email.py
+-rw-r--r--   0        0        0      134 2024-04-25 07:10:48.533212 cg-60.3.2/cg/utils/enums.py
+-rw-r--r--   0        0        0     3178 2024-04-25 07:10:48.533212 cg-60.3.2/cg/utils/files.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.533212 cg-60.3.2/cg/utils/flask/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-25 07:10:48.533212 cg-60.3.2/cg/utils/flask/enum.py
+-rw-r--r--   0        0        0      233 2024-04-25 07:10:48.533212 cg-60.3.2/cg/utils/flow_cell.py
+-rw-r--r--   0        0        0      834 2024-04-25 07:10:48.533212 cg-60.3.2/cg/utils/time.py
+-rw-r--r--   0        0        0     1224 2024-04-25 07:10:48.533212 cg-60.3.2/cg/utils/utils.py
+-rw-r--r--   0        0        0     1697 2024-04-25 07:10:48.537212 cg-60.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.537212 cg-60.3.2/tests/__init__.py
+-rw-r--r--   0        0        0     1158 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/conftest.py
+-rw-r--r--   0        0        0      231 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/coverage/conftest.py
+-rw-r--r--   0        0        0     6188 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/coverage/test_coverage.py
+-rw-r--r--   0        0        0     1693 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/crunchy/conftest.py
+-rw-r--r--   0        0        0     5438 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/crunchy/test_compress_fastq.py
+-rw-r--r--   0        0        0     2283 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/crunchy/test_config.py
+-rw-r--r--   0        0        0    14032 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/crunchy/test_crunchy.py
+-rw-r--r--   0        0        0     9109 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/crunchy/test_spring_decompression.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/demultiplex/__init__.py
+-rw-r--r--   0        0        0     4994 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/demultiplex/conftest.py
+-rw-r--r--   0        0        0     4010 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0        0        0     7986 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/demultiplex/test_demultiplex_api.py
+-rw-r--r--   0        0        0     4782 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/demultiplex/test_index.py
+-rw-r--r--   0        0        0     9468 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/demultiplex/test_override_cycles_validator.py
+-rw-r--r--   0        0        0     4042 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/demultiplex/test_read_sample_sheet.py
+-rw-r--r--   0        0        0    12389 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/demultiplex/test_sample_models.py
+-rw-r--r--   0        0        0      951 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/demultiplex/test_sample_sheet_creator.py
+-rw-r--r--   0        0        0     3175 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/demultiplex/test_sample_sheet_models.py
+-rw-r--r--   0        0        0    10932 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/demultiplex/test_sample_sheet_validator.py
+-rw-r--r--   0        0        0     4896 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/demultiplex/test_translate_sample_sheet.py
+-rw-r--r--   0        0        0     1450 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/demultiplex/test_validate.py
+-rw-r--r--   0        0        0     5094 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/downsample/test_downsample.py
+-rw-r--r--   0        0        0     1419 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/downsample/test_downsample_utils.py
+-rw-r--r--   0        0        0     1716 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/gens/test_gens_api.py
+-rw-r--r--   0        0        0     1950 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/gt/conftest.py
+-rw-r--r--   0        0        0     4276 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/gt/test_gt_api.py
+-rw-r--r--   0        0        0     1453 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/hk/conftest.py
+-rw-r--r--   0        0        0      684 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/hk/test__getattr__.py
+-rw-r--r--   0        0        0     1593 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/hk/test_add_file.py
+-rw-r--r--   0        0        0     3523 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/hk/test_bundles.py
+-rw-r--r--   0        0        0      871 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/hk/test_core.py
+-rw-r--r--   0        0        0    31172 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/hk/test_file.py
+-rw-r--r--   0        0        0     5080 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/hk/test_version.py
+-rw-r--r--   0        0        0     1840 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/lims/conftest.py
+-rw-r--r--   0        0        0     3197 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/lims/test_api.py
+-rw-r--r--   0        0        0     1451 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/lims/test_sample_sheet.py
+-rw-r--r--   0        0        0     9223 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/loqus/conftest.py
+-rw-r--r--   0        0        0     8994 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/loqus/test_loqusdb_api.py
+-rw-r--r--   0        0        0     2439 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/madeline/conftest.py
+-rw-r--r--   0        0        0     4653 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/madeline/test_madeline.py
+-rw-r--r--   0        0        0     3328 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/mip/conftest.py
+-rw-r--r--   0        0        0     2487 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/mip/test_config_mip.py
+-rw-r--r--   0        0        0      883 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/mutacc_auto/conftest.py
+-rw-r--r--   0        0        0     2473 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/mutacc_auto/test_mutacc_auto.py
+-rw-r--r--   0        0        0    11930 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/orderform/conftest.py
+-rw-r--r--   0        0        0     9484 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/orderform/test_excel_orderform_parser.py
+-rw-r--r--   0        0        0     4351 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/orderform/test_excel_sample_schema.py
+-rw-r--r--   0        0        0     1032 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/orderform/test_json_orderform_parser.py
+-rw-r--r--   0        0        0     2474 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/orderform/test_orderform_parser.py
+-rw-r--r--   0        0        0    16002 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/orderform/validators/test_excel_sample_validators.py
+-rw-r--r--   0        0        0     3670 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/scout/conftest.py
+-rw-r--r--   0        0        0     2269 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/scout/test_get_causative_variants.py
+-rw-r--r--   0        0        0     1376 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/scout/test_get_scout_cases.py
+-rw-r--r--   0        0        0     1840 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/scout/test_scout_load_config.py
+-rw-r--r--   0        0        0     7047 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/scout/test_scout_models.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0        0        0     2639 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/sequencing_metrics_parser/conftest.py
+-rw-r--r--   0        0        0     7069 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
+-rw-r--r--   0        0        0     2958 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/sequencing_metrics_parser/parsers/test_sequencing_metrics_parser_api.py
+-rw-r--r--   0        0        0     1131 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/slurm/conftest.py
+-rw-r--r--   0        0        0     4412 2024-04-25 07:10:48.537212 cg-60.3.2/tests/apps/slurm/test_slurm_api.py
+-rw-r--r--   0        0        0      831 2024-04-25 07:10:48.541211 cg-60.3.2/tests/apps/test_apps_environ.py
+-rw-r--r--   0        0        0      957 2024-04-25 07:10:48.541211 cg-60.3.2/tests/apps/test_osticket.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/add/__init__.py
+-rw-r--r--   0        0        0     1174 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/add/test_cli_add.py
+-rw-r--r--   0        0        0     2471 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/add/test_cli_add_customer.py
+-rw-r--r--   0        0        0     6841 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/add/test_cli_add_family.py
+-rw-r--r--   0        0        0     7588 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/add/test_cli_add_relationship.py
+-rw-r--r--   0        0        0     8382 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/add/test_cli_add_sample.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/backup/__init__.py
+-rw-r--r--   0        0        0      705 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/backup/conftest.py
+-rw-r--r--   0        0        0    11101 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/backup/test_backup_command.py
+-rw-r--r--   0        0        0     6865 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/clean/conftest.py
+-rw-r--r--   0        0        0     5536 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/clean/test_balsamic_clean.py
+-rw-r--r--   0        0        0     2557 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/clean/test_clean_flow_cell.py
+-rw-r--r--   0        0        0     1830 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/clean/test_clean_hk_bundle_files.py
+-rw-r--r--   0        0        0     2098 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/clean/test_hk_bundle_files.py
+-rw-r--r--   0        0        0     4610 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/clean/test_hk_case_bundle_files.py
+-rw-r--r--   0        0        0     3585 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/clean/test_microbial_clean.py
+-rw-r--r--   0        0        0     1881 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/clean/test_rsync_past_run_dirs.py
+-rw-r--r--   0        0        0     9707 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/compress/conftest.py
+-rw-r--r--   0        0        0     7709 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/compress/test_cli_compress_fastq.py
+-rw-r--r--   0        0        0     1416 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/compress/test_cli_decompress_spring.py
+-rw-r--r--   0        0        0     5205 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/compress/test_compress_helpers.py
+-rw-r--r--   0        0        0     1239 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/compress/test_store_fastq.py
+-rw-r--r--   0        0        0     7558 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/conftest.py
+-rw-r--r--   0        0        0    12747 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/delete/test_cli_delete_case.py
+-rw-r--r--   0        0        0     1873 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/delete/test_cli_delete_cases.py
+-rw-r--r--   0        0        0     3794 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/deliver/conftest.py
+-rw-r--r--   0        0        0     4428 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/deliver/test_deliver_base.py
+-rw-r--r--   0        0        0     1166 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/deliver/test_rsync_base.py
+-rw-r--r--   0        0        0     8569 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/deliver/test_run_deliver_cmd.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/demultiplex/__init__.py
+-rw-r--r--   0        0        0     5109 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0        0        0     4773 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/demultiplex/test_demultiplex_flowcell.py
+-rw-r--r--   0        0        0     1607 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/demultiplex/test_finish_demux.py
+-rw-r--r--   0        0        0     2989 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/demultiplex/test_validate_sample_sheet.py
+-rw-r--r--   0        0        0     4423 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/demultiplex/test_verify_syncing.py
+-rw-r--r--   0        0        0     1585 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/downsample/test_cli_downsample.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/generate/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/generate/report/__init__.py
+-rw-r--r--   0        0        0     1622 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/generate/report/conftest.py
+-rw-r--r--   0        0        0     2477 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/generate/report/test_cli_delivery_report.py
+-rw-r--r--   0        0        0     2760 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/generate/report/test_utils.py
+-rw-r--r--   0        0        0      563 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/generate/test_cli_base.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/get/__init__.py
+-rw-r--r--   0        0        0      863 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/get/test_cli_get.py
+-rw-r--r--   0        0        0     1526 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/get/test_cli_get_analysis.py
+-rw-r--r--   0        0        0     1242 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/get/test_cli_get_case.py
+-rw-r--r--   0        0        0     6208 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/get/test_cli_get_flow_cell.py
+-rw-r--r--   0        0        0     8835 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/get/test_cli_get_sample.py
+-rw-r--r--   0        0        0     1364 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/set/conftest.py
+-rw-r--r--   0        0        0     7311 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/set/test_cli_set_case.py
+-rw-r--r--   0        0        0     1460 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/set/test_cli_set_cases.py
+-rw-r--r--   0        0        0     2016 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/set/test_cli_set_flowcell.py
+-rw-r--r--   0        0        0     1685 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/set/test_cli_set_list_keys.py
+-rw-r--r--   0        0        0    12450 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/set/test_cli_set_sample.py
+-rw-r--r--   0        0        0     6124 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/set/test_cli_set_samples.py
+-rw-r--r--   0        0        0     7015 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/store/test_store.py
+-rw-r--r--   0        0        0     2332 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/test_base.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/upload/__init__.py
+-rw-r--r--   0        0        0    10057 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/upload/conftest.py
+-rw-r--r--   0        0        0     2295 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/upload/test_cli_scout.py
+-rw-r--r--   0        0        0     1789 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/upload/test_cli_upload.py
+-rw-r--r--   0        0        0      971 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/upload/test_cli_upload_auto.py
+-rw-r--r--   0        0        0     1669 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/upload/test_cli_upload_delivery_report.py
+-rw-r--r--   0        0        0      895 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/upload/test_cli_upload_fastq.py
+-rw-r--r--   0        0        0     1199 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/upload/test_cli_upload_genotype.py
+-rw-r--r--   0        0        0      694 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/upload/test_cli_upload_gens.py
+-rw-r--r--   0        0        0     9965 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/upload/test_cli_upload_nipt.py
+-rw-r--r--   0        0        0     4684 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/upload/test_cli_upload_nipt_ftp.py
+-rw-r--r--   0        0        0     1839 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/upload/test_cli_upload_nipt_statina.py
+-rw-r--r--   0        0        0     6177 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/upload/test_cli_upload_observations.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/workflow/__init__.py
+-rw-r--r--   0        0        0    30612 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/workflow/balsamic/conftest.py
+-rw-r--r--   0        0        0    13938 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
+-rw-r--r--   0        0        0     7957 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/workflow/balsamic/test_compound_commands.py
+-rw-r--r--   0        0        0     2336 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/workflow/balsamic/test_link.py
+-rw-r--r--   0        0        0     3554 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/workflow/balsamic/test_report_deliver.py
+-rw-r--r--   0        0        0     6209 2024-04-25 07:10:48.541211 cg-60.3.2/tests/cli/workflow/balsamic/test_run.py
+-rw-r--r--   0        0        0     6934 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/balsamic/test_store_housekeeper.py
+-rw-r--r--   0        0        0     8458 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/fastq/__init__.py
+-rw-r--r--   0        0        0     2298 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/fastq/test_fastq_base.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0        0        0     5237 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/fluffy/conftest.py
+-rw-r--r--   0        0        0     5687 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
+-rw-r--r--   0        0        0     3302 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/fluffy/test_cli_link.py
+-rw-r--r--   0        0        0     1896 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/fluffy/test_cli_run.py
+-rw-r--r--   0        0        0     2968 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/fluffy/test_cli_start.py
+-rw-r--r--   0        0        0     7815 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/fluffy/test_cli_store.py
+-rw-r--r--   0        0        0     2775 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/microsalt/conftest.py
+-rw-r--r--   0        0        0     6926 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/microsalt/test_microsalt_case_config.py
+-rw-r--r--   0        0        0     1000 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/microsalt/test_microsalt_run.py
+-rw-r--r--   0        0        0     6544 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/mip/conftest.py
+-rw-r--r--   0        0        0     7011 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/mip/test_cli_mip_base.py
+-rw-r--r--   0        0        0     1542 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
+-rw-r--r--   0        0        0      431 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/mip/test_cli_mip_dna_link.py
+-rw-r--r--   0        0        0     2108 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py
+-rw-r--r--   0        0        0     1273 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
+-rw-r--r--   0        0        0     3595 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/mip/test_cli_mip_dna_run.py
+-rw-r--r--   0        0        0     3884 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/mip/test_cli_mip_dna_start.py
+-rw-r--r--   0        0        0     1004 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
+-rw-r--r--   0        0        0      527 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/mip/test_cli_mip_rna_link.py
+-rw-r--r--   0        0        0      716 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/mip/test_cli_mip_rna_run.py
+-rw-r--r--   0        0        0     8559 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/mip/test_cli_mip_store.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/nf_analysis/__init__.py
+-rw-r--r--   0        0        0     7365 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/nf_analysis/test_cli_config_case.py
+-rw-r--r--   0        0        0     3831 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py
+-rw-r--r--   0        0        0     5087 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py
+-rw-r--r--   0        0        0     9211 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/nf_analysis/test_cli_run.py
+-rw-r--r--   0        0        0     2994 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/nf_analysis/test_cli_start.py
+-rw-r--r--   0        0        0     9877 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/nf_analysis/test_cli_store.py
+-rw-r--r--   0        0        0    10373 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py
+-rw-r--r--   0        0        0      978 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/raredisease/__init__.py
+-rw-r--r--   0        0        0     3940 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py
+-rw-r--r--   0        0        0      921 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/test_cli_workflow.py
+-rw-r--r--   0        0        0     4310 2024-04-25 07:10:48.545211 cg-60.3.2/tests/cli/workflow/test_cli_workflow_clean.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/clients/arnold/__init__.py
+-rw-r--r--   0        0        0     1080 2024-04-25 07:10:48.545211 cg-60.3.2/tests/clients/arnold/conftest.py
+-rw-r--r--   0        0        0     1503 2024-04-25 07:10:48.545211 cg-60.3.2/tests/clients/arnold/test_arnold_api_client.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/clients/janus/__init__.py
+-rw-r--r--   0        0        0     2381 2024-04-25 07:10:48.545211 cg-60.3.2/tests/clients/janus/conftest.py
+-rw-r--r--   0        0        0     1716 2024-04-25 07:10:48.545211 cg-60.3.2/tests/clients/janus/test_janus_api_client.py
+-rw-r--r--   0        0        0   132778 2024-04-25 07:10:48.545211 cg-60.3.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixture_plugins/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixture_plugins/delivery_fixtures/__init__.py
+-rw-r--r--   0        0        0     2653 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py
+-rw-r--r--   0        0        0     4972 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixture_plugins/delivery_fixtures/context_fixtures.py
+-rw-r--r--   0        0        0     1494 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixture_plugins/delivery_fixtures/path_fixtures.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixture_plugins/demultiplex_fixtures/__init__.py
+-rw-r--r--   0        0        0     4625 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py
+-rw-r--r--   0        0        0     3467 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py
+-rw-r--r--   0        0        0    19179 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py
+-rw-r--r--   0        0        0     3699 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py
+-rw-r--r--   0        0        0     6000 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py
+-rw-r--r--   0        0        0     8960 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py
+-rw-r--r--   0        0        0     1304 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixture_plugins/timestamp_fixtures.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
+-rw-r--r--   0        0        0    14644 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
+-rw-r--r--   0        0        0    15921 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixtures/analysis/mip/dna/ADM2.cram
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixtures/analysis/mip/dna/ADM3.cram
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixtures/analysis/mip/dna/adm1.cram
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixtures/analysis/mip/dna/adm1.mt.bam
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixtures/analysis/mip/dna/multiqc.html
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixtures/analysis/mip/dna/report.pdf
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixtures/analysis/mip/dna/smn.vcf
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixtures/analysis/mip/dna/snv.vcf
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixtures/analysis/mip/dna/snv_research.vcf
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixtures/analysis/mip/dna/str.vcf
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixtures/analysis/mip/dna/sv.vcf
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixtures/analysis/mip/dna/sv_research.vcf
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.545211 cg-60.3.2/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
+-rw-r--r--   0        0        0       70 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/analysis/nf-analysis/pipeline_params.config
+-rw-r--r--   0        0        0      195 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/analysis/nf-analysis/pipeline_resource_optimisation.config
+-rw-r--r--   0        0        0      195 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/analysis/nf-analysis/platform.config
+-rw-r--r--   0        0        0     8173 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/analysis/raredisease/multiqc_data.json
+-rw-r--r--   0        0        0    20005 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml
+-rw-r--r--   0        0        0     5497 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/analysis/rnafusion/multiqc_data.json
+-rw-r--r--   0        0        0    12499 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml
+-rw-r--r--   0        0        0     2873 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/analysis/sample_coverage.bed
+-rw-r--r--   0        0        0     6506 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/analysis/taxprofiler/multiqc_data.json
+-rw-r--r--   0        0        0    10513 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0     5771 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/analysis/tomte/multiqc_data.json
+-rw-r--r--   0        0        0    14859 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml
+-rw-r--r--   0        0        0    10961 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/balsamic/case/config.json
+-rw-r--r--   0        0        0     3465 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/balsamic/case/metadata.yml
+-rw-r--r--   0        0        0       63 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/balsamic/case/metadata_directory.yml
+-rw-r--r--   0        0        0      165 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
+-rw-r--r--   0        0        0     2705 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
+-rw-r--r--   0        0        0      692 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/crunchy/spring_metadata.json
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/ACC2655A1_S2_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0      412 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      484 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      658 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/SVE2648A1_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/demuxcomplete.txt
+-rw-r--r--   0        0        0     1757 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0        0        0        7 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0     6034 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0        0        0     1172 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0        0        0        7 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_1.fastq.gz
+-rw-r--r--   0        0        0        7 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_2.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13169A1_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/ACC13170A6_S2_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/BCLConvert/fastq/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0      288 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      361 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      414 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20231108_LH00188_0028_B22F52TLT3/demuxcomplete.txt
+-rw-r--r--   0        0        0      315 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      434 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0     8624 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml
+-rw-r--r--   0        0        0      568 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0      220 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      463 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      622 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0      345 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      650 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      896 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0      619 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A4_S2_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/ACC12642A7_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0      303 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      364 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      427 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230912_A00187_1009_AHK33MDRX3/demuxcomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0     4439 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0        0        0     1172 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0     5127 2024-04-25 07:10:48.549212 cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
+-rw-r--r--   0        0        0       43 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz
+-rw-r--r--   0        0        0       67 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz.md5
+-rw-r--r--   0        0        0   338370 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz
+-rw-r--r--   0        0        0       67 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz.md5
+-rw-r--r--   0        0        0   338349 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/CopyComplete.txt
+-rw-r--r--   0        0        0     2126 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json
+-rw-r--r--   0        0        0     1827 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json
+-rw-r--r--   0        0        0       90 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/README.txt
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAComplete.txt
+-rw-r--r--   0        0        0     6895 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml
+-rw-r--r--   0        0        0       37 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead1Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead2Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead3Complete.txt
+-rw-r--r--   0        0        0    24755 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml
+-rw-r--r--   0        0        0      692 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
+-rw-r--r--   0        0        0      724 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0       61 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SequencingComplete.txt
+-rw-r--r--   0        0        0     5775 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/CopyComplete.txt
+-rw-r--r--   0        0        0     2282 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json
+-rw-r--r--   0        0        0     1632 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json
+-rw-r--r--   0        0        0       75 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/README.txt
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAComplete.txt
+-rw-r--r--   0        0        0     6912 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml
+-rw-r--r--   0        0        0       36 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead1Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead2Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead3Complete.txt
+-rw-r--r--   0        0        0       36 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead4Complete.txt
+-rw-r--r--   0        0        0    24814 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml
+-rw-r--r--   0        0        0      814 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv
+-rw-r--r--   0        0        0      660 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0       61 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SequencingComplete.txt
+-rw-r--r--   0        0        0     5853 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/CopyComplete.txt
+-rw-r--r--   0        0        0    21848 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json
+-rw-r--r--   0        0        0    15512 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json
+-rw-r--r--   0        0        0       79 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/README.txt
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RTAComplete.txt
+-rw-r--r--   0        0        0      756 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml
+-rw-r--r--   0        0        0     4118 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv
+-rw-r--r--   0        0        0     1408 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0     5326 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/CopyComplete.txt
+-rw-r--r--   0        0        0    15041 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json
+-rw-r--r--   0        0        0    10649 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json
+-rw-r--r--   0        0        0       80 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/README.txt
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RTAComplete.txt
+-rw-r--r--   0        0        0      755 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml
+-rw-r--r--   0        0        0     2878 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv
+-rw-r--r--   0        0        0      928 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0     5359 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CopyComplete.txt
+-rw-r--r--   0        0        0    27887 2024-04-25 07:10:48.553212 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv
+-rw-r--r--   0        0        0   141870 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json
+-rwxr-xr-x   0        0        0   122682 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json
+-rw-r--r--   0        0        0      243 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/README.txt
+-rw-r--r--   0        0        0    28230 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTAComplete.txt
+-rw-r--r--   0        0        0    94426 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml
+-rw-r--r--   0        0        0     5819 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/SequenceComplete.txt
+-rw-r--r--   0        0        0     1757 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0        0        0     1757 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stdout
+-rw-r--r--   0        0        0       12 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/README.txt
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RTAComplete.txt
+-rw-r--r--   0        0        0     5945 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml
+-rw-r--r--   0        0        0      260 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/copycomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/demuxstarted.txt
+-rw-r--r--   0        0        0     1757 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0        0        0     1757 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout
+-rw-r--r--   0        0        0    47522 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json
+-rw-r--r--   0        0        0       12 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/README.txt
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0        0        0     6666 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0        0        0      254 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/copycomplete.txt
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/delivery.txt
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/demuxstarted.txt
+-rwxr-xr-x   0        0        0    47434 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CopyComplete.txt
+-rw-r--r--   0        0        0    10950 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv
+-rw-r--r--   0        0        0      225 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/Manifest.tsv
+-rw-r--r--   0        0        0       55 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/README.txt
+-rwxr-xr-x   0        0        0     2493 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg
+-rwxr-xr-x   0        0        0        1 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAComplete.txt
+-rwxr-xr-x   0        0        0        2 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAExited.txt
+-rwxr-xr-x   0        0        0      730 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml
+-rwxr-xr-x   0        0        0    79277 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml
+-rwxr-xr-x   0        0        0     2694 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
+-rw-r--r--   0        0        0    10950 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
+-rw-r--r--   0        0        0      619 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0        0        0       12 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/README.txt
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0        0        0      399 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CopyComplete.txt
+-rw-r--r--   0        0        0     4941 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv
+-rwxr-xr-x   0        0        0    20050 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stderr
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stdout
+-rw-r--r--   0        0        0      244 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/README.txt
+-rw-r--r--   0        0        0     6391 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTAComplete.txt
+-rw-r--r--   0        0        0    16428 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml
+-rw-r--r--   0        0        0     6728 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
+-rw-r--r--   0        0        0     5127 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SequenceComplete.txt
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/demuxstarted.txt
+-rw-r--r--   0        0        0      133 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/README.txt
+-rw-r--r--   0        0        0      724 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
+-rw-r--r--   0        0        0     5775 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
+-rw-r--r--   0        0        0      124 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/180509_D00450_0598_BHGYFNBCX2/README.txt
+-rw-r--r--   0        0        0      310 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/README.txt
+-rw-r--r--   0        0        0     5819 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
+-rw-r--r--   0        0        0      122 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/README.txt
+-rwxr-xr-x   0        0        0     2694 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
+-rw-r--r--   0        0        0      311 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/README.txt
+-rw-r--r--   0        0        0     6728 2024-04-25 07:10:48.557211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0        0        0      399 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
+-rw-r--r--   0        0        0      399 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_0.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_1.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/final_summary_PAS86456_72d9fceb_8a4fd683.txt
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_0.pod5
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_1.pod5
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_0.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_1.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/final_summary_PAS97781_595b5663_efc7f02e.txt
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_0.pod5
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_1.pod5
+-rw-r--r--   0        0        0   111989 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
+-rw-r--r--   0        0        0     5319 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml
+-rw-r--r--   0        0        0     5944 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
+-rwxr-xr-x   0        0        0     2603 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
+-rwxr-xr-x   0        0        0     2597 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml
+-rw-r--r--   0        0        0     5899 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
+-rw-r--r--   0        0        0     4941 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv
+-rw-r--r--   0        0        0    10950 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/spring/dummy_run_001.spring
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/spring/dummy_run_002.spring
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/demultiplexing/spring/dummy_spring_meta_data.json
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
+-rw-r--r--   0        0        0     5554 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/fluffy/SampleSheet.csv
+-rw-r--r--   0        0        0      901 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/fluffy/deliverables.yaml
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/fluffy/multiqc_report.html
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/fluffy/summary.csv
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/gt/yellowhog.bcf
+-rw-r--r--   0        0        0     5114 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/madeline/madeline.xml
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/mip/case_file.txt
+-rw-r--r--   0        0        0     3241 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0    21811 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/mip/dna/store/case_config.yaml
+-rw-r--r--   0        0        0    23364 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
+-rw-r--r--   0        0        0    37367 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
+-rw-r--r--   0        0        0       16 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
+-rw-r--r--   0        0        0       16 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0       16 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
+-rw-r--r--   0        0        0      123 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
+-rw-r--r--   0        0        0    62741 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
+-rw-r--r--   0        0        0    11242 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/mip/rna/case_config.yaml
+-rw-r--r--   0        0        0    12164 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
+-rw-r--r--   0        0        0     5231 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
+-rw-r--r--   0        0        0     9774 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/mip/rna/store/case_config.yaml
+-rw-r--r--   0        0        0     4624 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
+-rw-r--r--   0        0        0    13666 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/mip/sample_file.txt
+-rw-r--r--   0        0        0     1885 2024-04-25 07:10:48.561211 cg-60.3.2/tests/fixtures/apps/scout/643594.config.yaml
+-rw-r--r--   0        0        0     6027 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/apps/scout/case_export.json
+-rw-r--r--   0        0        0     9349 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/apps/scout/export_causatives.json
+-rw-r--r--   0        0        0     1315 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/apps/scout/none_case_export.json
+-rw-r--r--   0        0        0     3518 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/apps/scout/other_sex_case.json
+-rw-r--r--   0        0        0     8874 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/apps/scout/panel_export.bed
+-rw-r--r--   0        0        0     4169 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/apps/scout/panel_export.csv
+-rw-r--r--   0        0        0      619 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/SampleSheet.csv
+-rw-r--r--   0        0        0    63569 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0    42478 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0    69708 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0       42 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/apps/shipping/scout-deploy.yaml
+-rw-r--r--   0        0        0     1036 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/cgweb_orders/balsamic.json
+-rw-r--r--   0        0        0     1104 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/cgweb_orders/fastq.json
+-rw-r--r--   0        0        0     1313 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/cgweb_orders/metagenome.json
+-rw-r--r--   0        0        0     3038 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/cgweb_orders/microsalt.json
+-rw-r--r--   0        0        0     3705 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/cgweb_orders/mip.json
+-rw-r--r--   0        0        0     1364 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/cgweb_orders/mip_rna.json
+-rw-r--r--   0        0        0     2125 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/cgweb_orders/rml.json
+-rw-r--r--   0        0        0     1368 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/cgweb_orders/rnafusion.json
+-rw-r--r--   0        0        0     4684 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/cgweb_orders/sarscov2.json
+-rw-r--r--   0        0        0     5609 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/data/SampleSheet.csv
+-rw-r--r--   0        0        0      511 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/data/bcl_convert_sample_sheet.csv
+-rw-r--r--   0        0        0   258048 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/data/cgfixture.db
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/data/fastq.fastq.gz
+-rw-r--r--   0        0        0    49152 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/data/hkstore.db
+-rw-r--r--   0        0        0       73 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/data/yellowhog/pedigree.yaml
+-rw-r--r--   0        0        0       76 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/io/casava_five_parts.fastq.gz
+-rw-r--r--   0        0        0       90 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/io/casava_seven_parts.fastq.gz
+-rw-r--r--   0        0        0       96 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/io/casava_ten_parts.fastq.gz
+-rw-r--r--   0        0        0      153 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/io/example.csv
+-rw-r--r--   0        0        0       46 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/io/example.gz
+-rw-r--r--   0        0        0      147 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/io/example.tsv
+-rw-r--r--   0        0        0       20 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/io/example.txt
+-rw-r--r--   0        0        0       20 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/io/example2.txt
+-rw-r--r--   0        0        0      582 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/io/example_json.json
+-rw-r--r--   0        0        0      103 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/io/example_xml.xml
+-rw-r--r--   0        0        0       20 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/meta/qc_metrics/file_with_right_tags.json
+-rw-r--r--   0        0        0       20 2024-04-25 07:10:48.565211 cg-60.3.2/tests/fixtures/meta/qc_metrics/file_without_right_tags.json
+-rw-r--r--   0        0        0   156910 2024-04-25 07:10:48.569211 cg-60.3.2/tests/fixtures/orderforms/1508.30.balsamic.xlsx
+-rw-r--r--   0        0        0   156770 2024-04-25 07:10:48.569211 cg-60.3.2/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx
+-rw-r--r--   0        0        0   156737 2024-04-25 07:10:48.569211 cg-60.3.2/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx
+-rw-r--r--   0        0        0   156582 2024-04-25 07:10:48.569211 cg-60.3.2/tests/fixtures/orderforms/1508.30.fastq.xlsx
+-rw-r--r--   0        0        0   155627 2024-04-25 07:10:48.569211 cg-60.3.2/tests/fixtures/orderforms/1508.30.metagenome.xlsx
+-rw-r--r--   0        0        0   156850 2024-04-25 07:10:48.569211 cg-60.3.2/tests/fixtures/orderforms/1508.30.mip.xlsx
+-rw-r--r--   0        0        0   258580 2024-04-25 07:10:48.573212 cg-60.3.2/tests/fixtures/orderforms/1508.30.mip_rna.xlsx
+-rw-r--r--   0        0        0   258342 2024-04-25 07:10:48.573212 cg-60.3.2/tests/fixtures/orderforms/1508.30.rnafusion.xlsx
+-rw-r--r--   0        0        0    82677 2024-04-25 07:10:48.573212 cg-60.3.2/tests/fixtures/orderforms/1603.11.microbial.xlsx
+-rw-r--r--   0        0        0   149394 2024-04-25 07:10:48.573212 cg-60.3.2/tests/fixtures/orderforms/1604.17.rml.xlsx
+-rw-r--r--   0        0        0   223184 2024-04-25 07:10:48.573212 cg-60.3.2/tests/fixtures/orderforms/2184.9.sarscov2.xlsx
+-rw-r--r--   0        0        0    18639 2024-04-25 07:10:48.573212 cg-60.3.2/tests/fixtures/orderforms/NIPT-json.json
+-rw-r--r--   0        0        0     6052 2024-04-25 07:10:48.573212 cg-60.3.2/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
+-rw-r--r--   0        0        0     6611 2024-04-25 07:10:48.573212 cg-60.3.2/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
+-rw-r--r--   0        0        0     1417 2024-04-25 07:10:48.573212 cg-60.3.2/tests/fixtures/report/case_data.json
+-rw-r--r--   0        0        0     1109 2024-04-25 07:10:48.573212 cg-60.3.2/tests/fixtures/report/lims_exported_samples.json
+-rw-r--r--   0        0        0     1562 2024-04-25 07:10:48.573212 cg-60.3.2/tests/fixtures/report/lims_family.json
+-rw-r--r--   0        0        0     3296 2024-04-25 07:10:48.573212 cg-60.3.2/tests/io/conftest.py
+-rw-r--r--   0        0        0      431 2024-04-25 07:10:48.573212 cg-60.3.2/tests/io/test_io_config.py
+-rw-r--r--   0        0        0     8639 2024-04-25 07:10:48.573212 cg-60.3.2/tests/io/test_io_controller.py
+-rw-r--r--   0        0        0     3877 2024-04-25 07:10:48.573212 cg-60.3.2/tests/io/test_io_csv.py
+-rw-r--r--   0        0        0      482 2024-04-25 07:10:48.573212 cg-60.3.2/tests/io/test_io_gzip.py
+-rw-r--r--   0        0        0     1779 2024-04-25 07:10:48.573212 cg-60.3.2/tests/io/test_io_json.py
+-rw-r--r--   0        0        0     2914 2024-04-25 07:10:48.573212 cg-60.3.2/tests/io/test_io_txt.py
+-rw-r--r--   0        0        0     1027 2024-04-25 07:10:48.573212 cg-60.3.2/tests/io/test_io_xml.py
+-rw-r--r--   0        0        0     2131 2024-04-25 07:10:48.573212 cg-60.3.2/tests/io/test_io_yaml.py
+-rw-r--r--   0        0        0     1233 2024-04-25 07:10:48.573212 cg-60.3.2/tests/io/test_validate_path.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.573212 cg-60.3.2/tests/meta/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.573212 cg-60.3.2/tests/meta/archive/__init__.py
+-rw-r--r--   0        0        0    13131 2024-04-25 07:10:48.573212 cg-60.3.2/tests/meta/archive/conftest.py
+-rw-r--r--   0        0        0    16858 2024-04-25 07:10:48.573212 cg-60.3.2/tests/meta/archive/test_archive_api.py
+-rw-r--r--   0        0        0    10246 2024-04-25 07:10:48.573212 cg-60.3.2/tests/meta/archive/test_archive_cli.py
+-rw-r--r--   0        0        0    15766 2024-04-25 07:10:48.573212 cg-60.3.2/tests/meta/archive/test_archiving.py
+-rw-r--r--   0        0        0     3807 2024-04-25 07:10:48.573212 cg-60.3.2/tests/meta/backup/conftest.py
+-rw-r--r--   0        0        0    26368 2024-04-25 07:10:48.573212 cg-60.3.2/tests/meta/backup/test_meta_backup.py
+-rw-r--r--   0        0        0    10055 2024-04-25 07:10:48.573212 cg-60.3.2/tests/meta/backup/test_meta_pdc.py
+-rw-r--r--   0        0        0    12546 2024-04-25 07:10:48.573212 cg-60.3.2/tests/meta/clean/conftest.py
+-rw-r--r--   0        0        0    16944 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/clean/test_clean_flow_cells_api.py
+-rw-r--r--   0        0        0     2286 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/clean/test_clean_retrieved_spring_files.py
+-rw-r--r--   0        0        0     7691 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/compress/conftest.py
+-rw-r--r--   0        0        0     7961 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/compress/test_clean_fastq.py
+-rw-r--r--   0        0        0     1778 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/compress/test_compress_files.py
+-rw-r--r--   0        0        0     3644 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/compress/test_compress_meta_fastq.py
+-rw-r--r--   0        0        0     1180 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/compress/test_decompress_spring_meta.py
+-rw-r--r--   0        0        0     7013 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/compress/test_meta_compress_update_hk.py
+-rw-r--r--   0        0        0     8269 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/deliver/__init__.py
+-rw-r--r--   0        0        0     3471 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/deliver/conftest.py
+-rw-r--r--   0        0        0     5533 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/deliver/test_deliver_ticket.py
+-rw-r--r--   0        0        0    10277 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/deliver/test_delivery_api.py
+-rw-r--r--   0        0        0     1057 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/deliver/test_fastq_path_generator.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/delivery/__init__.py
+-rw-r--r--   0        0        0    16660 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/delivery/test_delivery_api.py
+-rw-r--r--   0        0        0     8874 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/demultiplex/conftest.py
+-rw-r--r--   0        0        0     5382 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/demultiplex/test_combine_sequencing_metrics.py
+-rw-r--r--   0        0        0     8339 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/demultiplex/test_demux_post_processing.py
+-rw-r--r--   0        0        0    12406 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/demultiplex/test_housekeeper_storage_functions.py
+-rw-r--r--   0        0        0     4392 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/demultiplex/test_status_db_storage_functions.py
+-rw-r--r--   0        0        0    22837 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/demultiplex/test_utils.py
+-rw-r--r--   0        0        0     6193 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/demultiplex/test_validation.py
+-rw-r--r--   0        0        0     4943 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/encryption/conftest.py
+-rw-r--r--   0        0        0    18133 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/encryption/test_encryption.py
+-rw-r--r--   0        0        0     3122 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/observations/conftest.py
+-rw-r--r--   0        0        0    16164 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/observations/test_meta_upload_observations.py
+-rw-r--r--   0        0        0     4974 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/orders/conftest.py
+-rw-r--r--   0        0        0     1749 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/orders/test_PoolSubmitter_validate_order.py
+-rw-r--r--   0        0        0     1470 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
+-rw-r--r--   0        0        0     1768 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/orders/test_SarsCov2Submitter_store_order.py
+-rw-r--r--   0        0        0     2032 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
+-rw-r--r--   0        0        0    19783 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/orders/test_meta_orders_api.py
+-rw-r--r--   0        0        0     7086 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/orders/test_meta_orders_lims.py
+-rw-r--r--   0        0        0    29515 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/orders/test_meta_orders_status.py
+-rw-r--r--   0        0        0     1677 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/orders/test_rnafusion_submitter.py
+-rw-r--r--   0        0        0     1068 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/orders/test_ticket_handler.py
+-rw-r--r--   0        0        0     4336 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/qc_metrics/conftest.py
+-rw-r--r--   0        0        0     1972 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/qc_metrics/test_collect_qc_metrics.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/report/__init__.py
+-rw-r--r--   0        0        0     6512 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/report/conftest.py
+-rw-r--r--   0        0        0      434 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/report/helper.py
+-rw-r--r--   0        0        0     2604 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/report/test_balsamic_api.py
+-rw-r--r--   0        0        0     4056 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/report/test_field_validators.py
+-rw-r--r--   0        0        0     2858 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/report/test_mip_dna_api.py
+-rw-r--r--   0        0        0    16042 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/report/test_report_api.py
+-rw-r--r--   0        0        0     1365 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/report/test_rnafusion_api.py
+-rw-r--r--   0        0        0     1250 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/report/test_tomte_api.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/rsync/__init__.py
+-rw-r--r--   0        0        0      916 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/rsync/conftest.py
+-rw-r--r--   0        0        0     9442 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/rsync/test_rsync.py
+-rw-r--r--   0        0        0     3147 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/test_invoice.py
+-rw-r--r--   0        0        0     1220 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/transfer/conftest.py
+-rw-r--r--   0        0        0     9892 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/transfer/test_external_data.py
+-rw-r--r--   0        0        0     4395 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/transfer/test_meta_transfer_lims.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/upload/__init__.py
+-rw-r--r--   0        0        0     2210 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/upload/balsamic/test_balsamic.py
+-rw-r--r--   0        0        0     4002 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/upload/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/upload/gisaid/__init__.py
+-rw-r--r--   0        0        0     2557 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/upload/gisaid/fixtures/four_samples.csv
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
+-rw-r--r--   0        0        0      211 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
+-rw-r--r--   0        0        0      371 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/upload/mutacc/__init__.py
+-rw-r--r--   0        0        0     3684 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/upload/mutacc/conftest.py
+-rw-r--r--   0        0        0     4188 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
+-rw-r--r--   0        0        0     1149 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/upload/nipt/conftest.py
+-rw-r--r--   0        0        0     1683 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/upload/nipt/test_models.py
+-rw-r--r--   0        0        0     1242 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/upload/nipt/test_nipt_upload_api.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/upload/scout/__init__.py
+-rw-r--r--   0        0        0    23954 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/upload/scout/conftest.py
+-rw-r--r--   0        0        0     4734 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/upload/scout/test_generate_load_config.py
+-rw-r--r--   0        0        0     4182 2024-04-25 07:10:48.577211 cg-60.3.2/tests/meta/upload/scout/test_meta_upload_scoutapi.py
+-rw-r--r--   0        0        0    33260 2024-04-25 07:10:48.581211 cg-60.3.2/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
+-rw-r--r--   0        0        0     7372 2024-04-25 07:10:48.581211 cg-60.3.2/tests/meta/upload/scout/test_scout_config_builder.py
+-rw-r--r--   0        0        0     2511 2024-04-25 07:10:48.581211 cg-60.3.2/tests/meta/upload/test_meta_upload_coverage.py
+-rw-r--r--   0        0        0     1473 2024-04-25 07:10:48.581211 cg-60.3.2/tests/meta/upload/test_upload_api.py
+-rw-r--r--   0        0        0     2547 2024-04-25 07:10:48.581211 cg-60.3.2/tests/meta/upload/test_upload_genotypes_api.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.581211 cg-60.3.2/tests/meta/workflow/__init__.py
+-rw-r--r--   0        0        0    10262 2024-04-25 07:10:48.581211 cg-60.3.2/tests/meta/workflow/conftest.py
+-rw-r--r--   0        0        0     3652 2024-04-25 07:10:48.581211 cg-60.3.2/tests/meta/workflow/microsalt/conftest.py
+-rw-r--r--   0        0        0      318 2024-04-25 07:10:48.581211 cg-60.3.2/tests/meta/workflow/microsalt/test_parsing_metrics.py
+-rw-r--r--   0        0        0     3714 2024-04-25 07:10:48.581211 cg-60.3.2/tests/meta/workflow/microsalt/test_quality_controller.py
+-rw-r--r--   0        0        0    14367 2024-04-25 07:10:48.581211 cg-60.3.2/tests/meta/workflow/microsalt/test_quality_controller_utils.py
+-rw-r--r--   0        0        0      825 2024-04-25 07:10:48.581211 cg-60.3.2/tests/meta/workflow/microsalt/test_report_generation.py
+-rw-r--r--   0        0        0    20848 2024-04-25 07:10:48.581211 cg-60.3.2/tests/meta/workflow/test_analysis.py
+-rw-r--r--   0        0        0     7934 2024-04-25 07:10:48.581211 cg-60.3.2/tests/meta/workflow/test_balsamic.py
+-rw-r--r--   0        0        0     3034 2024-04-25 07:10:48.581211 cg-60.3.2/tests/meta/workflow/test_fastq.py
+-rw-r--r--   0        0        0     1532 2024-04-25 07:10:48.581211 cg-60.3.2/tests/meta/workflow/test_microsalt.py
+-rw-r--r--   0        0        0     2721 2024-04-25 07:10:48.581211 cg-60.3.2/tests/meta/workflow/test_nf_analysis.py
+-rw-r--r--   0        0        0     7741 2024-04-25 07:10:48.581211 cg-60.3.2/tests/meta/workflow/test_prepare_fastq_api.py
+-rw-r--r--   0        0        0     1920 2024-04-25 07:10:48.581211 cg-60.3.2/tests/meta/workflow/test_raredisease.py
+-rw-r--r--   0        0        0     1674 2024-04-25 07:10:48.581211 cg-60.3.2/tests/meta/workflow/test_rnafusion.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.581211 cg-60.3.2/tests/mocks/__init__.py
+-rw-r--r--   0        0        0     1168 2024-04-25 07:10:48.581211 cg-60.3.2/tests/mocks/balsamic_analysis_mock.py
+-rw-r--r--   0        0        0     3500 2024-04-25 07:10:48.581211 cg-60.3.2/tests/mocks/crunchy.py
+-rw-r--r--   0        0        0    21778 2024-04-25 07:10:48.581211 cg-60.3.2/tests/mocks/hk_mock.py
+-rw-r--r--   0        0        0     4106 2024-04-25 07:10:48.581211 cg-60.3.2/tests/mocks/limsmock.py
+-rw-r--r--   0        0        0      572 2024-04-25 07:10:48.581211 cg-60.3.2/tests/mocks/madeline.py
+-rw-r--r--   0        0        0     1297 2024-04-25 07:10:48.581211 cg-60.3.2/tests/mocks/mip_analysis_mock.py
+-rw-r--r--   0        0        0     1525 2024-04-25 07:10:48.581211 cg-60.3.2/tests/mocks/osticket.py
+-rw-r--r--   0        0        0     3239 2024-04-25 07:10:48.581211 cg-60.3.2/tests/mocks/process_mock.py
+-rw-r--r--   0        0        0     4713 2024-04-25 07:10:48.581211 cg-60.3.2/tests/mocks/report.py
+-rw-r--r--   0        0        0     3915 2024-04-25 07:10:48.581211 cg-60.3.2/tests/mocks/scout.py
+-rw-r--r--   0        0        0      750 2024-04-25 07:10:48.581211 cg-60.3.2/tests/mocks/store_model.py
+-rw-r--r--   0        0        0     1532 2024-04-25 07:10:48.581211 cg-60.3.2/tests/mocks/tb_mock.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/balsamic/__init__.py
+-rw-r--r--   0        0        0     1194 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/balsamic/conftest.py
+-rw-r--r--   0        0        0     1030 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/balsamic/test_balsamic_analysis.py
+-rw-r--r--   0        0        0     1050 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/demultiplexing/__init__.py
+-rw-r--r--   0        0        0    11446 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/demultiplexing/test_run_parameters.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/downsample/__init__.py
+-rw-r--r--   0        0        0     2096 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/downsample/test_down_sample_meta_data.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/flow_cell/__init__.py
+-rw-r--r--   0        0        0     6659 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/flow_cell/test_flowcell_model.py
+-rw-r--r--   0        0        0     6637 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/mip/conftest.py
+-rw-r--r--   0        0        0     1239 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/mip/test_mip_analysis.py
+-rw-r--r--   0        0        0     2348 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/mip/test_mip_config.py
+-rw-r--r--   0        0        0     6392 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/mip/test_mip_metrics_deliverables.py
+-rw-r--r--   0        0        0     3959 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/mip/test_mip_sample_info.py
+-rw-r--r--   0        0        0     3314 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/nextflow/test_nextflow_deliver.py
+-rw-r--r--   0        0        0     1602 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/observations/conftest.py
+-rw-r--r--   0        0        0     2579 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/observations/test_observations_input_files.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/report/__init__.py
+-rw-r--r--   0        0        0     7327 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/report/test_validators.py
+-rw-r--r--   0        0        0     3855 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/rnafusion/test_rnafusion_sample.py
+-rw-r--r--   0        0        0     1374 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/test_cg_models.py
+-rw-r--r--   0        0        0      990 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/test_compression_data.py
+-rw-r--r--   0        0        0      729 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/test_fastq.py
+-rw-r--r--   0        0        0     2860 2024-04-25 07:10:48.581211 cg-60.3.2/tests/models/test_file_data.py
+-rw-r--r--   0        0        0     4539 2024-04-25 07:10:48.581211 cg-60.3.2/tests/server/conftest.py
+-rw-r--r--   0        0        0     3135 2024-04-25 07:10:48.581211 cg-60.3.2/tests/server/endpoints/test_delivery_message_endpoint.py
+-rw-r--r--   0        0        0     3239 2024-04-25 07:10:48.581211 cg-60.3.2/tests/server/endpoints/test_orders_endpoint.py
+-rw-r--r--   0        0        0      271 2024-04-25 07:10:48.581211 cg-60.3.2/tests/server/test_server_auto.py
+-rw-r--r--   0        0        0     1047 2024-04-25 07:10:48.581211 cg-60.3.2/tests/services/fastq_file_service/conftest.py
+-rw-r--r--   0        0        0     3634 2024-04-25 07:10:48.581211 cg-60.3.2/tests/services/fastq_file_service/test_fastq_file_service.py
+-rw-r--r--   0        0        0     4861 2024-04-25 07:10:48.581211 cg-60.3.2/tests/services/orders/order_status_service/conftest.py
+-rw-r--r--   0        0        0     2865 2024-04-25 07:10:48.581211 cg-60.3.2/tests/services/orders/order_status_service/test_order_summary_service.py
+-rw-r--r--   0        0        0      318 2024-04-25 07:10:48.581211 cg-60.3.2/tests/small_helpers.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.581211 cg-60.3.2/tests/store/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.581211 cg-60.3.2/tests/store/api/__init__.py
+-rw-r--r--   0        0        0     3032 2024-04-25 07:10:48.581211 cg-60.3.2/tests/store/api/conftest.py
+-rw-r--r--   0        0        0     1557 2024-04-25 07:10:48.581211 cg-60.3.2/tests/store/api/test_base.py
+-rw-r--r--   0        0        0    20096 2024-04-25 07:10:48.581211 cg-60.3.2/tests/store/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.581211 cg-60.3.2/tests/store/crud/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.581211 cg-60.3.2/tests/store/crud/add/__init__.py
+-rw-r--r--   0        0        0     1497 2024-04-25 07:10:48.581211 cg-60.3.2/tests/store/crud/add/test_store_add_application_version.py
+-rw-r--r--   0        0        0     3958 2024-04-25 07:10:48.581211 cg-60.3.2/tests/store/crud/add/test_store_add_base.py
+-rw-r--r--   0        0        0     2502 2024-04-25 07:10:48.581211 cg-60.3.2/tests/store/crud/add/test_store_add_customer.py
+-rw-r--r--   0        0        0     1704 2024-04-25 07:10:48.581211 cg-60.3.2/tests/store/crud/add/test_store_add_flow_celll.py
+-rw-r--r--   0        0        0    12290 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/crud/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/crud/delete/__init__.py
+-rw-r--r--   0        0        0     5611 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/crud/delete/test_delete.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/crud/read/__init__.py
+-rw-r--r--   0        0        0    57636 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/crud/read/test_read.py
+-rw-r--r--   0        0        0     5461 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/crud/read/test_read_analyses_to_clean.py
+-rw-r--r--   0        0        0     3553 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/crud/read/test_read_analyses_to_delivery_report.py
+-rw-r--r--   0        0        0    18463 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/crud/read/test_read_analysis.py
+-rw-r--r--   0        0        0     2743 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/crud/read/test_read_application_version.py
+-rw-r--r--   0        0        0     1105 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/crud/read/test_read_customer.py
+-rw-r--r--   0        0        0     1530 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/crud/read/test_read_pool.py
+-rw-r--r--   0        0        0    21503 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/crud/read/test_read_sample.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/crud/update/__init__.py
+-rw-r--r--   0        0        0      737 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/crud/update/test_update.py
+-rw-r--r--   0        0        0    11693 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/filters/test_status_analyses_filters.py
+-rw-r--r--   0        0        0     3397 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/filters/test_status_application_filters.py
+-rw-r--r--   0        0        0     2073 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/filters/test_status_application_limitations_filters.py
+-rw-r--r--   0        0        0    10452 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/filters/test_status_application_version_filters.py
+-rw-r--r--   0        0        0     2804 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/filters/test_status_bed_filters.py
+-rw-r--r--   0        0        0     2362 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/filters/test_status_bed_version_filters.py
+-rw-r--r--   0        0        0     3495 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/filters/test_status_case_sample_filters.py
+-rw-r--r--   0        0        0    39100 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/filters/test_status_cases_filters.py
+-rw-r--r--   0        0        0     1345 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/filters/test_status_collaboration_filters.py
+-rw-r--r--   0        0        0     2482 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/filters/test_status_customer_filters.py
+-rw-r--r--   0        0        0     5153 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/filters/test_status_flow_cell_filters.py
+-rw-r--r--   0        0        0     2226 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/filters/test_status_invoice_filters.py
+-rw-r--r--   0        0        0     5871 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/filters/test_status_metrics_filters.py
+-rw-r--r--   0        0        0     2404 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/filters/test_status_organism_filters.py
+-rw-r--r--   0        0        0     1804 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/filters/test_status_panel_filters.py
+-rw-r--r--   0        0        0     8720 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/filters/test_status_pool_filters.py
+-rw-r--r--   0        0        0    22875 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/filters/test_status_samples_filters.py
+-rw-r--r--   0        0        0     1576 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/filters/test_status_user_filters.py
+-rw-r--r--   0        0        0     2147 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/test_delivery.py
+-rw-r--r--   0        0        0     4127 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store/test_store_models.py
+-rw-r--r--   0        0        0    37040 2024-04-25 07:10:48.585211 cg-60.3.2/tests/store_helpers.py
+-rw-r--r--   0        0        0     4930 2024-04-25 07:10:48.585211 cg-60.3.2/tests/test_copy_novaseqx_flow_cell.py
+-rw-r--r--   0        0        0      911 2024-04-25 07:10:48.585211 cg-60.3.2/tests/test_store_helpers.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:10:48.585211 cg-60.3.2/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1754 2024-04-25 07:10:48.585211 cg-60.3.2/tests/utils/conftest.py
+-rw-r--r--   0        0        0      371 2024-04-25 07:10:48.585211 cg-60.3.2/tests/utils/test_calculations.py
+-rw-r--r--   0        0        0     2920 2024-04-25 07:10:48.585211 cg-60.3.2/tests/utils/test_commands.py
+-rw-r--r--   0        0        0      953 2024-04-25 07:10:48.585211 cg-60.3.2/tests/utils/test_date.py
+-rw-r--r--   0        0        0     1508 2024-04-25 07:10:48.585211 cg-60.3.2/tests/utils/test_dict.py
+-rw-r--r--   0        0        0     7154 2024-04-25 07:10:48.585211 cg-60.3.2/tests/utils/test_dispatcher.py
+-rw-r--r--   0        0        0     4100 2024-04-25 07:10:48.585211 cg-60.3.2/tests/utils/test_files.py
+-rw-r--r--   0        0        0     1170 2024-04-25 07:10:48.585211 cg-60.3.2/tests/utils/test_time.py
+-rw-r--r--   0        0        0     2366 2024-04-25 07:10:48.585211 cg-60.3.2/tests/utils/test_utils.py
+-rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 cg-60.3.2/PKG-INFO
```

### Comparing `cg-60.3.1/README.md` & `cg-60.3.2/README.md`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/coverage/api.py` & `cg-60.3.2/cg/apps/coverage/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/crunchy/crunchy.py` & `cg-60.3.2/cg/apps/crunchy/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/crunchy/files.py` & `cg-60.3.2/cg/apps/crunchy/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/crunchy/sbatch.py` & `cg-60.3.2/cg/apps/crunchy/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/demultiplex/demultiplex_api.py` & `cg-60.3.2/cg/apps/demultiplex/demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/demultiplex/sample_sheet/api.py` & `cg-60.3.2/cg/apps/demultiplex/sample_sheet/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     def set_force(self, force: bool) -> None:
         """Set force."""
         LOG.debug(f"Set force to {force}")
         self.force = force
 
     def _get_flow_cell(self, flow_cell_name: str) -> FlowCellDirectoryData:
         """
-        Return a flow cell given a path and the bcl converter.
+        Return a flow cell given a path.
         Raises:
             SampleSheetError: If the flow cell directory or the data it contains is not valid.
         """
         flow_cell_path: Path = Path(self.flow_cell_runs_dir, flow_cell_name)
         if not flow_cell_path.exists():
             message: str = f"Could not find flow cell {flow_cell_path}"
             LOG.warning(message)
```

### Comparing `cg-60.3.1/cg/apps/demultiplex/sample_sheet/index.py` & `cg-60.3.2/cg/apps/demultiplex/sample_sheet/index.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py` & `cg-60.3.2/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py` & `cg-60.3.2/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/demultiplex/sample_sheet/sample_models.py` & `cg-60.3.2/cg/apps/demultiplex/sample_sheet/sample_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py` & `cg-60.3.2/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py` & `cg-60.3.2/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py` & `cg-60.3.2/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/demultiplex/sample_sheet/validators.py` & `cg-60.3.2/cg/apps/demultiplex/sample_sheet/validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/demultiplex/sbatch.py` & `cg-60.3.2/cg/apps/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/downsample/downsample.py` & `cg-60.3.2/cg/apps/downsample/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/downsample/utils.py` & `cg-60.3.2/cg/apps/downsample/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/gens.py` & `cg-60.3.2/cg/apps/gens.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/gt.py` & `cg-60.3.2/cg/apps/gt.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/hermes/hermes_api.py` & `cg-60.3.2/cg/apps/hermes/hermes_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/hermes/models.py` & `cg-60.3.2/cg/apps/hermes/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/housekeeper/hk.py` & `cg-60.3.2/cg/apps/housekeeper/hk.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/invoice/render.py` & `cg-60.3.2/cg/apps/invoice/render.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/invoice/templates/KI_pool_invoice.xlsx` & `cg-60.3.2/cg/apps/invoice/templates/KI_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/invoice/templates/KI_sample_invoice.xlsx` & `cg-60.3.2/cg/apps/invoice/templates/KI_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/invoice/templates/KTH_pool_invoice.xlsx` & `cg-60.3.2/cg/apps/invoice/templates/KTH_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/invoice/templates/KTH_sample_invoice.xlsx` & `cg-60.3.2/cg/apps/invoice/templates/KTH_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/lims/api.py` & `cg-60.3.2/cg/apps/lims/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/lims/batch.py` & `cg-60.3.2/cg/apps/lims/batch.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/lims/order.py` & `cg-60.3.2/cg/apps/lims/order.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/lims/sample_sheet.py` & `cg-60.3.2/cg/apps/lims/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/loqus.py` & `cg-60.3.2/cg/apps/loqus.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/madeline/api.py` & `cg-60.3.2/cg/apps/madeline/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/mip/confighandler.py` & `cg-60.3.2/cg/apps/mip/confighandler.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/mutacc_auto.py` & `cg-60.3.2/cg/apps/mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/orderform/excel_orderform_parser.py` & `cg-60.3.2/cg/apps/orderform/excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/orderform/json_orderform_parser.py` & `cg-60.3.2/cg/apps/orderform/json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/orderform/orderform_parser.py` & `cg-60.3.2/cg/apps/orderform/orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/osticket.py` & `cg-60.3.2/cg/apps/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/scout/scout_export.py` & `cg-60.3.2/cg/apps/scout/scout_export.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/scout/scoutapi.py` & `cg-60.3.2/cg/apps/scout/scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/sequencing_metrics_parser/api.py` & `cg-60.3.2/cg/apps/sequencing_metrics_parser/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/sequencing_metrics_parser/models.py` & `cg-60.3.2/cg/apps/sequencing_metrics_parser/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/sequencing_metrics_parser/parser.py` & `cg-60.3.2/cg/apps/sequencing_metrics_parser/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             metrics_file_path=self.demux_metrics_path,
             metrics_model=DemuxMetrics,
         )
 
     def parse_metrics_file(
         self, metrics_file_path, metrics_model: Callable
     ) -> list[SequencingQualityMetrics | DemuxMetrics]:
-        """Parse specified BCL convert metrics file."""
+        """Parse specified metrics file."""
         LOG.info(f"Parsing BCLConvert metrics file: {metrics_file_path}")
         parsed_metrics: list[SequencingQualityMetrics | DemuxMetrics] = []
         metrics_content: list[dict] = ReadFile.get_content_from_file(
             file_format=FileFormat.CSV, file_path=metrics_file_path, read_to_dict=True
         )
         for sample_metrics_dict in metrics_content:
             parsed_metrics.append(metrics_model(**sample_metrics_dict))
```

### Comparing `cg-60.3.1/cg/apps/slurm/sbatch.py` & `cg-60.3.2/cg/apps/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/slurm/slurm_api.py` & `cg-60.3.2/cg/apps/slurm/slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/tb/api.py` & `cg-60.3.2/cg/apps/tb/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/apps/tb/models.py` & `cg-60.3.2/cg/apps/tb/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/add.py` & `cg-60.3.2/cg/cli/add.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/archive.py` & `cg-60.3.2/cg/cli/archive.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/backup.py` & `cg-60.3.2/cg/cli/backup.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/base.py` & `cg-60.3.2/cg/cli/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/clean.py` & `cg-60.3.2/cg/cli/clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/compress/base.py` & `cg-60.3.2/cg/cli/compress/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/compress/fastq.py` & `cg-60.3.2/cg/cli/compress/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/compress/helpers.py` & `cg-60.3.2/cg/cli/compress/helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/delete/base.py` & `cg-60.3.2/cg/cli/delete/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/delete/case.py` & `cg-60.3.2/cg/cli/delete/case.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/delete/cases.py` & `cg-60.3.2/cg/cli/delete/cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/delete/observations.py` & `cg-60.3.2/cg/cli/delete/observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/deliver/base.py` & `cg-60.3.2/cg/cli/deliver/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/demultiplex/base.py` & `cg-60.3.2/cg/cli/demultiplex/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py` & `cg-60.3.2/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/demultiplex/demux.py` & `cg-60.3.2/cg/cli/demultiplex/demux.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/demultiplex/finish.py` & `cg-60.3.2/cg/cli/demultiplex/finish.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/demultiplex/sample_sheet.py` & `cg-60.3.2/cg/cli/demultiplex/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/downsample.py` & `cg-60.3.2/cg/cli/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/generate/report/base.py` & `cg-60.3.2/cg/cli/generate/report/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/generate/report/options.py` & `cg-60.3.2/cg/cli/generate/report/options.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/generate/report/utils.py` & `cg-60.3.2/cg/cli/generate/report/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/get.py` & `cg-60.3.2/cg/cli/get.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/set/base.py` & `cg-60.3.2/cg/cli/set/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/set/case.py` & `cg-60.3.2/cg/cli/set/case.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/set/cases.py` & `cg-60.3.2/cg/cli/set/cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/store/base.py` & `cg-60.3.2/cg/cli/store/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/store/store.py` & `cg-60.3.2/cg/cli/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/transfer.py` & `cg-60.3.2/cg/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/upload/base.py` & `cg-60.3.2/cg/cli/upload/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/upload/clinical_delivery.py` & `cg-60.3.2/cg/cli/upload/clinical_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/upload/coverage.py` & `cg-60.3.2/cg/cli/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/upload/delivery_report.py` & `cg-60.3.2/cg/cli/upload/delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/upload/fohm.py` & `cg-60.3.2/cg/cli/upload/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/upload/genotype.py` & `cg-60.3.2/cg/cli/upload/genotype.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/upload/gens.py` & `cg-60.3.2/cg/cli/upload/gens.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/upload/gisaid.py` & `cg-60.3.2/cg/cli/upload/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/upload/mutacc.py` & `cg-60.3.2/cg/cli/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/upload/nipt/base.py` & `cg-60.3.2/cg/cli/upload/nipt/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/upload/nipt/ftp.py` & `cg-60.3.2/cg/cli/upload/nipt/ftp.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/upload/nipt/statina.py` & `cg-60.3.2/cg/cli/upload/nipt/statina.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/upload/observations/observations.py` & `cg-60.3.2/cg/cli/upload/observations/observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/upload/observations/utils.py` & `cg-60.3.2/cg/cli/upload/observations/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/upload/scout.py` & `cg-60.3.2/cg/cli/upload/scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/upload/utils.py` & `cg-60.3.2/cg/cli/upload/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/upload/validate.py` & `cg-60.3.2/cg/cli/upload/validate.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/workflow/balsamic/base.py` & `cg-60.3.2/cg/cli/workflow/balsamic/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/workflow/balsamic/options.py` & `cg-60.3.2/cg/cli/workflow/balsamic/options.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/workflow/balsamic/pon.py` & `cg-60.3.2/cg/cli/workflow/balsamic/pon.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/workflow/balsamic/qc.py` & `cg-60.3.2/cg/cli/workflow/balsamic/qc.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/workflow/balsamic/umi.py` & `cg-60.3.2/cg/cli/workflow/balsamic/umi.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/workflow/base.py` & `cg-60.3.2/cg/cli/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/workflow/commands.py` & `cg-60.3.2/cg/cli/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/workflow/fastq/base.py` & `cg-60.3.2/cg/cli/workflow/fastq/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/workflow/fastq/fastq_service.py` & `cg-60.3.2/cg/cli/workflow/fastq/fastq_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/workflow/fluffy/base.py` & `cg-60.3.2/cg/cli/workflow/fluffy/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/workflow/jasen/base.py` & `cg-60.3.2/cg/cli/workflow/jasen/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/workflow/microsalt/base.py` & `cg-60.3.2/cg/cli/workflow/microsalt/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/workflow/mip/base.py` & `cg-60.3.2/cg/cli/workflow/mip/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/workflow/mip/options.py` & `cg-60.3.2/cg/cli/workflow/mip/options.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/workflow/mip_dna/base.py` & `cg-60.3.2/cg/cli/workflow/mip_dna/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/workflow/mip_rna/base.py` & `cg-60.3.2/cg/cli/workflow/mip_rna/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/workflow/mutant/base.py` & `cg-60.3.2/cg/cli/workflow/mutant/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/workflow/nf_analysis.py` & `cg-60.3.2/cg/cli/workflow/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/workflow/raredisease/base.py` & `cg-60.3.2/cg/cli/workflow/raredisease/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/workflow/rnafusion/base.py` & `cg-60.3.2/cg/cli/workflow/rnafusion/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/workflow/taxprofiler/base.py` & `cg-60.3.2/cg/cli/workflow/taxprofiler/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/cli/workflow/tomte/base.py` & `cg-60.3.2/cg/cli/workflow/tomte/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/clients/arnold/api.py` & `cg-60.3.2/cg/clients/arnold/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/clients/janus/api.py` & `cg-60.3.2/cg/clients/janus/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/constants/__init__.py` & `cg-60.3.2/cg/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/constants/bcl_convert_metrics.py` & `cg-60.3.2/cg/constants/bcl_convert_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/constants/constants.py` & `cg-60.3.2/cg/constants/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/constants/delivery.py` & `cg-60.3.2/cg/constants/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/constants/demultiplexing.py` & `cg-60.3.2/cg/constants/demultiplexing.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 class DemultiplexingDirsAndFiles(StrEnum):
     """Demultiplexing related directories and files."""
 
     COPY_COMPLETE: str = "CopyComplete.txt"
     DELIVERY: str = "delivery.txt"
     DEMUX_STARTED: str = "demuxstarted.txt"
     DEMUX_COMPLETE: str = "demuxcomplete.txt"
-    HISEQ_X_COPY_COMPLETE: str = "copycomplete.txt"
-    HISEQ_X_TILE_DIR: str = "l1t11"
     RTACOMPLETE: str = "RTAComplete.txt"
     RUN_PARAMETERS_PASCAL_CASE: str = "RunParameters.xml"
     RUN_PARAMETERS_CAMEL_CASE: str = "runParameters.xml"
     SAMPLE_SHEET_FILE_NAME: str = "SampleSheet.csv"
     UNALIGNED_DIR_NAME: str = "Unaligned"
     QUEUED_FOR_POST_PROCESSING: str = "post_processing_queued.txt"
     ANALYSIS_COMPLETED: str = "Secondary_Analysis_Complete.txt"
@@ -81,30 +79,14 @@
         INDEX_2: str = "index2"
         SAMPLE_NAME: str = "SampleName"
         CONTROL: str = "Control"
         RECIPE: str = "Recipe"
         OPERATOR: str = "Operator"
         SAMPLE_PROJECT_BCL2FASTQ: str = "Project"
 
-        @classmethod
-        def column_names(cls) -> list[str]:
-            return [
-                cls.FLOW_CELL_ID,
-                cls.LANE,
-                cls.SAMPLE_INTERNAL_ID_BCL2FASTQ,
-                cls.SAMPLE_REFERENCE,
-                cls.INDEX_1,
-                cls.INDEX_2,
-                cls.SAMPLE_NAME,
-                cls.CONTROL,
-                cls.RECIPE,
-                cls.OPERATOR,
-                cls.SAMPLE_PROJECT_BCL2FASTQ,
-            ]
-
 
 class SampleSheetBCLConvertSections:
     """Class with all necessary constants for building a version 2 sample sheet."""
 
     class Header(StrEnum):
         HEADER: str = "[Header]"
         RUN_NAME: str = "RunName"
@@ -176,20 +158,16 @@
     FULL_8_INDEX: str = "I8;"
     IGNORED_10_INDEX: str = "N10;"
     IGNORED_8_INDEX: str = "N8;"
     INDEX_8_IGNORED_2: str = "I8N2;"
     INDEX_8_IGNORED_2_REVERSED: str = "N2I8;"
 
 
-BCL2FASTQ_METRICS_DIRECTORY_NAME: str = "Stats"
-BCL2FASTQ_METRICS_FILE_NAME: str = "Stats.json"
 CUSTOM_INDEX_TAIL = "NNNNNNNNN"
-DRAGEN_PASSED_FILTER_PCT: float = 100.00000
 FASTQ_FILE_SUFFIXES: list[str] = [".fastq", ".gz"]
-INDEX_CHECK: str = "indexcheck"
 UNDETERMINED: str = "Undetermined"
 
 NEW_NOVASEQ_CONTROL_SOFTWARE_VERSION: str = "1.7.0"
 NEW_NOVASEQ_REAGENT_KIT_VERSION: str = "1.5"
 
 FORWARD_INDEX_CYCLE_PATTERN: str = r"I(\d+)N(\d+)"
 REVERSE_INDEX_CYCLE_PATTERN: str = r"N(\d+)I(\d+)"
```

### Comparing `cg-60.3.1/cg/constants/encryption.py` & `cg-60.3.2/cg/constants/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/constants/gene_panel.py` & `cg-60.3.2/cg/constants/gene_panel.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/constants/housekeeper_tags.py` & `cg-60.3.2/cg/constants/housekeeper_tags.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/constants/lims.py` & `cg-60.3.2/cg/constants/lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/constants/metrics.py` & `cg-60.3.2/cg/constants/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/constants/nextflow.py` & `cg-60.3.2/cg/constants/nextflow.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/constants/nf_analysis.py` & `cg-60.3.2/cg/constants/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/constants/observations.py` & `cg-60.3.2/cg/constants/observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/constants/orderforms.py` & `cg-60.3.2/cg/constants/orderforms.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/constants/priority.py` & `cg-60.3.2/cg/constants/priority.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/constants/report.py` & `cg-60.3.2/cg/constants/report.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/constants/scout.py` & `cg-60.3.2/cg/constants/scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/constants/sequencing.py` & `cg-60.3.2/cg/constants/sequencing.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/constants/subject.py` & `cg-60.3.2/cg/constants/subject.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/exc.py` & `cg-60.3.2/cg/exc.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/io/api.py` & `cg-60.3.2/cg/io/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/io/config.py` & `cg-60.3.2/cg/io/config.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/io/controller.py` & `cg-60.3.2/cg/io/controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/io/csv.py` & `cg-60.3.2/cg/io/csv.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/io/json.py` & `cg-60.3.2/cg/io/json.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/io/png.py` & `cg-60.3.2/cg/io/png.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/io/txt.py` & `cg-60.3.2/cg/io/txt.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/io/validate_path.py` & `cg-60.3.2/cg/io/validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/io/xml.py` & `cg-60.3.2/cg/io/xml.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/io/yaml.py` & `cg-60.3.2/cg/io/yaml.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/archive/archive.py` & `cg-60.3.2/cg/meta/archive/archive.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/archive/ddn/constants.py` & `cg-60.3.2/cg/meta/archive/ddn/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/archive/ddn/ddn_data_flow_client.py` & `cg-60.3.2/cg/meta/archive/ddn/ddn_data_flow_client.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/archive/ddn/models.py` & `cg-60.3.2/cg/meta/archive/ddn/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/archive/ddn/utils.py` & `cg-60.3.2/cg/meta/archive/ddn/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/archive/models.py` & `cg-60.3.2/cg/meta/archive/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/backup/backup.py` & `cg-60.3.2/cg/meta/backup/backup.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/backup/pdc.py` & `cg-60.3.2/cg/meta/backup/pdc.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/clean/api.py` & `cg-60.3.2/cg/meta/clean/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/clean/clean_flow_cells.py` & `cg-60.3.2/cg/meta/clean/clean_flow_cells.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/clean/clean_retrieved_spring_files.py` & `cg-60.3.2/cg/meta/clean/clean_retrieved_spring_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/compress/compress.py` & `cg-60.3.2/cg/meta/compress/compress.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/compress/files.py` & `cg-60.3.2/cg/meta/compress/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/deliver/deliver.py` & `cg-60.3.2/cg/meta/deliver/deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/deliver/deliver_ticket.py` & `cg-60.3.2/cg/meta/deliver/deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/deliver/fastq_path_generator.py` & `cg-60.3.2/cg/meta/deliver/fastq_path_generator.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/delivery/delivery.py` & `cg-60.3.2/cg/meta/delivery/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/demultiplex/combine_sequencing_metrics.py` & `cg-60.3.2/cg/meta/demultiplex/combine_sequencing_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/demultiplex/demux_post_processing.py` & `cg-60.3.2/cg/meta/demultiplex/demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/demultiplex/files.py` & `cg-60.3.2/cg/meta/demultiplex/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/demultiplex/housekeeper_storage_functions.py` & `cg-60.3.2/cg/meta/demultiplex/housekeeper_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/demultiplex/status_db_storage_functions.py` & `cg-60.3.2/cg/meta/demultiplex/status_db_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/demultiplex/utils.py` & `cg-60.3.2/cg/meta/demultiplex/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/demultiplex/validation.py` & `cg-60.3.2/cg/meta/demultiplex/validation.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/encryption/encryption.py` & `cg-60.3.2/cg/meta/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/encryption/sbatch.py` & `cg-60.3.2/cg/meta/encryption/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/invoice.py` & `cg-60.3.2/cg/meta/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/meta.py` & `cg-60.3.2/cg/meta/meta.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/observations/balsamic_observations_api.py` & `cg-60.3.2/cg/meta/observations/balsamic_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/observations/mip_dna_observations_api.py` & `cg-60.3.2/cg/meta/observations/mip_dna_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/observations/observations_api.py` & `cg-60.3.2/cg/meta/observations/observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/orders/api.py` & `cg-60.3.2/cg/meta/orders/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/orders/case_submitter.py` & `cg-60.3.2/cg/meta/orders/case_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/orders/fastq_submitter.py` & `cg-60.3.2/cg/meta/orders/fastq_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/orders/lims.py` & `cg-60.3.2/cg/meta/orders/lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/orders/metagenome_submitter.py` & `cg-60.3.2/cg/meta/orders/metagenome_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/orders/microbial_submitter.py` & `cg-60.3.2/cg/meta/orders/microbial_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/orders/pool_submitter.py` & `cg-60.3.2/cg/meta/orders/pool_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/orders/rnafusion_submitter.py` & `cg-60.3.2/cg/meta/orders/rnafusion_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/orders/sars_cov_2_submitter.py` & `cg-60.3.2/cg/meta/orders/sars_cov_2_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/orders/submitter.py` & `cg-60.3.2/cg/meta/orders/submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/orders/ticket_handler.py` & `cg-60.3.2/cg/meta/orders/ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/qc_metrics/collect_qc_metrics.py` & `cg-60.3.2/cg/meta/qc_metrics/collect_qc_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/balsamic.py` & `cg-60.3.2/cg/meta/report/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/balsamic_qc.py` & `cg-60.3.2/cg/meta/report/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/balsamic_umi.py` & `cg-60.3.2/cg/meta/report/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/field_validators.py` & `cg-60.3.2/cg/meta/report/field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/mip_dna.py` & `cg-60.3.2/cg/meta/report/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/report_api.py` & `cg-60.3.2/cg/meta/report/report_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/rnafusion.py` & `cg-60.3.2/cg/meta/report/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/templates/delivery-report.html` & `cg-60.3.2/cg/meta/report/templates/delivery-report.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/templates/macros/data_analysis/data_analysis.html` & `cg-60.3.2/cg/meta/report/templates/macros/data_analysis/data_analysis.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/templates/macros/data_analysis/limitations.html` & `cg-60.3.2/cg/meta/report/templates/macros/data_analysis/limitations.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html` & `cg-60.3.2/cg/meta/report/templates/macros/data_analysis/qc_metrics/balsamic_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html` & `cg-60.3.2/cg/meta/report/templates/macros/data_analysis/qc_metrics/mip_dna_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html` & `cg-60.3.2/cg/meta/report/templates/macros/data_analysis/qc_metrics/qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html` & `cg-60.3.2/cg/meta/report/templates/macros/data_analysis/qc_metrics/rnafusion_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html` & `cg-60.3.2/cg/meta/report/templates/macros/data_analysis/qc_metrics/tomte_qc_metrics.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/templates/macros/header.html` & `cg-60.3.2/cg/meta/report/templates/macros/header.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/templates/macros/order.html` & `cg-60.3.2/cg/meta/report/templates/macros/order.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/templates/macros/sample_prep.html` & `cg-60.3.2/cg/meta/report/templates/macros/sample_prep.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html` & `cg-60.3.2/cg/meta/report/templates/macros/uploaded_files/balsamic_uploaded_files.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html` & `cg-60.3.2/cg/meta/report/templates/macros/uploaded_files/mip_dna_uploaded_files.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html` & `cg-60.3.2/cg/meta/report/templates/macros/uploaded_files/uploaded_files.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/templates/static/css/bootstrap.min.css` & `cg-60.3.2/cg/meta/report/templates/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/templates/static/images/SWEDAC_logo.png` & `cg-60.3.2/cg/meta/report/templates/static/images/SWEDAC_logo.png`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/report/tomte.py` & `cg-60.3.2/cg/meta/report/tomte.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/rsync/rsync_api.py` & `cg-60.3.2/cg/meta/rsync/rsync_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/tar/tar.py` & `cg-60.3.2/cg/meta/tar/tar.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/transfer/external_data.py` & `cg-60.3.2/cg/meta/transfer/external_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/transfer/lims.py` & `cg-60.3.2/cg/meta/transfer/lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/upload/balsamic/balsamic.py` & `cg-60.3.2/cg/meta/upload/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/upload/coverage.py` & `cg-60.3.2/cg/meta/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/upload/fohm/fohm.py` & `cg-60.3.2/cg/meta/upload/fohm/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/upload/gisaid/constants.py` & `cg-60.3.2/cg/meta/upload/gisaid/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/upload/gisaid/gisaid.py` & `cg-60.3.2/cg/meta/upload/gisaid/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/upload/gisaid/models.py` & `cg-60.3.2/cg/meta/upload/gisaid/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/upload/gt.py` & `cg-60.3.2/cg/meta/upload/gt.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/upload/microsalt/microsalt_upload_api.py` & `cg-60.3.2/cg/meta/upload/microsalt/microsalt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/upload/mip/mip_dna.py` & `cg-60.3.2/cg/meta/upload/mip/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/upload/mip/mip_rna.py` & `cg-60.3.2/cg/meta/upload/mip/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/upload/mutacc.py` & `cg-60.3.2/cg/meta/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/upload/nf_analysis.py` & `cg-60.3.2/cg/meta/upload/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/upload/nipt/models.py` & `cg-60.3.2/cg/meta/upload/nipt/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/upload/nipt/nipt.py` & `cg-60.3.2/cg/meta/upload/nipt/nipt.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/upload/scout/balsamic_config_builder.py` & `cg-60.3.2/cg/meta/upload/scout/balsamic_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/upload/scout/balsamic_umi_config_builder.py` & `cg-60.3.2/cg/meta/upload/scout/balsamic_umi_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/upload/scout/hk_tags.py` & `cg-60.3.2/cg/meta/upload/scout/hk_tags.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/upload/scout/mip_config_builder.py` & `cg-60.3.2/cg/meta/upload/scout/mip_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/upload/scout/rnafusion_config_builder.py` & `cg-60.3.2/cg/meta/upload/scout/rnafusion_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/upload/scout/scout_config_builder.py` & `cg-60.3.2/cg/meta/upload/scout/scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/upload/scout/uploadscoutapi.py` & `cg-60.3.2/cg/meta/upload/scout/uploadscoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/upload/upload_api.py` & `cg-60.3.2/cg/meta/upload/upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/analysis.py` & `cg-60.3.2/cg/meta/workflow/analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/balsamic.py` & `cg-60.3.2/cg/meta/workflow/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/balsamic_pon.py` & `cg-60.3.2/cg/meta/workflow/balsamic_pon.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/balsamic_qc.py` & `cg-60.3.2/cg/meta/workflow/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/balsamic_umi.py` & `cg-60.3.2/cg/meta/workflow/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/downsample/downsample.py` & `cg-60.3.2/cg/meta/workflow/downsample/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/downsample/sbatch.py` & `cg-60.3.2/cg/meta/workflow/downsample/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/fastq.py` & `cg-60.3.2/cg/meta/workflow/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/fluffy.py` & `cg-60.3.2/cg/meta/workflow/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/jasen.py` & `cg-60.3.2/cg/meta/workflow/jasen.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/microsalt/metrics_parser/models.py` & `cg-60.3.2/cg/meta/workflow/microsalt/metrics_parser/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/microsalt/microsalt.py` & `cg-60.3.2/cg/meta/workflow/microsalt/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/microsalt/quality_controller/models.py` & `cg-60.3.2/cg/meta/workflow/microsalt/quality_controller/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/microsalt/quality_controller/quality_controller.py` & `cg-60.3.2/cg/meta/workflow/microsalt/quality_controller/quality_controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/microsalt/quality_controller/report_generator.py` & `cg-60.3.2/cg/meta/workflow/microsalt/quality_controller/report_generator.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/microsalt/quality_controller/result_logger.py` & `cg-60.3.2/cg/meta/workflow/microsalt/quality_controller/result_logger.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/microsalt/quality_controller/utils.py` & `cg-60.3.2/cg/meta/workflow/microsalt/quality_controller/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/microsalt/utils.py` & `cg-60.3.2/cg/meta/workflow/microsalt/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/mip.py` & `cg-60.3.2/cg/meta/workflow/mip.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/mip_dna.py` & `cg-60.3.2/cg/meta/workflow/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/mip_rna.py` & `cg-60.3.2/cg/meta/workflow/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/mutant.py` & `cg-60.3.2/cg/meta/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/nf_analysis.py` & `cg-60.3.2/cg/meta/workflow/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/nf_handlers.py` & `cg-60.3.2/cg/meta/workflow/nf_handlers.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/prepare_fastq.py` & `cg-60.3.2/cg/meta/workflow/prepare_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/raredisease.py` & `cg-60.3.2/cg/meta/workflow/raredisease.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/rnafusion.py` & `cg-60.3.2/cg/meta/workflow/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/taxprofiler.py` & `cg-60.3.2/cg/meta/workflow/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/meta/workflow/tomte.py` & `cg-60.3.2/cg/meta/workflow/tomte.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/balsamic/config.py` & `cg-60.3.2/cg/models/balsamic/config.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/balsamic/metrics.py` & `cg-60.3.2/cg/models/balsamic/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/cg_config.py` & `cg-60.3.2/cg/models/cg_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/compression_data.py` & `cg-60.3.2/cg/models/compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/deliverables/metric_deliverables.py` & `cg-60.3.2/cg/models/deliverables/metric_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/demultiplex/run_parameters.py` & `cg-60.3.2/cg/models/demultiplex/run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/demultiplex/sbatch.py` & `cg-60.3.2/cg/models/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/downsample/downsample_data.py` & `cg-60.3.2/cg/models/downsample/downsample_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/fastq.py` & `cg-60.3.2/cg/models/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/file_data.py` & `cg-60.3.2/cg/models/file_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/flow_cell/flow_cell.py` & `cg-60.3.2/cg/models/flow_cell/flow_cell.py`

 * *Files 6% similar despite different names*

```diff
@@ -135,24 +135,14 @@
 
     @property
     def copy_complete_path(self) -> Path:
         """Return copy complete path."""
         return Path(self.path, DemultiplexingDirsAndFiles.COPY_COMPLETE)
 
     @property
-    def hiseq_x_copy_complete_path(self) -> Path:
-        """Return copy complete path for HiSeqX."""
-        return Path(self.path, DemultiplexingDirsAndFiles.HISEQ_X_COPY_COMPLETE)
-
-    @property
-    def hiseq_x_delivery_started_path(self) -> Path:
-        """Return delivery started path for HiSeqX."""
-        return Path(self.path, DemultiplexingDirsAndFiles.DELIVERY)
-
-    @property
     def demultiplexing_started_path(self) -> Path:
         """Return demux started path."""
         return Path(self.path, DemultiplexingDirsAndFiles.DEMUX_STARTED)
 
     @property
     def trailblazer_config_path(self) -> Path:
         """Return file to SLURM job ids path."""
```

### Comparing `cg-60.3.1/cg/models/invoice/invoice.py` & `cg-60.3.2/cg/models/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/lims/sample.py` & `cg-60.3.2/cg/models/lims/sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/mip/mip_config.py` & `cg-60.3.2/cg/models/mip/mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/mip/mip_metrics_deliverables.py` & `cg-60.3.2/cg/models/mip/mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/mip/mip_sample_info.py` & `cg-60.3.2/cg/models/mip/mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/nf_analysis.py` & `cg-60.3.2/cg/models/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/observations/input_files.py` & `cg-60.3.2/cg/models/observations/input_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/orders/constants.py` & `cg-60.3.2/cg/models/orders/constants.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/orders/excel_sample.py` & `cg-60.3.2/cg/models/orders/excel_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/orders/json_sample.py` & `cg-60.3.2/cg/models/orders/json_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/orders/order.py` & `cg-60.3.2/cg/models/orders/order.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/orders/orderform_schema.py` & `cg-60.3.2/cg/models/orders/orderform_schema.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/orders/sample_base.py` & `cg-60.3.2/cg/models/orders/sample_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/orders/samples.py` & `cg-60.3.2/cg/models/orders/samples.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/orders/validators/excel_sample_validators.py` & `cg-60.3.2/cg/models/orders/validators/excel_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/orders/validators/json_sample_validators.py` & `cg-60.3.2/cg/models/orders/validators/json_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/raredisease/raredisease.py` & `cg-60.3.2/cg/models/raredisease/raredisease.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/report/metadata.py` & `cg-60.3.2/cg/models/report/metadata.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/report/report.py` & `cg-60.3.2/cg/models/report/report.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/report/sample.py` & `cg-60.3.2/cg/models/report/sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/report/validators.py` & `cg-60.3.2/cg/models/report/validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/rnafusion/rnafusion.py` & `cg-60.3.2/cg/models/rnafusion/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/scout/scout_load_config.py` & `cg-60.3.2/cg/models/scout/scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/slurm/sbatch.py` & `cg-60.3.2/cg/models/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/taxprofiler/taxprofiler.py` & `cg-60.3.2/cg/models/taxprofiler/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/tomte/tomte.py` & `cg-60.3.2/cg/models/tomte/tomte.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/models/workflow/mutant.py` & `cg-60.3.2/cg/models/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/resources/__init__.py` & `cg-60.3.2/cg/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/resources/rnafusion_bundle_filenames.yaml` & `cg-60.3.2/cg/resources/rnafusion_bundle_filenames.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/resources/taxprofiler_bundle_filenames.yaml` & `cg-60.3.2/cg/resources/taxprofiler_bundle_filenames.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/resources/tomte_bundle_filenames.yaml` & `cg-60.3.2/cg/resources/tomte_bundle_filenames.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/server/admin.py` & `cg-60.3.2/cg/server/admin.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/server/api.py` & `cg-60.3.2/cg/server/api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/server/app.py` & `cg-60.3.2/cg/server/app.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/server/config.py` & `cg-60.3.2/cg/server/config.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/server/dto/orders/orders_request.py` & `cg-60.3.2/cg/server/dto/orders/orders_request.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/server/ext.py` & `cg-60.3.2/cg/server/ext.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/server/invoices/templates/invoices/index.html` & `cg-60.3.2/cg/server/invoices/templates/invoices/index.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/server/invoices/templates/invoices/invoice.html` & `cg-60.3.2/cg/server/invoices/templates/invoices/invoice.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/server/invoices/templates/invoices/layout.html` & `cg-60.3.2/cg/server/invoices/templates/invoices/layout.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/server/invoices/templates/invoices/new.html` & `cg-60.3.2/cg/server/invoices/templates/invoices/new.html`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/server/invoices/views.py` & `cg-60.3.2/cg/server/invoices/views.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/services/delivery_message/delivery_message_service.py` & `cg-60.3.2/cg/services/delivery_message/delivery_message_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/services/delivery_message/messages/__init__.py` & `cg-60.3.2/cg/services/delivery_message/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/services/delivery_message/messages/analysis_scout_message.py` & `cg-60.3.2/cg/services/delivery_message/messages/analysis_scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/services/delivery_message/messages/covid_message.py` & `cg-60.3.2/cg/services/delivery_message/messages/covid_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/services/delivery_message/messages/fastq_analysis_scout_message.py` & `cg-60.3.2/cg/services/delivery_message/messages/fastq_analysis_scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/services/delivery_message/messages/fastq_message.py` & `cg-60.3.2/cg/services/delivery_message/messages/fastq_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/services/delivery_message/messages/fastq_scout_message.py` & `cg-60.3.2/cg/services/delivery_message/messages/fastq_scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/services/delivery_message/messages/microsalt_mwr_message.py` & `cg-60.3.2/cg/services/delivery_message/messages/microsalt_mwr_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/services/delivery_message/messages/microsalt_mwx_message.py` & `cg-60.3.2/cg/services/delivery_message/messages/microsalt_mwx_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/services/delivery_message/messages/scout_message.py` & `cg-60.3.2/cg/services/delivery_message/messages/scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/services/delivery_message/messages/statina_message.py` & `cg-60.3.2/cg/services/delivery_message/messages/statina_message.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/services/delivery_message/messages/utils.py` & `cg-60.3.2/cg/services/delivery_message/messages/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/services/delivery_message/utils.py` & `cg-60.3.2/cg/services/delivery_message/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/services/fastq_file_service/fastq_file_service.py` & `cg-60.3.2/cg/services/fastq_file_service/fastq_file_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/services/fastq_file_service/utils.py` & `cg-60.3.2/cg/services/fastq_file_service/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/services/orders/order_service/order_service.py` & `cg-60.3.2/cg/services/orders/order_service/order_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/services/orders/order_service/utils.py` & `cg-60.3.2/cg/services/orders/order_service/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/services/orders/order_status_service/order_summary_service.py` & `cg-60.3.2/cg/services/orders/order_status_service/order_summary_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/services/orders/order_status_service/utils.py` & `cg-60.3.2/cg/services/orders/order_status_service/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/services/slurm_service/slurm_cli_service.py` & `cg-60.3.2/cg/services/slurm_service/slurm_cli_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/services/slurm_upload_service/slurm_upload_service.py` & `cg-60.3.2/cg/services/slurm_upload_service/slurm_upload_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/base.py` & `cg-60.3.2/cg/store/base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/crud/create.py` & `cg-60.3.2/cg/store/crud/create.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/crud/delete.py` & `cg-60.3.2/cg/store/crud/delete.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/crud/read.py` & `cg-60.3.2/cg/store/crud/read.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/crud/update.py` & `cg-60.3.2/cg/store/crud/update.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/database.py` & `cg-60.3.2/cg/store/database.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/filters/status_analysis_filters.py` & `cg-60.3.2/cg/store/filters/status_analysis_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/filters/status_application_filters.py` & `cg-60.3.2/cg/store/filters/status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/filters/status_application_limitations_filters.py` & `cg-60.3.2/cg/store/filters/status_application_limitations_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/filters/status_application_version_filters.py` & `cg-60.3.2/cg/store/filters/status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/filters/status_bed_filters.py` & `cg-60.3.2/cg/store/filters/status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/filters/status_bed_version_filters.py` & `cg-60.3.2/cg/store/filters/status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/filters/status_case_filters.py` & `cg-60.3.2/cg/store/filters/status_case_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/filters/status_case_sample_filters.py` & `cg-60.3.2/cg/store/filters/status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/filters/status_collaboration_filters.py` & `cg-60.3.2/cg/store/filters/status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/filters/status_customer_filters.py` & `cg-60.3.2/cg/store/filters/status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/filters/status_flow_cell_filters.py` & `cg-60.3.2/cg/store/filters/status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/filters/status_invoice_filters.py` & `cg-60.3.2/cg/store/filters/status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/filters/status_metrics_filters.py` & `cg-60.3.2/cg/store/filters/status_metrics_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/filters/status_order_filters.py` & `cg-60.3.2/cg/store/filters/status_order_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/filters/status_organism_filters.py` & `cg-60.3.2/cg/store/filters/status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/filters/status_panel_filters.py` & `cg-60.3.2/cg/store/filters/status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/filters/status_pool_filters.py` & `cg-60.3.2/cg/store/filters/status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/filters/status_sample_filters.py` & `cg-60.3.2/cg/store/filters/status_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/filters/status_user_filters.py` & `cg-60.3.2/cg/store/filters/status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/models.py` & `cg-60.3.2/cg/store/models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/store/store.py` & `cg-60.3.2/cg/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/utils/checksum/checksum.py` & `cg-60.3.2/cg/utils/checksum/checksum.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/utils/click/EnumChoice.py` & `cg-60.3.2/cg/utils/click/EnumChoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/utils/commands.py` & `cg-60.3.2/cg/utils/commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/utils/date.py` & `cg-60.3.2/cg/utils/date.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/utils/dict.py` & `cg-60.3.2/cg/utils/dict.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/utils/dispatcher.py` & `cg-60.3.2/cg/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/utils/email.py` & `cg-60.3.2/cg/utils/email.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/utils/files.py` & `cg-60.3.2/cg/utils/files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/utils/flask/enum.py` & `cg-60.3.2/cg/utils/flask/enum.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/utils/time.py` & `cg-60.3.2/cg/utils/time.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/cg/utils/utils.py` & `cg-60.3.2/cg/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/pyproject.toml` & `cg-60.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cg"
-version = "60.3.1"
+version = "60.3.2"
 description = "Clinical Genomics command center"
 authors = ["Clinical Genomics <support@clinicalgenomics.se>"]
 readme = "README.md"
 homepage = "https://github.com/Clinical-Genomics/cg"
 repository = "https://github.com/Clinical-Genomics/cg"
 classifiers = [
   "Programming Language :: Python",
```

### Comparing `cg-60.3.1/tests/apps/conftest.py` & `cg-60.3.2/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/coverage/test_coverage.py` & `cg-60.3.2/tests/apps/coverage/test_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/crunchy/conftest.py` & `cg-60.3.2/tests/apps/crunchy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/crunchy/test_compress_fastq.py` & `cg-60.3.2/tests/apps/crunchy/test_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/crunchy/test_config.py` & `cg-60.3.2/tests/apps/crunchy/test_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/crunchy/test_crunchy.py` & `cg-60.3.2/tests/apps/crunchy/test_crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/crunchy/test_spring_decompression.py` & `cg-60.3.2/tests/apps/crunchy/test_spring_decompression.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/demultiplex/conftest.py` & `cg-60.3.2/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,122 @@
+from datetime import datetime
 from pathlib import Path
+from typing import Any
 
 import pytest
 
-from cg.apps.demultiplex.sample_sheet.override_cycles_validator import OverrideCyclesValidator
-from cg.apps.demultiplex.sample_sheet.sample_models import FlowCellSample
+from cg.apps.demultiplex.sample_sheet.sample_sheet_models import SampleSheet
+from cg.apps.demultiplex.sample_sheet.sample_sheet_validator import SampleSheetValidator
+from cg.constants.constants import FileFormat
 from cg.constants.demultiplexing import SampleSheetBcl2FastqSections, SampleSheetBCLConvertSections
+from cg.io.controller import ReadFile
+
+
+@pytest.fixture(scope="function")
+def sample_sheet_validator() -> SampleSheetValidator:
+    """Return a sample sheet validator."""
+    return SampleSheetValidator()
+
+
+@pytest.fixture
+def hiseq_x_single_index_sample_sheet_content(
+    hiseq_x_single_index_sample_sheet_path: Path,
+) -> list[list[str]]:
+    """Return the content of a single-index HiSeq X sample sheet."""
+    return ReadFile.get_content_from_file(
+        file_format=FileFormat.CSV, file_path=hiseq_x_single_index_sample_sheet_path
+    )
+
+
+@pytest.fixture
+def hiseq_x_dual_index_sample_sheet_content(
+    hiseq_x_dual_index_sample_sheet_path: Path,
+) -> list[list[str]]:
+    """Return the content of a dual-index HiSeq X sample sheet."""
+    return ReadFile.get_content_from_file(
+        file_format=FileFormat.CSV, file_path=hiseq_x_dual_index_sample_sheet_path
+    )
+
+
+@pytest.fixture
+def hiseq_2500_dual_index_sample_sheet_content(
+    hiseq_2500_dual_index_sample_sheet_path: Path,
+) -> list[list[str]]:
+    """Return the content of a dual-index HiSeq 2500 sample sheet."""
+    return ReadFile.get_content_from_file(
+        file_format=FileFormat.CSV, file_path=hiseq_2500_dual_index_sample_sheet_path
+    )
+
+
+@pytest.fixture
+def hiseq_2500_custom_index_sample_sheet_content(
+    hiseq_2500_custom_index_sample_sheet_path: Path,
+) -> list[list[str]]:
+    """Return the content of a custom-index HiSeq 2500 sample sheet."""
+    return ReadFile.get_content_from_file(
+        file_format=FileFormat.CSV, file_path=hiseq_2500_custom_index_sample_sheet_path
+    )
+
+
+@pytest.fixture
+def novaseq_6000_pre_1_5_kits_sample_sheet_content(
+    novaseq_6000_pre_1_5_kits_correct_sample_sheet_path: Path,
+) -> list[list[str]]:
+    """Return the content of a NovaSeq 6000 sample sheet."""
+    return ReadFile.get_content_from_file(
+        file_format=FileFormat.CSV, file_path=novaseq_6000_pre_1_5_kits_correct_sample_sheet_path
+    )
 
 
 @pytest.fixture
-def bcl_convert_samples_similar_index1() -> list[FlowCellSample]:
-    """Return a list of three FlowCellSampleBCLConvert with updated indexes."""
-    sample_1 = FlowCellSample(lane=1, sample_id="ACC123", index="CAGAAGAT", index2="GCGCAAGC")
-    sample_2 = FlowCellSample(lane=1, sample_id="ACC456", index="CAGAAGAG", index2="CAATGTAT")
-    sample_3 = FlowCellSample(lane=2, sample_id="ACC789", index="AAGCGATA", index2="AACCGCAA")
-    return [sample_1, sample_2, sample_3]
+def novaseq_6000_post_1_5_kits_sample_sheet_content(
+    novaseq_6000_post_1_5_kits_correct_sample_sheet_path: Path,
+) -> list[list[str]]:
+    """Return the content of a NovaSeq 6000 sample sheet."""
+    return ReadFile.get_content_from_file(
+        file_format=FileFormat.CSV, file_path=novaseq_6000_post_1_5_kits_correct_sample_sheet_path
+    )
 
 
 @pytest.fixture
-def bcl_convert_samples_similar_index2() -> list[FlowCellSample]:
-    """Return a list of three FlowCellSampleBCLConvert with updated indexes."""
-    sample_1 = FlowCellSample(lane=1, sample_id="ACC123", index="GCGCAAGC", index2="CAATGTAC")
-    sample_2 = FlowCellSample(lane=1, sample_id="ACC456", index="CAATGTAT", index2="CAATGTAT")
-    sample_3 = FlowCellSample(lane=2, sample_id="ACC789", index="AAGCGATA", index2="AACCGCAA")
-    return [sample_1, sample_2, sample_3]
+def novaseq_x_sample_sheet_content(novaseq_x_correct_sample_sheet: Path) -> list[list[str]]:
+    """Return the content of a NovaSeqX sample sheet."""
+    return ReadFile.get_content_from_file(
+        file_format=FileFormat.CSV, file_path=novaseq_x_correct_sample_sheet
+    )
 
 
-# Sample sheet validation
+# Sample sheet parts
 
 
 @pytest.fixture
-def sample_sheet_line_sample_1() -> list[str]:
-    """Return the line in the sample sheet corresponding to a sample."""
+def bcl_convert_sample_sheet_line_entry_1() -> list[str]:
+    """Return a sample sheet line entry from the HiSeqX double index flow cell."""
     return [
-        "HWHMWDMXX",
         "1",
-        "ACC7628A68",
-        "hg19",
-        "ATTCCACACT",
-        "TGGTCTTGTT",
-        "814206",
-        "N",
-        "R1",
-        "script",
-        "814206",
+        "ACC4519A1",
+        "ATTCAGAA",
+        "TATAGCCT",
+        "Y151;I8;I8;Y151",
+        "1",
+        "1",
     ]
 
 
 @pytest.fixture
-def sample_sheet_line_sample_2() -> list[str]:
-    """Return the line in the sample sheet corresponding to a sample."""
+def bcl_convert_sample_sheet_line_entry_2() -> list[str]:
+    """Return a sample sheet line entry from the HiSeqX double index flow cell."""
     return [
-        "HWHMWDMXX",
+        "2",
+        "ACC4519A2",
+        "GAATTCGT",
+        "TATAGCCT",
+        "Y151;I8;I8;Y151",
+        "1",
         "1",
-        "ACC7628A1",
-        "hg19",
-        "AGTTAGCTGG",
-        "GATGAGAATG",
-        "814206",
-        "N",
-        "R1",
-        "script",
-        "814206",
     ]
 
 
 @pytest.fixture
 def sample_sheet_bcl2fastq_data_header() -> list[list[str]]:
     """Return the content of a Bcl2fastq sample sheet data header without samples."""
     return [
@@ -82,14 +134,31 @@
             SampleSheetBcl2FastqSections.Data.OPERATOR.value,
             SampleSheetBcl2FastqSections.Data.SAMPLE_PROJECT_BCL2FASTQ.value,
         ],
     ]
 
 
 @pytest.fixture
+def sample_sheet_bcl_convert_data_header() -> list[list[str]]:
+    """Return the content of a BCLConvert sample sheet data header without samples."""
+    return [
+        [SampleSheetBCLConvertSections.Data.HEADER],
+        [
+            SampleSheetBCLConvertSections.Data.LANE.value,
+            SampleSheetBCLConvertSections.Data.SAMPLE_INTERNAL_ID.value,
+            SampleSheetBCLConvertSections.Data.INDEX_1.value,
+            SampleSheetBCLConvertSections.Data.INDEX_2.value,
+            SampleSheetBCLConvertSections.Data.OVERRIDE_CYCLES.value,
+            SampleSheetBCLConvertSections.Data.BARCODE_MISMATCHES_1.value,
+            SampleSheetBCLConvertSections.Data.BARCODE_MISMATCHES_2.value,
+        ],
+    ]
+
+
+@pytest.fixture
 def sample_sheet_bcl2fastq_data_header_with_replaced_sample_id() -> list[list[str]]:
     """Return the content of a Bcl2fastq sample sheet data header without samples."""
     return [
         [SampleSheetBcl2FastqSections.Data.HEADER],
         [
             SampleSheetBcl2FastqSections.Data.FLOW_CELL_ID.value,
             SampleSheetBcl2FastqSections.Data.LANE.value,
@@ -102,210 +171,87 @@
             SampleSheetBcl2FastqSections.Data.RECIPE.value,
             SampleSheetBcl2FastqSections.Data.OPERATOR.value,
             SampleSheetBcl2FastqSections.Data.SAMPLE_PROJECT_BCL2FASTQ.value,
         ],
     ]
 
 
-@pytest.fixture
-def sample_sheet_samples_no_header(
-    sample_sheet_line_sample_1: list[str], sample_sheet_line_sample_2: list[str]
-) -> list[list[str]]:
-    """Return the content of a sample sheet with samples but without a sample header."""
-    return [
-        [SampleSheetBcl2FastqSections.Data.HEADER],
-        sample_sheet_line_sample_1,
-        sample_sheet_line_sample_2,
-    ]
+# Incorrect sample sheets
 
 
 @pytest.fixture
-def valid_sample_sheet_bcl2fastq(
-    sample_sheet_bcl2fastq_data_header: list[list[str]],
-    sample_sheet_line_sample_1: list[str],
-    sample_sheet_line_sample_2: list[str],
-) -> list[list[str]]:
-    """Return the content of a valid Bcl2fastq sample sheet."""
-    return sample_sheet_bcl2fastq_data_header + [
-        sample_sheet_line_sample_1,
-        sample_sheet_line_sample_2,
-    ]
+def sample_sheet_content_missing_data_header() -> list[list[str]]:
+    """Return a sample sheet without data and without the data header."""
+    return [["[Header]"], ["[Reads]"], ["[BCLConvert_Settings]"]]
 
 
 @pytest.fixture
-def sample_sheet_bcl2fastq_duplicate_same_lane(
-    valid_sample_sheet_bcl2fastq: list[list[str]], sample_sheet_line_sample_2: list[str]
+def sample_sheet_samples_no_column_names(
+    bcl_convert_sample_sheet_line_entry_1: list[str],
+    bcl_convert_sample_sheet_line_entry_2: list[str],
 ) -> list[list[str]]:
-    """Return the content of a Bcl2fastq sample sheet with a duplicated sample in the same lane."""
-    valid_sample_sheet_bcl2fastq.append(sample_sheet_line_sample_2)
-    return valid_sample_sheet_bcl2fastq
+    """Return the content of a sample sheet with samples but without the column names."""
+    return [
+        [SampleSheetBCLConvertSections.Data.HEADER],
+        bcl_convert_sample_sheet_line_entry_1,
+        bcl_convert_sample_sheet_line_entry_2,
+    ]
 
 
 @pytest.fixture
-def sample_sheet_bcl2fastq_duplicate_different_lane(
-    valid_sample_sheet_bcl2fastq: list[list[str]],
+def novaseq_6000_sample_sheet_with_reversed_cycles_content(
+    novaseq_6000_sample_sheet_with_reversed_cycles: Path,
 ) -> list[list[str]]:
-    """Return the content of a Bcl2fastq sample sheet with a duplicated sample in a different lane."""
-    valid_sample_sheet_bcl2fastq.append(
-        [
-            "HWHMWDMXX",
-            "2",
-            "ACC7628A1",
-            "hg19",
-            "AGTTAGCTGG",
-            "GATGAGAATG",
-            "814206",
-            "N",
-            "R1",
-            "script",
-            "814206",
-        ]
-    )
-    return valid_sample_sheet_bcl2fastq
-
-
-@pytest.fixture
-def novaseq6000_flow_cell_sample_1() -> FlowCellSample:
-    """Return a NovaSeq sample."""
-    return FlowCellSample(
-        lane=1,
-        sample_id="ACC7628A68",
-        index="ATTCCACACT",
-        index2="TGGTCTTGTT",
-    )
-
-
-@pytest.fixture
-def novaseq6000_flow_cell_sample_2() -> FlowCellSample:
-    """Return a NovaSeq sample."""
-    return FlowCellSample(
-        lane=2,
-        sample_id="ACC7628A1",
-        index="ATTCCACACT",
-        index2="TGGTCTTGTT",
-    )
-
-
-@pytest.fixture
-def novaseq6000_flow_cell_sample_no_dual_index() -> FlowCellSample:
-    """Return a NovaSeq sample without dual indexes."""
-    return FlowCellSample(
-        lane=2,
-        sample_id="ACC7628A1",
-        index="ATTCCACACT",
+    """Return the content of a NovaSeq 6000 sample sheet with reversed cycles."""
+    return ReadFile.get_content_from_file(
+        file_format=FileFormat.CSV, file_path=novaseq_6000_sample_sheet_with_reversed_cycles
     )
 
 
 @pytest.fixture
-def novaseq6000_flow_cell_sample_before_adapt_indexes() -> FlowCellSample:
-    """Return a NovaSeq sample without dual indexes."""
-    return FlowCellSample(
-        lane=2,
-        sample_id="ACC7628A1",
-        index="ATTCCACACT-TGGTCTTGTT",
+def novaseq_x_sample_sheet_with_forward_cycles_content(
+    novaseq_x_sample_sheet_with_forward_cycles: Path,
+) -> list[list[str]]:
+    """Return the content of a NovaSeqX sample sheet with forward cycles."""
+    return ReadFile.get_content_from_file(
+        file_format=FileFormat.CSV, file_path=novaseq_x_sample_sheet_with_forward_cycles
     )
 
 
-@pytest.fixture
-def index1_8_nt_sequence_from_lims() -> str:
-    """Return an index 1 sequence."""
-    return "GTCTACAC"
-
-
-@pytest.fixture
-def index2_8_nt_sequence_from_lims() -> str:
-    """Return an index 2 sequence."""
-    return "GCCAAGGT"
-
-
-@pytest.fixture
-def index1_10_nt_sequence_from_lims() -> str:
-    """Return an index 1 sequence."""
-    return "CCGGTTCATG"
-
-
-@pytest.fixture
-def index2_10_nt_sequence_from_lims() -> str:
-    """Return an index 2 sequence."""
-    return "CAAGACGTCT"
-
-
-@pytest.fixture
-def raw_index_sequence(
-    index1_8_nt_sequence_from_lims: str, index2_8_nt_sequence_from_lims: str
-) -> str:
-    """Return a raw index."""
-    return f"{index1_8_nt_sequence_from_lims}-{index2_8_nt_sequence_from_lims}"
-
-
-@pytest.fixture
-def bcl_convert_flow_cell_sample(raw_index_sequence: str) -> FlowCellSample:
-    """Return a BCL Convert sample."""
-    return FlowCellSample(lane=1, index=raw_index_sequence, sample_id="ACC123")
+# Sample sheet objects
 
 
 @pytest.fixture
-def bcl_convert_sample_sheet_path(illumina_demultiplexed_runs_directory):
-    return Path(
-        illumina_demultiplexed_runs_directory,
-        "230504_A00689_0804_BHY7FFDRX2",
-        "SampleSheet.csv",
+def novaseq_6000_post_1_5_kits_sample_sheet_object(
+    sample_sheet_validator: SampleSheetValidator,
+    novaseq_6000_post_1_5_kits_correct_sample_sheet_path: Path,
+) -> SampleSheet:
+    """Return a NovaSeq 6000 sample sheet object."""
+    return sample_sheet_validator.get_sample_sheet_object_from_file(
+        file_path=novaseq_6000_post_1_5_kits_correct_sample_sheet_path
     )
 
 
-@pytest.fixture
-def override_cycles_validator() -> OverrideCyclesValidator:
-    """Return an override cycles validator without any initialised attribute."""
-    return OverrideCyclesValidator()
-
-
-@pytest.fixture
-def processed_flow_cell_sample_8_index(
-    index1_8_nt_sequence_from_lims: str, index2_8_nt_sequence_from_lims: str
-) -> dict[str, str]:
-    """Return a BCL Convert sample with processed 8-nt indexes and no override cycles."""
-    return {
-        "Lane": 1,
-        "Sample_ID": "ACC123",
-        "Index": index1_8_nt_sequence_from_lims,
-        "Index2": index2_8_nt_sequence_from_lims,
-    }
+# HK bundle objects
 
 
 @pytest.fixture
-def processed_flow_cell_sample_10_index(
-    index1_10_nt_sequence_from_lims: str, index2_10_nt_sequence_from_lims: str
-) -> dict[str, str]:
-    """Return a BCL Convert sample with processed 10-nt indexes and no override cycles."""
+def sample_sheet_bcl2fastq_bundle_data(
+    tmp_flow_cell_with_bcl2fastq_sample_sheet: Path,
+    timestamp_yesterday: datetime,
+) -> dict[str, Any]:
+    """Return a sample sheet bundle data dictionary."""
+    flow_cell_id: str = tmp_flow_cell_with_bcl2fastq_sample_sheet.name[-9:]
     return {
-        "Lane": 1,
-        "Sample_ID": "ACC123",
-        "Index": index1_10_nt_sequence_from_lims,
-        "Index2": index2_10_nt_sequence_from_lims,
+        "name": flow_cell_id,
+        "created": timestamp_yesterday,
+        "expires": timestamp_yesterday,
+        "files": [
+            {
+                "path": Path(
+                    tmp_flow_cell_with_bcl2fastq_sample_sheet, "SampleSheet.csv"
+                ).as_posix(),
+                "archive": False,
+                "tags": ["samplesheet", flow_cell_id],
+            },
+        ],
     }
-
-
-@pytest.fixture
-def forward_index2_cycle_processed_flow_cell_8_nt_sample(
-    processed_flow_cell_sample_8_index: dict[str, str],
-) -> dict[str, str]:
-    """Return a BCL Convert sample with processed 8-nt indexes and forward index 2 cycle."""
-    processed_flow_cell_sample_8_index["OverrideCycles"] = "Y151;I8N2;I8N2;Y151"
-    return processed_flow_cell_sample_8_index
-
-
-@pytest.fixture
-def reverse_index2_cycle_processed_flow_cell_8_nt_sample(
-    processed_flow_cell_sample_8_index: dict[str, str],
-) -> dict[str, str]:
-    """Return a BCL Convert sample with processed 8-nt indexes and reversed index 2 cycle."""
-    processed_flow_cell_sample_8_index["OverrideCycles"] = "Y151;I8N2;N2I8;Y151"
-    return processed_flow_cell_sample_8_index
-
-
-@pytest.fixture
-def processed_flow_cell_10_nt_sample(
-    processed_flow_cell_sample_10_index: dict[str, str],
-) -> dict[str, str]:
-    """Return a BCL Convert sample with processed 10-nt indexes."""
-    processed_flow_cell_sample_10_index["OverrideCycles"] = "Y151;I10;I10;Y151"
-    return processed_flow_cell_sample_10_index
```

### Comparing `cg-60.3.1/tests/apps/demultiplex/test_create_sample_sheet.py` & `cg-60.3.2/tests/apps/demultiplex/test_create_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/demultiplex/test_demultiplex_api.py` & `cg-60.3.2/tests/apps/demultiplex/test_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/demultiplex/test_index.py` & `cg-60.3.2/tests/apps/demultiplex/test_index.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/demultiplex/test_override_cycles_validator.py` & `cg-60.3.2/tests/apps/demultiplex/test_override_cycles_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/demultiplex/test_read_sample_sheet.py` & `cg-60.3.2/tests/apps/demultiplex/test_read_sample_sheet.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,48 +61,50 @@
 
     # THEN the returned value is a dictionary
     assert isinstance(samples_per_lane, dict)
     # THEN the dictionary has two entries
     assert len(samples_per_lane) == 2
 
 
-def test_get_raw_samples_valid_sample_sheet(valid_sample_sheet_bcl2fastq: list[list[str]]):
+def test_get_raw_samples_valid_sample_sheet(
+    hiseq_x_single_index_sample_sheet_content: list[list[str]],
+):
     """Test that getting raw samples from a valid sample sheet gets a correct list of dictionaries."""
     # GIVEN a valid sample sheet
 
     # WHEN getting the list of raw samples from it
     raw_samples: list[dict[str, str]] = get_raw_samples_from_content(
-        sample_sheet_content=valid_sample_sheet_bcl2fastq
+        sample_sheet_content=hiseq_x_single_index_sample_sheet_content
     )
 
     # THEN it returns a list with 2 dictionaries
-    assert len(raw_samples) == 2
+    assert len(raw_samples) == 9
     # THEN the list contains dictionaries
     assert isinstance(raw_samples[0], dict)
     # THEN the sample contains the key "Lane"
     assert "Lane" in raw_samples[0].keys()
 
 
-def test_get_raw_samples_no_header(sample_sheet_samples_no_header: list[list[str]], caplog):
+def test_get_raw_samples_no_header(sample_sheet_samples_no_column_names: list[list[str]], caplog):
     """Test that getting samples from a sample sheet without header fails."""
     # GIVEN a sample sheet without header
     caplog.set_level(logging.INFO)
 
     # WHEN trying to get the samples from the sample sheet
     with pytest.raises(SampleSheetError):
-        get_raw_samples_from_content(sample_sheet_content=sample_sheet_samples_no_header)
+        get_raw_samples_from_content(sample_sheet_content=sample_sheet_samples_no_column_names)
 
     # THEN an exception is raised because of the missing header
     assert "Could not find header in sample sheet" in caplog.text
 
 
-def test_get_raw_samples_no_samples(sample_sheet_bcl2fastq_data_header: list[list[str]], caplog):
+def test_get_raw_samples_no_samples(sample_sheet_bcl_convert_data_header: list[list[str]], caplog):
     """Test that getting samples from a sample sheet without samples fails."""
     # GIVEN a sample sheet without samples
     caplog.set_level(logging.INFO)
 
     # WHEN trying to get the samples from the sample sheet
     with pytest.raises(SampleSheetError):
-        get_raw_samples_from_content(sample_sheet_content=sample_sheet_bcl2fastq_data_header)
+        get_raw_samples_from_content(sample_sheet_content=sample_sheet_bcl_convert_data_header)
 
     # THEN an exception is raised because of the missing samples
     assert "Could not find any samples in sample sheet" in caplog.text
```

### Comparing `cg-60.3.1/tests/apps/demultiplex/test_sample_models.py` & `cg-60.3.2/tests/apps/demultiplex/test_sample_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/demultiplex/test_sample_sheet_creator.py` & `cg-60.3.2/tests/apps/demultiplex/test_sample_sheet_creator.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/demultiplex/test_sample_sheet_models.py` & `cg-60.3.2/tests/apps/demultiplex/test_sample_sheet_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/demultiplex/test_sample_sheet_validator.py` & `cg-60.3.2/tests/apps/demultiplex/test_sample_sheet_validator.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/demultiplex/test_translate_sample_sheet.py` & `cg-60.3.2/tests/apps/demultiplex/test_translate_sample_sheet.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,26 +85,26 @@
 
     # THEN the new header has BCLConvert column names
     assert new_content == sample_sheet_bcl2fastq_data_header_with_replaced_sample_id
 
 
 def test_replace_sample_sheet_header_bcl_convert(
     sample_sheet_context: CGConfig,
-    sample_sheet_bcl2fastq_data_header_with_replaced_sample_id: list[list[str]],
+    sample_sheet_bcl_convert_data_header: list[list[str]],
 ):
     """Test that the header of a BCLConvert sample sheet can not be replaced."""
     # GIVEN a sample sheet API
     api: SampleSheetAPI = sample_sheet_context.sample_sheet_api
 
     # GIVEN a BCLConvert sample sheet content
 
     # WHEN replacing the header
     with pytest.raises(SampleSheetError) as error:
         # THEN an error is raised
-        api._replace_sample_header(sample_sheet_bcl2fastq_data_header_with_replaced_sample_id)
+        api._replace_sample_header(sample_sheet_bcl_convert_data_header)
     assert "Could not find BCL2FASTQ data header in sample sheet" in str(error.value)
 
 
 def test_translate_sample_sheet(
     sample_sheet_context_broken_flow_cells: CGConfig,
     tmp_flow_cell_with_bcl2fastq_sample_sheet: Path,
 ):
```

### Comparing `cg-60.3.1/tests/apps/demultiplex/test_validate.py` & `cg-60.3.2/tests/apps/demultiplex/test_validate.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/downsample/test_downsample.py` & `cg-60.3.2/tests/apps/downsample/test_downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/downsample/test_downsample_utils.py` & `cg-60.3.2/tests/apps/downsample/test_downsample_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/gens/test_gens_api.py` & `cg-60.3.2/tests/apps/gens/test_gens_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/gt/conftest.py` & `cg-60.3.2/tests/apps/gt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/gt/test_gt_api.py` & `cg-60.3.2/tests/apps/gt/test_gt_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/hk/conftest.py` & `cg-60.3.2/tests/apps/hk/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/hk/test__getattr__.py` & `cg-60.3.2/tests/apps/hk/test__getattr__.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/hk/test_add_file.py` & `cg-60.3.2/tests/apps/hk/test_add_file.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/hk/test_bundles.py` & `cg-60.3.2/tests/apps/hk/test_bundles.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/hk/test_core.py` & `cg-60.3.2/tests/apps/hk/test_core.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/hk/test_file.py` & `cg-60.3.2/tests/apps/hk/test_file.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/hk/test_version.py` & `cg-60.3.2/tests/apps/hk/test_version.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/lims/conftest.py` & `cg-60.3.2/tests/apps/lims/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/lims/test_api.py` & `cg-60.3.2/tests/apps/lims/test_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/lims/test_sample_sheet.py` & `cg-60.3.2/tests/apps/lims/test_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/loqus/conftest.py` & `cg-60.3.2/tests/apps/loqus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/loqus/test_loqusdb_api.py` & `cg-60.3.2/tests/apps/loqus/test_loqusdb_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/madeline/conftest.py` & `cg-60.3.2/tests/apps/madeline/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/madeline/test_madeline.py` & `cg-60.3.2/tests/apps/madeline/test_madeline.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/mip/conftest.py` & `cg-60.3.2/tests/apps/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/mip/test_config_mip.py` & `cg-60.3.2/tests/apps/mip/test_config_mip.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/mutacc_auto/conftest.py` & `cg-60.3.2/tests/apps/mutacc_auto/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/mutacc_auto/test_mutacc_auto.py` & `cg-60.3.2/tests/apps/mutacc_auto/test_mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/orderform/conftest.py` & `cg-60.3.2/tests/apps/orderform/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/orderform/test_excel_orderform_parser.py` & `cg-60.3.2/tests/apps/orderform/test_excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/orderform/test_excel_sample_schema.py` & `cg-60.3.2/tests/apps/orderform/test_excel_sample_schema.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/orderform/test_json_orderform_parser.py` & `cg-60.3.2/tests/apps/orderform/test_json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/orderform/test_orderform_parser.py` & `cg-60.3.2/tests/apps/orderform/test_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/orderform/validators/test_excel_sample_validators.py` & `cg-60.3.2/tests/apps/orderform/validators/test_excel_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/scout/conftest.py` & `cg-60.3.2/tests/apps/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/scout/test_get_causative_variants.py` & `cg-60.3.2/tests/apps/scout/test_get_causative_variants.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/scout/test_get_scout_cases.py` & `cg-60.3.2/tests/apps/scout/test_get_scout_cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/scout/test_scout_load_config.py` & `cg-60.3.2/tests/apps/scout/test_scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/scout/test_scout_models.py` & `cg-60.3.2/tests/apps/scout/test_scout_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/sequencing_metrics_parser/conftest.py` & `cg-60.3.2/tests/apps/sequencing_metrics_parser/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py` & `cg-60.3.2/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import pytest
 
 from cg.apps.sequencing_metrics_parser.models import DemuxMetrics, SequencingQualityMetrics
 from cg.apps.sequencing_metrics_parser.parser import MetricsParser
 
 
-def test_parse_bcl_convert_metrics(
+def test_parse_metrics(
     bcl_convert_metrics_dir_path: Path,
 ):
     """Test to parse BCLConvert metrics."""
     # GIVEN paths to a BCLConvert metrics files
     # WHEN parsing the files
     bcl_convert_metrics_parser = MetricsParser(
         bcl_convert_metrics_dir_path=bcl_convert_metrics_dir_path
@@ -29,15 +29,15 @@
     """Test to parse BCLConvert metrics with non-existing path."""
     # GIVEN paths to a BCLConvert metrics files that do not exist
     # WHEN parsing the files assert that a FileNotFoundError is raised
     with pytest.raises(FileNotFoundError):
         MetricsParser(bcl_convert_metrics_dir_path=Path("non-existing-path"))
 
 
-def test_parse_bcl_convert_quality_metrics(
+def test_parse_quality_metrics(
     parsed_bcl_convert_metrics: MetricsParser,
     bcl_convert_quality_metric_model_with_data: SequencingQualityMetrics,
 ):
     """Test to parse BCLConvert quality metrics."""
     # GIVEN a parsed BCLConvert metrics
 
     # ASSERT that the parsed quality metrics are correct
@@ -47,15 +47,15 @@
     assert isinstance(quality_metrics_model, SequencingQualityMetrics)
 
     # ASSERT that the parsed quality metrics has the correct values
     for attr_name, attr_value in quality_metrics_model.model_dump().items():
         assert getattr(bcl_convert_quality_metric_model_with_data, attr_name) == attr_value
 
 
-def test_parse_bcl_convert_demux_metrics(
+def test_parse_demux_metrics(
     parsed_bcl_convert_metrics: MetricsParser,
     bcl_convert_demux_metric_model_with_data: DemuxMetrics,
 ):
     """Test to parse BCLConvert demux metrics."""
     # GIVEN a parsed BCLConvert metrics
 
     # ASSERT that the parsed demux metrics are correct
```

### Comparing `cg-60.3.1/tests/apps/sequencing_metrics_parser/parsers/test_sequencing_metrics_parser_api.py` & `cg-60.3.2/tests/apps/sequencing_metrics_parser/parsers/test_sequencing_metrics_parser_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,24 +33,22 @@
     assert (
         len(sequencing_statistics_list)
         == len(parsed_bcl_convert_metrics.get_sample_internal_ids()) * 2
     )
 
 
 def test_create_undetermined_non_pooled_metrics(
-    bcl_convert_flow_cell: FlowCellDirectoryData,
+    hiseq_x_single_index_demultiplexed_flow_cell_with_sample_sheet: FlowCellDirectoryData,
 ):
     """Test creating undetermined sequencing statistics from demultiplex metrics."""
     # GIVEN a directory with a demultiplexed flow cell with undetermined reads
-    sample_sheet_path = Path(bcl_convert_flow_cell.path, "SampleSheet.csv")
-    bcl_convert_flow_cell.set_sample_sheet_path_hk(hk_path=sample_sheet_path)
 
     # WHEN creating undetermined sequencing statistics from bcl convert metrics
     metrics: list[SampleLaneSequencingMetrics] = create_undetermined_non_pooled_metrics(
-        flow_cell=bcl_convert_flow_cell
+        flow_cell=hiseq_x_single_index_demultiplexed_flow_cell_with_sample_sheet
     )
 
     # THEN metrics are created for the undetermined reads
     assert isinstance(metrics, list)
     assert isinstance(metrics[0], SampleLaneSequencingMetrics)
```

### Comparing `cg-60.3.1/tests/apps/slurm/conftest.py` & `cg-60.3.2/tests/apps/slurm/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/slurm/test_slurm_api.py` & `cg-60.3.2/tests/apps/slurm/test_slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/test_apps_environ.py` & `cg-60.3.2/tests/apps/test_apps_environ.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/apps/test_osticket.py` & `cg-60.3.2/tests/apps/test_osticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/add/test_cli_add.py` & `cg-60.3.2/tests/cli/add/test_cli_add.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/add/test_cli_add_customer.py` & `cg-60.3.2/tests/cli/add/test_cli_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/add/test_cli_add_family.py` & `cg-60.3.2/tests/cli/add/test_cli_add_family.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/add/test_cli_add_relationship.py` & `cg-60.3.2/tests/cli/add/test_cli_add_relationship.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/add/test_cli_add_sample.py` & `cg-60.3.2/tests/cli/add/test_cli_add_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/backup/conftest.py` & `cg-60.3.2/tests/cli/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/backup/test_backup_command.py` & `cg-60.3.2/tests/cli/backup/test_backup_command.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/clean/conftest.py` & `cg-60.3.2/tests/cli/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/clean/test_balsamic_clean.py` & `cg-60.3.2/tests/cli/clean/test_balsamic_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/clean/test_clean_flow_cell.py` & `cg-60.3.2/tests/cli/clean/test_clean_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/clean/test_clean_hk_bundle_files.py` & `cg-60.3.2/tests/cli/clean/test_clean_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/clean/test_hk_bundle_files.py` & `cg-60.3.2/tests/cli/clean/test_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/clean/test_hk_case_bundle_files.py` & `cg-60.3.2/tests/cli/clean/test_hk_case_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/clean/test_microbial_clean.py` & `cg-60.3.2/tests/cli/clean/test_microbial_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/clean/test_rsync_past_run_dirs.py` & `cg-60.3.2/tests/cli/clean/test_rsync_past_run_dirs.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/compress/conftest.py` & `cg-60.3.2/tests/cli/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/compress/test_cli_compress_fastq.py` & `cg-60.3.2/tests/cli/compress/test_cli_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/compress/test_cli_decompress_spring.py` & `cg-60.3.2/tests/cli/compress/test_cli_decompress_spring.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/compress/test_compress_helpers.py` & `cg-60.3.2/tests/cli/compress/test_compress_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/compress/test_store_fastq.py` & `cg-60.3.2/tests/cli/compress/test_store_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/conftest.py` & `cg-60.3.2/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/delete/test_cli_delete_case.py` & `cg-60.3.2/tests/cli/delete/test_cli_delete_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/delete/test_cli_delete_cases.py` & `cg-60.3.2/tests/cli/delete/test_cli_delete_cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/deliver/conftest.py` & `cg-60.3.2/tests/cli/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/deliver/test_deliver_base.py` & `cg-60.3.2/tests/cli/deliver/test_deliver_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/deliver/test_rsync_base.py` & `cg-60.3.2/tests/cli/deliver/test_rsync_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/deliver/test_run_deliver_cmd.py` & `cg-60.3.2/tests/cli/deliver/test_run_deliver_cmd.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/demultiplex/test_create_sample_sheet.py` & `cg-60.3.2/tests/cli/demultiplex/test_create_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/demultiplex/test_demultiplex_flowcell.py` & `cg-60.3.2/tests/cli/demultiplex/test_demultiplex_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/demultiplex/test_finish_demux.py` & `cg-60.3.2/tests/cli/demultiplex/test_finish_demux.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/demultiplex/test_validate_sample_sheet.py` & `cg-60.3.2/tests/cli/demultiplex/test_validate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/demultiplex/test_verify_syncing.py` & `cg-60.3.2/tests/cli/demultiplex/test_verify_syncing.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/downsample/test_cli_downsample.py` & `cg-60.3.2/tests/cli/downsample/test_cli_downsample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/generate/report/conftest.py` & `cg-60.3.2/tests/cli/generate/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/generate/report/test_cli_delivery_report.py` & `cg-60.3.2/tests/cli/generate/report/test_cli_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/generate/report/test_utils.py` & `cg-60.3.2/tests/cli/generate/report/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/generate/test_cli_base.py` & `cg-60.3.2/tests/cli/generate/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/get/test_cli_get.py` & `cg-60.3.2/tests/cli/get/test_cli_get.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/get/test_cli_get_analysis.py` & `cg-60.3.2/tests/cli/get/test_cli_get_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/get/test_cli_get_case.py` & `cg-60.3.2/tests/cli/get/test_cli_get_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/get/test_cli_get_flow_cell.py` & `cg-60.3.2/tests/cli/get/test_cli_get_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/get/test_cli_get_sample.py` & `cg-60.3.2/tests/cli/get/test_cli_get_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/set/conftest.py` & `cg-60.3.2/tests/cli/set/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/set/test_cli_set_case.py` & `cg-60.3.2/tests/cli/set/test_cli_set_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/set/test_cli_set_cases.py` & `cg-60.3.2/tests/cli/set/test_cli_set_cases.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/set/test_cli_set_flowcell.py` & `cg-60.3.2/tests/cli/set/test_cli_set_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/set/test_cli_set_list_keys.py` & `cg-60.3.2/tests/cli/set/test_cli_set_list_keys.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/set/test_cli_set_sample.py` & `cg-60.3.2/tests/cli/set/test_cli_set_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/set/test_cli_set_samples.py` & `cg-60.3.2/tests/cli/set/test_cli_set_samples.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/store/test_store.py` & `cg-60.3.2/tests/cli/store/test_store.py`

 * *Files 5% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     # THEN assert that we log that we stored FASTQ files
     assert f"Stored fastq files for {sample_id}" in caplog.text
 
 
 def test_store_flow_cell(
     caplog,
     cli_runner: CliRunner,
-    bcl2fastq_flow_cell_id: str,
+    novaseq_6000_pre_1_5_kits_flow_cell_id: str,
     mocker,
     populated_compress_context: CGConfig,
     sample_id: str,
 ):
     """Test to run store flow cell command."""
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a sample
@@ -137,15 +137,15 @@
 
     # GIVEN that decompression is not finished
     mocker.patch.object(CompressAPI, "add_decompressed_fastq")
     CompressAPI.add_decompressed_fastq.return_value = True
 
     # WHEN running the store flow cell command
     res = cli_runner.invoke(
-        store_flow_cell, [bcl2fastq_flow_cell_id], obj=populated_compress_context
+        store_flow_cell, [novaseq_6000_pre_1_5_kits_flow_cell_id], obj=populated_compress_context
     )
 
     # THEN assert that the command exits successfully
     assert res.exit_code == EXIT_SUCCESS
 
     # THEN assert that we log that we stored FASTQ files
     assert f"Stored fastq files for {sample_id}" in caplog.text
@@ -176,15 +176,15 @@
     # THEN assert that we log that we stored FASTQ files
     assert f"Stored fastq files for {sample_id}" in caplog.text
 
 
 def test_store_store_demultiplexed_flow_cell(
     caplog,
     cli_runner: CliRunner,
-    bcl2fastq_flow_cell_id: str,
+    novaseq_6000_pre_1_5_kits_flow_cell_id: str,
     helpers,
     mocker,
     real_populated_compress_context: CGConfig,
     sample_id: str,
 ):
     """Test to run store demultiplexed flow cell command."""
     caplog.set_level(logging.DEBUG)
@@ -196,12 +196,14 @@
     Store.get_samples_from_flow_cell.return_value = [sample]
 
     # GIVEN an updated metadata file
     mocker.patch("cg.cli.store.store.update_metadata_paths", return_value=None)
 
     # WHEN running the store demultiplexed flow cell command
     res = cli_runner.invoke(
-        store_demultiplexed_flow_cell, [bcl2fastq_flow_cell_id], obj=real_populated_compress_context
+        store_demultiplexed_flow_cell,
+        [novaseq_6000_pre_1_5_kits_flow_cell_id],
+        obj=real_populated_compress_context,
     )
 
     # THEN assert that the command exits successfully
     assert res.exit_code == EXIT_SUCCESS
```

### Comparing `cg-60.3.1/tests/cli/test_base.py` & `cg-60.3.2/tests/cli/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/upload/conftest.py` & `cg-60.3.2/tests/cli/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/upload/test_cli_scout.py` & `cg-60.3.2/tests/cli/upload/test_cli_scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/upload/test_cli_upload.py` & `cg-60.3.2/tests/cli/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/upload/test_cli_upload_auto.py` & `cg-60.3.2/tests/cli/upload/test_cli_upload_auto.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/upload/test_cli_upload_delivery_report.py` & `cg-60.3.2/tests/cli/upload/test_cli_upload_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/upload/test_cli_upload_fastq.py` & `cg-60.3.2/tests/cli/upload/test_cli_upload_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/upload/test_cli_upload_genotype.py` & `cg-60.3.2/tests/cli/upload/test_cli_upload_genotype.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/upload/test_cli_upload_gens.py` & `cg-60.3.2/tests/cli/upload/test_cli_upload_gens.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/upload/test_cli_upload_nipt.py` & `cg-60.3.2/tests/cli/upload/test_cli_upload_nipt.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/upload/test_cli_upload_nipt_ftp.py` & `cg-60.3.2/tests/cli/upload/test_cli_upload_nipt_ftp.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/upload/test_cli_upload_nipt_statina.py` & `cg-60.3.2/tests/cli/upload/test_cli_upload_nipt_statina.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/upload/test_cli_upload_observations.py` & `cg-60.3.2/tests/cli/upload/test_cli_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/balsamic/conftest.py` & `cg-60.3.2/tests/cli/workflow/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py` & `cg-60.3.2/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/balsamic/test_compound_commands.py` & `cg-60.3.2/tests/cli/workflow/balsamic/test_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/balsamic/test_link.py` & `cg-60.3.2/tests/cli/workflow/balsamic/test_link.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/balsamic/test_report_deliver.py` & `cg-60.3.2/tests/cli/workflow/balsamic/test_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/balsamic/test_run.py` & `cg-60.3.2/tests/cli/workflow/balsamic/test_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/balsamic/test_store_housekeeper.py` & `cg-60.3.2/tests/cli/workflow/balsamic/test_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/conftest.py` & `cg-60.3.2/tests/cli/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/fastq/test_fastq_base.py` & `cg-60.3.2/tests/cli/workflow/fastq/test_fastq_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/fluffy/conftest.py` & `cg-60.3.2/tests/cli/workflow/fluffy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py` & `cg-60.3.2/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/fluffy/test_cli_link.py` & `cg-60.3.2/tests/cli/workflow/fluffy/test_cli_link.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/fluffy/test_cli_run.py` & `cg-60.3.2/tests/cli/workflow/fluffy/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/fluffy/test_cli_start.py` & `cg-60.3.2/tests/cli/workflow/fluffy/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/fluffy/test_cli_store.py` & `cg-60.3.2/tests/cli/workflow/fluffy/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/microsalt/conftest.py` & `cg-60.3.2/tests/cli/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/microsalt/test_microsalt_case_config.py` & `cg-60.3.2/tests/cli/workflow/microsalt/test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/microsalt/test_microsalt_run.py` & `cg-60.3.2/tests/cli/workflow/microsalt/test_microsalt_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/mip/conftest.py` & `cg-60.3.2/tests/cli/workflow/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_base.py` & `cg-60.3.2/tests/cli/workflow/mip/test_cli_mip_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py` & `cg-60.3.2/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py` & `cg-60.3.2/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_dna_panel.py` & `cg-60.3.2/tests/cli/workflow/mip/test_cli_mip_dna_panel.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_dna_run.py` & `cg-60.3.2/tests/cli/workflow/mip/test_cli_mip_dna_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_dna_start.py` & `cg-60.3.2/tests/cli/workflow/mip/test_cli_mip_dna_start.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py` & `cg-60.3.2/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_rna_link.py` & `cg-60.3.2/tests/cli/workflow/mip/test_cli_mip_rna_link.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_rna_run.py` & `cg-60.3.2/tests/cli/workflow/mip/test_cli_mip_rna_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/mip/test_cli_mip_store.py` & `cg-60.3.2/tests/cli/workflow/mip/test_cli_mip_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_config_case.py` & `cg-60.3.2/tests/cli/workflow/nf_analysis/test_cli_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py` & `cg-60.3.2/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py` & `cg-60.3.2/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_run.py` & `cg-60.3.2/tests/cli/workflow/nf_analysis/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_start.py` & `cg-60.3.2/tests/cli/workflow/nf_analysis/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_store.py` & `cg-60.3.2/tests/cli/workflow/nf_analysis/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py` & `cg-60.3.2/tests/cli/workflow/nf_analysis/test_cli_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py` & `cg-60.3.2/tests/cli/workflow/nf_analysis/test_cli_workflow_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py` & `cg-60.3.2/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/test_cli_workflow.py` & `cg-60.3.2/tests/cli/workflow/test_cli_workflow.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/cli/workflow/test_cli_workflow_clean.py` & `cg-60.3.2/tests/cli/workflow/test_cli_workflow_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/clients/arnold/conftest.py` & `cg-60.3.2/tests/clients/arnold/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/clients/arnold/test_arnold_api_client.py` & `cg-60.3.2/tests/clients/arnold/test_arnold_api_client.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/clients/janus/conftest.py` & `cg-60.3.2/tests/clients/janus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/clients/janus/test_janus_api_client.py` & `cg-60.3.2/tests/clients/janus/test_janus_api_client.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/conftest.py` & `cg-60.3.2/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1245,40 +1245,36 @@
     yield base_store
 
 
 @pytest.fixture
 def store_with_demultiplexed_samples(
     store: Store,
     helpers: StoreHelpers,
-    bcl_convert_demultiplexed_flow_cell_sample_internal_ids: list[str],
-    bcl2fastq_demultiplexed_flow_cell_sample_internal_ids: list[str],
-    flow_cell_name_demultiplexed_with_bcl2fastq: str,
-    flow_cell_name_demultiplexed_with_bcl_convert: str,
+    selected_novaseq_6000_post_1_5_kits_sample_ids: list[str],
+    selected_hiseq_x_dual_index_sample_ids: list[str],
+    hiseq_x_dual_index_flow_cell_id: str,
+    novaseq_6000_post_1_5_kits_flow_cell_id: str,
 ) -> Store:
     """Return a store with samples that have been demultiplexed with BCL Convert and BCL2Fastq."""
-    helpers.add_flow_cell(
-        store, flow_cell_name_demultiplexed_with_bcl_convert, sequencer_type="novaseq"
-    )
-    helpers.add_flow_cell(
-        store, flow_cell_name_demultiplexed_with_bcl2fastq, sequencer_type="hiseqx"
-    )
-    for i, sample_internal_id in enumerate(bcl_convert_demultiplexed_flow_cell_sample_internal_ids):
+    helpers.add_flow_cell(store, novaseq_6000_post_1_5_kits_flow_cell_id, sequencer_type="novaseq")
+    helpers.add_flow_cell(store, hiseq_x_dual_index_flow_cell_id, sequencer_type="hiseqx")
+    for i, sample_internal_id in enumerate(selected_novaseq_6000_post_1_5_kits_sample_ids):
         helpers.add_sample(store, internal_id=sample_internal_id, name=f"sample_bcl_convert_{i}")
         helpers.ensure_sample_lane_sequencing_metrics(
             store,
             sample_internal_id=sample_internal_id,
-            flow_cell_name=flow_cell_name_demultiplexed_with_bcl_convert,
+            flow_cell_name=novaseq_6000_post_1_5_kits_flow_cell_id,
         )
 
-    for i, sample_internal_id in enumerate(bcl2fastq_demultiplexed_flow_cell_sample_internal_ids):
+    for i, sample_internal_id in enumerate(selected_hiseq_x_dual_index_sample_ids):
         helpers.add_sample(store, internal_id=sample_internal_id, name=f"sample_bcl2fastq_{i}")
         helpers.ensure_sample_lane_sequencing_metrics(
             store,
             sample_internal_id=sample_internal_id,
-            flow_cell_name=flow_cell_name_demultiplexed_with_bcl2fastq,
+            flow_cell_name=hiseq_x_dual_index_flow_cell_id,
         )
     return store
 
 
 @pytest.fixture
 def updated_store_with_demultiplexed_samples(
     store: Store,
@@ -3731,20 +3727,14 @@
 
 @pytest.fixture(scope="session")
 def expected_total_reads() -> int:
     return 1_000_000
 
 
 @pytest.fixture
-def flow_cell_name() -> str:
-    """Return flow cell name."""
-    return "HVKJCDRXX"
-
-
-@pytest.fixture
 def flow_cell_full_name(flow_cell_name: str) -> str:
     """Return flow cell full name."""
     return f"201203_D00483_0200_A{flow_cell_name}"
 
 
 @pytest.fixture(name="expected_average_q30_for_sample")
 def expected_average_q30_for_sample() -> float:
@@ -3767,28 +3757,28 @@
 def store_with_sequencing_metrics(
     store: Store,
     sample_id: str,
     father_sample_id: str,
     mother_sample_id: str,
     expected_total_reads: int,
     flow_cell_name: str,
-    flow_cell_name_demultiplexed_with_bcl_convert: str,
-    flow_cell_name_demultiplexed_with_bcl2fastq: str,
+    novaseq_6000_post_1_5_kits_flow_cell_id: str,
+    hiseq_x_dual_index_flow_cell_id: str,
     helpers: StoreHelpers,
 ) -> Store:
     """Return a store with multiple samples with sample lane sequencing metrics."""
     sample_sequencing_metrics_details: list[str | int | float] = [
         (sample_id, flow_cell_name, 1, expected_total_reads / 2, 90.5, 32),
         (sample_id, flow_cell_name, 2, expected_total_reads / 2, 90.4, 31),
-        (mother_sample_id, flow_cell_name_demultiplexed_with_bcl2fastq, 2, 2_000_000, 85.5, 30),
-        (mother_sample_id, flow_cell_name_demultiplexed_with_bcl2fastq, 1, 2_000_000, 80.5, 30),
-        (father_sample_id, flow_cell_name_demultiplexed_with_bcl2fastq, 2, 2_000_000, 83.5, 30),
-        (father_sample_id, flow_cell_name_demultiplexed_with_bcl2fastq, 1, 2_000_000, 81.5, 30),
-        (mother_sample_id, flow_cell_name_demultiplexed_with_bcl_convert, 3, 1_500_000, 80.5, 33),
-        (mother_sample_id, flow_cell_name_demultiplexed_with_bcl_convert, 2, 1_500_000, 80.5, 33),
+        (mother_sample_id, hiseq_x_dual_index_flow_cell_id, 2, 2_000_000, 85.5, 30),
+        (mother_sample_id, hiseq_x_dual_index_flow_cell_id, 1, 2_000_000, 80.5, 30),
+        (father_sample_id, hiseq_x_dual_index_flow_cell_id, 2, 2_000_000, 83.5, 30),
+        (father_sample_id, hiseq_x_dual_index_flow_cell_id, 1, 2_000_000, 81.5, 30),
+        (mother_sample_id, novaseq_6000_post_1_5_kits_flow_cell_id, 3, 1_500_000, 80.5, 33),
+        (mother_sample_id, novaseq_6000_post_1_5_kits_flow_cell_id, 2, 1_500_000, 80.5, 33),
     ]
     helpers.add_flow_cell(store=store, flow_cell_name=flow_cell_name)
     helpers.add_sample(
         store=store, customer_id="cust500", internal_id=sample_id, name=sample_id, sex=Sex.MALE
     )
     helpers.add_multiple_sample_lane_sequencing_metrics_entries(
         metrics_data=sample_sequencing_metrics_details, store=store
```

### Comparing `cg-60.3.1/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py` & `cg-60.3.2/tests/fixture_plugins/delivery_fixtures/bundle_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixture_plugins/delivery_fixtures/context_fixtures.py` & `cg-60.3.2/tests/fixture_plugins/delivery_fixtures/context_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixture_plugins/delivery_fixtures/path_fixtures.py` & `cg-60.3.2/tests/fixture_plugins/delivery_fixtures/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py` & `cg-60.3.2/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 import pytest
 
 from cg.constants.demultiplexing import DemultiplexingDirsAndFiles
 from cg.models.flow_cell.flow_cell import FlowCellDirectoryData
 
-# Functional flow cell runs
+# Canonical flow cell runs
 
 
 @pytest.fixture(scope="module")
 def hiseq_x_single_index_flow_cell(
     hiseq_x_single_index_flow_cell_dir: Path,
 ) -> FlowCellDirectoryData:
     """Return a single-index HiSeqX flow cell."""
@@ -41,28 +41,30 @@
     """Return a custom-index HiSeq2500 flow cell."""
     return FlowCellDirectoryData(flow_cell_path=hiseq_2500_custom_index_flow_cell_dir)
 
 
 @pytest.fixture
 def novaseq_6000_pre_1_5_kits_flow_cell(
     illumina_flow_cells_directory: Path,
+    novaseq_6000_pre_1_5_kits_flow_cell_full_name: str,
 ) -> FlowCellDirectoryData:
     """Return a Novaseq6000 flow cell with index settings pre 1.5 kits."""
     return FlowCellDirectoryData(
-        Path(illumina_flow_cells_directory, "190927_A00689_0069_BHLYWYDSXX")
+        Path(illumina_flow_cells_directory, novaseq_6000_pre_1_5_kits_flow_cell_full_name)
     )
 
 
 @pytest.fixture
 def novaseq_6000_post_1_5_kits_flow_cell(
     illumina_flow_cells_directory: Path,
+    novaseq_6000_post_1_5_kits_flow_cell_full_name: str,
 ) -> FlowCellDirectoryData:
     """Return a Novaseq6000 flow cell with index settings post 1.5 kits."""
     return FlowCellDirectoryData(
-        Path(illumina_flow_cells_directory, "230912_A00187_1009_AHK33MDRX3")
+        Path(illumina_flow_cells_directory, novaseq_6000_post_1_5_kits_flow_cell_full_name)
     )
 
 
 @pytest.fixture
 def novaseq_x_flow_cell(novaseq_x_flow_cell_dir: Path) -> FlowCellDirectoryData:
     """Return a NovaSeqX flow cell."""
     return FlowCellDirectoryData(novaseq_x_flow_cell_dir)
@@ -110,29 +112,17 @@
     tmp_flow_cell_directory_bclconvert: Path,
 ) -> FlowCellDirectoryData:
     """Create a flow cell object with flow cell that is demultiplexed."""
     return FlowCellDirectoryData(tmp_flow_cell_directory_bclconvert)
 
 
 @pytest.fixture
-def bcl_convert_flow_cell(
-    bclconvert_flow_cell_dir_name: Path,
+def hiseq_x_single_index_demultiplexed_flow_cell_with_sample_sheet(
     illumina_demultiplexed_runs_directory: Path,
+    hiseq_x_single_index_flow_cell_name: str,
+    hiseq_x_single_index_sample_sheet_path: Path,
 ) -> FlowCellDirectoryData:
-    """Return a flow cell object with flow cell that is demultiplexed."""
-    path = Path(illumina_demultiplexed_runs_directory, bclconvert_flow_cell_dir_name)
-    return FlowCellDirectoryData(flow_cell_path=path)
-
-
-# Flow cell attributes
-
-
-@pytest.fixture
-def bcl2fastq_flow_cell_id() -> str:
-    """Return flow cell id from bcl2fastq flow cell object."""
-    return "HLYWYDSXX"
-
-
-@pytest.fixture
-def bcl_convert_flow_cell_id(novaseq_6000_post_1_5_kits_flow_cell: FlowCellDirectoryData) -> str:
-    """Return flow cell id from bcl_convert flow cell object."""
-    return novaseq_6000_post_1_5_kits_flow_cell.id
+    """Return a Novaseq6000 flow cell with a sample sheet."""
+    path = Path(illumina_demultiplexed_runs_directory, hiseq_x_single_index_flow_cell_name)
+    flow_cell = FlowCellDirectoryData(path)
+    flow_cell.set_sample_sheet_path_hk(hiseq_x_single_index_sample_sheet_path)
+    return flow_cell
```

### Comparing `cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py` & `cg-60.3.2/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py`

 * *Files 12% similar despite different names*

```diff
@@ -119,41 +119,21 @@
     tmp_broken_flow_cells_directory: Path,
 ) -> Path:
     """This is a path to a flow cell directory with the sample sheet missing."""
     return Path(tmp_broken_flow_cells_directory, "20231108_LH00188_0028_B22F52TLT3")
 
 
 @pytest.fixture
-def tmp_flow_cells_directory_malformed_sample_sheet(
-    tmp_flow_cell_name_malformed_sample_sheet: str, tmp_illumina_flow_cells_directory
-) -> Path:
-    """This is a path to a flow cell directory with a sample sheet with malformed headers."""
-    return Path(tmp_illumina_flow_cells_directory, tmp_flow_cell_name_malformed_sample_sheet)
-
-
-@pytest.fixture
 def tmp_flow_cells_directory_ready_for_demultiplexing_bcl_convert(
     bcl_convert_flow_cell_full_name: str, tmp_illumina_flow_cells_directory
 ) -> Path:
     """This is a path to a flow cell directory with the run parameters missing."""
     return Path(tmp_illumina_flow_cells_directory, bcl_convert_flow_cell_full_name)
 
 
-@pytest.fixture
-def tmp_flow_cells_directory_ready_for_demultiplexing_bcl2fastq(
-    tmp_flow_cell_name_ready_for_demultiplexing_bcl2fastq: str,
-    tmp_illumina_flow_cells_directory,
-) -> Path:
-    """This is a path to a flow cell directory with the run parameters missing."""
-    return Path(
-        tmp_illumina_flow_cells_directory,
-        tmp_flow_cell_name_ready_for_demultiplexing_bcl2fastq,
-    )
-
-
 # Temporary demultiplexed runs fixtures
 @pytest.fixture
 def tmp_illumina_demultiplexed_flow_cells_directory(
     tmp_path: Path, illumina_demultiplexed_runs_directory
 ) -> Path:
     """Return the path to a temporary demultiplex-runs directory.
     Generates a copy of the original demultiplexed-runs
@@ -201,29 +181,14 @@
     tmp_demultiplexed_runs_not_finished_directory: Path,
     bcl2fastq_flow_cell_full_name: str,
 ) -> Path:
     """Copy the content of a demultiplexed but not finished directory to a temporary location."""
     return Path(tmp_demultiplexed_runs_not_finished_directory, bcl2fastq_flow_cell_full_name)
 
 
-@pytest.fixture
-def novaseq6000_bcl_convert_sample_sheet_path() -> Path:
-    """Return the path to a NovaSeq 6000 BCL convert sample sheet."""
-    return Path(
-        "tests",
-        "fixtures",
-        "apps",
-        "sequencing_metrics_parser",
-        "230622_A00621_0864_AHY7FFDRX2",
-        "Unaligned",
-        "Reports",
-        "SampleSheet.csv",
-    )
-
-
 # Directory fixtures
 
 
 @pytest.fixture(scope="session")
 def demultiplex_fixtures(apps_dir: Path) -> Path:
     """Return the path to the demultiplex fixture directory."""
     return Path(apps_dir, "demultiplexing")
@@ -283,16 +248,18 @@
     return Path(demultiplex_fixtures, "demultiplexed-runs-unfinished")
 
 
 ###
 
 
 @pytest.fixture
-def novaseq_6000_post_1_5_kits_flow_cell_path(tmp_illumina_flow_cells_directory: Path) -> Path:
-    return Path(tmp_illumina_flow_cells_directory, "230912_A00187_1009_AHK33MDRX3")
+def novaseq_6000_post_1_5_kits_flow_cell_path(
+    tmp_illumina_flow_cells_directory: Path, novaseq_6000_post_1_5_kits_flow_cell_full_name: str
+) -> Path:
+    return Path(tmp_illumina_flow_cells_directory, novaseq_6000_post_1_5_kits_flow_cell_full_name)
 
 
 @pytest.fixture
 def novaseq_6000_post_1_5_kits_correct_sample_sheet_path(
     novaseq_6000_post_1_5_kits_flow_cell_path: Path,
 ) -> Path:
     return Path(novaseq_6000_post_1_5_kits_flow_cell_path, CORRECT_SAMPLE_SHEET)
@@ -338,46 +305,28 @@
 def hiseq_x_single_index_sample_sheet_path(hiseq_x_single_index_flow_cell_dir: Path) -> Path:
     """Return the path to a single-index HiSeqX sample sheet."""
     return Path(
         hiseq_x_single_index_flow_cell_dir, DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME
     )
 
 
-@pytest.fixture
-def hiseq_x_single_index_bcl2fastq_sample_sheet_path(
-    hiseq_x_single_index_flow_cell_dir: Path,
-    bcl2fastq_sample_sheet_file_name: str,
-) -> Path:
-    """Return the path to a single-index HiSeqX Bcl2fastq sample sheet."""
-    return Path(hiseq_x_single_index_flow_cell_dir, bcl2fastq_sample_sheet_file_name)
-
-
 @pytest.fixture(scope="session")
 def hiseq_x_dual_index_flow_cell_dir(
     illumina_flow_cells_directory, hiseq_x_dual_index_flow_cell_name: str
 ) -> Path:
     """Return the path to a dual-index HiSeqX flow cell."""
     return Path(illumina_flow_cells_directory, hiseq_x_dual_index_flow_cell_name)
 
 
 @pytest.fixture
 def hiseq_x_dual_index_sample_sheet_path(hiseq_x_dual_index_flow_cell_dir: Path) -> Path:
     """Return the path to a dual-index HiSeqX sample sheet."""
     return Path(hiseq_x_dual_index_flow_cell_dir, DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME)
 
 
-@pytest.fixture
-def hiseq_x_dual_index_bcl2fastq_sample_sheet_path(
-    hiseq_x_dual_index_flow_cell_dir: Path,
-    bcl2fastq_sample_sheet_file_name: str,
-) -> Path:
-    """Return the path to a dual-index HiSeqX Bcl2fastq sample sheet."""
-    return Path(hiseq_x_dual_index_flow_cell_dir, bcl2fastq_sample_sheet_file_name)
-
-
 @pytest.fixture(scope="session")
 def hiseq_2500_dual_index_flow_cell_dir(
     illumina_flow_cells_directory, hiseq_2500_dual_index_flow_cell_name: str
 ) -> Path:
     """Return the path to a HiSeq2500 flow cell."""
     return Path(illumina_flow_cells_directory, hiseq_2500_dual_index_flow_cell_name)
 
@@ -386,23 +335,14 @@
 def hiseq_2500_dual_index_sample_sheet_path(hiseq_2500_dual_index_flow_cell_dir: Path) -> Path:
     """Return the path to a dual-index HiSeq2500 sample sheet."""
     return Path(
         hiseq_2500_dual_index_flow_cell_dir, DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME
     )
 
 
-@pytest.fixture
-def hiseq_2500_dual_index_bcl2fastq_sample_sheet_path(
-    hiseq_2500_dual_index_flow_cell_dir: Path,
-    bcl2fastq_sample_sheet_file_name: str,
-) -> Path:
-    """Return the path to a dual-index HiSeq2500 Bcl2fastq sample sheet."""
-    return Path(hiseq_2500_dual_index_flow_cell_dir, bcl2fastq_sample_sheet_file_name)
-
-
 @pytest.fixture(scope="session")
 def hiseq_2500_custom_index_flow_cell_dir(
     illumina_flow_cells_directory, hiseq_2500_custom_index_flow_cell_name: str
 ) -> Path:
     """Return the path to a HiSeq2500 flow cell."""
     return Path(illumina_flow_cells_directory, hiseq_2500_custom_index_flow_cell_name)
 
@@ -412,23 +352,14 @@
     """Return the path to a custom-index HiSeq2500 sample sheet."""
     return Path(
         hiseq_2500_custom_index_flow_cell_dir, DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME
     )
 
 
 @pytest.fixture
-def hiseq_2500_custom_index_bcl2fastq_sample_sheet_path(
-    hiseq_2500_custom_index_flow_cell_dir: Path,
-    bcl2fastq_sample_sheet_file_name: str,
-) -> Path:
-    """Return the path to a custom-index HiSeq2500 Bcl2fastq sample sheet."""
-    return Path(hiseq_2500_custom_index_flow_cell_dir, bcl2fastq_sample_sheet_file_name)
-
-
-@pytest.fixture
 def novaseq_x_flow_cell_dir(illumina_flow_cells_directory: Path) -> Path:
     """Return the path to a NovaSeqX flow cell."""
     return Path(illumina_flow_cells_directory, "20231108_LH00188_0028_B22F52TLT3")
 
 
 @pytest.fixture(scope="session")
 def bcl2fastq_flow_cell_dir(
@@ -442,26 +373,14 @@
 def bcl_convert_flow_cell_dir(
     illumina_flow_cells_directory, bcl_convert_flow_cell_full_name: str
 ) -> Path:
     """Return the path to the bcl_convert flow cell demultiplex fixture directory."""
     return Path(illumina_flow_cells_directory, bcl_convert_flow_cell_full_name)
 
 
-@pytest.fixture(scope="session")
-def novaseq_bcl2fastq_sample_sheet_path(bcl2fastq_flow_cell_dir: Path) -> Path:
-    """Return the path to a NovaSeq6000 Bcl2fastq sample sheet."""
-    return Path(bcl2fastq_flow_cell_dir, DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME)
-
-
-@pytest.fixture(scope="session")
-def novaseq_bcl_convert_sample_sheet_path(bcl_convert_flow_cell_dir: Path) -> Path:
-    """Return the path to a NovaSeq6000 bcl_convert sample sheet."""
-    return Path(bcl_convert_flow_cell_dir, DemultiplexingDirsAndFiles.SAMPLE_SHEET_FILE_NAME)
-
-
 @pytest.fixture
 def novaseq_6000_sample_sheet_with_reversed_cycles(sample_sheet_dir: Path) -> Path:
     """Return the path to a NovaSeq6000 sample sheet with reversed index2 cycles."""
     return Path(sample_sheet_dir, "novaseq_6000_sample_sheet_with_reversed_cycles.csv")
 
 
 @pytest.fixture
@@ -574,22 +493,14 @@
 def demultiplexed_flow_cell(
     illumina_demultiplexed_runs_directory, bcl2fastq_flow_cell_full_name: str
 ) -> Path:
     """Return the path to a demultiplexed flow cell with bcl2fastq."""
     return Path(illumina_demultiplexed_runs_directory, bcl2fastq_flow_cell_full_name)
 
 
-@pytest.fixture
-def bcl_convert_demultiplexed_flow_cell(
-    illumina_demultiplexed_runs_directory, bcl_convert_flow_cell_full_name: str
-) -> Path:
-    """Return the path to a demultiplexed flow cell with BCLConvert."""
-    return Path(illumina_demultiplexed_runs_directory, bcl_convert_flow_cell_full_name)
-
-
 # Fixtures for test demultiplex flow cell
 @pytest.fixture
 def tmp_empty_demultiplexed_runs_directory(
     tmp_illumina_demultiplexed_flow_cells_directory,
 ) -> Path:
     return Path(tmp_illumina_demultiplexed_flow_cells_directory, "empty")
```

### Comparing `cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py` & `cg-60.3.2/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py` & `cg-60.3.2/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixture_plugins/timestamp_fixtures.py` & `cg-60.3.2/tests/fixture_plugins/timestamp_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json` & `cg-60.3.2/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json` & `cg-60.3.2/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/analysis/raredisease/multiqc_data.json` & `cg-60.3.2/tests/fixtures/analysis/raredisease/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml` & `cg-60.3.2/tests/fixtures/analysis/raredisease/raredisease_case_enough_reads_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/analysis/rnafusion/multiqc_data.json` & `cg-60.3.2/tests/fixtures/analysis/rnafusion/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml` & `cg-60.3.2/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/analysis/sample_coverage.bed` & `cg-60.3.2/tests/fixtures/analysis/sample_coverage.bed`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/analysis/taxprofiler/multiqc_data.json` & `cg-60.3.2/tests/fixtures/analysis/taxprofiler/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml` & `cg-60.3.2/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/analysis/tomte/multiqc_data.json` & `cg-60.3.2/tests/fixtures/analysis/tomte/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml` & `cg-60.3.2/tests/fixtures/analysis/tomte/tomte_case_enough_reads_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/balsamic/case/config.json` & `cg-60.3.2/tests/fixtures/apps/balsamic/case/config.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/balsamic/case/metadata.yml` & `cg-60.3.2/tests/fixtures/apps/balsamic/case/metadata.yml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml` & `cg-60.3.2/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/crunchy/spring_metadata.json` & `cg-60.3.2/tests/fixtures/apps/crunchy/spring_metadata.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170517_ST-E00266_0210_BHJCFFALXX/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Demultiplex_Stats.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Quality_Metrics.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [Header]
 FileFormatVersion,2
-RunName,22522YLT3
-InstrumentPlatform,NovaSeqX
+RunName,HY7FFDRX2
+InstrumentPlatform,NovaSeq6000
 IndexOrientation,Forward
-IndexSettings,NovaSeqX
+IndexSettings,NovaSeq6000Post1.5Kits
 [Reads]
 Read1Cycles,51
 Read2Cycles,51
 Index1Cycles,8
 Index2Cycles,8
 [BCLConvert_Settings]
 SoftwareVersion,4.1.7
 FastqCompressionFormat,gzip
 [BCLConvert_Data]
 Lane,Sample_ID,Index,Index2,OverrideCycles,AdapterRead1,AdapterRead2,BarcodeMismatchesIndex1,BarcodeMismatchesIndex2
 1,ACC11927A2,TTGAATAG,GTTATGGA,Y51;I8;I8;Y51,,,1,1
-1,ACC11927A5,TCTGGCGA,GTTGAATT,Y51;I8;I8;Y51,,,1,1
 2,ACC11927A2,TTGAATAG,GTTATGGA,Y51;I8;I8;Y51,,,1,1
 2,ACC11927A5,TCTGGCGA,GTTGAATT,Y51;I8;I8;Y51,,,1,1
```

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv`

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

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv` & `cg-60.3.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stderr` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stdout` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RunParameters.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml`

 * *Files 7% similar despite different names*

#### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml`

```diff
@@ -1,65 +1,68 @@
 <?xml version="1.0" encoding="utf-8"?>
 <RunParameters xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
-  <Side>A</Side>
+  <Side>B</Side>
   <Application>control-software</Application>
-  <SystemSuiteVersion>1.0.1.7385</SystemSuiteVersion>
+  <SystemSuiteVersion>1.1.0.18335</SystemSuiteVersion>
   <CloudUploadMode>InstrumentPerformance</CloudUploadMode>
-  <InstrumentType>NovaSeqXPlus</InstrumentType>
+  <RunSetupMode>Manual</RunSetupMode>
+  <SecondaryAnalysisMode>None</SecondaryAnalysisMode>
+  <InstrumentType>Other</InstrumentType>
   <InstrumentSerialNumber>LH00188</InstrumentSerialNumber>
-  <RunId>20230508_LH00188_0003_A22522YLT3</RunId>
-  <RunCounter>3</RunCounter>
+  <RunId>20231108_LH00188_0028_B22F52TLT3</RunId>
+  <RunCounter>28</RunCounter>
   <RecipeName>10B Sequencing</RecipeName>
-  <RecipeVersion>10B-01.00.00</RecipeVersion>
-  <ExperimentName>22522YLT3</ExperimentName>
+  <RecipeVersion>10B-01.01.00</RecipeVersion>
+  <ExperimentName>22F52TLT3</ExperimentName>
   <FlowCellName>NovaSeqXSeries B3</FlowCellName>
   <FlowCellType>NovaSeqXSeriesB3</FlowCellType>
   <ScanSpeedMmPerSec>1.2345678</ScanSpeedMmPerSec>
   <ConsumableInfo>
     <ConsumableInfo>
-      <SerialNumber>22522YLT3</SerialNumber>
-      <LotNumber>20737128</LotNumber>
+      <SerialNumber>22F52TLT3</SerialNumber>
+      <LotNumber>20775712</LotNumber>
       <PartNumber>20080370</PartNumber>
-      <ExpirationDate>2024-02-28T00:00:00+01:00</ExpirationDate>
+      <ExpirationDate>2025-01-10T00:00:00+01:00</ExpirationDate>
       <Type>FlowCell</Type>
       <Mode>10B</Mode>
     </ConsumableInfo>
     <ConsumableInfo>
-      <SerialNumber>LC4001354-LC3</SerialNumber>
-      <LotNumber>20707596</LotNumber>
+      <SerialNumber>LC4035429-LC3</SerialNumber>
+      <LotNumber>20756816</LotNumber>
       <PartNumber>20066614</PartNumber>
-      <ExpirationDate>2023-12-14T00:00:00+01:00</ExpirationDate>
+      <ExpirationDate>2025-01-25T00:00:00+01:00</ExpirationDate>
       <Type>Reagent</Type>
       <Mode>10B</Mode>
     </ConsumableInfo>
     <ConsumableInfo>
-      <SerialNumber>LC2212060272-1</SerialNumber>
-      <LotNumber>22120701</LotNumber>
+      <SerialNumber>LC2308090505-1</SerialNumber>
+      <LotNumber>23080801</LotNumber>
       <PartNumber>20089853</PartNumber>
-      <ExpirationDate>2023-06-02T00:00:00+02:00</ExpirationDate>
+      <ExpirationDate>2025-02-09T00:00:00+01:00</ExpirationDate>
       <Type>Buffer</Type>
       <Mode>10B</Mode>
     </ConsumableInfo>
     <ConsumableInfo>
-      <SerialNumber>LC1006247-LC1</SerialNumber>
-      <LotNumber>1000015508</LotNumber>
+      <SerialNumber>LC1024891-LC1</SerialNumber>
+      <LotNumber>1000018777</LotNumber>
       <PartNumber>20072271</PartNumber>
-      <ExpirationDate>2024-03-25T00:00:00+01:00</ExpirationDate>
+      <ExpirationDate>2025-08-08T00:00:00+02:00</ExpirationDate>
       <Type>SampleTube</Type>
       <Mode>10B</Mode>
     </ConsumableInfo>
     <ConsumableInfo>
-      <SerialNumber>LC2000247-LC1</SerialNumber>
-      <LotNumber>17714646</LotNumber>
+      <SerialNumber>LC2006634-LC1</SerialNumber>
+      <LotNumber>17847279</LotNumber>
       <PartNumber>20081650</PartNumber>
-      <ExpirationDate>2023-11-08T00:00:00+01:00</ExpirationDate>
+      <ExpirationDate>2024-02-01T00:00:00+01:00</ExpirationDate>
       <Type>Lyo</Type>
       <Mode>10B</Mode>
     </ConsumableInfo>
   </ConsumableInfo>
   <PlannedReads>
     <Read ReadName="Read1" Cycles="151"/>
     <Read ReadName="Index1" Cycles="10"/>
-    <Read ReadName="Index2" Cycles="8"/>
+    <Read ReadName="Index2" Cycles="10"/>
     <Read ReadName="Read2" Cycles="151"/>
   </PlannedReads>
+  <SecondaryAnalysisInfo/>
 </RunParameters>
```

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml`

 * *Files 8% similar despite different names*

#### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml`

```diff
@@ -1,65 +1,68 @@
 <?xml version="1.0" encoding="utf-8"?>
 <RunParameters xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
-  <Side>A</Side>
+  <Side>B</Side>
   <Application>control-software</Application>
-  <SystemSuiteVersion>1.0.1.7385</SystemSuiteVersion>
+  <SystemSuiteVersion>1.1.0.18335</SystemSuiteVersion>
   <CloudUploadMode>InstrumentPerformance</CloudUploadMode>
-  <InstrumentType>Other</InstrumentType>
+  <RunSetupMode>Manual</RunSetupMode>
+  <SecondaryAnalysisMode>None</SecondaryAnalysisMode>
+  <InstrumentType>NovaSeqXPlus</InstrumentType>
   <InstrumentSerialNumber>LH00188</InstrumentSerialNumber>
-  <RunId>20230508_LH00188_0003_A22522YLT3</RunId>
-  <RunCounter>3</RunCounter>
+  <RunId>20231108_LH00188_0028_B22F52TLT3</RunId>
+  <RunCounter>28</RunCounter>
   <RecipeName>10B Sequencing</RecipeName>
-  <RecipeVersion>10B-01.00.00</RecipeVersion>
-  <ExperimentName>22522YLT3</ExperimentName>
+  <RecipeVersion>10B-01.01.00</RecipeVersion>
+  <ExperimentName>22F52TLT3</ExperimentName>
   <FlowCellName>NovaSeqXSeries B3</FlowCellName>
   <FlowCellType>NovaSeqXSeriesB3</FlowCellType>
   <ScanSpeedMmPerSec>1.2345678</ScanSpeedMmPerSec>
   <ConsumableInfo>
     <ConsumableInfo>
-      <SerialNumber>22522YLT3</SerialNumber>
-      <LotNumber>20737128</LotNumber>
+      <SerialNumber>22F52TLT3</SerialNumber>
+      <LotNumber>20775712</LotNumber>
       <PartNumber>20080370</PartNumber>
-      <ExpirationDate>2024-02-28T00:00:00+01:00</ExpirationDate>
+      <ExpirationDate>2025-01-10T00:00:00+01:00</ExpirationDate>
       <Type>FlowCell</Type>
       <Mode>10B</Mode>
     </ConsumableInfo>
     <ConsumableInfo>
-      <SerialNumber>LC4001354-LC3</SerialNumber>
-      <LotNumber>20707596</LotNumber>
+      <SerialNumber>LC4035429-LC3</SerialNumber>
+      <LotNumber>20756816</LotNumber>
       <PartNumber>20066614</PartNumber>
-      <ExpirationDate>2023-12-14T00:00:00+01:00</ExpirationDate>
+      <ExpirationDate>2025-01-25T00:00:00+01:00</ExpirationDate>
       <Type>Reagent</Type>
       <Mode>10B</Mode>
     </ConsumableInfo>
     <ConsumableInfo>
-      <SerialNumber>LC2212060272-1</SerialNumber>
-      <LotNumber>22120701</LotNumber>
+      <SerialNumber>LC2308090505-1</SerialNumber>
+      <LotNumber>23080801</LotNumber>
       <PartNumber>20089853</PartNumber>
-      <ExpirationDate>2023-06-02T00:00:00+02:00</ExpirationDate>
+      <ExpirationDate>2025-02-09T00:00:00+01:00</ExpirationDate>
       <Type>Buffer</Type>
       <Mode>10B</Mode>
     </ConsumableInfo>
     <ConsumableInfo>
-      <SerialNumber>LC1006247-LC1</SerialNumber>
-      <LotNumber>1000015508</LotNumber>
+      <SerialNumber>LC1024891-LC1</SerialNumber>
+      <LotNumber>1000018777</LotNumber>
       <PartNumber>20072271</PartNumber>
-      <ExpirationDate>2024-03-25T00:00:00+01:00</ExpirationDate>
+      <ExpirationDate>2025-08-08T00:00:00+02:00</ExpirationDate>
       <Type>SampleTube</Type>
       <Mode>10B</Mode>
     </ConsumableInfo>
     <ConsumableInfo>
-      <SerialNumber>LC2000247-LC1</SerialNumber>
-      <LotNumber>17714646</LotNumber>
+      <SerialNumber>LC2006634-LC1</SerialNumber>
+      <LotNumber>17847279</LotNumber>
       <PartNumber>20081650</PartNumber>
-      <ExpirationDate>2023-11-08T00:00:00+01:00</ExpirationDate>
+      <ExpirationDate>2024-02-01T00:00:00+01:00</ExpirationDate>
       <Type>Lyo</Type>
       <Mode>10B</Mode>
     </ConsumableInfo>
   </ConsumableInfo>
   <PlannedReads>
     <Read ReadName="Read1" Cycles="151"/>
     <Read ReadName="Index1" Cycles="10"/>
     <Read ReadName="Index2" Cycles="8"/>
     <Read ReadName="Read2" Cycles="151"/>
   </PlannedReads>
+  <SecondaryAnalysisInfo/>
 </RunParameters>
```

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv` & `cg-60.3.2/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/fluffy/SampleSheet.csv` & `cg-60.3.2/tests/fixtures/apps/fluffy/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/fluffy/deliverables.yaml` & `cg-60.3.2/tests/fixtures/apps/fluffy/deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/madeline/madeline.xml` & `cg-60.3.2/tests/fixtures/apps/madeline/madeline.xml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/mip/case_metrics_deliverables.yaml` & `cg-60.3.2/tests/fixtures/apps/mip/case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/mip/dna/store/case_config.yaml` & `cg-60.3.2/tests/fixtures/apps/mip/dna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml` & `cg-60.3.2/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml` & `cg-60.3.2/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf` & `cg-60.3.2/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/mip/rna/case_config.yaml` & `cg-60.3.2/tests/fixtures/apps/mip/rna/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml` & `cg-60.3.2/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/mip/rna/store/bundle_data.yaml` & `cg-60.3.2/tests/fixtures/apps/mip/rna/store/bundle_data.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/mip/rna/store/case_config.yaml` & `cg-60.3.2/tests/fixtures/apps/mip/rna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml` & `cg-60.3.2/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml` & `cg-60.3.2/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/scout/643594.config.yaml` & `cg-60.3.2/tests/fixtures/apps/scout/643594.config.yaml`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/scout/case_export.json` & `cg-60.3.2/tests/fixtures/apps/scout/case_export.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/scout/export_causatives.json` & `cg-60.3.2/tests/fixtures/apps/scout/export_causatives.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/scout/none_case_export.json` & `cg-60.3.2/tests/fixtures/apps/scout/none_case_export.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/scout/other_sex_case.json` & `cg-60.3.2/tests/fixtures/apps/scout/other_sex_case.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/scout/panel_export.bed` & `cg-60.3.2/tests/fixtures/apps/scout/panel_export.bed`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/scout/panel_export.csv` & `cg-60.3.2/tests/fixtures/apps/scout/panel_export.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv` & `cg-60.3.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv` & `cg-60.3.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv` & `cg-60.3.2/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/cgweb_orders/balsamic.json` & `cg-60.3.2/tests/fixtures/cgweb_orders/balsamic.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/cgweb_orders/fastq.json` & `cg-60.3.2/tests/fixtures/cgweb_orders/fastq.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/cgweb_orders/metagenome.json` & `cg-60.3.2/tests/fixtures/cgweb_orders/metagenome.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/cgweb_orders/microsalt.json` & `cg-60.3.2/tests/fixtures/cgweb_orders/microsalt.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/cgweb_orders/mip.json` & `cg-60.3.2/tests/fixtures/cgweb_orders/mip.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/cgweb_orders/mip_rna.json` & `cg-60.3.2/tests/fixtures/cgweb_orders/mip_rna.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/cgweb_orders/rml.json` & `cg-60.3.2/tests/fixtures/cgweb_orders/rml.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/cgweb_orders/rnafusion.json` & `cg-60.3.2/tests/fixtures/cgweb_orders/rnafusion.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/cgweb_orders/sarscov2.json` & `cg-60.3.2/tests/fixtures/cgweb_orders/sarscov2.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/data/SampleSheet.csv` & `cg-60.3.2/tests/fixtures/data/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/data/cgfixture.db` & `cg-60.3.2/tests/fixtures/data/cgfixture.db`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/data/hkstore.db` & `cg-60.3.2/tests/fixtures/data/hkstore.db`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/io/example_json.json` & `cg-60.3.2/tests/fixtures/io/example_json.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/orderforms/1508.30.balsamic.xlsx` & `cg-60.3.2/tests/fixtures/orderforms/1508.30.balsamic.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx` & `cg-60.3.2/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx` & `cg-60.3.2/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/orderforms/1508.30.fastq.xlsx` & `cg-60.3.2/tests/fixtures/orderforms/1508.30.fastq.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/orderforms/1508.30.metagenome.xlsx` & `cg-60.3.2/tests/fixtures/orderforms/1508.30.metagenome.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/orderforms/1508.30.mip.xlsx` & `cg-60.3.2/tests/fixtures/orderforms/1508.30.mip.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/orderforms/1508.30.mip_rna.xlsx` & `cg-60.3.2/tests/fixtures/orderforms/1508.30.mip_rna.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/orderforms/1508.30.rnafusion.xlsx` & `cg-60.3.2/tests/fixtures/orderforms/1508.30.rnafusion.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/orderforms/1603.11.microbial.xlsx` & `cg-60.3.2/tests/fixtures/orderforms/1603.11.microbial.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/orderforms/1604.17.rml.xlsx` & `cg-60.3.2/tests/fixtures/orderforms/1604.17.rml.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/orderforms/2184.9.sarscov2.xlsx` & `cg-60.3.2/tests/fixtures/orderforms/2184.9.sarscov2.xlsx`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/orderforms/NIPT-json.json` & `cg-60.3.2/tests/fixtures/orderforms/NIPT-json.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json` & `cg-60.3.2/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/orderforms/mip_uploaded_json_orderform.json` & `cg-60.3.2/tests/fixtures/orderforms/mip_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/report/case_data.json` & `cg-60.3.2/tests/fixtures/report/case_data.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/report/lims_exported_samples.json` & `cg-60.3.2/tests/fixtures/report/lims_exported_samples.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/fixtures/report/lims_family.json` & `cg-60.3.2/tests/fixtures/report/lims_family.json`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/io/conftest.py` & `cg-60.3.2/tests/io/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/io/test_io_controller.py` & `cg-60.3.2/tests/io/test_io_controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/io/test_io_csv.py` & `cg-60.3.2/tests/io/test_io_csv.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/io/test_io_json.py` & `cg-60.3.2/tests/io/test_io_json.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/io/test_io_txt.py` & `cg-60.3.2/tests/io/test_io_txt.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/io/test_io_xml.py` & `cg-60.3.2/tests/io/test_io_xml.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/io/test_io_yaml.py` & `cg-60.3.2/tests/io/test_io_yaml.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/io/test_validate_path.py` & `cg-60.3.2/tests/io/test_validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/archive/conftest.py` & `cg-60.3.2/tests/meta/archive/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/archive/test_archive_api.py` & `cg-60.3.2/tests/meta/archive/test_archive_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/archive/test_archive_cli.py` & `cg-60.3.2/tests/meta/archive/test_archive_cli.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/archive/test_archiving.py` & `cg-60.3.2/tests/meta/archive/test_archiving.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/backup/conftest.py` & `cg-60.3.2/tests/meta/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/backup/test_meta_backup.py` & `cg-60.3.2/tests/meta/backup/test_meta_backup.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/backup/test_meta_pdc.py` & `cg-60.3.2/tests/meta/backup/test_meta_pdc.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/clean/conftest.py` & `cg-60.3.2/tests/meta/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/clean/test_clean_flow_cells_api.py` & `cg-60.3.2/tests/meta/clean/test_clean_flow_cells_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/clean/test_clean_retrieved_spring_files.py` & `cg-60.3.2/tests/meta/clean/test_clean_retrieved_spring_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/compress/conftest.py` & `cg-60.3.2/tests/meta/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/compress/test_clean_fastq.py` & `cg-60.3.2/tests/meta/compress/test_clean_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/compress/test_compress_files.py` & `cg-60.3.2/tests/meta/compress/test_compress_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/compress/test_compress_meta_fastq.py` & `cg-60.3.2/tests/meta/compress/test_compress_meta_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/compress/test_decompress_spring_meta.py` & `cg-60.3.2/tests/meta/compress/test_decompress_spring_meta.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/compress/test_meta_compress_update_hk.py` & `cg-60.3.2/tests/meta/compress/test_meta_compress_update_hk.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,51 +12,55 @@
 from cg.store.store import Store
 from tests.cli.conftest import MockCompressAPI
 from tests.meta.compress.conftest import MockCompressionData
 from tests.store_helpers import StoreHelpers
 
 
 def test_get_flow_cell_id_when_hiseqx(
-    compress_api: CompressAPI, bcl2fastq_flow_cell_id: str, bcl2fastq_flow_cell_full_name: str
+    compress_api: CompressAPI,
+    hiseq_x_single_index_flow_cell_id: str,
+    hiseq_x_single_index_flow_cell_name: str,
 ):
     """Test extracting the flow cell id from a fastq file path."""
 
     # GIVEN a CompressAPI and a flow cell id within a fastq file path
     fastq_path: Path = compress_api.demux_root.joinpath(
         Path(
-            bcl2fastq_flow_cell_full_name,
-            f"{bcl2fastq_flow_cell_id}-l6t11_Undetermined_GACGTCTT_L006_R1_001.fastq.gz",
+            hiseq_x_single_index_flow_cell_name,
+            f"{hiseq_x_single_index_flow_cell_id}-l6t11_Undetermined_GACGTCTT_L006_R1_001.fastq.gz",
         )
     )
 
     # WHEN retrieving the flow cell id
     returned_flow_cell_name: str = compress_api.get_flow_cell_id(fastq_path=fastq_path)
 
     # THEN the flow cell id retrieved should be identical to the flow cell id used
-    assert returned_flow_cell_name == bcl2fastq_flow_cell_id
+    assert returned_flow_cell_name == hiseq_x_single_index_flow_cell_id
 
 
 def test_get_flow_cell_id_when_novaseq(
-    compress_api: CompressAPI, bcl2fastq_flow_cell_id: str, bcl2fastq_flow_cell_full_name: str
+    compress_api: CompressAPI,
+    novaseq_6000_pre_1_5_kits_flow_cell_id: str,
+    bcl2fastq_flow_cell_full_name: str,
 ):
     """Test extracting the flow cell id from a fastq file path."""
 
     # GIVEN a CompressAPI and a flow cell id within a fastq file path
     fastq_path: Path = compress_api.demux_root.joinpath(
         Path(
             bcl2fastq_flow_cell_full_name,
-            f"{bcl2fastq_flow_cell_id}_ACC10950A36_S36_L001_R1_001.fastq.gz",
+            f"{novaseq_6000_pre_1_5_kits_flow_cell_id}_ACC10950A36_S36_L001_R1_001.fastq.gz",
         )
     )
 
     # WHEN retrieving the flow cell id
     returned_flow_cell_name: str = compress_api.get_flow_cell_id(fastq_path=fastq_path)
 
     # THEN the flow cell id retrieved should be identical to the flow cell id used
-    assert returned_flow_cell_name == bcl2fastq_flow_cell_id
+    assert returned_flow_cell_name == novaseq_6000_pre_1_5_kits_flow_cell_id
 
 
 def test_add_fastq_housekeeper_when_no_fastq_in_hk(
     compress_api: MockCompressAPI,
     real_housekeeper_api: Generator[HousekeeperAPI, None, None],
     decompress_hk_spring_bundle: dict,
     compression_files: MockCompressionData,
```

### Comparing `cg-60.3.1/tests/meta/conftest.py` & `cg-60.3.2/tests/meta/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -113,29 +113,29 @@
     """Return the string of a path to a (fake) binary."""
     return Path("usr", "bin", "binary").as_posix()
 
 
 @pytest.fixture
 def stats_sample_data(
     sample_id: str,
-    bcl2fastq_flow_cell_id: str,
-    bcl_convert_flow_cell_id: str,
+    novaseq_6000_pre_1_5_kits_flow_cell_id: str,
+    novaseq_6000_post_1_5_kits_flow_cell_id: str,
 ) -> dict:
     return {
         "samples": [
             {
                 "name": sample_id,
                 "index": "ACGTACAT",
-                "flowcell": bcl2fastq_flow_cell_id,
+                "flowcell": novaseq_6000_pre_1_5_kits_flow_cell_id,
                 "type": Sequencers.NOVASEQ,
             },
             {
                 "name": "ADM1136A3",
                 "index": "ACGTACAT",
-                "flowcell": bcl_convert_flow_cell_id,
+                "flowcell": novaseq_6000_post_1_5_kits_flow_cell_id,
                 "type": Sequencers.NOVASEQ,
             },
         ]
     }
 
 
 @pytest.fixture
```

### Comparing `cg-60.3.1/tests/meta/deliver/conftest.py` & `cg-60.3.2/tests/meta/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/deliver/test_deliver_ticket.py` & `cg-60.3.2/tests/meta/deliver/test_deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/deliver/test_delivery_api.py` & `cg-60.3.2/tests/meta/deliver/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/deliver/test_fastq_path_generator.py` & `cg-60.3.2/tests/meta/deliver/test_fastq_path_generator.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/delivery/test_delivery_api.py` & `cg-60.3.2/tests/meta/delivery/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/demultiplex/conftest.py` & `cg-60.3.2/tests/meta/demultiplex/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,24 +71,18 @@
 
     tmp_flow_cell_demux_path: Path = Path(project_dir, "demultiplexed-runs")
     tmp_flow_cell_demux_path.mkdir(exist_ok=True, parents=True)
 
     return tmp_flow_cell_demux_path
 
 
-@pytest.fixture(name="flow_cell_project_id")
-def flow_cell_project_id() -> int:
-    """Return flow cell run project id."""
-    return 174578
-
-
 @pytest.fixture(name="populated_flow_cell_store")
 def populated_flow_cell_store(
     family_name: str,
-    bcl2fastq_flow_cell_id: str,
+    novaseq_6000_pre_1_5_kits_flow_cell_id: str,
     sample_id: str,
     store: Store,
     helpers: StoreHelpers,
 ) -> Store:
     """Populate a store with a NovaSeq flow cell."""
 
     populated_flow_cell_store: Store = store
@@ -97,25 +91,25 @@
     helpers.add_relationship(
         store=populated_flow_cell_store,
         sample=sample,
         case=family,
     )
     helpers.add_flow_cell(
         store=populated_flow_cell_store,
-        flow_cell_name=bcl2fastq_flow_cell_id,
+        flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id,
         sequencer_type="novaseq",
         samples=[sample],
     )
     return populated_flow_cell_store
 
 
 @pytest.fixture(name="active_flow_cell_store")
 def active_flow_cell_store(
     family_name: str,
-    bcl2fastq_flow_cell_id: str,
+    novaseq_6000_pre_1_5_kits_flow_cell_id: str,
     sample_id: str,
     base_store: Store,
     helpers: StoreHelpers,
 ) -> Store:
     """Populate a store with a Novaseq flow cell, with active samples on it."""
     active_flow_cell_store: Store = base_store
     sample: Sample = helpers.add_sample(store=active_flow_cell_store, internal_id=sample_id)
@@ -125,72 +119,80 @@
     helpers.add_relationship(
         store=active_flow_cell_store,
         sample=sample,
         case=family,
     )
     helpers.add_flow_cell(
         store=active_flow_cell_store,
-        flow_cell_name=bcl2fastq_flow_cell_id,
+        flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id,
         sequencer_type="novaseq",
         samples=[sample],
     )
     return active_flow_cell_store
 
 
 @pytest.fixture(name="sample_level_housekeeper_api")
 def sample_level_housekeeper_api(
-    bcl2fastq_flow_cell_id: str,
+    novaseq_6000_pre_1_5_kits_flow_cell_id: str,
     real_housekeeper_api: HousekeeperAPI,
     sample_id: str,
     tmp_fastq_paths: list[Path],
     helpers,
 ) -> HousekeeperAPI:
     """Return a mocked Housekeeper API, containing a sample bundle with related FASTQ files."""
     sample_level_housekeeper_api = real_housekeeper_api
     bundle_data = {
         "name": sample_id,
         "created": datetime.now(),
         "version": "1.0",
         "files": [
-            {"path": path.as_posix(), "tags": ["fastq", bcl2fastq_flow_cell_id], "archive": False}
+            {
+                "path": path.as_posix(),
+                "tags": ["fastq", novaseq_6000_pre_1_5_kits_flow_cell_id],
+                "archive": False,
+            }
             for path in tmp_fastq_paths
         ],
     }
     helpers.ensure_hk_bundle(store=sample_level_housekeeper_api, bundle_data=bundle_data)
     return sample_level_housekeeper_api
 
 
 @pytest.fixture(name="flow_cell_name_housekeeper_api")
 def flow_cell_name_housekeeper_api(
-    bcl2fastq_flow_cell_id: str,
+    novaseq_6000_pre_1_5_kits_flow_cell_id: str,
     real_housekeeper_api: HousekeeperAPI,
     sample_id: str,
     tmp_fastq_paths: list[Path],
     tmp_sample_sheet_path: Path,
     helpers,
 ) -> HousekeeperAPI:
     """Return a mocked Housekeeper API, containing a sample bundle with related FASTQ files."""
     flow_cell_housekeeper_api = real_housekeeper_api
     bundle_data = {
         "name": sample_id,
         "created": datetime.now(),
         "version": "1.0",
         "files": [
-            {"path": path.as_posix(), "tags": ["fastq", bcl2fastq_flow_cell_id], "archive": False}
+            {
+                "path": path.as_posix(),
+                "tags": ["fastq", novaseq_6000_pre_1_5_kits_flow_cell_id],
+                "archive": False,
+            }
             for path in tmp_fastq_paths
         ],
     }
     flow_cell_bundle_data = {
-        "name": bcl2fastq_flow_cell_id,
+        "name": novaseq_6000_pre_1_5_kits_flow_cell_id,
         "created": datetime.now(),
         "version": "1.0",
         "files": [
             {
                 "path": tmp_sample_sheet_path.as_posix(),
-                "tags": ["samplesheet", bcl2fastq_flow_cell_id],
+                "tags": ["samplesheet", novaseq_6000_pre_1_5_kits_flow_cell_id],
                 "archive": False,
             }
         ],
     }
 
     helpers.ensure_hk_bundle(store=flow_cell_housekeeper_api, bundle_data=bundle_data)
     helpers.ensure_hk_bundle(store=flow_cell_housekeeper_api, bundle_data=flow_cell_bundle_data)
```

### Comparing `cg-60.3.1/tests/meta/demultiplex/test_combine_sequencing_metrics.py` & `cg-60.3.2/tests/meta/demultiplex/test_combine_sequencing_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/demultiplex/test_demux_post_processing.py` & `cg-60.3.2/tests/meta/demultiplex/test_demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/demultiplex/test_housekeeper_storage_functions.py` & `cg-60.3.2/tests/meta/demultiplex/test_housekeeper_storage_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,31 +210,35 @@
     for file in files:
         assert file.path.split("/")[-1] in expected_file_names
 
 
 def test_store_fastq_path_in_housekeeper_correct_tags(
     populated_housekeeper_api: HousekeeperAPI,
     empty_fastq_file_path: Path,
-    bcl_convert_flow_cell_id: str,
+    novaseq_6000_post_1_5_kits_flow_cell_id: str,
 ):
     """Test that a fastq file is stored in Housekeeper with the correct tags."""
     sample_id: str = "sample_internal_id"
     # GIVEN a fastq file that has not been added to Housekeeper
     assert not populated_housekeeper_api.files(path=empty_fastq_file_path.as_posix()).first()
 
     # WHEN adding the fastq file to housekeeper
     populated_housekeeper_api.store_fastq_path_in_housekeeper(
         sample_internal_id=sample_id,
         sample_fastq_path=empty_fastq_file_path,
-        flow_cell_id=bcl_convert_flow_cell_id,
+        flow_cell_id=novaseq_6000_post_1_5_kits_flow_cell_id,
     )
 
     # THEN the file was added to Housekeeper with the correct tags
     file: File = populated_housekeeper_api.get_files(bundle=sample_id).first()
-    expected_tags: set[str] = {SequencingFileTag.FASTQ.value, bcl_convert_flow_cell_id, sample_id}
+    expected_tags: set[str] = {
+        SequencingFileTag.FASTQ.value,
+        novaseq_6000_post_1_5_kits_flow_cell_id,
+        sample_id,
+    }
     assert {tag.name for tag in file.tags} == expected_tags
 
 
 @pytest.mark.parametrize(
     "file_tag",
     [SequencingFileTag.FASTQ, SequencingFileTag.SPRING, SequencingFileTag.SPRING_METADATA],
 )
```

### Comparing `cg-60.3.1/tests/meta/demultiplex/test_status_db_storage_functions.py` & `cg-60.3.2/tests/meta/demultiplex/test_status_db_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/demultiplex/test_utils.py` & `cg-60.3.2/tests/meta/demultiplex/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,25 +261,25 @@
 
 def test_parse_flow_cell_directory_data_invalid():
     """Test that a FlowCellDirectoryData object is not created when the given path is invalid."""
     with pytest.raises(FlowCellError):
         FlowCellDirectoryData(Path("invalid_path"))
 
 
-def test_parse_flow_cell_directory_data_valid():
+def test_parse_flow_cell_directory_data_valid(novaseq_6000_post_1_5_kits_flow_cell_full_name: str):
     # GIVEN a flow cell directory which is valid
+
     # WHEN parsing the flow cell directory data
-    flow_cell_run_directory = "20230508_LH00188_0003_A22522YLT3"
-    result = FlowCellDirectoryData(Path(flow_cell_run_directory))
+    result = FlowCellDirectoryData(Path(novaseq_6000_post_1_5_kits_flow_cell_full_name))
 
     # THEN a FlowCellDirectoryData object should be returned
     assert isinstance(result, FlowCellDirectoryData)
 
     # THEN the flow cell path and bcl converter should be set
-    assert result.path == Path(flow_cell_run_directory)
+    assert result.path == Path(novaseq_6000_post_1_5_kits_flow_cell_full_name)
 
 
 def test_parse_manifest_file(novaseq_x_manifest_file: Path):
     # GIVEN a manifest file
 
     # WHEN parsing the manifest file
     files_at_source: list[Path] = parse_manifest_file(novaseq_x_manifest_file)
@@ -509,43 +509,45 @@
         Path(file[0].strip()) for file in read_csv(delimiter="\t", file_path=manifest_file)
     ]
     for manifest_file in files_in_file:
         assert manifest_file in files_in_manifest
 
 
 def test_add_flow_cell_name_to_fastq_file_path(
-    bcl2fastq_flow_cell_id: str, demultiplex_fastq_file_path
+    hiseq_x_single_index_flow_cell_id: str, demultiplex_fastq_file_path
 ):
     # GIVEN a fastq file path and a flow cell name
 
     # WHEN adding the flow cell name to the fastq file path
     rename_fastq_file_path: Path = add_flow_cell_name_to_fastq_file_path(
-        fastq_file_path=demultiplex_fastq_file_path, flow_cell_name=bcl2fastq_flow_cell_id
+        fastq_file_path=demultiplex_fastq_file_path,
+        flow_cell_name=hiseq_x_single_index_flow_cell_id,
     )
 
     # THEN the fastq file path should be returned with the flow cell name added
     assert rename_fastq_file_path == Path(
         demultiplex_fastq_file_path.parent,
-        f"{bcl2fastq_flow_cell_id}_{demultiplex_fastq_file_path.name}",
+        f"{hiseq_x_single_index_flow_cell_id}_{demultiplex_fastq_file_path.name}",
     )
 
 
 def test_add_flow_cell_name_to_fastq_file_path_when_flow_cell_name_already_in_name(
-    bcl2fastq_flow_cell_id: str, demultiplex_fastq_file_path
+    novaseq_6000_pre_1_5_kits_flow_cell_id: str, demultiplex_fastq_file_path
 ):
     # GIVEN a fastq file path and a flow cell name
 
     # GIVEN that the flow cell name is already in the fastq file path
     demultiplex_fastq_file_path = Path(
-        f"{bcl2fastq_flow_cell_id}_{demultiplex_fastq_file_path.name}"
+        f"{novaseq_6000_pre_1_5_kits_flow_cell_id}_{demultiplex_fastq_file_path.name}"
     )
 
     # WHEN adding the flow cell name to the fastq file path
     renamed_fastq_file_path: Path = add_flow_cell_name_to_fastq_file_path(
-        fastq_file_path=demultiplex_fastq_file_path, flow_cell_name=bcl2fastq_flow_cell_id
+        fastq_file_path=demultiplex_fastq_file_path,
+        flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id,
     )
 
     # THEN the fastq file path should be returned equal to the original fastq file path
     assert renamed_fastq_file_path == demultiplex_fastq_file_path
 
 
 def test_get_undetermined_fastqs_no_matching_files(tmp_path):
```

### Comparing `cg-60.3.1/tests/meta/demultiplex/test_validation.py` & `cg-60.3.2/tests/meta/demultiplex/test_validation.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/encryption/conftest.py` & `cg-60.3.2/tests/meta/encryption/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/encryption/test_encryption.py` & `cg-60.3.2/tests/meta/encryption/test_encryption.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/observations/conftest.py` & `cg-60.3.2/tests/meta/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/observations/test_meta_upload_observations.py` & `cg-60.3.2/tests/meta/observations/test_meta_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/orders/conftest.py` & `cg-60.3.2/tests/meta/orders/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/orders/test_PoolSubmitter_validate_order.py` & `cg-60.3.2/tests/meta/orders/test_PoolSubmitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py` & `cg-60.3.2/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/orders/test_SarsCov2Submitter_store_order.py` & `cg-60.3.2/tests/meta/orders/test_SarsCov2Submitter_store_order.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/orders/test_SarsCov2Submitter_validate_order.py` & `cg-60.3.2/tests/meta/orders/test_SarsCov2Submitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/orders/test_meta_orders_api.py` & `cg-60.3.2/tests/meta/orders/test_meta_orders_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/orders/test_meta_orders_lims.py` & `cg-60.3.2/tests/meta/orders/test_meta_orders_lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/orders/test_meta_orders_status.py` & `cg-60.3.2/tests/meta/orders/test_meta_orders_status.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/orders/test_rnafusion_submitter.py` & `cg-60.3.2/tests/meta/orders/test_rnafusion_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/orders/test_ticket_handler.py` & `cg-60.3.2/tests/meta/orders/test_ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/qc_metrics/conftest.py` & `cg-60.3.2/tests/meta/qc_metrics/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/qc_metrics/test_collect_qc_metrics.py` & `cg-60.3.2/tests/meta/qc_metrics/test_collect_qc_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/report/conftest.py` & `cg-60.3.2/tests/meta/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/report/test_balsamic_api.py` & `cg-60.3.2/tests/meta/report/test_balsamic_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/report/test_field_validators.py` & `cg-60.3.2/tests/meta/report/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/report/test_mip_dna_api.py` & `cg-60.3.2/tests/meta/report/test_mip_dna_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/report/test_report_api.py` & `cg-60.3.2/tests/meta/report/test_report_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/report/test_rnafusion_api.py` & `cg-60.3.2/tests/meta/report/test_rnafusion_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/report/test_tomte_api.py` & `cg-60.3.2/tests/meta/report/test_tomte_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/rsync/conftest.py` & `cg-60.3.2/tests/meta/rsync/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/rsync/test_rsync.py` & `cg-60.3.2/tests/meta/rsync/test_rsync.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/test_invoice.py` & `cg-60.3.2/tests/meta/test_invoice.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/transfer/conftest.py` & `cg-60.3.2/tests/meta/transfer/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/transfer/test_external_data.py` & `cg-60.3.2/tests/meta/transfer/test_external_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/transfer/test_meta_transfer_lims.py` & `cg-60.3.2/tests/meta/transfer/test_meta_transfer_lims.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/upload/balsamic/test_balsamic.py` & `cg-60.3.2/tests/meta/upload/balsamic/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/upload/conftest.py` & `cg-60.3.2/tests/meta/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/upload/gisaid/fixtures/four_samples.csv` & `cg-60.3.2/tests/meta/upload/gisaid/fixtures/four_samples.csv`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/upload/mutacc/conftest.py` & `cg-60.3.2/tests/meta/upload/mutacc/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/upload/mutacc/test_meta_upload_mutacc.py` & `cg-60.3.2/tests/meta/upload/mutacc/test_meta_upload_mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/upload/nipt/conftest.py` & `cg-60.3.2/tests/meta/upload/nipt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/upload/nipt/test_models.py` & `cg-60.3.2/tests/meta/upload/nipt/test_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/upload/nipt/test_nipt_upload_api.py` & `cg-60.3.2/tests/meta/upload/nipt/test_nipt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/upload/scout/conftest.py` & `cg-60.3.2/tests/meta/upload/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/upload/scout/test_generate_load_config.py` & `cg-60.3.2/tests/meta/upload/scout/test_generate_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/upload/scout/test_meta_upload_scoutapi.py` & `cg-60.3.2/tests/meta/upload/scout/test_meta_upload_scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py` & `cg-60.3.2/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/upload/scout/test_scout_config_builder.py` & `cg-60.3.2/tests/meta/upload/scout/test_scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/upload/test_meta_upload_coverage.py` & `cg-60.3.2/tests/meta/upload/test_meta_upload_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/upload/test_upload_api.py` & `cg-60.3.2/tests/meta/upload/test_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/upload/test_upload_genotypes_api.py` & `cg-60.3.2/tests/meta/upload/test_upload_genotypes_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/workflow/conftest.py` & `cg-60.3.2/tests/meta/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/workflow/microsalt/conftest.py` & `cg-60.3.2/tests/meta/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/workflow/microsalt/test_quality_controller.py` & `cg-60.3.2/tests/meta/workflow/microsalt/test_quality_controller.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/workflow/microsalt/test_quality_controller_utils.py` & `cg-60.3.2/tests/meta/workflow/microsalt/test_quality_controller_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/workflow/microsalt/test_report_generation.py` & `cg-60.3.2/tests/meta/workflow/microsalt/test_report_generation.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/workflow/test_analysis.py` & `cg-60.3.2/tests/meta/workflow/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/workflow/test_balsamic.py` & `cg-60.3.2/tests/meta/workflow/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/workflow/test_fastq.py` & `cg-60.3.2/tests/meta/workflow/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/workflow/test_microsalt.py` & `cg-60.3.2/tests/meta/workflow/test_microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/workflow/test_nf_analysis.py` & `cg-60.3.2/tests/meta/workflow/test_nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/workflow/test_prepare_fastq_api.py` & `cg-60.3.2/tests/meta/workflow/test_prepare_fastq_api.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/workflow/test_raredisease.py` & `cg-60.3.2/tests/meta/workflow/test_raredisease.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/meta/workflow/test_rnafusion.py` & `cg-60.3.2/tests/meta/workflow/test_rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/mocks/balsamic_analysis_mock.py` & `cg-60.3.2/tests/mocks/balsamic_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/mocks/crunchy.py` & `cg-60.3.2/tests/mocks/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/mocks/hk_mock.py` & `cg-60.3.2/tests/mocks/hk_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/mocks/limsmock.py` & `cg-60.3.2/tests/mocks/limsmock.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/mocks/madeline.py` & `cg-60.3.2/tests/mocks/madeline.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/mocks/mip_analysis_mock.py` & `cg-60.3.2/tests/mocks/mip_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/mocks/osticket.py` & `cg-60.3.2/tests/mocks/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/mocks/process_mock.py` & `cg-60.3.2/tests/mocks/process_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/mocks/report.py` & `cg-60.3.2/tests/mocks/report.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/mocks/scout.py` & `cg-60.3.2/tests/mocks/scout.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/mocks/store_model.py` & `cg-60.3.2/tests/mocks/store_model.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/mocks/tb_mock.py` & `cg-60.3.2/tests/mocks/tb_mock.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/models/balsamic/conftest.py` & `cg-60.3.2/tests/models/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/models/balsamic/test_balsamic_analysis.py` & `cg-60.3.2/tests/models/balsamic/test_balsamic_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/models/conftest.py` & `cg-60.3.2/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/models/demultiplexing/test_run_parameters.py` & `cg-60.3.2/tests/models/demultiplexing/test_run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/models/downsample/test_down_sample_meta_data.py` & `cg-60.3.2/tests/models/downsample/test_down_sample_meta_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/models/flow_cell/test_flowcell_model.py` & `cg-60.3.2/tests/models/flow_cell/test_flowcell_model.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/models/mip/conftest.py` & `cg-60.3.2/tests/models/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/models/mip/test_mip_analysis.py` & `cg-60.3.2/tests/models/mip/test_mip_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/models/mip/test_mip_config.py` & `cg-60.3.2/tests/models/mip/test_mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/models/mip/test_mip_metrics_deliverables.py` & `cg-60.3.2/tests/models/mip/test_mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/models/mip/test_mip_sample_info.py` & `cg-60.3.2/tests/models/mip/test_mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/models/nextflow/test_nextflow_deliver.py` & `cg-60.3.2/tests/models/nextflow/test_nextflow_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/models/observations/conftest.py` & `cg-60.3.2/tests/models/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/models/observations/test_observations_input_files.py` & `cg-60.3.2/tests/models/observations/test_observations_input_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/models/report/test_validators.py` & `cg-60.3.2/tests/models/report/test_validators.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/models/rnafusion/test_rnafusion_sample.py` & `cg-60.3.2/tests/models/rnafusion/test_rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/models/test_cg_models.py` & `cg-60.3.2/tests/models/test_cg_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/models/test_compression_data.py` & `cg-60.3.2/tests/models/test_compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/models/test_fastq.py` & `cg-60.3.2/tests/models/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/models/test_file_data.py` & `cg-60.3.2/tests/models/test_file_data.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/server/conftest.py` & `cg-60.3.2/tests/server/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/server/endpoints/test_delivery_message_endpoint.py` & `cg-60.3.2/tests/server/endpoints/test_delivery_message_endpoint.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/server/endpoints/test_orders_endpoint.py` & `cg-60.3.2/tests/server/endpoints/test_orders_endpoint.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/services/fastq_file_service/conftest.py` & `cg-60.3.2/tests/services/fastq_file_service/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/services/fastq_file_service/test_fastq_file_service.py` & `cg-60.3.2/tests/services/fastq_file_service/test_fastq_file_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/services/orders/order_status_service/conftest.py` & `cg-60.3.2/tests/services/orders/order_status_service/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/services/orders/order_status_service/test_order_summary_service.py` & `cg-60.3.2/tests/services/orders/order_status_service/test_order_summary_service.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/api/conftest.py` & `cg-60.3.2/tests/store/api/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from cg.store.models import CaseSample
 from cg.store.store import Store
 from tests.store_helpers import StoreHelpers
 
 
 @pytest.fixture(name="store_failing_sequencing_qc")
 def store_failing_sequencing_qc(
-    bcl2fastq_flow_cell_id: str,
+    novaseq_6000_pre_1_5_kits_flow_cell_id: str,
     sample_id: str,
     ticket_id: str,
     timestamp_now: dt.datetime,
     helpers,
     store: Store,
 ) -> Store:
     """Populate a store with a Fluffy case, with a sample that has been sequenced on two flow cells."""
@@ -36,24 +36,24 @@
         reads=5,
         original_ticket=ticket_id,
         last_sequenced_at=timestamp_now,
     )
 
     helpers.add_flow_cell(
         store=store,
-        flow_cell_name=bcl2fastq_flow_cell_id,
+        flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id,
         samples=[store_sample],
         date=timestamp_now,
     )
 
     helpers.add_relationship(store=store, case=store_case, sample=store_sample)
     helpers.ensure_sample_lane_sequencing_metrics(
         store=store,
         sample_internal_id=store_sample.internal_id,
-        flow_cell_name=bcl2fastq_flow_cell_id,
+        flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id,
         flow_cell_lane_number=1,
         sample_total_reads_in_lane=5,
         sample_base_percentage_passing_q30=30,
     )
     return store
```

### Comparing `cg-60.3.1/tests/store/api/test_base.py` & `cg-60.3.2/tests/store/api/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/conftest.py` & `cg-60.3.2/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/crud/add/test_store_add_application_version.py` & `cg-60.3.2/tests/store/crud/add/test_store_add_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/crud/add/test_store_add_base.py` & `cg-60.3.2/tests/store/crud/add/test_store_add_base.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/crud/add/test_store_add_customer.py` & `cg-60.3.2/tests/store/crud/add/test_store_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/crud/add/test_store_add_flow_celll.py` & `cg-60.3.2/tests/store/crud/add/test_store_add_flow_celll.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 from cg.store.models import Flowcell
 from cg.store.store import Store
 from tests.store_helpers import StoreHelpers
 
 
 def test_add_flowcell(
     base_store: Store,
-    bcl2fastq_flow_cell_id: str,
+    novaseq_6000_pre_1_5_kits_flow_cell_id: str,
     helpers: StoreHelpers,
     sequencer_name: str,
     timestamp_now: datetime,
 ):
     """Test adding a flow cell to the database."""
 
     # GIVEN a database with no flow cell
 
     # WHEN adding flow cell
     flow_cell: Flowcell = base_store.add_flow_cell(
-        flow_cell_name=bcl2fastq_flow_cell_id,
+        flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id,
         sequencer_name=sequencer_name,
         sequencer_type=Sequencers.NOVASEQ,
         date=timestamp_now,
         flow_cell_status=FlowCellStatus.ON_DISK,
     )
 
     # THEN flow cell should be returned
@@ -32,26 +32,26 @@
 
     # THEN the flow cell status should be "ondisk"
     assert flow_cell.status == FlowCellStatus.ON_DISK
 
 
 def test_add_flowcell_status(
     base_store: Store,
-    bcl2fastq_flow_cell_id: str,
+    novaseq_6000_pre_1_5_kits_flow_cell_id: str,
     helpers: StoreHelpers,
     sequencer_name: str,
     timestamp_now: datetime,
 ):
     """Test adding a flow cell with a status to the database."""
 
     # GIVEN a database with no flow cell
 
     # WHEN adding flow cell
     flow_cell: Flowcell = base_store.add_flow_cell(
-        flow_cell_name=bcl2fastq_flow_cell_id,
+        flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id,
         sequencer_name=sequencer_name,
         sequencer_type=Sequencers.NOVASEQ,
         date=timestamp_now,
         flow_cell_status=FlowCellStatus.PROCESSING,
     )
 
     # THEN the flow cell status should be "processing"
```

### Comparing `cg-60.3.1/tests/store/crud/conftest.py` & `cg-60.3.2/tests/store/crud/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -246,18 +246,18 @@
         )
     yield store
 
 
 @pytest.fixture
 def re_sequenced_sample_store(
     store: Store,
-    bcl_convert_flow_cell_id: str,
+    novaseq_6000_post_1_5_kits_flow_cell_id: str,
     case_id: str,
     family_name: str,
-    bcl2fastq_flow_cell_id: str,
+    novaseq_6000_pre_1_5_kits_flow_cell_id: str,
     sample_id: str,
     ticket_id: str,
     timestamp_now: datetime,
     helpers,
 ) -> Store:
     """Populate a store with a Fluffy case, with a sample that has been sequenced on two flow cells."""
     re_sequenced_sample_store: Store = store
@@ -278,31 +278,31 @@
         last_sequenced_at=timestamp_now,
     )
 
     one_day_ahead_of_now = timestamp_now + timedelta(days=1)
 
     helpers.add_flow_cell(
         store=re_sequenced_sample_store,
-        flow_cell_name=bcl_convert_flow_cell_id,
+        flow_cell_name=novaseq_6000_post_1_5_kits_flow_cell_id,
         samples=[store_sample],
         date=timestamp_now,
     )
 
     helpers.add_flow_cell(
         store=re_sequenced_sample_store,
-        flow_cell_name=bcl2fastq_flow_cell_id,
+        flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id,
         samples=[store_sample],
         date=one_day_ahead_of_now,
     )
 
     helpers.add_relationship(store=re_sequenced_sample_store, case=store_case, sample=store_sample)
     helpers.ensure_sample_lane_sequencing_metrics(
         store=re_sequenced_sample_store,
         sample_internal_id=store_sample.internal_id,
-        flow_cell_name=bcl2fastq_flow_cell_id,
+        flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id,
         flow_cell_lane_number=1,
         sample_total_reads_in_lane=120000000,
         sample_base_percentage_passing_q30=90,
     )
     return re_sequenced_sample_store
```

### Comparing `cg-60.3.1/tests/store/crud/delete/test_delete.py` & `cg-60.3.2/tests/store/crud/delete/test_delete.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from cg.store.models import Case, CaseSample, Flowcell, Sample
 from cg.store.store import Store
 from tests.meta.demultiplex.conftest import populated_flow_cell_store
 
 
-def test_delete_flow_cell(bcl2fastq_flow_cell_id: str, populated_flow_cell_store: Store):
+def test_delete_flow_cell(
+    novaseq_6000_pre_1_5_kits_flow_cell_id: str, populated_flow_cell_store: Store
+):
     """Test deleting a flow cell in Store."""
 
     # GIVEN a database containing a flow cell
     flow_cell: Flowcell = populated_flow_cell_store.get_flow_cell_by_name(
-        flow_cell_name=bcl2fastq_flow_cell_id
+        flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id
     )
 
     assert flow_cell
 
     # WHEN removing flow cell
-    populated_flow_cell_store.delete_flow_cell(flow_cell_id=bcl2fastq_flow_cell_id)
+    populated_flow_cell_store.delete_flow_cell(flow_cell_id=novaseq_6000_pre_1_5_kits_flow_cell_id)
 
     # THEN no entry should be found for the flow cell
     results: Flowcell = populated_flow_cell_store.get_flow_cell_by_name(
-        flow_cell_name=bcl2fastq_flow_cell_id
+        flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id
     )
 
     assert not results
 
 
 def test_store_api_delete_relationships_between_sample_and_cases(
     sample_id_in_single_case: str,
```

### Comparing `cg-60.3.1/tests/store/crud/read/test_read.py` & `cg-60.3.2/tests/store/crud/read/test_read.py`

 * *Files 3% similar despite different names*

```diff
@@ -576,57 +576,61 @@
     # THEN a flow cells should be returned
     assert flow_cells
 
     # THEN a flow cell model should be returned
     assert isinstance(flow_cells[0], Flowcell)
 
 
-def test_get_flow_cell(bcl2fastq_flow_cell_id: str, re_sequenced_sample_store: Store):
+def test_get_flow_cell(
+    novaseq_6000_pre_1_5_kits_flow_cell_id: str, re_sequenced_sample_store: Store
+):
     """Test returning the latest flow cell from the database."""
 
     # GIVEN a store with two flow cells
 
     # WHEN fetching the latest flow cell
     flow_cell: Flowcell = re_sequenced_sample_store.get_flow_cell_by_name(
-        flow_cell_name=bcl2fastq_flow_cell_id
+        flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id
     )
 
     # THEN the returned flow cell should have the same name as the one in the database
-    assert flow_cell.name == bcl2fastq_flow_cell_id
+    assert flow_cell.name == novaseq_6000_pre_1_5_kits_flow_cell_id
 
 
 def test_get_flow_cells_by_case(
     base_store: Store,
-    bcl2fastq_flow_cell_id: str,
-    bcl_convert_flow_cell_id: str,
+    novaseq_6000_pre_1_5_kits_flow_cell_id: str,
+    novaseq_6000_post_1_5_kits_flow_cell_id: str,
     case: Case,
     helpers: StoreHelpers,
     sample: Sample,
 ):
     """Test returning the latest flow cell from the database by case."""
 
     # GIVEN a store with two flow cell
-    helpers.add_flow_cell(store=base_store, flow_cell_name=bcl2fastq_flow_cell_id, samples=[sample])
+    helpers.add_flow_cell(
+        store=base_store, flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id, samples=[sample]
+    )
 
-    helpers.add_flow_cell(store=base_store, flow_cell_name=bcl_convert_flow_cell_id)
+    helpers.add_flow_cell(store=base_store, flow_cell_name=novaseq_6000_post_1_5_kits_flow_cell_id)
 
     # WHEN fetching the latest flow cell
     flow_cells: list[Flowcell] = base_store.get_flow_cells_by_case(case=case)
 
     # THEN the flow cell samples for the case should be returned
     for flow_cell in flow_cells:
         for sample in flow_cell.samples:
             assert sample in case.samples
 
     # THEN the returned flow cell should have the same name as the one in the database
-    assert flow_cells[0].name == bcl2fastq_flow_cell_id
+    assert flow_cells[0].name == novaseq_6000_pre_1_5_kits_flow_cell_id
 
 
 def test_get_flow_cells_by_statuses(
-    bcl_convert_flow_cell_id: str, re_sequenced_sample_store: Store
+    novaseq_6000_post_1_5_kits_flow_cell_id: str, re_sequenced_sample_store: Store
 ):
     """Test returning the latest flow cell from the database by statuses."""
 
     # GIVEN a store with two flow cells
 
     # WHEN fetching the latest flow cell
     flow_cells: list[Flowcell] = re_sequenced_sample_store.get_flow_cells_by_statuses(
@@ -634,15 +638,15 @@
     )
 
     # THEN the flow cell status should be "ondisk"
     for flow_cell in flow_cells:
         assert flow_cell.status == FlowCellStatus.ON_DISK
 
     # THEN the returned flow cell should have the same name as the one in the database
-    assert flow_cells[0].name == bcl_convert_flow_cell_id
+    assert flow_cells[0].name == novaseq_6000_post_1_5_kits_flow_cell_id
 
 
 def test_get_flow_cells_by_statuses_when_multiple_matches(re_sequenced_sample_store: Store):
     """Test returning the latest flow cell from the database by statuses when multiple matches."""
 
     # GIVEN a store with two flow cells
 
@@ -678,56 +682,57 @@
     )
 
     # THEN no flow cells should be returned
     assert not list(flow_cells)
 
 
 def test_get_flow_cell_by_enquiry_and_status(
-    bcl2fastq_flow_cell_id: str, re_sequenced_sample_store: Store
+    novaseq_6000_pre_1_5_kits_flow_cell_id: str, re_sequenced_sample_store: Store
 ):
     """Test returning the latest flow cell from the database by enquiry and status."""
 
     # GIVEN a store with two flow cells
 
     # WHEN fetching the latest flow cell
     flow_cell: list[Flowcell] = re_sequenced_sample_store.get_flow_cell_by_name_pattern_and_status(
-        flow_cell_statuses=[FlowCellStatus.ON_DISK], name_pattern=bcl2fastq_flow_cell_id[:4]
+        flow_cell_statuses=[FlowCellStatus.ON_DISK],
+        name_pattern=novaseq_6000_pre_1_5_kits_flow_cell_id[:4],
     )
 
     # THEN the returned flow cell should have the same name as the one in the database
-    assert flow_cell[0].name == bcl2fastq_flow_cell_id
+    assert flow_cell[0].name == novaseq_6000_pre_1_5_kits_flow_cell_id
 
     # THEN the returned flow cell should have the same status as the query
     assert flow_cell[0].status == FlowCellStatus.ON_DISK
 
 
 def test_get_samples_from_flow_cell(
-    bcl2fastq_flow_cell_id: str, sample_id: str, re_sequenced_sample_store: Store
+    novaseq_6000_pre_1_5_kits_flow_cell_id: str, sample_id: str, re_sequenced_sample_store: Store
 ):
     """Test returning samples present on the latest flow cell from the database."""
 
     # GIVEN a store with two flow cells
 
     # WHEN fetching the samples from the latest flow cell
     samples: list[Sample] = re_sequenced_sample_store.get_samples_from_flow_cell(
-        flow_cell_id=bcl2fastq_flow_cell_id
+        flow_cell_id=novaseq_6000_pre_1_5_kits_flow_cell_id
     )
 
     # THEN the returned sample id should have the same id as the one in the database
     assert samples[0].internal_id == sample_id
 
 
 def test_get_latest_flow_cell_on_case(
-    re_sequenced_sample_store: Store, case_id: str, bcl2fastq_flow_cell_id: str
+    re_sequenced_sample_store: Store, case_id: str, novaseq_6000_pre_1_5_kits_flow_cell_id: str
 ):
     """Test returning the latest sequenced flow cell on a case."""
 
     # GIVEN a store with two flow cells in it, one being the latest sequenced of the two
     latest_flow_cell: Flowcell = re_sequenced_sample_store.get_flow_cell_by_name(
-        flow_cell_name=bcl2fastq_flow_cell_id
+        flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id
     )
 
     # WHEN fetching the latest flow cell on a case with a sample that has been sequenced on both flow cells
     latest_flow_cell_on_case: Flowcell = re_sequenced_sample_store.get_latest_flow_cell_on_case(
         family_id=case_id
     )
 
@@ -752,92 +757,94 @@
     # THEN log no flow cells found
     assert "No flow cells found" in caplog.text
 
 
 def test_are_all_flow_cells_on_disk_when_not_on_disk(
     base_store: Store,
     caplog,
-    bcl2fastq_flow_cell_id: str,
-    bcl_convert_flow_cell_id: str,
+    novaseq_6000_pre_1_5_kits_flow_cell_id: str,
+    novaseq_6000_post_1_5_kits_flow_cell_id: str,
     case_id: str,
     helpers: StoreHelpers,
     sample: Sample,
 ):
     """Test check if all flow cells for samples on a case is on disk when not on disk."""
     caplog.set_level(logging.DEBUG)
     # GIVEN a store with two flow cell
     helpers.add_flow_cell(
         store=base_store,
-        flow_cell_name=bcl2fastq_flow_cell_id,
+        flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id,
         samples=[sample],
         status=FlowCellStatus.PROCESSING,
     )
 
     helpers.add_flow_cell(
         store=base_store,
-        flow_cell_name=bcl_convert_flow_cell_id,
+        flow_cell_name=novaseq_6000_post_1_5_kits_flow_cell_id,
         samples=[sample],
         status=FlowCellStatus.RETRIEVED,
     )
 
     # WHEN fetching the latest flow cell
     is_on_disk = base_store.are_all_flow_cells_on_disk(case_id=case_id)
 
     # THEN return false
     assert is_on_disk is False
 
 
 def test_are_all_flow_cells_on_disk_when_requested(
     base_store: Store,
     caplog,
-    bcl2fastq_flow_cell_id: str,
-    bcl_convert_flow_cell_id: str,
+    novaseq_6000_pre_1_5_kits_flow_cell_id: str,
+    novaseq_6000_post_1_5_kits_flow_cell_id: str,
     case_id: str,
     helpers: StoreHelpers,
     sample: Sample,
     request,
 ):
     """Test check if all flow cells for samples on a case is on disk when requested."""
     caplog.set_level(logging.DEBUG)
     # GIVEN a store with two flow cell
     helpers.add_flow_cell(
         store=base_store,
-        flow_cell_name=bcl2fastq_flow_cell_id,
+        flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id,
         samples=[sample],
         status=FlowCellStatus.REMOVED,
     )
     helpers.add_flow_cell(
         store=base_store,
-        flow_cell_name=bcl_convert_flow_cell_id,
+        flow_cell_name=novaseq_6000_post_1_5_kits_flow_cell_id,
         samples=[sample],
         status=FlowCellStatus.REQUESTED,
     )
 
     # WHEN fetching the latest flow cell
     is_on_disk = base_store.are_all_flow_cells_on_disk(case_id=case_id)
 
     # THEN return false
     assert is_on_disk is False
 
 
 def test_are_all_flow_cells_on_disk(
     base_store: Store,
     caplog,
-    bcl2fastq_flow_cell_id: str,
-    bcl_convert_flow_cell_id: str,
+    novaseq_6000_pre_1_5_kits_flow_cell_id: str,
+    novaseq_6000_post_1_5_kits_flow_cell_id: str,
     case_id: str,
     helpers: StoreHelpers,
     sample: Sample,
 ):
     """Test check if all flow cells for samples on a case is on disk."""
     caplog.set_level(logging.DEBUG)
 
     # GIVEN a store with two flow cell
-    helpers.add_flow_cell(store=base_store, flow_cell_name=bcl2fastq_flow_cell_id, samples=[sample])
-    helpers.add_flow_cell(store=base_store, flow_cell_name=bcl_convert_flow_cell_id)
+    helpers.add_flow_cell(
+        store=base_store, flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id, samples=[sample]
+    )
+    helpers.add_flow_cell(store=base_store, flow_cell_name=novaseq_6000_post_1_5_kits_flow_cell_id)
 
     # WHEN fetching the latest flow cell
     is_on_disk = base_store.are_all_flow_cells_on_disk(case_id=case_id)
 
     # THEN return true
     assert is_on_disk is True
 
@@ -1344,55 +1351,55 @@
     assert metrics_entry.flow_cell_name == flow_cell_name
     assert metrics_entry.flow_cell_lane_number == lane
     assert metrics_entry.sample_internal_id == sample_id
 
 
 def test_get_number_of_reads_for_flow_cell_from_sample_lane_metrics(
     store_with_sequencing_metrics: Store,
-    flow_cell_name_demultiplexed_with_bcl2fastq: str,
+    hiseq_x_dual_index_flow_cell_id: str,
     expected_total_reads_flow_cell_bcl2fastq: int,
 ):
     # GIVEN a store with sequencing metrics
     # WHEN getting total read counts for a flow cell
     reads = store_with_sequencing_metrics.get_number_of_reads_for_flow_cell(
-        flow_cell_name=flow_cell_name_demultiplexed_with_bcl2fastq
+        flow_cell_name=hiseq_x_dual_index_flow_cell_id
     )
     # THEN assert that the total read count is correct
     assert reads == expected_total_reads_flow_cell_bcl2fastq
 
 
 def test_get_average_bases_above_q30_for_sample_from_metrics(
     store_with_sequencing_metrics: Store,
     expected_average_q30_for_sample: float,
     mother_sample_id: str,
-    flow_cell_name_demultiplexed_with_bcl2fastq: str,
+    hiseq_x_dual_index_flow_cell_id: str,
 ):
     # GIVEN a store with sequencing metrics
 
     # WHEN getting average bases above q30 for a sample
     average_bases_above_q30 = store_with_sequencing_metrics.get_average_q30_for_sample_on_flow_cell(
         sample_internal_id=mother_sample_id,
-        flow_cell_name=flow_cell_name_demultiplexed_with_bcl2fastq,
+        flow_cell_name=hiseq_x_dual_index_flow_cell_id,
     )
 
     # THEN assert that the average bases above q30 is correct
     assert average_bases_above_q30 == expected_average_q30_for_sample
 
 
 def test_get_average_passing_q30_for_sample_from_metrics(
     store_with_sequencing_metrics: Store,
     expected_average_q30_for_flow_cell: float,
-    flow_cell_name_demultiplexed_with_bcl2fastq: str,
+    hiseq_x_dual_index_flow_cell_id: str,
 ):
     # GIVEN a store with sequencing metrics
 
     # WHEN getting average passing q30 for a sample
     average_passing_q30 = (
         store_with_sequencing_metrics.get_average_percentage_passing_q30_for_flow_cell(
-            flow_cell_name=flow_cell_name_demultiplexed_with_bcl2fastq,
+            flow_cell_name=hiseq_x_dual_index_flow_cell_id,
         )
     )
 
     # THEN assert that the average passing q30 is correct
     assert average_passing_q30 == expected_average_q30_for_flow_cell
```

### Comparing `cg-60.3.1/tests/store/crud/read/test_read_analyses_to_clean.py` & `cg-60.3.2/tests/store/crud/read/test_read_analyses_to_clean.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/crud/read/test_read_analyses_to_delivery_report.py` & `cg-60.3.2/tests/store/crud/read/test_read_analyses_to_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/crud/read/test_read_analysis.py` & `cg-60.3.2/tests/store/crud/read/test_read_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/crud/read/test_read_application_version.py` & `cg-60.3.2/tests/store/crud/read/test_read_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/crud/read/test_read_customer.py` & `cg-60.3.2/tests/store/crud/read/test_read_customer.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/crud/read/test_read_pool.py` & `cg-60.3.2/tests/store/crud/read/test_read_pool.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/crud/read/test_read_sample.py` & `cg-60.3.2/tests/store/crud/read/test_read_sample.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/crud/update/test_update.py` & `cg-60.3.2/tests/store/crud/update/test_update.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/filters/test_status_analyses_filters.py` & `cg-60.3.2/tests/store/filters/test_status_analyses_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/filters/test_status_application_filters.py` & `cg-60.3.2/tests/store/filters/test_status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/filters/test_status_application_limitations_filters.py` & `cg-60.3.2/tests/store/filters/test_status_application_limitations_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/filters/test_status_application_version_filters.py` & `cg-60.3.2/tests/store/filters/test_status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/filters/test_status_bed_filters.py` & `cg-60.3.2/tests/store/filters/test_status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/filters/test_status_bed_version_filters.py` & `cg-60.3.2/tests/store/filters/test_status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/filters/test_status_case_sample_filters.py` & `cg-60.3.2/tests/store/filters/test_status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/filters/test_status_cases_filters.py` & `cg-60.3.2/tests/store/filters/test_status_cases_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/filters/test_status_collaboration_filters.py` & `cg-60.3.2/tests/store/filters/test_status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/filters/test_status_customer_filters.py` & `cg-60.3.2/tests/store/filters/test_status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/filters/test_status_flow_cell_filters.py` & `cg-60.3.2/tests/store/filters/test_status_flow_cell_filters.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,35 +11,37 @@
 from cg.store.store import Store
 from tests.store_helpers import StoreHelpers
 
 
 def test_get_flow_cells_by_case(
     base_store: Store,
     case: Case,
-    bcl2fastq_flow_cell_id: str,
+    novaseq_6000_pre_1_5_kits_flow_cell_id: str,
     helpers: StoreHelpers,
     sample: Sample,
 ):
     """Test that a flow cell is returned when there is a flow cell with matching flow cell case."""
 
     # GIVEN a flow cell that exist in status db
-    helpers.add_flow_cell(store=base_store, flow_cell_name=bcl2fastq_flow_cell_id, samples=[sample])
+    helpers.add_flow_cell(
+        store=base_store, flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id, samples=[sample]
+    )
 
     # GIVEN a flow cell Query
 
     # WHEN getting flow cell
     returned_flow_cell: list[Flowcell] | None = filter_flow_cells_by_case(
         flow_cells=base_store._get_join_flow_cell_sample_links_query(), case=case
     )
 
     # THEN a Flowcell type should be returned
     assert isinstance(returned_flow_cell[0], Flowcell)
 
     # THEN returned flow cell should have the same name as the flow cell in the database
-    assert returned_flow_cell[0].name == bcl2fastq_flow_cell_id
+    assert returned_flow_cell[0].name == novaseq_6000_pre_1_5_kits_flow_cell_id
 
 
 def test_get_flow_cells_by_case_when_no_flow_cell_for_case(
     base_store: Store,
     case: Case,
 ):
     """Test that a flow cell is not returned when there is a flow cell with no matching flow cell for case."""
@@ -51,86 +53,90 @@
         flow_cells=base_store._get_join_flow_cell_sample_links_query(), case=case
     )
 
     # THEN returned flow cell should be the original flow cell
     assert not list(returned_flow_cell)
 
 
-def test_get_flow_cell_by_id(base_store: Store, helpers: StoreHelpers, bcl2fastq_flow_cell_id: str):
+def test_get_flow_cell_by_id(
+    base_store: Store, helpers: StoreHelpers, novaseq_6000_pre_1_5_kits_flow_cell_id: str
+):
     """Test that a flow cell is returned when there is a flow cell with matching flow cell id."""
 
     # GIVEN a flow cell that exist in status db
     flow_cell: Flowcell = helpers.add_flow_cell(
-        store=base_store, flow_cell_name=bcl2fastq_flow_cell_id
+        store=base_store, flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id
     )
 
     # GIVEN a flow cell Query
 
     # WHEN getting flow cell
     returned_flow_cell: Query = filter_flow_cell_by_name(
-        flow_cells=base_store._get_query(table=Flowcell), flow_cell_name=bcl2fastq_flow_cell_id
+        flow_cells=base_store._get_query(table=Flowcell),
+        flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id,
     )
 
     # THEN returned flow cell should be the original flow cell
     assert isinstance(returned_flow_cell, Query)
 
     assert flow_cell is returned_flow_cell.first()
 
 
 def test_get_flow_cell_by_id_and_by_enquiry(
-    base_store: Store, helpers: StoreHelpers, bcl2fastq_flow_cell_id: str
+    base_store: Store, helpers: StoreHelpers, novaseq_6000_pre_1_5_kits_flow_cell_id: str
 ):
     """Test that a flow cell is returned when there is a flow cell with enquiry flow cell id."""
 
     # GIVEN a flow cell that exist in status db
     flow_cell: Flowcell = helpers.add_flow_cell(
-        store=base_store, flow_cell_name=bcl2fastq_flow_cell_id
+        store=base_store, flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id
     )
 
     # GIVEN a flow cell Query
 
     # WHEN getting flow cell
     returned_flow_cell: list[Flowcell] = filter_flow_cell_by_name_search(
-        flow_cells=base_store._get_query(table=Flowcell), name_search=bcl2fastq_flow_cell_id[:4]
+        flow_cells=base_store._get_query(table=Flowcell),
+        name_search=novaseq_6000_pre_1_5_kits_flow_cell_id[:4],
     )
 
     # THEN a list of flow cells should be returned
     assert isinstance(returned_flow_cell[0], Flowcell)
 
     assert flow_cell is returned_flow_cell[0]
 
 
 def test_get_flow_cells_with_statuses(
-    base_store: Store, helpers: StoreHelpers, bcl2fastq_flow_cell_id: str
+    base_store: Store, helpers: StoreHelpers, novaseq_6000_pre_1_5_kits_flow_cell_id: str
 ):
     """Test that a flow cell is returned when there is a flow cell with matching flow cell id."""
 
     # GIVEN a flow cell that exist in status db
-    helpers.add_flow_cell(store=base_store, flow_cell_name=bcl2fastq_flow_cell_id)
+    helpers.add_flow_cell(store=base_store, flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id)
 
     # GIVEN a flow cell Query
 
     # WHEN getting flow cell
     returned_flow_cell_query: Query = filter_flow_cells_with_statuses(
         flow_cells=base_store._get_query(table=Flowcell),
         flow_cell_statuses=[FlowCellStatus.ON_DISK, FlowCellStatus.PROCESSING],
     )
 
     # THEN a query should be returned
     assert isinstance(returned_flow_cell_query, Query)
 
 
 def test_filter_flow_cells_by_name(
-    base_store: Store, helpers: StoreHelpers, bcl2fastq_flow_cell_id: str
+    base_store: Store, helpers: StoreHelpers, novaseq_6000_pre_1_5_kits_flow_cell_id: str
 ):
     """Test flow cell is returned by name."""
 
     # GIVEN a flow cell that exist in status db
     flow_cell: Flowcell = helpers.add_flow_cell(
-        store=base_store, flow_cell_name=bcl2fastq_flow_cell_id
+        store=base_store, flow_cell_name=novaseq_6000_pre_1_5_kits_flow_cell_id
     )
 
     # GIVEN a flow cell Query
 
     # WHEN getting flow cell
     returned_flow_cell_query: Query = filter_flow_cell_by_name(
         flow_cells=base_store._get_query(table=Flowcell), flow_cell_name=flow_cell.name
```

### Comparing `cg-60.3.1/tests/store/filters/test_status_invoice_filters.py` & `cg-60.3.2/tests/store/filters/test_status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/filters/test_status_metrics_filters.py` & `cg-60.3.2/tests/store/filters/test_status_metrics_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/filters/test_status_organism_filters.py` & `cg-60.3.2/tests/store/filters/test_status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/filters/test_status_panel_filters.py` & `cg-60.3.2/tests/store/filters/test_status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/filters/test_status_pool_filters.py` & `cg-60.3.2/tests/store/filters/test_status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/filters/test_status_samples_filters.py` & `cg-60.3.2/tests/store/filters/test_status_samples_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/filters/test_status_user_filters.py` & `cg-60.3.2/tests/store/filters/test_status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/test_delivery.py` & `cg-60.3.2/tests/store/test_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store/test_store_models.py` & `cg-60.3.2/tests/store/test_store_models.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/store_helpers.py` & `cg-60.3.2/tests/store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/test_copy_novaseqx_flow_cell.py` & `cg-60.3.2/tests/test_copy_novaseqx_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/test_store_helpers.py` & `cg-60.3.2/tests/test_store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/utils/conftest.py` & `cg-60.3.2/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/utils/test_commands.py` & `cg-60.3.2/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/utils/test_date.py` & `cg-60.3.2/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/utils/test_dict.py` & `cg-60.3.2/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/utils/test_dispatcher.py` & `cg-60.3.2/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/utils/test_files.py` & `cg-60.3.2/tests/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/utils/test_time.py` & `cg-60.3.2/tests/utils/test_time.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/tests/utils/test_utils.py` & `cg-60.3.2/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-60.3.1/PKG-INFO` & `cg-60.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 60.3.1
+Version: 60.3.2
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

