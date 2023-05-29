# Comparing `tmp/cg-32.2.5.tar.gz` & `tmp/cg-32.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cg-32.2.5.tar", last modified: Sat May 27 11:20:57 2023, max compression
+gzip compressed data, was "dist/cg-32.2.7.tar", last modified: Mon May 29 10:48:24 2023, max compression
```

## Comparing `cg-32.2.5.tar` & `cg-32.2.7.tar`

### file list

```diff
@@ -1,1263 +1,1267 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-27 11:20:49.000000 cg-32.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-27 11:20:57.000000 cg-32.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-27 11:20:49.000000 cg-32.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-27 11:20:49.000000 cg-32.2.5/cg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15866 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/crud/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/crud/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/crud/find.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/cgstats/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/cgstats/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/demux_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/dragen_demux_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/support_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/unaligned.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/parsers/adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/parsers/conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/parsers/demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/parsers/quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/parsers/run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/coverage/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/crunchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/crunchy/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/crunchy/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/crunchy/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/demultiplex/demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/demultiplex/demux_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/demultiplex/sample_sheet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/demultiplex/sample_sheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/demultiplex/sample_sheet/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/demultiplex/sample_sheet/dummy_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/demultiplex/sample_sheet/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/demultiplex/sample_sheet/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/demultiplex/sample_sheet/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/hermes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/hermes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/hermes/hermes_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/hermes/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/housekeeper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/housekeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/housekeeper/hk.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/housekeeper/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/invoice/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/invoice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/invoice/templates/KI_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/invoice/templates/KI_sample_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/lims/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/lims/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/lims/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/lims/samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/loqus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/madeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/madeline/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/mip/confighandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/orderform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/orderform/excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/orderform/json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/orderform/orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/scout/scout_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/scout/scoutapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/models/bcl_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/slurm/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/slurm/slurm_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/tb/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/tb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/tb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/tb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/compress/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/compress/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/compress/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/delete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/delete/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/delete/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/delete/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/delete/observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/deliver/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/demultiplex/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/demultiplex/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/demultiplex/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/demultiplex/finish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/demultiplex/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/demultiplex/sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/generate/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/generate/report/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/generate/report/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/generate/report/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/set/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/set/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/set/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/set/cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/store/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/store/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/clinical_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/fohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/nipt/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/nipt/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/nipt/statina.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/upload/observations/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/observations/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/observations/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/balsamic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/balsamic/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/balsamic/pon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/balsamic/qc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/balsamic/umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/fastq/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/fluffy/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/microsalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/microsalt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/mip/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/mip/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/mip_dna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/mip_dna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/mip_dna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/mip_rna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/mip_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/mip_rna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/mutant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/mutant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/mutant/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/nextflow/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/rnafusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/rnafusion/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/taxprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/taxprofiler/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/tower/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/tower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/tower/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/constants/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/bcl_convert_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/cgstats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/demultiplexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/gene_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/housekeeper_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/nextflow.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/orderforms.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/pdc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/pedigree.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/sample_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/scout_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/sequencing.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/tb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-27 11:20:49.000000 cg-32.2.5/cg/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-27 11:20:49.000000 cg-32.2.5/cg/io/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-27 11:20:49.000000 cg-32.2.5/cg/io/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-27 11:20:49.000000 cg-32.2.5/cg/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-27 11:20:49.000000 cg-32.2.5/cg/io/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-27 11:20:49.000000 cg-32.2.5/cg/io/validate_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-27 11:20:49.000000 cg-32.2.5/cg/io/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/archive/ddn_dataflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/backup/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/backup/pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/clean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/clean/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/clean/demultiplexed_flow_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/clean/flow_cell_run_directories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/compress/compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/compress/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/deliver_ticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/demultiplex/delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/demultiplex/demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/demultiplex/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/encryption/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/observations/balsamic_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/observations/mip_dna_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/observations/observations_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/balsamic_qc_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/balsamic_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/balsamic_umi_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/case_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/fastq_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/fluffy_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/metagenome_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/microbial_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/microsalt_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/mip_dna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/mip_rna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/pool_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/rml_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/sars_cov_2_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/report/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/report/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/report/field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/report/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/report/report_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/report/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/report/templates/balsamic_report.html
--rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/report/templates/bootstrap.html
--rw-r--r--   0 runner    (1001) docker     (123)    77831 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/report/templates/mip-dna_report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/rsync/rsync_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/rsync/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/tar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/tar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/tar/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/transfer/external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/transfer/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/transfer/lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/balsamic/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/upload/fohm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/fohm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/fohm/fohm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/gisaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/gisaid/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/gisaid/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/gisaid/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/upload/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/mip/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/mip/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/nipt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/nipt/nipt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/upload/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/rnafusion/rnafusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/scout/balsamic_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/scout/balsamic_umi_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/scout/hk_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/scout/mip_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/scout/rnafusion_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/scout/scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18719 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/scout/uploadscoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/balsamic_pon.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/balsamic_qc.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/fluffy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/mip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/mutant.py
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/nextflow_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/prepare_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    17110 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/taxprofiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/tower_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/balsamic/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/balsamic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/balsamic/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12924 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/cg_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/cgstats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/cgstats/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/cgstats/stats_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/compression_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/deliverables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/deliverables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/deliverables/metric_deliverables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/demultiplex/demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/demultiplex/flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/demultiplex/run_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/file_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/invoice/invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/lims/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/lims/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/mip/mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/mip/mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/mip/mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/mip/mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/nextflow/deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/nextflow/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/observations/input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/orders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/orders/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/orders/excel_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/orders/json_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/orders/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/orders/orderform_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/orders/sample_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/orders/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/report/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/report/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/report/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/report/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/rnafusion/rnafusion_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/scout/scout_load_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/slurm/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/taxprofiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/workflow/mutant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-05-27 11:20:49.000000 cg-32.2.5/cg/resources/20181012_Indices.csv
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-27 11:20:49.000000 cg-32.2.5/cg/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-27 11:20:49.000000 cg-32.2.5/cg/resources/rnafusion_bundle_filenames.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    19037 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/server/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/invoices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/server/invoices/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/server/invoices/templates/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/invoices/templates/invoices/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/invoices/templates/invoices/invoice.html
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/invoices/templates/invoices/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/invoices/templates/invoices/new.html
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/invoices/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/server/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/server/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/templates/admin/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/store/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/api/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/api/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/api/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/api/find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    28994 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/api/find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    38700 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/api/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_analysis_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_case_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    29946 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/utils/checksum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/checksum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/checksum/checksum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/utils/click/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/click/EnumChoice.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/utils/flask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/flask/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-27 11:20:56.000000 cg-32.2.5/cg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40436 2023-05-27 11:20:57.000000 cg-32.2.5/cg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 11:20:56.000000 cg-32.2.5/cg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-27 11:20:56.000000 cg-32.2.5/cg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 11:20:56.000000 cg-32.2.5/cg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-27 11:20:56.000000 cg-32.2.5/cg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-27 11:20:56.000000 cg-32.2.5/cg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-27 11:20:49.000000 cg-32.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-27 11:20:49.000000 cg-32.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 11:20:57.000000 cg-32.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-27 11:20:49.000000 cg-32.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/cgstats/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/cgstats/crud/test_create_novaseq.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/cgstats/crud/test_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/cgstats/parsers/test_adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/cgstats/parsers/test_conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/cgstats/parsers/test_demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/cgstats/parsers/test_quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/cgstats/parsers/test_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/cgstats/test_cgstats_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/cgstats/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/coverage/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/coverage/test_coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/crunchy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/crunchy/test_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/crunchy/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/crunchy/test_crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/crunchy/test_spring_decompression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/demultiplex/test_convert_to_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/demultiplex/test_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/demultiplex/test_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/demultiplex/test_validate_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/gens/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/gens/test_gens_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/gt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/gt/test_gt_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/hk/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/hk/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/hk/test__getattr__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/hk/test_add_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/hk/test_bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/hk/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/hk/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/hk/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/lims/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/lims/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/loqus/
--rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/loqus/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/loqus/test_loqusdb_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/madeline/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/madeline/test_madeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/mip/test_config_mip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/mutacc_auto/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/mutacc_auto/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/mutacc_auto/test_mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/orderform/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/orderform/test_excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/orderform/test_excel_sample_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/orderform/test_json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/orderform/test_orderform_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/scout/test_get_causative_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/scout/test_get_scout_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/scout/test_scout_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/scout/test_scout_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/sequencing_metrics_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/sequencing_metrics_parser/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/sequencing_metrics_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/sequencing_metrics_parser/parsers/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/slurm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/slurm/test_slurm_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/test_apps_environ.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/test_osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/vogue/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/vogue/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/vogue/test_vogue_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/add/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/add/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/add/test_cli_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/add/test_cli_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/add/test_cli_add_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/add/test_cli_add_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/add/test_cli_add_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/backup/test_backup_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/clean/test_balsamic_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/clean/test_clean_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/clean/test_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/clean/test_hk_case_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/clean/test_microbial_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/clean/test_rsync_past_run_dirs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/compress/test_cli_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/compress/test_cli_decompress_spring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/compress/test_compress_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/compress/test_store_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/delete/test_cli_delete_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/delete/test_cli_delete_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/deliver/test_deliver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/deliver/test_rsync_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/deliver/test_run_deliver_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/demultiplex/test_add_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/demultiplex/test_demultiplex_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/demultiplex/test_finish_demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/demultiplex/test_stats_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/demultiplex/test_validate_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/generate/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/generate/report/test_cli_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/generate/report/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/generate/test_cli_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/get/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/get/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/get/test_cli_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/get/test_cli_get_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/get/test_cli_get_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/get/test_cli_get_flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/get/test_cli_get_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/set/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/set/test_cli_set_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/set/test_cli_set_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/set/test_cli_set_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/set/test_cli_set_list_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/set/test_cli_set_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/set/test_cli_set_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/store/test_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/test_clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_scout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_upload_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_upload_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_upload_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_upload_genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_upload_gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_upload_nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_upload_nipt_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_upload_nipt_statina.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_upload_observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_upload_vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/balsamic/test_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/balsamic/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/balsamic/test_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/balsamic/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/balsamic/test_store_housekeeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/fastq/test_fastq_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/fluffy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/fluffy/test_cli_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/fluffy/test_cli_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/fluffy/test_cli_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/fluffy/test_cli_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/microsalt/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/workflow/microsalt/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/microsalt/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/microsalt/test_microsalt_case_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/microsalt/test_microsalt_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_dna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_dna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_dna_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_rna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_rna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/rnafusion/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/workflow/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/taxprofiler/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/test_cli_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/test_cli_workflow_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    62393 2023-05-27 11:20:49.000000 cg-32.2.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/DEMUX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/analysis/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/analysis/balsamic/tn_wgs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/analysis/microsalt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
--rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/analysis/mip/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/ADM2.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/ADM3.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/adm1.mt.bam
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/multiqc.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/report.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/smn.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/snv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/str.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/sv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/sv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/analysis/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/rnafusion/multiqc_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/sample_coverage.bed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/balsamic/case/
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/balsamic/case/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/balsamic/case/metadata.yml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/balsamic/case/metadata_directory.yml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/crunchy/spring_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)    53877 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/RunParameters_different_index_cycles.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/raw_lims_samples/
--rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/fluffy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/fluffy/2020-23219-05/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/fluffy/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/fluffy/deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/fluffy/multiqc_report.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/fluffy/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/gt/yellowhog.bcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/madeline/madeline.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/case_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/mip/dna/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/mip/dna/store/
--rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/dna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
--rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/mip/rna/
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/rna/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/mip/rna/store/
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/rna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/sample_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/scout/643594.config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/scout/case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/scout/export_causatives.json
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/scout/none_case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/scout/other_sex_case.json
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/scout/panel_export.bed
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/scout/panel_export.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/sequencing_metrics_parser/
--rw-r--r--   0 runner    (1001) docker     (123)    63569 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/sequencing_metrics_parser/Adapter_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)    42478 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/sequencing_metrics_parser/Demultiplex_Stats.csv
--rw-r--r--   0 runner    (1001) docker     (123)    69862 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/sequencing_metrics_parser/Quality_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/sequencing_metrics_parser/RunInfo.xml
--rw-r--r--   0 runner    (1001) docker     (123)    42872 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/sequencing_metrics_parser/SampleSheet.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/shipping/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/shipping/scout-deploy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/cgweb_orders/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/cgweb_orders/balsamic.json
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/cgweb_orders/fastq.json
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/cgweb_orders/metagenome.json
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/cgweb_orders/microsalt.json
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/cgweb_orders/mip.json
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/cgweb_orders/mip_rna.json
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/cgweb_orders/rml.json
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/cgweb_orders/sarscov2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/data/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/data/cgfixture.db
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/data/fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/data/hkstore.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/data/yellowhog/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/data/yellowhog/pedigree.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/io/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/io/example_csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/io/example_json.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/orderforms/
--rw-r--r--   0 runner    (1001) docker     (123)   257271 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/1508.27.balsamic.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   256694 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257319 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   256733 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/1508.27.fastq.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257317 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/1508.27.mip.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257230 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/1508.27.mip_rna.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    95490 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/1603.11.microbial.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   158941 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/1604.15.rml.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    88438 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/1605.10.metagenome.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   228196 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/NIPT-json.json
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/report/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/report/case_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/report/lims_exported_samples.json
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/report/lims_family.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-27 11:20:49.000000 cg-32.2.5/tests/io/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-05-27 11:20:49.000000 cg-32.2.5/tests/io/test_io_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-27 11:20:49.000000 cg-32.2.5/tests/io/test_io_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-27 11:20:49.000000 cg-32.2.5/tests/io/test_io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-27 11:20:49.000000 cg-32.2.5/tests/io/test_io_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-27 11:20:49.000000 cg-32.2.5/tests/io/test_validate_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/archive/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/archive/test_archiving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/backup/test_meta_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/backup/test_meta_pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/clean/test_clean_demultiplexed_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/clean/test_clean_flow_cell_run_directories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/compress/test_clean_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/compress/test_compress_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/compress/test_compress_meta_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/compress/test_decompress_spring_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/compress/test_meta_compress_update_hk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/deliver/test_deliver_ticket.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/deliver/test_delivery_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)    11200 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13452 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/demultiplex/test_delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/demultiplex/test_demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/demultiplex/test_rename_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/encryption/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/encryption/test_encryption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/observations/test_meta_upload_observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/orders/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/orders/test_PoolSubmitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/orders/test_SarsCov2Submitter_store_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    19748 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/orders/test_meta_orders_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/orders/test_meta_orders_lims.py
--rw-r--r--   0 runner    (1001) docker     (123)    29658 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/orders/test_meta_orders_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/orders/test_ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/report/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/report/test_balsamic_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/report/test_field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/report/test_mip_dna_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/report/test_report_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/rsync/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/rsync/test_rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/test_invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/transfer/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/transfer/test_external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16507 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/transfer/test_meta_transfer_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/transfer/test_meta_transfer_lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/balsamic/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/gisaid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/upload/gisaid/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/gisaid/fixtures/four_samples.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/upload/mutacc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/mutacc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/mutacc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/nipt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/nipt/test_nipt_upload_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23429 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/scout/test_generate_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/scout/test_meta_upload_scoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/scout/test_scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/test_meta_upload_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/test_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/test_upload_genotypes_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/upload/vogue/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/vogue/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/vogue/test_upload_vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/workflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/workflow/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/workflow/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/workflow/test_microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/workflow/test_prepare_fastq_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/balsamic_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/hk_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/limsmock.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/madeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/mip_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/osticket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/process_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/store_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/tb_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/balsamic/test_balsamic_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/models/demultiplexing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/demultiplexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/demultiplexing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/demultiplexing/test_demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/demultiplexing/test_flowcell_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/demultiplexing/test_run_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/mip/test_mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/mip/test_mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/mip/test_mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/mip/test_mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/nextflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/nextflow/test_nextflow_deliver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/observations/test_observations_input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/report/test_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/rnafusion/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/rnafusion/test_rnafusion_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/test_cg_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/test_compression_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/test_file_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/test_flowcell_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/server/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-27 11:20:49.000000 cg-32.2.5/tests/server/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-27 11:20:49.000000 cg-32.2.5/tests/server/test_server_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-27 11:20:49.000000 cg-32.2.5/tests/server/test_server_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-27 11:20:49.000000 cg-32.2.5/tests/small_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/store/api/add/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/add/test_store_add_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/add/test_store_add_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/add/test_store_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/add/test_store_add_flow_celll.py
--rw-r--r--   0 runner    (1001) docker     (123)    17674 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/store/api/delete/
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/delete/test_store_api_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/store/api/find/
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/find/test_find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/find/test_find_basic_data_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    27415 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/find/test_find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/find/test_find_business_data_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/find/test_find_business_data_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    12223 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/find/test_find_business_data_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/store/api/status/
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/status/test_analyses_to_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/status/test_analyses_to_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/status/test_store_api_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/status/test_store_api_status_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    54170 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/status/test_store_api_status_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/status/test_store_api_status_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/status/test_store_api_status_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/status/test_store_api_status_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_analyses_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    38171 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_cases_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    22968 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_samples_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/test_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/test_store_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30182 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-27 11:20:49.000000 cg-32.2.5/tests/test_store_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-27 11:20:49.000000 cg-32.2.5/tests/utils/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-27 11:20:49.000000 cg-32.2.5/tests/utils/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-27 11:20:49.000000 cg-32.2.5/tests/utils/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-27 11:20:49.000000 cg-32.2.5/tests/utils/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-05-27 11:20:49.000000 cg-32.2.5/tests/utils/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-27 11:20:49.000000 cg-32.2.5/tests/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-29 10:48:14.000000 cg-32.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-29 10:48:24.000000 cg-32.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-29 10:48:14.000000 cg-32.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-29 10:48:14.000000 cg-32.2.7/cg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16023 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/crud/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/crud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/crud/find.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/cgstats/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/cgstats/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/db/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/db/models/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/db/models/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/db/models/demux_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/db/models/dragen_demux_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/db/models/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/db/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/db/models/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/db/models/support_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/db/models/unaligned.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/db/models/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/parsers/adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/parsers/conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/parsers/demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/parsers/quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/parsers/run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/cgstats/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/coverage/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/crunchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/crunchy/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/crunchy/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/crunchy/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/demultiplex/demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/demultiplex/demux_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/demultiplex/sample_sheet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/demultiplex/sample_sheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/demultiplex/sample_sheet/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/demultiplex/sample_sheet/dummy_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/demultiplex/sample_sheet/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/demultiplex/sample_sheet/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/demultiplex/sample_sheet/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/hermes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/hermes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/hermes/hermes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/hermes/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/housekeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/housekeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/housekeeper/hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/housekeeper/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/invoice/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/invoice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/invoice/templates/KI_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/invoice/templates/KI_sample_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/lims/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/lims/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/lims/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/lims/sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/loqus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/madeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/madeline/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/mip/confighandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/orderform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/orderform/excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/orderform/json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/orderform/orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/scout/scout_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/scout/scoutapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/sequencing_metrics_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/sequencing_metrics_parser/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/sequencing_metrics_parser/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/sequencing_metrics_parser/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/sequencing_metrics_parser/models/bcl_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/sequencing_metrics_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/sequencing_metrics_parser/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/slurm/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/slurm/slurm_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/apps/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/tb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/tb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/tb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-29 10:48:14.000000 cg-32.2.7/cg/apps/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/compress/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/compress/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/compress/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/delete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/delete/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/delete/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/delete/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/delete/observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/deliver/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/demultiplex/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/demultiplex/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/demultiplex/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/demultiplex/finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/demultiplex/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/demultiplex/sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/generate/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/generate/report/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/generate/report/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/generate/report/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/set/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/set/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/set/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/set/cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/store/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/store/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/upload/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/upload/clinical_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/upload/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/upload/delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/upload/fohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/upload/genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/upload/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/upload/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/upload/nipt/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/upload/nipt/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/upload/nipt/statina.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/upload/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/upload/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/upload/observations/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/upload/observations/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/upload/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/upload/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/upload/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/upload/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/balsamic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/balsamic/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/balsamic/pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/balsamic/qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/balsamic/umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/fastq/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/fluffy/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/microsalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/microsalt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/mip/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/mip/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/workflow/mip_dna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/mip_dna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/mip_dna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/workflow/mip_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/mip_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/mip_rna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/workflow/mutant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/mutant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/mutant/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/workflow/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/nextflow/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/rnafusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/rnafusion/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/workflow/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/taxprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/taxprofiler/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/cli/workflow/tower/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/tower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-29 10:48:14.000000 cg-32.2.7/cg/cli/workflow/tower/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/bcl_convert_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/cgstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/demultiplexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/gene_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/housekeeper_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/nextflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/orderforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/pdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/sample_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/scout_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/sequencing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-29 10:48:14.000000 cg-32.2.7/cg/constants/tb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-29 10:48:14.000000 cg-32.2.7/cg/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-29 10:48:14.000000 cg-32.2.7/cg/io/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-29 10:48:14.000000 cg-32.2.7/cg/io/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-29 10:48:14.000000 cg-32.2.7/cg/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-29 10:48:14.000000 cg-32.2.7/cg/io/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-29 10:48:14.000000 cg-32.2.7/cg/io/validate_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-29 10:48:14.000000 cg-32.2.7/cg/io/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-29 10:48:14.000000 cg-32.2.7/cg/io/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/archive/ddn_dataflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/backup/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/backup/pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/clean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/clean/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/clean/demultiplexed_flow_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/clean/flow_cell_run_directories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/compress/compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/compress/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/deliver_ticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/demultiplex/delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/demultiplex/demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/demultiplex/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/encryption/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/observations/balsamic_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/observations/mip_dna_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/observations/observations_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/orders/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/orders/balsamic_qc_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/orders/balsamic_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/orders/balsamic_umi_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/orders/case_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/orders/fastq_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/orders/fluffy_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/orders/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/orders/metagenome_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/orders/microbial_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/orders/microsalt_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/orders/mip_dna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/orders/mip_rna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/orders/pool_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/orders/rml_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/orders/sars_cov_2_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/orders/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/orders/ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/report/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/report/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/report/field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/report/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/report/report_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/report/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/report/templates/balsamic_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/report/templates/bootstrap.html
+-rw-r--r--   0 runner    (1001) docker     (123)    77831 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/report/templates/mip-dna_report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/rsync/rsync_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/rsync/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/tar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/tar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/tar/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/transfer/external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/transfer/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/transfer/lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/balsamic/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/upload/fohm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/fohm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/fohm/fohm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/gisaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/gisaid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/gisaid/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/gisaid/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/upload/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/mip/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/mip/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/nipt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/nipt/nipt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/upload/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/rnafusion/rnafusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/scout/balsamic_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/scout/balsamic_umi_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/scout/hk_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/scout/mip_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/scout/rnafusion_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/scout/scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18719 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/scout/uploadscoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/upload/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/workflow/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/workflow/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/workflow/balsamic_pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/workflow/balsamic_qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/workflow/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/workflow/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/workflow/fluffy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/workflow/microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/workflow/mip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/workflow/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/workflow/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/workflow/mutant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/workflow/nextflow_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/workflow/prepare_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17110 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/workflow/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/workflow/taxprofiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-29 10:48:14.000000 cg-32.2.7/cg/meta/workflow/tower_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/balsamic/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/balsamic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/balsamic/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12924 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/cg_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/models/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/cgstats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/cgstats/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/cgstats/stats_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/compression_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/models/deliverables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/deliverables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/deliverables/metric_deliverables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/models/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/demultiplex/demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/demultiplex/flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/demultiplex/run_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/file_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/models/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/invoice/invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/models/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/lims/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/mip/mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/mip/mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/mip/mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/mip/mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/nextflow/deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/nextflow/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/observations/input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/models/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/orders/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/orders/excel_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/orders/json_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/orders/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/orders/orderform_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/orders/sample_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/orders/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/report/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/report/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/report/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/rnafusion/rnafusion_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/models/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/scout/scout_load_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/models/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/slurm/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/models/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/taxprofiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/models/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-29 10:48:14.000000 cg-32.2.7/cg/models/workflow/mutant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-05-29 10:48:14.000000 cg-32.2.7/cg/resources/20181012_Indices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-29 10:48:14.000000 cg-32.2.7/cg/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-29 10:48:14.000000 cg-32.2.7/cg/resources/rnafusion_bundle_filenames.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-05-29 10:48:14.000000 cg-32.2.7/cg/server/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19037 2023-05-29 10:48:14.000000 cg-32.2.7/cg/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-29 10:48:14.000000 cg-32.2.7/cg/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-29 10:48:14.000000 cg-32.2.7/cg/server/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-29 10:48:14.000000 cg-32.2.7/cg/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-29 10:48:14.000000 cg-32.2.7/cg/server/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/server/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-29 10:48:14.000000 cg-32.2.7/cg/server/invoices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/server/invoices/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/server/invoices/templates/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-29 10:48:14.000000 cg-32.2.7/cg/server/invoices/templates/invoices/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-29 10:48:14.000000 cg-32.2.7/cg/server/invoices/templates/invoices/invoice.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-29 10:48:14.000000 cg-32.2.7/cg/server/invoices/templates/invoices/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-29 10:48:14.000000 cg-32.2.7/cg/server/invoices/templates/invoices/new.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-05-29 10:48:14.000000 cg-32.2.7/cg/server/invoices/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/server/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/server/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-29 10:48:14.000000 cg-32.2.7/cg/server/templates/admin/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/store/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/api/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/api/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/api/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/api/find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28994 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/api/find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38700 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/api/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/filters/status_analysis_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/filters/status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/filters/status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/filters/status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/filters/status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/filters/status_case_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/filters/status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/filters/status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/filters/status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/filters/status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/filters/status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/filters/status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/filters/status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/filters/status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/filters/status_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/filters/status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29946 2023-05-29 10:48:14.000000 cg-32.2.7/cg/store/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-29 10:48:14.000000 cg-32.2.7/cg/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/utils/checksum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/utils/checksum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-29 10:48:14.000000 cg-32.2.7/cg/utils/checksum/checksum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/utils/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-29 10:48:14.000000 cg-32.2.7/cg/utils/click/EnumChoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/utils/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-29 10:48:14.000000 cg-32.2.7/cg/utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-29 10:48:14.000000 cg-32.2.7/cg/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-29 10:48:14.000000 cg-32.2.7/cg/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-29 10:48:14.000000 cg-32.2.7/cg/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-29 10:48:14.000000 cg-32.2.7/cg/utils/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-29 10:48:14.000000 cg-32.2.7/cg/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-29 10:48:14.000000 cg-32.2.7/cg/utils/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg/utils/flask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/cg/utils/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-29 10:48:14.000000 cg-32.2.7/cg/utils/flask/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-29 10:48:14.000000 cg-32.2.7/cg/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-29 10:48:14.000000 cg-32.2.7/cg/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/cg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-29 10:48:23.000000 cg-32.2.7/cg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40545 2023-05-29 10:48:24.000000 cg-32.2.7/cg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:48:23.000000 cg-32.2.7/cg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 10:48:23.000000 cg-32.2.7/cg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:48:23.000000 cg-32.2.7/cg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-29 10:48:23.000000 cg-32.2.7/cg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-29 10:48:23.000000 cg-32.2.7/cg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-29 10:48:14.000000 cg-32.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-29 10:48:14.000000 cg-32.2.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 10:48:24.000000 cg-32.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-29 10:48:14.000000 cg-32.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/cgstats/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/cgstats/crud/test_create_novaseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/cgstats/crud/test_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/cgstats/parsers/test_adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/cgstats/parsers/test_conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/cgstats/parsers/test_demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/cgstats/parsers/test_quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/cgstats/parsers/test_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/cgstats/test_cgstats_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/cgstats/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/coverage/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/coverage/test_coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/crunchy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/crunchy/test_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/crunchy/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/crunchy/test_crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/crunchy/test_spring_decompression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/demultiplex/test_convert_to_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/demultiplex/test_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/demultiplex/test_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/demultiplex/test_validate_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/apps/gens/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/gens/test_gens_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/gt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/gt/test_gt_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/apps/hk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/hk/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/hk/test__getattr__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/hk/test_add_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/hk/test_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/hk/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/hk/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/hk/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/lims/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/lims/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/lims/test_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/apps/loqus/
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/loqus/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/loqus/test_loqusdb_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/madeline/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/madeline/test_madeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/mip/test_config_mip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/apps/mutacc_auto/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/mutacc_auto/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/mutacc_auto/test_mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/orderform/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/orderform/test_excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/orderform/test_excel_sample_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/orderform/test_json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/orderform/test_orderform_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/scout/test_get_causative_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/scout/test_get_scout_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/scout/test_scout_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/scout/test_scout_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/apps/sequencing_metrics_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/sequencing_metrics_parser/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/apps/sequencing_metrics_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/sequencing_metrics_parser/parsers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/slurm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/slurm/test_slurm_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/test_apps_environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/test_osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/apps/vogue/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/vogue/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-29 10:48:14.000000 cg-32.2.7/tests/apps/vogue/test_vogue_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/add/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/add/test_cli_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/add/test_cli_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/add/test_cli_add_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/add/test_cli_add_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/add/test_cli_add_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/backup/test_backup_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/clean/test_balsamic_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/clean/test_clean_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/clean/test_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/clean/test_hk_case_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/clean/test_microbial_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/clean/test_rsync_past_run_dirs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/compress/test_cli_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/compress/test_cli_decompress_spring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/compress/test_compress_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/compress/test_store_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/delete/test_cli_delete_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/delete/test_cli_delete_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/deliver/test_deliver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/deliver/test_rsync_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/deliver/test_run_deliver_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/demultiplex/test_add_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/demultiplex/test_demultiplex_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/demultiplex/test_finish_demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/demultiplex/test_stats_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/demultiplex/test_validate_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/generate/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/generate/report/test_cli_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/generate/report/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/generate/test_cli_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/get/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/get/test_cli_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/get/test_cli_get_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/get/test_cli_get_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/get/test_cli_get_flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/get/test_cli_get_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/set/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/set/test_cli_set_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/set/test_cli_set_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/set/test_cli_set_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/set/test_cli_set_list_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/set/test_cli_set_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/set/test_cli_set_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/store/test_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/test_clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/upload/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/upload/test_cli_scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/upload/test_cli_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/upload/test_cli_upload_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/upload/test_cli_upload_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/upload/test_cli_upload_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/upload/test_cli_upload_genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/upload/test_cli_upload_gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/upload/test_cli_upload_nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/upload/test_cli_upload_nipt_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/upload/test_cli_upload_nipt_statina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/upload/test_cli_upload_observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/upload/test_cli_upload_vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/balsamic/test_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/balsamic/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/balsamic/test_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/balsamic/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/balsamic/test_store_housekeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/fastq/test_fastq_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/fluffy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/fluffy/test_cli_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/fluffy/test_cli_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/fluffy/test_cli_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/fluffy/test_cli_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/microsalt/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/workflow/microsalt/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/microsalt/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/microsalt/test_microsalt_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/microsalt/test_microsalt_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/mip/test_cli_mip_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/mip/test_cli_mip_dna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/mip/test_cli_mip_dna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/mip/test_cli_mip_dna_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/mip/test_cli_mip_rna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/mip/test_cli_mip_rna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/mip/test_cli_mip_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/rnafusion/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/cli/workflow/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/taxprofiler/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/test_cli_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-29 10:48:14.000000 cg-32.2.7/tests/cli/workflow/test_cli_workflow_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62393 2023-05-29 10:48:14.000000 cg-32.2.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/DEMUX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/analysis/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/analysis/balsamic/tn_wgs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/analysis/microsalt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
+-rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/analysis/mip/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/analysis/mip/dna/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/mip/dna/ADM2.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/mip/dna/ADM3.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/mip/dna/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/mip/dna/adm1.mt.bam
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/mip/dna/multiqc.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/mip/dna/report.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/mip/dna/smn.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/mip/dna/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/mip/dna/snv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/mip/dna/str.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/mip/dna/sv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/mip/dna/sv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/analysis/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/rnafusion/multiqc_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/analysis/sample_coverage.bed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/balsamic/case/
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/balsamic/case/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/balsamic/case/metadata.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/balsamic/case/metadata_directory.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/crunchy/spring_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    53877 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/RunParameters_different_index_cycles.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/hiseq_run/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/raw_lims_samples/
+-rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/fluffy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/fluffy/2020-23219-05/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/fluffy/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/fluffy/deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/fluffy/multiqc_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/fluffy/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/gt/yellowhog.bcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/madeline/madeline.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/mip/case_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/mip/dna/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/mip/dna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/mip/dna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/mip/rna/
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/mip/rna/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/mip/rna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/mip/rna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/mip/sample_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/scout/643594.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/scout/case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/scout/export_causatives.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/scout/none_case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/scout/other_sex_case.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/scout/panel_export.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/scout/panel_export.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/sequencing_metrics_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)    63569 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/sequencing_metrics_parser/Adapter_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    42478 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/sequencing_metrics_parser/Demultiplex_Stats.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    69862 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/sequencing_metrics_parser/Quality_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/sequencing_metrics_parser/RunInfo.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    42872 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/sequencing_metrics_parser/SampleSheet.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/apps/shipping/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/apps/shipping/scout-deploy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/cgweb_orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/cgweb_orders/balsamic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/cgweb_orders/fastq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/cgweb_orders/metagenome.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/cgweb_orders/microsalt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/cgweb_orders/mip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/cgweb_orders/mip_rna.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/cgweb_orders/rml.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/cgweb_orders/sarscov2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/data/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/data/cgfixture.db
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/data/fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/data/hkstore.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/data/yellowhog/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/data/yellowhog/pedigree.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/io/example_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/io/example_json.json
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/io/example_xml.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/orderforms/
+-rw-r--r--   0 runner    (1001) docker     (123)   257271 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/orderforms/1508.27.balsamic.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   256694 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257319 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   256733 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/orderforms/1508.27.fastq.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257317 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/orderforms/1508.27.mip.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257230 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/orderforms/1508.27.mip_rna.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    95490 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/orderforms/1603.11.microbial.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   158941 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/orderforms/1604.15.rml.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    88438 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/orderforms/1605.10.metagenome.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   228196 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/orderforms/NIPT-json.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/fixtures/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/report/case_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/report/lims_exported_samples.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-29 10:48:14.000000 cg-32.2.7/tests/fixtures/report/lims_family.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-29 10:48:14.000000 cg-32.2.7/tests/io/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-05-29 10:48:14.000000 cg-32.2.7/tests/io/test_io_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-29 10:48:14.000000 cg-32.2.7/tests/io/test_io_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-29 10:48:14.000000 cg-32.2.7/tests/io/test_io_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-29 10:48:14.000000 cg-32.2.7/tests/io/test_io_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-29 10:48:14.000000 cg-32.2.7/tests/io/test_io_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-29 10:48:14.000000 cg-32.2.7/tests/io/test_validate_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/archive/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/archive/test_archiving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/backup/test_meta_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/backup/test_meta_pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/clean/test_clean_demultiplexed_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/clean/test_clean_flow_cell_run_directories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/compress/test_clean_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/compress/test_compress_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/compress/test_compress_meta_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/compress/test_decompress_spring_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/compress/test_meta_compress_update_hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/meta/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/deliver/test_deliver_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/deliver/test_delivery_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)    11200 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13452 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/demultiplex/test_delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/demultiplex/test_demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/demultiplex/test_rename_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/encryption/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/encryption/test_encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/observations/test_meta_upload_observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/orders/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/orders/test_PoolSubmitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/orders/test_SarsCov2Submitter_store_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19748 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/orders/test_meta_orders_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/orders/test_meta_orders_lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29658 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/orders/test_meta_orders_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/orders/test_ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/report/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/report/test_balsamic_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/report/test_field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/report/test_mip_dna_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/report/test_report_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/rsync/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/rsync/test_rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/test_invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/transfer/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/transfer/test_external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16507 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/transfer/test_meta_transfer_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/transfer/test_meta_transfer_lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/balsamic/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/gisaid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/meta/upload/gisaid/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/gisaid/fixtures/four_samples.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/meta/upload/mutacc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/mutacc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/mutacc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/nipt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/nipt/test_nipt_upload_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23429 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/scout/test_generate_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/scout/test_meta_upload_scoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/scout/test_scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/test_meta_upload_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/test_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/test_upload_genotypes_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/meta/upload/vogue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/vogue/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/upload/vogue/test_upload_vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/workflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/workflow/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/workflow/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/workflow/test_microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-29 10:48:14.000000 cg-32.2.7/tests/meta/workflow/test_prepare_fastq_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-29 10:48:14.000000 cg-32.2.7/tests/mocks/balsamic_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-29 10:48:14.000000 cg-32.2.7/tests/mocks/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-05-29 10:48:14.000000 cg-32.2.7/tests/mocks/hk_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-29 10:48:14.000000 cg-32.2.7/tests/mocks/limsmock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-29 10:48:14.000000 cg-32.2.7/tests/mocks/madeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-29 10:48:14.000000 cg-32.2.7/tests/mocks/mip_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-29 10:48:14.000000 cg-32.2.7/tests/mocks/osticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-29 10:48:14.000000 cg-32.2.7/tests/mocks/process_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-29 10:48:14.000000 cg-32.2.7/tests/mocks/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-29 10:48:14.000000 cg-32.2.7/tests/mocks/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-29 10:48:14.000000 cg-32.2.7/tests/mocks/store_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-29 10:48:14.000000 cg-32.2.7/tests/mocks/tb_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/balsamic/test_balsamic_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/models/demultiplexing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/demultiplexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/demultiplexing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/demultiplexing/test_demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/demultiplexing/test_flowcell_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/demultiplexing/test_run_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/mip/test_mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/mip/test_mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/mip/test_mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/mip/test_mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/nextflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/nextflow/test_nextflow_deliver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/observations/test_observations_input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/report/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/rnafusion/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/rnafusion/test_rnafusion_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/test_cg_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/test_compression_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/test_file_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-29 10:48:14.000000 cg-32.2.7/tests/models/test_flowcell_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-29 10:48:14.000000 cg-32.2.7/tests/server/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-29 10:48:14.000000 cg-32.2.7/tests/server/test_server_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-29 10:48:14.000000 cg-32.2.7/tests/server/test_server_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-29 10:48:14.000000 cg-32.2.7/tests/small_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/store/api/add/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/api/add/test_store_add_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/api/add/test_store_add_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/api/add/test_store_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/api/add/test_store_add_flow_celll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17674 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/api/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/store/api/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/api/delete/test_store_api_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/store/api/find/
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/api/find/test_find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/api/find/test_find_basic_data_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27415 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/api/find/test_find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/api/find/test_find_business_data_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/api/find/test_find_business_data_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12223 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/api/find/test_find_business_data_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/store/api/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/api/status/test_analyses_to_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/api/status/test_analyses_to_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/api/status/test_store_api_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/api/status/test_store_api_status_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54170 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/api/status/test_store_api_status_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/api/status/test_store_api_status_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/api/status/test_store_api_status_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/api/status/test_store_api_status_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/api/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/filters/test_status_analyses_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/filters/test_status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/filters/test_status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/filters/test_status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/filters/test_status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/filters/test_status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38171 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/filters/test_status_cases_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/filters/test_status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/filters/test_status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/filters/test_status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/filters/test_status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/filters/test_status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/filters/test_status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/filters/test_status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22968 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/filters/test_status_samples_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/filters/test_status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/test_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store/test_store_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30182 2023-05-29 10:48:14.000000 cg-32.2.7/tests/store_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-29 10:48:14.000000 cg-32.2.7/tests/test_store_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:24.000000 cg-32.2.7/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:48:14.000000 cg-32.2.7/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-29 10:48:14.000000 cg-32.2.7/tests/utils/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-29 10:48:14.000000 cg-32.2.7/tests/utils/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-29 10:48:14.000000 cg-32.2.7/tests/utils/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-29 10:48:14.000000 cg-32.2.7/tests/utils/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-05-29 10:48:14.000000 cg-32.2.7/tests/utils/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-29 10:48:14.000000 cg-32.2.7/tests/utils/test_utils.py
```

### Comparing `cg-32.2.5/PKG-INFO` & `cg-32.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 32.2.5
+Version: 32.2.7
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-32.2.5/README.md` & `cg-32.2.7/README.md`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/cgstats/crud/create.py` & `cg-32.2.7/cg/apps/cgstats/crud/create.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,21 @@
     Flowcell,
     Project,
     Supportparams,
     Sample,
     Unaligned,
 )
 from cg.apps.cgstats.stats import StatsAPI
-from cg.apps.demultiplex.sample_sheet.models import NovaSeqSample, SampleSheet
-from cg.constants.demultiplexing import DRAGEN_PASSED_FILTER_PCT
+from cg.apps.demultiplex.sample_sheet.models import (
+    FlowCellSample,
+    FlowCellSampleBcl2Fastq,
+    FlowCellSampleDragen,
+    SampleSheet,
+)
+from cg.constants.demultiplexing import DRAGEN_PASSED_FILTER_PCT, BclConverter
 from cg.constants.symbols import PERIOD
 from cg.models.demultiplex.demux_results import DemuxResults, LogfileParameters
 
 LOG = logging.getLogger(__name__)
 
 
 def create_support_parameters(manager: StatsAPI, demux_results: DemuxResults) -> Supportparams:
@@ -202,23 +207,23 @@
             manager=manager, project_name=project_name
         )
         project_name_to_id[project_name] = project.project_id
     return project_name_to_id
 
 
 def get_or_create_sample(
-    manager: StatsAPI, sample: NovaSeqSample, project_name_to_id: Dict[str, int]
+    manager: StatsAPI, sample: FlowCellSample, project_name_to_id: Dict[str, int]
 ) -> Sample:
     """Create a new Sample object in the cgstats database if it doesn't already exist."""
 
     if sample.project == "indexcheck":
         LOG.debug("Skip adding indexcheck sample to database")
         return None
 
-    barcode = f"{sample.index}+{sample.second_index}" if sample.second_index else sample.index
+    barcode = f"{sample.index}+{sample.index2}" if sample.index2 else sample.index
 
     stats_sample: Optional[Sample] = manager.find_handler.get_sample_by_name_and_barcode(
         sample_name=sample.sample_id, barcode=barcode
     )
 
     if not stats_sample:
         project_id = project_name_to_id[sample.project]
@@ -244,15 +249,15 @@
     tables in cgstats for samples demultiplexed with Dragen"""
 
     demux_samples: Dict[int, dict] = manager.find_handler.get_dragen_demux_samples(
         demux_results=demux_results,
         sample_sheet=sample_sheet,
     )
 
-    sample: NovaSeqSample
+    sample: FlowCellSampleDragen
     for sample in sample_sheet.samples:
         stats_sample: Sample = get_or_create_sample(
             manager=manager, sample=sample, project_name_to_id=project_name_to_id
         )
 
         if not stats_sample:
             continue
@@ -280,15 +285,15 @@
 
     demux_samples: Dict[int, Dict[str, DemuxSample]] = manager.find_handler.get_demux_samples(
         conversion_stats=demux_results.conversion_stats,
         demux_stats_path=demux_results.demux_stats_path,
         sample_sheet=sample_sheet,
     )
 
-    sample: NovaSeqSample
+    sample: FlowCellSampleBcl2Fastq
     for sample in sample_sheet.samples:
         stats_sample: Sample = get_or_create_sample(
             manager=manager, sample=sample, project_name_to_id=project_name_to_id
         )
 
         if not stats_sample:
             continue
@@ -316,16 +321,16 @@
 ) -> None:
     """dispatches sample object and unaligned object creation for samples based on the
     bcl-converter used in demultiplexing."""
     LOG.info(f"Creating samples for flow cell {demux_results.flow_cell.full_name}")
     sample_sheet: SampleSheet = demux_results.flow_cell.get_sample_sheet()
 
     create_samples_function = {
-        "dragen": _create_dragen_samples,
-        "bcl2fastq": _create_bcl2fastq_samples,
+        BclConverter.DRAGEN.value: _create_dragen_samples,
+        BclConverter.BCL2FASTQ.value: _create_bcl2fastq_samples,
     }
     create_samples_function[demux_results.bcl_converter](
         manager, demux_results, project_name_to_id, demux_id, sample_sheet
     )
 
 
 def create_novaseq_flowcell(manager: StatsAPI, demux_results: DemuxResults):
@@ -400,16 +405,16 @@
         LOG.info("Support parameters already exists")
 
     return support_parameters
 
 
 def get_document_stats_path_from_demux(demux_results: DemuxResults) -> str:
     stats_path = {
-        "bcl2fastq": demux_results.conversion_stats_path,
-        "dragen": demux_results.demux_stats_path,
+        BclConverter.BCL2FASTQ.value: demux_results.conversion_stats_path,
+        BclConverter.DRAGEN.value: demux_results.demux_stats_path,
     }
     document_path: str = str(stats_path[demux_results.bcl_converter])
     return document_path
 
 
 def get_or_create_datasource(
     manager: StatsAPI, demux_results: DemuxResults, support_parameters_id: int
```

### Comparing `cg-32.2.5/cg/apps/cgstats/crud/delete.py` & `cg-32.2.7/cg/apps/cgstats/crud/delete.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/cgstats/crud/find.py` & `cg-32.2.7/cg/apps/cgstats/crud/find.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Flowcell,
     Project,
     Sample,
     Unaligned,
 )
 from cg.apps.cgstats.parsers.conversion_stats import ConversionStats, SampleConversionResults
 from cg.apps.cgstats.parsers.demux_stats import DemuxStats, SampleBarcodeStats
-from cg.apps.demultiplex.sample_sheet.models import NovaSeqSample, SampleSheet
+from cg.apps.demultiplex.sample_sheet.models import FlowCellSample, SampleSheet
 from cg.models.cgstats.stats_sample import StatsSample
 from cg.models.demultiplex.demux_results import DemuxResults
 
 LOG = logging.getLogger(__name__)
 SAMPLE_PATTERN = "{}\_%"
 
 
@@ -167,24 +167,20 @@
         """Gather information from demultiplexing results and create samples with the correct
         information"""
         LOG.info("Gather post demultiplexing statistics for demultiplexed samples")
         demux_samples: Dict[int, Dict[str, DemuxSample]] = {}
         demux_stats: DemuxStats = DemuxStats(demux_stats_path=demux_stats_path)
         raw_clusters: Dict[int, int] = conversion_stats.raw_clusters_per_lane
         flowcell_id: str = conversion_stats.flowcell_id
-        sample: NovaSeqSample
+        sample: FlowCellSample
         for sample in sample_sheet.samples:
             lane: int = sample.lane
             if lane not in demux_samples:
                 demux_samples[lane] = {}
-            barcode = (
-                "+".join([sample.index, sample.second_index])
-                if sample.second_index
-                else sample.index
-            )
+            barcode = "+".join([sample.index, sample.index2]) if sample.index2 else sample.index
             sample_barcode_stats: SampleBarcodeStats = demux_stats.lanes_to_barcode[lane][barcode]
             sample_conversion_stats: SampleConversionResults = conversion_stats.lanes_to_barcode[
                 lane
             ][barcode]
             lane_raw_cluster: int = raw_clusters[lane]
             sample_id: str = sample.sample_id
             demux_samples[lane][sample_id] = DemuxSample(
```

### Comparing `cg-32.2.5/cg/apps/cgstats/db/models/base.py` & `cg-32.2.7/cg/apps/cgstats/db/models/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/cgstats/db/models/datasource.py` & `cg-32.2.7/cg/apps/cgstats/db/models/datasource.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/cgstats/db/models/demux.py` & `cg-32.2.7/cg/apps/cgstats/db/models/demux.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/cgstats/db/models/demux_sample.py` & `cg-32.2.7/cg/apps/cgstats/db/models/demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/cgstats/db/models/dragen_demux_sample.py` & `cg-32.2.7/cg/apps/cgstats/db/models/dragen_demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/cgstats/db/models/sample.py` & `cg-32.2.7/cg/apps/cgstats/db/models/sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/cgstats/db/models/support_params.py` & `cg-32.2.7/cg/apps/cgstats/db/models/support_params.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/cgstats/db/models/unaligned.py` & `cg-32.2.7/cg/apps/cgstats/db/models/unaligned.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/cgstats/db/models/version.py` & `cg-32.2.7/cg/apps/cgstats/db/models/version.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/cgstats/parsers/adapter_metrics.py` & `cg-32.2.7/cg/apps/cgstats/parsers/adapter_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/cgstats/parsers/conversion_stats.py` & `cg-32.2.7/cg/apps/cgstats/parsers/conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/cgstats/parsers/demux_stats.py` & `cg-32.2.7/cg/apps/cgstats/parsers/demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py` & `cg-32.2.7/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/cgstats/parsers/quality_metrics.py` & `cg-32.2.7/cg/apps/cgstats/parsers/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/cgstats/parsers/run_info.py` & `cg-32.2.7/cg/apps/cgstats/parsers/run_info.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/cgstats/stats.py` & `cg-32.2.7/cg/apps/cgstats/stats.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/coverage/api.py` & `cg-32.2.7/cg/apps/coverage/api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/crunchy/crunchy.py` & `cg-32.2.7/cg/apps/crunchy/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/crunchy/files.py` & `cg-32.2.7/cg/apps/crunchy/files.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/crunchy/sbatch.py` & `cg-32.2.7/cg/apps/crunchy/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/demultiplex/demultiplex_api.py` & `cg-32.2.7/cg/apps/demultiplex/demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/demultiplex/demux_report.py` & `cg-32.2.7/cg/apps/demultiplex/demux_report.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/demultiplex/sample_sheet/create.py` & `cg-32.2.7/cg/apps/demultiplex/sample_sheet/create.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import logging
 from typing import List
 from typing_extensions import Literal
 
 from cg.apps.demultiplex.sample_sheet.novaseq_sample_sheet import SampleSheetCreator
-from cg.apps.lims.samplesheet import LimsFlowcellSample
+from cg.apps.demultiplex.sample_sheet.models import FlowCellSample
 from cg.constants.sequencing import Sequencers
 from cg.constants.demultiplexing import BclConverter
 from cg.exc import FlowCellError
 from cg.models.demultiplex.flow_cell import FlowCell
 
 LOG = logging.getLogger(__name__)
 
 
 def create_sample_sheet(
     bcl_converter: Literal[BclConverter.BCL2FASTQ, BclConverter.DRAGEN],
     flow_cell: FlowCell,
-    lims_samples: List[LimsFlowcellSample],
+    lims_samples: List[FlowCellSample],
     force: bool = False,
 ) -> List[List[str]]:
     """Create a sample sheet for a flow cell."""
     if flow_cell.sample_sheet_path.exists():
         message = f"Sample sheet {flow_cell.sample_sheet_path} already exists!"
         LOG.warning(message)
         raise FileExistsError(message)
```

### Comparing `cg-32.2.5/cg/apps/demultiplex/sample_sheet/index.py` & `cg-32.2.7/cg/apps/demultiplex/sample_sheet/index.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Functions that deals with modifications of the indexes"""
 import csv
 import logging
 from typing import Dict, List, Set
 
-from cg.apps.lims.samplesheet import LimsFlowcellSample
+from cg.apps.demultiplex.sample_sheet.models import FlowCellSample
 from cg.resources import VALID_INDEXES_PATH
 from packaging import version
 from pydantic import BaseModel
 
 LOG = logging.getLogger(__name__)
 NEW_CONTROL_SOFTWARE_VERSION = "1.7.0"
 NEW_REAGENT_KIT_VERSION = "1.5"
@@ -16,15 +16,15 @@
 
 
 def index_exists(index: str, indexes: Set[str]) -> bool:
     """Determines if an index is already present in the existing indexes."""
     return any(existing_index.startswith(index) for existing_index in indexes)
 
 
-def get_indexes_by_lane(samples: List[LimsFlowcellSample]) -> Dict[int, Set[str]]:
+def get_indexes_by_lane(samples: List[FlowCellSample]) -> Dict[int, Set[str]]:
     """Group the indexes from samples by lane."""
     indexes_by_lane = {}
     for sample in samples:
         lane: int = sample.lane
         if lane not in indexes_by_lane:
             indexes_by_lane[lane] = set()
         indexes_by_lane[lane].add(sample.index)
@@ -96,15 +96,15 @@
     """Adds bases to index two depending on if it should be reverse complement or not."""
     if reverse_complement:
         return "AC" + index_string
     return index_string + "AC"
 
 
 def adapt_indexes(
-    samples: List[LimsFlowcellSample],
+    samples: List[FlowCellSample],
     control_software_version: str,
     reagent_kit_version: str,
     expected_index_length: int,
 ) -> None:
     """Adapts the indexes: pads all indexes so that all indexes have a length equal to the
     number  of index reads, and takes the reverse complement of index 2 in case of the new
     novaseq software control version (1.7) in combination with the new reagent kit
```

### Comparing `cg-32.2.5/cg/apps/demultiplex/sample_sheet/models.py` & `cg-32.2.7/cg/apps/demultiplex/sample_sheet/models.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 import logging
 from pydantic import BaseModel, Field
 from typing import List
 
+from cg.constants.constants import GenomeVersion
 from cg.constants.demultiplexing import SampleSheetHeaderColumnNames
 
 LOG = logging.getLogger(__name__)
 
 
-class NovaSeqSample(BaseModel):
+class FlowCellSample(BaseModel):
     """This model is used when parsing/validating existing sample sheets."""
 
-    flow_cell: str = Field(..., alias=SampleSheetHeaderColumnNames.FLOW_CELL_ID.value)
-    lane: int = Field(..., alias="Lane")
-    sample_id: str = Field(..., alias="SampleID")
-    reference: str = Field(..., alias="SampleRef")
+    flowcell_id: str = Field(..., alias=SampleSheetHeaderColumnNames.FLOW_CELL_ID.value)
+    lane: int = Field(..., alias=SampleSheetHeaderColumnNames.LANE.value)
+    sample_id: str
+    sample_ref: str = Field(GenomeVersion.hg19.value, alias="SampleRef")
     index: str = Field(..., alias="index")
+    index2: str = ""
     sample_name: str = Field(..., alias="SampleName")
-    control: str = Field(..., alias="Control")
-    recipe: str = Field(..., alias="Recipe")
-    operator: str = Field(..., alias="Operator")
+    control: str = Field("N", alias="Control")
+    recipe: str = Field("R1", alias="Recipe")
+    operator: str = Field("script", alias="Operator")
     project: str = Field(..., alias="Project")
-    second_index: str = Field(..., alias="index2")
+
+    class Config:
+        allow_population_by_field_name = True
 
 
-class SampleBcl2Fastq(NovaSeqSample):
+class FlowCellSampleBcl2Fastq(FlowCellSample):
     sample_id: str = Field(..., alias="SampleID")
     project: str = Field(..., alias="Project")
 
 
-class SampleDragen(NovaSeqSample):
+class FlowCellSampleDragen(FlowCellSample):
     sample_id: str = Field(..., alias="Sample_ID")
     project: str = Field(..., alias="Sample_Project")
 
 
 class SampleSheet(BaseModel):
-    samples: List[NovaSeqSample]
+    samples: List[FlowCellSample]
 
 
 class SampleSheetBcl2Fastq(SampleSheet):
-    samples: List[SampleBcl2Fastq]
+    samples: List[FlowCellSampleBcl2Fastq]
 
 
 class SampleSheetDragen(SampleSheet):
-    samples: List[SampleDragen]
+    samples: List[FlowCellSampleDragen]
```

### Comparing `cg-32.2.5/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py` & `cg-32.2.7/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 from typing import Dict, List, Set
 
 from cg.apps.demultiplex.sample_sheet import index
 from cg.apps.demultiplex.sample_sheet.dummy_sample import dummy_sample
 from cg.apps.demultiplex.sample_sheet.index import Index
 from cg.apps.demultiplex.sample_sheet.validate import validate_sample_sheet
-from cg.apps.lims.samplesheet import LimsFlowcellSample
+from cg.apps.demultiplex.sample_sheet.models import FlowCellSample
 from cg.constants.demultiplexing import (
     SAMPLE_SHEET_HEADERS,
     SAMPLE_SHEET_SETTINGS_HEADER,
     SAMPLE_SHEET_SETTING_BARCODE_MISMATCH_INDEX1,
     SAMPLE_SHEET_SETTING_BARCODE_MISMATCH_INDEX2,
     SampleSheetHeaderColumnNames,
 )
@@ -24,20 +24,20 @@
 class SampleSheetCreator:
     """Create a raw sample sheet for Novaseq flow cells."""
 
     def __init__(
         self,
         bcl_converter: str,
         flow_cell: FlowCell,
-        lims_samples: List[LimsFlowcellSample],
+        lims_samples: List[FlowCellSample],
         force: bool = False,
     ):
         self.bcl_converter = bcl_converter
         self.flow_cell_id: str = flow_cell.id
-        self.lims_samples: List[LimsFlowcellSample] = lims_samples
+        self.lims_samples: List[FlowCellSample] = lims_samples
         self.run_parameters: RunParameters = flow_cell.run_parameters
         self.force = force
 
     @property
     def valid_indexes(self) -> List[Index]:
         return index.get_valid_indexes(dual_indexes_only=True)
 
@@ -51,39 +51,39 @@
         indexes_by_lane: Dict[int, Set[str]] = index.get_indexes_by_lane(samples=self.lims_samples)
         for lane, lane_indexes in indexes_by_lane.items():
             LOG.debug(f"Add dummy samples for lane {lane}")
             for index_obj in self.valid_indexes:
                 if index.index_exists(index=index_obj.sequence, indexes=lane_indexes):
                     LOG.debug(f"Index {index_obj.sequence} already in use")
                     continue
-                dummy_sample_obj: LimsFlowcellSample = dummy_sample(
-                    flowcell=self.flow_cell_id,
+                dummy_flow_cell_sample: FlowCellSample = dummy_sample(
+                    flow_cell_id=self.flow_cell_id,
                     dummy_index=index_obj.sequence,
                     lane=lane,
                     name=index_obj.name,
                     bcl_converter=self.bcl_converter,
                 )
-                LOG.debug(f"Adding dummy sample {dummy_sample_obj} to lane {lane}")
-                self.lims_samples.append(dummy_sample_obj)
+                LOG.debug(f"Adding dummy sample {dummy_flow_cell_sample} to lane {lane}")
+                self.lims_samples.append(dummy_flow_cell_sample)
 
     def remove_unwanted_samples(self) -> None:
         """Filter out samples with indexes of unwanted length and single indexes."""
         LOG.info("Removing all samples without dual indexes")
         samples_to_keep = []
-        sample: LimsFlowcellSample
+        sample: FlowCellSample
         for sample in self.lims_samples:
             if not index.is_dual_index(sample.index):
                 LOG.warning(f"Removing sample {sample} since it does not have dual index")
                 continue
             samples_to_keep.append(sample)
         self.lims_samples = samples_to_keep
 
     @staticmethod
     def convert_sample_to_header_dict(
-        sample: LimsFlowcellSample,
+        sample: FlowCellSample,
         sample_sheet_headers: List[str],
     ) -> List[str]:
         """Convert a lims sample object to a dict with keys that corresponds to the sample sheet
         headers."""
         LOG.debug(f"Use sample sheet header {sample_sheet_headers}")
         sample_dict = sample.dict(by_alias=True)
         return [str(sample_dict[header]) for header in sample_sheet_headers]
```

### Comparing `cg-32.2.5/cg/apps/demultiplex/sample_sheet/validate.py` & `cg-32.2.7/cg/apps/demultiplex/sample_sheet/validate.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 import logging
 from pathlib import Path
 from typing import Dict, List, Union
 from pydantic import parse_obj_as
 from typing_extensions import Literal
 
 from cg.apps.demultiplex.sample_sheet.models import (
-    NovaSeqSample,
+    FlowCellSample,
     SampleSheet,
-    SampleBcl2Fastq,
-    SampleDragen,
+    FlowCellSampleBcl2Fastq,
+    FlowCellSampleDragen,
 )
 from cg.constants.constants import FileFormat
 from cg.constants.demultiplexing import (
     BclConverter,
     SampleSheetHeaderColumnNames,
 )
 from cg.exc import SampleSheetError
 from cg.io.controller import ReadFile
 
 LOG = logging.getLogger(__name__)
 
 
-def validate_samples_are_unique(samples: List[NovaSeqSample]) -> None:
+def validate_samples_are_unique(samples: List[FlowCellSample]) -> None:
     """Validate that each sample only exists once."""
     sample_ids: set = set()
     for sample in samples:
         sample_id: str = sample.sample_id.split("_")[0]
         if sample_id in sample_ids:
             message: str = f"Sample {sample.sample_id} exists multiple times in sample sheet"
             LOG.warning(message)
             raise SampleSheetError(message)
         sample_ids.add(sample_id)
 
 
-def get_samples_by_lane(samples: List[NovaSeqSample]) -> Dict[int, List[NovaSeqSample]]:
+def get_samples_by_lane(samples: List[FlowCellSample]) -> Dict[int, List[FlowCellSample]]:
     """Group and return samples by lane."""
     LOG.info("Order samples by lane")
-    sample_by_lane: Dict[int, List[NovaSeqSample]] = {}
+    sample_by_lane: Dict[int, List[FlowCellSample]] = {}
     for sample in samples:
         if sample.lane not in sample_by_lane:
             sample_by_lane[sample.lane] = []
         sample_by_lane[sample.lane].append(sample)
     return sample_by_lane
 
 
-def validate_samples_unique_per_lane(samples: List[NovaSeqSample]) -> None:
+def validate_samples_unique_per_lane(samples: List[FlowCellSample]) -> None:
     """Validate that each sample only exists once per lane in a sample sheet."""
 
-    sample_by_lane: Dict[int, List[NovaSeqSample]] = get_samples_by_lane(samples)
+    sample_by_lane: Dict[int, List[FlowCellSample]] = get_samples_by_lane(samples)
     for lane, lane_samples in sample_by_lane.items():
         LOG.info(f"Validate that samples are unique in lane {lane}")
         validate_samples_are_unique(samples=lane_samples)
 
 
 def get_raw_samples(sample_sheet_content: List[List[str]]) -> List[Dict[str, str]]:
     """Return the samples in a sample sheet as a list of dictionaries."""
@@ -80,20 +80,22 @@
 
 
 def validate_sample_sheet(
     sample_sheet_content: List[List[str]],
     bcl_converter: Literal[BclConverter.BCL2FASTQ, BclConverter.DRAGEN],
 ) -> SampleSheet:
     """Return a validated sample sheet object."""
-    novaseq_sample: Dict[str, Union[SampleBcl2Fastq, SampleDragen]] = {
-        BclConverter.BCL2FASTQ: SampleBcl2Fastq,
-        BclConverter.DRAGEN: SampleDragen,
+    novaseq_sample: Dict[str, Union[FlowCellSampleBcl2Fastq, FlowCellSampleDragen]] = {
+        BclConverter.BCL2FASTQ.value: FlowCellSampleBcl2Fastq,
+        BclConverter.DRAGEN.value: FlowCellSampleDragen,
     }
     raw_samples: List[Dict[str, str]] = get_raw_samples(sample_sheet_content=sample_sheet_content)
-    sample_type: Union[SampleBcl2Fastq, SampleDragen] = novaseq_sample[bcl_converter]
+    sample_type: Union[FlowCellSampleBcl2Fastq, FlowCellSampleDragen] = novaseq_sample[
+        bcl_converter
+    ]
     samples = parse_obj_as(List[sample_type], raw_samples)
     validate_samples_unique_per_lane(samples=samples)
     return SampleSheet(samples=samples)
 
 
 def get_sample_sheet_from_file(
     infile: Path,
```

### Comparing `cg-32.2.5/cg/apps/demultiplex/sbatch.py` & `cg-32.2.7/cg/apps/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/gens.py` & `cg-32.2.7/cg/apps/gens.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/gt.py` & `cg-32.2.7/cg/apps/gt.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/hermes/hermes_api.py` & `cg-32.2.7/cg/apps/hermes/hermes_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/hermes/models.py` & `cg-32.2.7/cg/apps/hermes/models.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/housekeeper/hk.py` & `cg-32.2.7/cg/apps/housekeeper/hk.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/invoice/render.py` & `cg-32.2.7/cg/apps/invoice/render.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/invoice/templates/KI_pool_invoice.xlsx` & `cg-32.2.7/cg/apps/invoice/templates/KI_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/invoice/templates/KI_sample_invoice.xlsx` & `cg-32.2.7/cg/apps/invoice/templates/KI_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/invoice/templates/KTH_pool_invoice.xlsx` & `cg-32.2.7/cg/apps/invoice/templates/KTH_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/invoice/templates/KTH_sample_invoice.xlsx` & `cg-32.2.7/cg/apps/invoice/templates/KTH_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/lims/api.py` & `cg-32.2.7/cg/apps/lims/api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/lims/batch.py` & `cg-32.2.7/cg/apps/lims/batch.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/lims/order.py` & `cg-32.2.7/cg/apps/lims/order.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/lims/samplesheet.py` & `cg-32.2.7/cg/apps/lims/sample_sheet.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,107 +1,83 @@
-"""Functions to get sample sheet information from Lims"""
+"""Functions to get sample sheet information from Lims."""
 import logging
 import re
 from typing import Iterable, List, Optional, Union
 
-from pydantic import BaseModel, Field
-
 from genologics.entities import Artifact, Container, Sample
 from genologics.lims import Lims
 
-from cg.constants.constants import GenomeVersion
-from cg.constants.demultiplexing import SampleSheetHeaderColumnNames
+from cg.apps.demultiplex.sample_sheet.models import FlowCellSampleBcl2Fastq, FlowCellSampleDragen
+from cg.constants.demultiplexing import BclConverter
 
 LOG = logging.getLogger(__name__)
 
 
-class LimsFlowcellSample(BaseModel):
-    flowcell_id: str = Field(..., alias=SampleSheetHeaderColumnNames.FLOW_CELL_ID.value)
-    lane: int = Field(..., alias="Lane")
-    sample_id: str
-    sample_ref: str = Field(GenomeVersion.hg19.value, alias="SampleRef")
-    index: str
-    index2: str = ""
-    description: str = ""
-    sample_name: str = Field(..., alias="SampleName")
-    control: str = Field("N", alias="Control")
-    recipe: str = Field("R1", alias="Recipe")
-    operator: str = Field("script", alias="Operator")
-    project: str
-
-    class Config:
-        allow_population_by_field_name = True
-
-
-class LimsFlowcellSampleBcl2Fastq(LimsFlowcellSample):
-    sample_id: str = Field(..., alias="SampleID")
-    project: str = Field(..., alias="Project")
-
-
-class LimsFlowcellSampleDragen(LimsFlowcellSample):
-    sample_id: str = Field(..., alias="Sample_ID")
-    project: str = Field(..., alias="Sample_Project")
-
-
 def get_placement_lane(lane: str) -> int:
-    """Parse out the lane information from an artifact.placement"""
+    """Parse out the lane information from an artifact.placement."""
     return int(lane.split(":")[0])
 
 
 def get_non_pooled_artifacts(artifact: Artifact) -> List[Artifact]:
-    """Find the parent artifact of the sample. Should hold the reagent_label"""
+    """Find the parent artifact of the sample. Should hold the reagent_label."""
     artifacts = []
 
     if len(artifact.samples) == 1:
         artifacts.append(artifact)
         return artifacts
 
     for artifact_input in artifact.input_artifact_list():
         artifacts.extend(get_non_pooled_artifacts(artifact_input))
 
     return artifacts
 
 
 def get_reagent_label(artifact) -> Optional[str]:
-    """Get the first and only reagent label from an artifact"""
+    """Get the first and only reagent label from an artifact."""
     labels: List[str] = artifact.reagent_labels
     if len(labels) > 1:
-        raise ValueError("Expecting at most one reagent label. Got ({}).".format(len(labels)))
+        raise ValueError(f"Expecting at most one reagent label. Got ({len(labels)}).")
     return labels[0] if labels else None
 
 
+def extract_sequence_in_parentheses(label: str) -> Optional[str]:
+    """Return the sequence in parentheses from the reagent label or None if not found."""
+    match = re.match(r"^[^(]+ \(([^)]+)\)$", label)
+    return match.group(1) if match else None
+
+
 def get_index(lims: Lims, label: str) -> str:
-    """Parse out the sequence from a reagent label"""
+    """Parse out the sequence from a reagent label."""
 
-    reagent_types = lims.get_reagent_types(name=label)
+    reagent_types: List = lims.get_reagent_types(name=label)
 
     if len(reagent_types) > 1:
-        raise ValueError("Expecting at most one reagent type. Got ({}).".format(len(reagent_types)))
+        raise ValueError(f"Expecting at most one reagent type. Got ({len(reagent_types)}).")
 
     try:
         reagent_type = reagent_types.pop()
     except IndexError:
         return ""
-    sequence = reagent_type.sequence
+    sequence: str = reagent_type.sequence
 
-    match = re.match(r"^.+ \((.+)\)$", label)
+    match = extract_sequence_in_parentheses(label=label)
     if match:
-        assert match.group(1) == sequence
+        assert match == sequence
 
     return sequence
 
 
-def flowcell_samples(
+def flow_cell_samples(
     lims: Lims, flowcell_id: str, bcl_converter: str
-) -> Iterable[Union[LimsFlowcellSampleBcl2Fastq, LimsFlowcellSampleDragen]]:
+) -> Iterable[Union[FlowCellSampleBcl2Fastq, FlowCellSampleDragen]]:
     lims_flowcell_sample = {
-        "bcl2fastq": LimsFlowcellSampleBcl2Fastq,
-        "dragen": LimsFlowcellSampleDragen,
+        BclConverter.BCL2FASTQ.value: FlowCellSampleBcl2Fastq,
+        BclConverter.DRAGEN.value: FlowCellSampleDragen,
     }
-    LOG.info("Fetching samples from lims for flowcell %s", flowcell_id)
+    LOG.info(f"Fetching samples from lims for flowcell {flowcell_id}")
     containers: List[Container] = lims.get_containers(name=flowcell_id)
     if not containers:
         return []
     container: Container = containers[-1]  # only take the last one. See ÖA#217.
     raw_lanes: List[str] = sorted(container.placements.keys())
     for raw_lane in raw_lanes:
         lane: int = get_placement_lane(raw_lane)
```

### Comparing `cg-32.2.5/cg/apps/loqus.py` & `cg-32.2.7/cg/apps/loqus.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/madeline/api.py` & `cg-32.2.7/cg/apps/madeline/api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/mip/confighandler.py` & `cg-32.2.7/cg/apps/mip/confighandler.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/mutacc_auto.py` & `cg-32.2.7/cg/apps/mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/orderform/excel_orderform_parser.py` & `cg-32.2.7/cg/apps/orderform/excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/orderform/json_orderform_parser.py` & `cg-32.2.7/cg/apps/orderform/json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/orderform/orderform_parser.py` & `cg-32.2.7/cg/apps/orderform/orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/osticket.py` & `cg-32.2.7/cg/apps/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/scout/scout_export.py` & `cg-32.2.7/cg/apps/scout/scout_export.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/scout/scoutapi.py` & `cg-32.2.7/cg/apps/scout/scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py` & `cg-32.2.7/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/sequencing_metrics_parser/models/bcl_convert.py` & `cg-32.2.7/cg/apps/sequencing_metrics_parser/models/bcl_convert.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py` & `cg-32.2.7/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py` & `cg-32.2.7/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py` & `cg-32.2.7/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py` & `cg-32.2.7/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/slurm/sbatch.py` & `cg-32.2.7/cg/apps/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/slurm/slurm_api.py` & `cg-32.2.7/cg/apps/slurm/slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/tb/api.py` & `cg-32.2.7/cg/apps/tb/api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/tb/models.py` & `cg-32.2.7/cg/apps/tb/models.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/apps/vogue.py` & `cg-32.2.7/cg/apps/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/add.py` & `cg-32.2.7/cg/cli/add.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/backup.py` & `cg-32.2.7/cg/cli/backup.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/base.py` & `cg-32.2.7/cg/cli/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/clean.py` & `cg-32.2.7/cg/cli/clean.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/compress/base.py` & `cg-32.2.7/cg/cli/compress/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/compress/fastq.py` & `cg-32.2.7/cg/cli/compress/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/compress/helpers.py` & `cg-32.2.7/cg/cli/compress/helpers.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/delete/base.py` & `cg-32.2.7/cg/cli/delete/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/delete/case.py` & `cg-32.2.7/cg/cli/delete/case.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/delete/cases.py` & `cg-32.2.7/cg/cli/delete/cases.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/delete/observations.py` & `cg-32.2.7/cg/cli/delete/observations.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/deliver/base.py` & `cg-32.2.7/cg/cli/deliver/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/demultiplex/add.py` & `cg-32.2.7/cg/cli/demultiplex/add.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/demultiplex/base.py` & `cg-32.2.7/cg/cli/demultiplex/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/demultiplex/demux.py` & `cg-32.2.7/cg/cli/demultiplex/demux.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/demultiplex/finish.py` & `cg-32.2.7/cg/cli/demultiplex/finish.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/demultiplex/report.py` & `cg-32.2.7/cg/cli/demultiplex/report.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/demultiplex/sample_sheet.py` & `cg-32.2.7/cg/cli/demultiplex/sample_sheet.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from typing import List, Union
 
 import click
 from pydantic import ValidationError
 
 from cg.apps.demultiplex.demultiplex_api import DemultiplexingAPI
 from cg.apps.demultiplex.sample_sheet.create import create_sample_sheet
-from cg.apps.demultiplex.sample_sheet.validate import get_sample_sheet_from_file
-from cg.apps.lims.samplesheet import (
-    LimsFlowcellSample,
-    LimsFlowcellSampleBcl2Fastq,
-    LimsFlowcellSampleDragen,
-    flowcell_samples,
+from cg.apps.demultiplex.sample_sheet.models import (
+    FlowCellSample,
+    FlowCellSampleBcl2Fastq,
+    FlowCellSampleDragen,
 )
+from cg.apps.demultiplex.sample_sheet.validate import get_sample_sheet_from_file
+from cg.apps.lims.sample_sheet import flow_cell_samples
 from cg.constants.constants import FileFormat
 from cg.constants.demultiplexing import OPTION_BCL_CONVERTER
 from cg.exc import FlowCellError
 from cg.io.controller import WriteFile
 from cg.models.cg_config import CGConfig
 from cg.models.demultiplex.flow_cell import FlowCell
 
@@ -70,16 +70,16 @@
     if not flowcell_path.exists():
         LOG.warning(f"Could not find flow cell {flowcell_path}")
         raise click.Abort
     try:
         flow_cell = FlowCell(flow_cell_path=flowcell_path, bcl_converter=bcl_converter)
     except FlowCellError as error:
         raise click.Abort from error
-    lims_samples: List[Union[LimsFlowcellSampleBcl2Fastq, LimsFlowcellSampleDragen]] = list(
-        flowcell_samples(
+    lims_samples: List[Union[FlowCellSampleBcl2Fastq, FlowCellSampleDragen]] = list(
+        flow_cell_samples(
             lims=context.lims_api,
             flowcell_id=flow_cell.id,
             bcl_converter=bcl_converter,
         )
     )
     if not lims_samples:
         LOG.warning(f"Could not find any samples in lims for {flow_cell.id}")
@@ -122,16 +122,16 @@
             flow_cell = FlowCell(flow_cell_path=sub_dir, bcl_converter=bcl_converter)
         except FlowCellError:
             continue
         if flow_cell.sample_sheet_exists():
             LOG.info("Sample sheet already exists")
             continue
         LOG.info(f"Creating sample sheet for flowcell {flow_cell.id}")
-        lims_samples: List[LimsFlowcellSample] = list(
-            flowcell_samples(
+        lims_samples: List[FlowCellSample] = list(
+            flow_cell_samples(
                 lims=context.lims_api,
                 flowcell_id=flow_cell.id,
                 bcl_converter=bcl_converter,
             )
         )
         if not lims_samples:
             LOG.warning(f"Could not find any samples in lims for {flow_cell.id}")
```

### Comparing `cg-32.2.5/cg/cli/generate/report/base.py` & `cg-32.2.7/cg/cli/generate/report/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/generate/report/options.py` & `cg-32.2.7/cg/cli/generate/report/options.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/generate/report/utils.py` & `cg-32.2.7/cg/cli/generate/report/utils.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/get.py` & `cg-32.2.7/cg/cli/get.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/set/base.py` & `cg-32.2.7/cg/cli/set/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/set/case.py` & `cg-32.2.7/cg/cli/set/case.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/set/cases.py` & `cg-32.2.7/cg/cli/set/cases.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/store/fastq.py` & `cg-32.2.7/cg/cli/store/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/store/store.py` & `cg-32.2.7/cg/cli/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/transfer.py` & `cg-32.2.7/cg/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/upload/base.py` & `cg-32.2.7/cg/cli/upload/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/upload/clinical_delivery.py` & `cg-32.2.7/cg/cli/upload/clinical_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/upload/coverage.py` & `cg-32.2.7/cg/cli/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/upload/delivery_report.py` & `cg-32.2.7/cg/cli/upload/delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/upload/fohm.py` & `cg-32.2.7/cg/cli/upload/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/upload/genotype.py` & `cg-32.2.7/cg/cli/upload/genotype.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/upload/gens.py` & `cg-32.2.7/cg/cli/upload/gens.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/upload/gisaid.py` & `cg-32.2.7/cg/cli/upload/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/upload/mutacc.py` & `cg-32.2.7/cg/cli/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/upload/nipt/base.py` & `cg-32.2.7/cg/cli/upload/nipt/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/upload/nipt/ftp.py` & `cg-32.2.7/cg/cli/upload/nipt/ftp.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/upload/nipt/statina.py` & `cg-32.2.7/cg/cli/upload/nipt/statina.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/upload/observations/observations.py` & `cg-32.2.7/cg/cli/upload/observations/observations.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/upload/observations/utils.py` & `cg-32.2.7/cg/cli/upload/observations/utils.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/upload/scout.py` & `cg-32.2.7/cg/cli/upload/scout.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/upload/utils.py` & `cg-32.2.7/cg/cli/upload/utils.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/upload/validate.py` & `cg-32.2.7/cg/cli/upload/validate.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/upload/vogue.py` & `cg-32.2.7/cg/cli/upload/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/workflow/balsamic/base.py` & `cg-32.2.7/cg/cli/workflow/balsamic/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/workflow/balsamic/options.py` & `cg-32.2.7/cg/cli/workflow/balsamic/options.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/workflow/balsamic/pon.py` & `cg-32.2.7/cg/cli/workflow/balsamic/pon.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/workflow/balsamic/qc.py` & `cg-32.2.7/cg/cli/workflow/balsamic/qc.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/workflow/balsamic/umi.py` & `cg-32.2.7/cg/cli/workflow/balsamic/umi.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/workflow/base.py` & `cg-32.2.7/cg/cli/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/workflow/commands.py` & `cg-32.2.7/cg/cli/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/workflow/fastq/base.py` & `cg-32.2.7/cg/cli/workflow/fastq/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/workflow/fluffy/base.py` & `cg-32.2.7/cg/cli/workflow/fluffy/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/workflow/microsalt/base.py` & `cg-32.2.7/cg/cli/workflow/microsalt/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/workflow/mip/base.py` & `cg-32.2.7/cg/cli/workflow/mip/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/workflow/mip/options.py` & `cg-32.2.7/cg/cli/workflow/mip/options.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/workflow/mip_dna/base.py` & `cg-32.2.7/cg/cli/workflow/mip_dna/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/workflow/mip_rna/base.py` & `cg-32.2.7/cg/cli/workflow/mip_rna/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/workflow/mutant/base.py` & `cg-32.2.7/cg/cli/workflow/mutant/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/workflow/nextflow/options.py` & `cg-32.2.7/cg/cli/workflow/nextflow/options.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/workflow/rnafusion/base.py` & `cg-32.2.7/cg/cli/workflow/rnafusion/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/workflow/rnafusion/options.py` & `cg-32.2.7/cg/cli/workflow/rnafusion/options.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/cli/workflow/taxprofiler/base.py` & `cg-32.2.7/cg/cli/workflow/taxprofiler/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/constants/__init__.py` & `cg-32.2.7/cg/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/constants/bcl_convert_metrics.py` & `cg-32.2.7/cg/constants/bcl_convert_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/constants/compression.py` & `cg-32.2.7/cg/constants/compression.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/constants/constants.py` & `cg-32.2.7/cg/constants/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,15 @@
 
 
 class FileFormat(StrEnum):
     FASTQ: str = "fastq"
     JSON: str = "json"
     YAML: str = "yaml"
     CSV: str = "csv"
+    XML: str = "xml"
 
 
 class GenomeVersion(StrEnum):
     hg19: str = "hg19"
     hg38: str = "hg38"
     canfam3: str = "canfam3"
 
@@ -136,14 +137,15 @@
     JSON: str = ".json"
     KEY: str = ".key"
     NO_EXTENSION: str = ""
     SPRING: str = ".spring"
     TAR: str = ".tar"
     TMP: str = ".tmp"
     VCF: str = ".vcf"
+    XML: str = ".xml"
 
 
 class APIMethods(StrEnum):
     POST: str = "POST"
     PUT: str = "PUT"
     GET: str = "GET"
     DELETE: str = "DELETE"
```

### Comparing `cg-32.2.5/cg/constants/delivery.py` & `cg-32.2.7/cg/constants/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/constants/demultiplexing.py` & `cg-32.2.7/cg/constants/demultiplexing.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/constants/encryption.py` & `cg-32.2.7/cg/constants/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/constants/gene_panel.py` & `cg-32.2.7/cg/constants/gene_panel.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/constants/housekeeper_tags.py` & `cg-32.2.7/cg/constants/housekeeper_tags.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/constants/lims.py` & `cg-32.2.7/cg/constants/lims.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/constants/nextflow.py` & `cg-32.2.7/cg/constants/nextflow.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/constants/observations.py` & `cg-32.2.7/cg/constants/observations.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/constants/orderforms.py` & `cg-32.2.7/cg/constants/orderforms.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/constants/priority.py` & `cg-32.2.7/cg/constants/priority.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/constants/report.py` & `cg-32.2.7/cg/constants/report.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/constants/rnafusion.py` & `cg-32.2.7/cg/constants/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/constants/scout_upload.py` & `cg-32.2.7/cg/constants/scout_upload.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/constants/sequencing.py` & `cg-32.2.7/cg/constants/sequencing.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/constants/subject.py` & `cg-32.2.7/cg/constants/subject.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/exc.py` & `cg-32.2.7/cg/exc.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/io/api.py` & `cg-32.2.7/cg/io/api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/io/controller.py` & `cg-32.2.7/cg/io/controller.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 from typing import Any
 from requests import Response
 
 from cg.constants.constants import FileFormat, APIMethods
 from cg.io.json import read_json, write_json, write_json_stream, read_json_stream
 from cg.io.yaml import read_yaml, write_yaml, read_yaml_stream, write_yaml_stream
 from cg.io.csv import read_csv, write_csv, read_csv_stream, write_csv_stream
+from cg.io.xml import read_xml, write_xml
 from cg.io.api import put, post, patch, delete, get
 
 
 class ReadFile:
     """Reading file using different methods."""
 
     read_file = {
         FileFormat.CSV: read_csv,
         FileFormat.JSON: read_json,
         FileFormat.YAML: read_yaml,
+        FileFormat.XML: read_xml,
     }
 
     @classmethod
     def get_content_from_file(cls, file_format: str, file_path: Path, **kwargs) -> Any:
         """Read file using file format dispatch table."""
         return cls.read_file[file_format](file_path=file_path, **kwargs)
 
@@ -42,14 +44,15 @@
 class WriteFile:
     """Write file using different methods."""
 
     write_file = {
         FileFormat.CSV: write_csv,
         FileFormat.JSON: write_json,
         FileFormat.YAML: write_yaml,
+        FileFormat.XML: write_xml,
     }
 
     @classmethod
     def write_file_from_content(cls, content: Any, file_format: str, file_path: Path) -> None:
         """Write file using file format dispatch table."""
         cls.write_file[file_format](content=content, file_path=file_path)
```

### Comparing `cg-32.2.5/cg/io/csv.py` & `cg-32.2.7/cg/io/csv.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/io/json.py` & `cg-32.2.7/cg/io/json.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/io/validate_path.py` & `cg-32.2.7/cg/io/validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/io/yaml.py` & `cg-32.2.7/cg/io/yaml.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/archive/ddn_dataflow.py` & `cg-32.2.7/cg/meta/archive/ddn_dataflow.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/backup/backup.py` & `cg-32.2.7/cg/meta/backup/backup.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/backup/pdc.py` & `cg-32.2.7/cg/meta/backup/pdc.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/clean/api.py` & `cg-32.2.7/cg/meta/clean/api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/clean/demultiplexed_flow_cells.py` & `cg-32.2.7/cg/meta/clean/demultiplexed_flow_cells.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/clean/flow_cell_run_directories.py` & `cg-32.2.7/cg/meta/clean/flow_cell_run_directories.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/compress/compress.py` & `cg-32.2.7/cg/meta/compress/compress.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/compress/files.py` & `cg-32.2.7/cg/meta/compress/files.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/deliver.py` & `cg-32.2.7/cg/meta/deliver.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/deliver_ticket.py` & `cg-32.2.7/cg/meta/deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/demultiplex/delete_demultiplex_api.py` & `cg-32.2.7/cg/meta/demultiplex/delete_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/demultiplex/demux_post_processing.py` & `cg-32.2.7/cg/meta/demultiplex/demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/demultiplex/files.py` & `cg-32.2.7/cg/meta/demultiplex/files.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/encryption/encryption.py` & `cg-32.2.7/cg/meta/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/invoice.py` & `cg-32.2.7/cg/meta/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/meta.py` & `cg-32.2.7/cg/meta/meta.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/observations/balsamic_observations_api.py` & `cg-32.2.7/cg/meta/observations/balsamic_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/observations/mip_dna_observations_api.py` & `cg-32.2.7/cg/meta/observations/mip_dna_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/observations/observations_api.py` & `cg-32.2.7/cg/meta/observations/observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/orders/api.py` & `cg-32.2.7/cg/meta/orders/api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/orders/case_submitter.py` & `cg-32.2.7/cg/meta/orders/case_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/orders/fastq_submitter.py` & `cg-32.2.7/cg/meta/orders/fastq_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/orders/lims.py` & `cg-32.2.7/cg/meta/orders/lims.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/orders/metagenome_submitter.py` & `cg-32.2.7/cg/meta/orders/metagenome_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/orders/microbial_submitter.py` & `cg-32.2.7/cg/meta/orders/microbial_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/orders/pool_submitter.py` & `cg-32.2.7/cg/meta/orders/pool_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/orders/sars_cov_2_submitter.py` & `cg-32.2.7/cg/meta/orders/sars_cov_2_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/orders/submitter.py` & `cg-32.2.7/cg/meta/orders/submitter.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/orders/ticket_handler.py` & `cg-32.2.7/cg/meta/orders/ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/report/balsamic.py` & `cg-32.2.7/cg/meta/report/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/report/balsamic_umi.py` & `cg-32.2.7/cg/meta/report/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/report/field_validators.py` & `cg-32.2.7/cg/meta/report/field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/report/mip_dna.py` & `cg-32.2.7/cg/meta/report/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/report/report_api.py` & `cg-32.2.7/cg/meta/report/report_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/report/templates/balsamic_report.html` & `cg-32.2.7/cg/meta/report/templates/balsamic_report.html`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/report/templates/bootstrap.html` & `cg-32.2.7/cg/meta/report/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/report/templates/mip-dna_report.html` & `cg-32.2.7/cg/meta/report/templates/mip-dna_report.html`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/rsync/rsync_api.py` & `cg-32.2.7/cg/meta/rsync/rsync_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/tar/tar.py` & `cg-32.2.7/cg/meta/tar/tar.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/transfer/external_data.py` & `cg-32.2.7/cg/meta/transfer/external_data.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/transfer/flowcell.py` & `cg-32.2.7/cg/meta/transfer/flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/transfer/lims.py` & `cg-32.2.7/cg/meta/transfer/lims.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/upload/balsamic/balsamic.py` & `cg-32.2.7/cg/meta/upload/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/upload/coverage.py` & `cg-32.2.7/cg/meta/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/upload/fohm/fohm.py` & `cg-32.2.7/cg/meta/upload/fohm/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/upload/gisaid/constants.py` & `cg-32.2.7/cg/meta/upload/gisaid/constants.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/upload/gisaid/gisaid.py` & `cg-32.2.7/cg/meta/upload/gisaid/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/upload/gisaid/models.py` & `cg-32.2.7/cg/meta/upload/gisaid/models.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/upload/gt.py` & `cg-32.2.7/cg/meta/upload/gt.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/upload/mip/mip_dna.py` & `cg-32.2.7/cg/meta/upload/mip/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/upload/mip/mip_rna.py` & `cg-32.2.7/cg/meta/upload/mip/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/upload/mutacc.py` & `cg-32.2.7/cg/meta/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/upload/nipt/nipt.py` & `cg-32.2.7/cg/meta/upload/nipt/nipt.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/upload/rnafusion/rnafusion.py` & `cg-32.2.7/cg/meta/upload/rnafusion/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/upload/scout/balsamic_config_builder.py` & `cg-32.2.7/cg/meta/upload/scout/balsamic_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/upload/scout/balsamic_umi_config_builder.py` & `cg-32.2.7/cg/meta/upload/scout/balsamic_umi_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/upload/scout/hk_tags.py` & `cg-32.2.7/cg/meta/upload/scout/hk_tags.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/upload/scout/mip_config_builder.py` & `cg-32.2.7/cg/meta/upload/scout/mip_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/upload/scout/rnafusion_config_builder.py` & `cg-32.2.7/cg/meta/upload/scout/rnafusion_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/upload/scout/scout_config_builder.py` & `cg-32.2.7/cg/meta/upload/scout/scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/upload/scout/uploadscoutapi.py` & `cg-32.2.7/cg/meta/upload/scout/uploadscoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/upload/upload_api.py` & `cg-32.2.7/cg/meta/upload/upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/upload/vogue.py` & `cg-32.2.7/cg/meta/upload/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/workflow/analysis.py` & `cg-32.2.7/cg/meta/workflow/analysis.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/workflow/balsamic.py` & `cg-32.2.7/cg/meta/workflow/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/workflow/balsamic_pon.py` & `cg-32.2.7/cg/meta/workflow/balsamic_pon.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/workflow/balsamic_qc.py` & `cg-32.2.7/cg/meta/workflow/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/workflow/balsamic_umi.py` & `cg-32.2.7/cg/meta/workflow/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/workflow/fastq.py` & `cg-32.2.7/cg/meta/workflow/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/workflow/fluffy.py` & `cg-32.2.7/cg/meta/workflow/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/workflow/microsalt.py` & `cg-32.2.7/cg/meta/workflow/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/workflow/mip.py` & `cg-32.2.7/cg/meta/workflow/mip.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/workflow/mip_dna.py` & `cg-32.2.7/cg/meta/workflow/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/workflow/mip_rna.py` & `cg-32.2.7/cg/meta/workflow/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/workflow/mutant.py` & `cg-32.2.7/cg/meta/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/workflow/nextflow_common.py` & `cg-32.2.7/cg/meta/workflow/nextflow_common.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/workflow/prepare_fastq.py` & `cg-32.2.7/cg/meta/workflow/prepare_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/workflow/rnafusion.py` & `cg-32.2.7/cg/meta/workflow/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/workflow/taxprofiler.py` & `cg-32.2.7/cg/meta/workflow/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/meta/workflow/tower_common.py` & `cg-32.2.7/cg/meta/workflow/tower_common.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/balsamic/config.py` & `cg-32.2.7/cg/models/balsamic/config.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/balsamic/metrics.py` & `cg-32.2.7/cg/models/balsamic/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/cg_config.py` & `cg-32.2.7/cg/models/cg_config.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/cgstats/stats_sample.py` & `cg-32.2.7/cg/models/cgstats/stats_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/compression_data.py` & `cg-32.2.7/cg/models/compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/deliverables/metric_deliverables.py` & `cg-32.2.7/cg/models/deliverables/metric_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/demultiplex/demux_results.py` & `cg-32.2.7/cg/models/demultiplex/demux_results.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/demultiplex/flow_cell.py` & `cg-32.2.7/cg/models/demultiplex/flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/demultiplex/run_parameters.py` & `cg-32.2.7/cg/models/demultiplex/run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/demultiplex/sbatch.py` & `cg-32.2.7/cg/models/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/file_data.py` & `cg-32.2.7/cg/models/file_data.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/invoice/invoice.py` & `cg-32.2.7/cg/models/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/lims/sample.py` & `cg-32.2.7/cg/models/lims/sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/mip/mip_config.py` & `cg-32.2.7/cg/models/mip/mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/mip/mip_metrics_deliverables.py` & `cg-32.2.7/cg/models/mip/mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/mip/mip_sample_info.py` & `cg-32.2.7/cg/models/mip/mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/nextflow/deliverables.py` & `cg-32.2.7/cg/models/nextflow/deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/nextflow/sample.py` & `cg-32.2.7/cg/models/nextflow/sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/observations/input_files.py` & `cg-32.2.7/cg/models/observations/input_files.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/orders/constants.py` & `cg-32.2.7/cg/models/orders/constants.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/orders/excel_sample.py` & `cg-32.2.7/cg/models/orders/excel_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/orders/json_sample.py` & `cg-32.2.7/cg/models/orders/json_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/orders/order.py` & `cg-32.2.7/cg/models/orders/order.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/orders/orderform_schema.py` & `cg-32.2.7/cg/models/orders/orderform_schema.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/orders/sample_base.py` & `cg-32.2.7/cg/models/orders/sample_base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/orders/samples.py` & `cg-32.2.7/cg/models/orders/samples.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/report/metadata.py` & `cg-32.2.7/cg/models/report/metadata.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/report/report.py` & `cg-32.2.7/cg/models/report/report.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/report/sample.py` & `cg-32.2.7/cg/models/report/sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/report/validators.py` & `cg-32.2.7/cg/models/report/validators.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/rnafusion/rnafusion_sample.py` & `cg-32.2.7/cg/models/rnafusion/rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/scout/scout_load_config.py` & `cg-32.2.7/cg/models/scout/scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/slurm/sbatch.py` & `cg-32.2.7/cg/models/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/models/workflow/mutant.py` & `cg-32.2.7/cg/models/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/resources/20181012_Indices.csv` & `cg-32.2.7/cg/resources/20181012_Indices.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/resources/rnafusion_bundle_filenames.csv` & `cg-32.2.7/cg/resources/rnafusion_bundle_filenames.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/server/admin.py` & `cg-32.2.7/cg/server/admin.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/server/api.py` & `cg-32.2.7/cg/server/api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/server/app.py` & `cg-32.2.7/cg/server/app.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/server/config.py` & `cg-32.2.7/cg/server/config.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/server/ext.py` & `cg-32.2.7/cg/server/ext.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/server/invoices/templates/invoices/index.html` & `cg-32.2.7/cg/server/invoices/templates/invoices/index.html`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/server/invoices/templates/invoices/invoice.html` & `cg-32.2.7/cg/server/invoices/templates/invoices/invoice.html`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/server/invoices/templates/invoices/layout.html` & `cg-32.2.7/cg/server/invoices/templates/invoices/layout.html`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/server/invoices/templates/invoices/new.html` & `cg-32.2.7/cg/server/invoices/templates/invoices/new.html`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/server/invoices/views.py` & `cg-32.2.7/cg/server/invoices/views.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/api/add.py` & `cg-32.2.7/cg/store/api/add.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/api/base.py` & `cg-32.2.7/cg/store/api/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/api/core.py` & `cg-32.2.7/cg/store/api/core.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/api/delete.py` & `cg-32.2.7/cg/store/api/delete.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/api/find_basic_data.py` & `cg-32.2.7/cg/store/api/find_basic_data.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/api/find_business_data.py` & `cg-32.2.7/cg/store/api/find_business_data.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/api/status.py` & `cg-32.2.7/cg/store/api/status.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/filters/status_analysis_filters.py` & `cg-32.2.7/cg/store/filters/status_analysis_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/filters/status_application_filters.py` & `cg-32.2.7/cg/store/filters/status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/filters/status_application_version_filters.py` & `cg-32.2.7/cg/store/filters/status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/filters/status_bed_filters.py` & `cg-32.2.7/cg/store/filters/status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/filters/status_bed_version_filters.py` & `cg-32.2.7/cg/store/filters/status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/filters/status_case_filters.py` & `cg-32.2.7/cg/store/filters/status_case_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/filters/status_case_sample_filters.py` & `cg-32.2.7/cg/store/filters/status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/filters/status_collaboration_filters.py` & `cg-32.2.7/cg/store/filters/status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/filters/status_customer_filters.py` & `cg-32.2.7/cg/store/filters/status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/filters/status_flow_cell_filters.py` & `cg-32.2.7/cg/store/filters/status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/filters/status_invoice_filters.py` & `cg-32.2.7/cg/store/filters/status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/filters/status_organism_filters.py` & `cg-32.2.7/cg/store/filters/status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/filters/status_panel_filters.py` & `cg-32.2.7/cg/store/filters/status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/filters/status_pool_filters.py` & `cg-32.2.7/cg/store/filters/status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/filters/status_sample_filters.py` & `cg-32.2.7/cg/store/filters/status_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/filters/status_user_filters.py` & `cg-32.2.7/cg/store/filters/status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/store/models.py` & `cg-32.2.7/cg/store/models.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/utils/checksum/checksum.py` & `cg-32.2.7/cg/utils/checksum/checksum.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/utils/click/EnumChoice.py` & `cg-32.2.7/cg/utils/click/EnumChoice.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/utils/commands.py` & `cg-32.2.7/cg/utils/commands.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/utils/date.py` & `cg-32.2.7/cg/utils/date.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/utils/dict.py` & `cg-32.2.7/cg/utils/dict.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/utils/dispatcher.py` & `cg-32.2.7/cg/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/utils/email.py` & `cg-32.2.7/cg/utils/email.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/utils/flask/enum.py` & `cg-32.2.7/cg/utils/flask/enum.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg/utils/utils.py` & `cg-32.2.7/cg/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/cg.egg-info/PKG-INFO` & `cg-32.2.7/cg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 32.2.5
+Version: 32.2.7
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-32.2.5/cg.egg-info/SOURCES.txt` & `cg-32.2.7/cg.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 cg/apps/invoice/templates/KI_sample_invoice.xlsx
 cg/apps/invoice/templates/KTH_pool_invoice.xlsx
 cg/apps/invoice/templates/KTH_sample_invoice.xlsx
 cg/apps/lims/__init__.py
 cg/apps/lims/api.py
 cg/apps/lims/batch.py
 cg/apps/lims/order.py
-cg/apps/lims/samplesheet.py
+cg/apps/lims/sample_sheet.py
 cg/apps/madeline/__init__.py
 cg/apps/madeline/api.py
 cg/apps/mip/__init__.py
 cg/apps/mip/confighandler.py
 cg/apps/orderform/__init__.py
 cg/apps/orderform/excel_orderform_parser.py
 cg/apps/orderform/json_orderform_parser.py
@@ -235,14 +235,15 @@
 cg/constants/tb.py
 cg/io/__init__.py
 cg/io/api.py
 cg/io/controller.py
 cg/io/csv.py
 cg/io/json.py
 cg/io/validate_path.py
+cg/io/xml.py
 cg/io/yaml.py
 cg/meta/__init__.py
 cg/meta/deliver.py
 cg/meta/deliver_ticket.py
 cg/meta/invoice.py
 cg/meta/meta.py
 cg/meta/archive/__init__.py
@@ -507,14 +508,15 @@
 tests/apps/hk/test_add_file.py
 tests/apps/hk/test_bundles.py
 tests/apps/hk/test_core.py
 tests/apps/hk/test_file.py
 tests/apps/hk/test_version.py
 tests/apps/lims/conftest.py
 tests/apps/lims/test_api.py
+tests/apps/lims/test_sample_sheet.py
 tests/apps/loqus/conftest.py
 tests/apps/loqus/test_loqusdb_api.py
 tests/apps/madeline/conftest.py
 tests/apps/madeline/test_madeline.py
 tests/apps/mip/conftest.py
 tests/apps/mip/test_config_mip.py
 tests/apps/mutacc_auto/conftest.py
@@ -792,14 +794,15 @@
 tests/fixtures/data/SampleSheet.csv
 tests/fixtures/data/cgfixture.db
 tests/fixtures/data/fastq.fastq.gz
 tests/fixtures/data/hkstore.db
 tests/fixtures/data/yellowhog/pedigree.yaml
 tests/fixtures/io/example_csv.csv
 tests/fixtures/io/example_json.json
+tests/fixtures/io/example_xml.xml
 tests/fixtures/orderforms/1508.27.balsamic.xlsx
 tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx
 tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx
 tests/fixtures/orderforms/1508.27.fastq.xlsx
 tests/fixtures/orderforms/1508.27.mip.xlsx
 tests/fixtures/orderforms/1508.27.mip_rna.xlsx
 tests/fixtures/orderforms/1603.11.microbial.xlsx
@@ -812,14 +815,15 @@
 tests/fixtures/report/case_data.json
 tests/fixtures/report/lims_exported_samples.json
 tests/fixtures/report/lims_family.json
 tests/io/conftest.py
 tests/io/test_io_controller.py
 tests/io/test_io_csv.py
 tests/io/test_io_json.py
+tests/io/test_io_xml.py
 tests/io/test_io_yaml.py
 tests/io/test_validate_path.py
 tests/meta/__init__.py
 tests/meta/conftest.py
 tests/meta/test_invoice.py
 tests/meta/archive/conftest.py
 tests/meta/archive/test_archiving.py
```

### Comparing `cg-32.2.5/requirements.txt` & `cg-32.2.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/setup.py` & `cg-32.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     with io.open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
         LONG_DESCRIPTION = "\n" + f.read()
 except FileNotFoundError:
     LONG_DESCRIPTION = DESCRIPTION
 
 setup(
     name=NAME,
-    version="32.2.5",
+    version="32.2.7",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     url=URL,
     include_package_data=True,
```

### Comparing `cg-32.2.5/tests/apps/cgstats/conftest.py` & `cg-32.2.7/tests/apps/cgstats/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/cgstats/crud/test_create_novaseq.py` & `cg-32.2.7/tests/apps/cgstats/crud/test_create_novaseq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/cgstats/crud/test_delete.py` & `cg-32.2.7/tests/apps/cgstats/crud/test_delete.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/cgstats/parsers/test_conversion_stats.py` & `cg-32.2.7/tests/apps/cgstats/parsers/test_conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/cgstats/parsers/test_demux_stats.py` & `cg-32.2.7/tests/apps/cgstats/parsers/test_demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/cgstats/parsers/test_run_info.py` & `cg-32.2.7/tests/apps/cgstats/parsers/test_run_info.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/cgstats/test_cgstats_create.py` & `cg-32.2.7/tests/apps/cgstats/test_cgstats_create.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/cgstats/test_stats.py` & `cg-32.2.7/tests/apps/cgstats/test_stats.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/conftest.py` & `cg-32.2.7/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/coverage/test_coverage.py` & `cg-32.2.7/tests/apps/coverage/test_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/crunchy/conftest.py` & `cg-32.2.7/tests/apps/crunchy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/crunchy/test_compress_fastq.py` & `cg-32.2.7/tests/apps/crunchy/test_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/crunchy/test_config.py` & `cg-32.2.7/tests/apps/crunchy/test_config.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/crunchy/test_crunchy.py` & `cg-32.2.7/tests/apps/crunchy/test_crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/crunchy/test_spring_decompression.py` & `cg-32.2.7/tests/apps/crunchy/test_spring_decompression.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/demultiplex/conftest.py` & `cg-32.2.7/tests/apps/demultiplex/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from pathlib import Path
 from typing import List
 
 import pytest
 
 from cg.apps.demultiplex.sample_sheet.index import Index
 from cg.apps.demultiplex.sample_sheet.novaseq_sample_sheet import SampleSheetCreator
-from cg.apps.lims.samplesheet import (
-    LimsFlowcellSampleBcl2Fastq,
-    LimsFlowcellSampleDragen,
-)
-from cg.apps.demultiplex.sample_sheet.validate import NovaSeqSample
+from cg.apps.demultiplex.sample_sheet.models import FlowCellSampleBcl2Fastq, FlowCellSampleDragen
 from cg.constants.demultiplexing import SampleSheetHeaderColumnNames
 from cg.models.demultiplex.flow_cell import FlowCell
 from cg.models.demultiplex.run_parameters import RunParameters
 
 
 @pytest.fixture(name="output_dirs_bcl2fastq")
 def fixture_output_dirs_bcl2fastq(demultiplexed_runs: Path) -> Path:
@@ -38,48 +34,48 @@
 def fixture_index_obj() -> Index:
     return Index(name="C07 - UDI0051", sequence="AACAGGTT-ATACCAAG")
 
 
 @pytest.fixture(name="lims_novaseq_bcl2fastq_samples")
 def fixture_lims_novaseq_bcl2fastq_samples(
     lims_novaseq_samples_raw: List[dict],
-) -> List[LimsFlowcellSampleBcl2Fastq]:
+) -> List[FlowCellSampleBcl2Fastq]:
     """Return a list of parsed flow cell samples"""
-    return [LimsFlowcellSampleBcl2Fastq(**sample) for sample in lims_novaseq_samples_raw]
+    return [FlowCellSampleBcl2Fastq(**sample) for sample in lims_novaseq_samples_raw]
 
 
 @pytest.fixture(name="lims_novaseq_dragen_samples")
 def fixture_lims_novaseq_dragen_samples(
     lims_novaseq_samples_raw: List[dict],
-) -> List[LimsFlowcellSampleDragen]:
+) -> List[FlowCellSampleDragen]:
     """Return a list of parsed flowcell samples"""
-    return [LimsFlowcellSampleDragen(**sample) for sample in lims_novaseq_samples_raw]
+    return [FlowCellSampleDragen(**sample) for sample in lims_novaseq_samples_raw]
 
 
 @pytest.fixture(name="novaseq_run_parameters_object")
 def fixture_novaseq_run_parameters_object(novaseq_run_parameters: Path) -> RunParameters:
     return RunParameters(novaseq_run_parameters)
 
 
 @pytest.fixture(name="novaseq_bcl2fastq_sample_sheet_object")
 def fixture_novaseq_bcl2fastq_sample_sheet_object(
     bcl2fastq_flow_cell: FlowCell,
-    lims_novaseq_bcl2fastq_samples: List[LimsFlowcellSampleBcl2Fastq],
+    lims_novaseq_bcl2fastq_samples: List[FlowCellSampleBcl2Fastq],
 ) -> SampleSheetCreator:
     return SampleSheetCreator(
         flow_cell=bcl2fastq_flow_cell,
         lims_samples=lims_novaseq_bcl2fastq_samples,
         bcl_converter="bcl2fastq",
     )
 
 
 @pytest.fixture(name="novaseq_dragen_sample_sheet_object")
 def fixture_novaseq_dragen_sample_sheet_object(
     dragen_flow_cell: FlowCell,
-    lims_novaseq_dragen_samples: List[LimsFlowcellSampleDragen],
+    lims_novaseq_dragen_samples: List[FlowCellSampleDragen],
     novaseq_run_parameters_object: RunParameters,
 ) -> SampleSheetCreator:
     return SampleSheetCreator(
         flow_cell=dragen_flow_cell,
         lims_samples=lims_novaseq_dragen_samples,
         bcl_converter="dragen",
     )
@@ -280,17 +276,17 @@
 @pytest.fixture(name="valid_sample_sheet_dragen_path")
 def fixture_valid_sample_sheet_dragen_path() -> Path:
     """Return the path to a NovaSeq S2 sample sheet, used in dragen demultiplexing."""
     return Path("tests", "fixtures", "apps", "demultiplexing", "SampleSheetS2_Dragen.csv")
 
 
 @pytest.fixture(name="novaseq_sample_1")
-def fixture_novaseq_sample_1() -> NovaSeqSample:
+def fixture_novaseq_sample_1() -> FlowCellSampleBcl2Fastq:
     """Return a NovaSeq sample."""
-    return NovaSeqSample(
+    return FlowCellSampleBcl2Fastq(
         FCID="HWHMWDMXX",
         Lane=1,
         SampleID="ACC7628A68",
         SampleRef="hg19",
         index="ATTCCACACT",
         index2="TGGTCTTGTT",
         SampleName="814206",
@@ -298,17 +294,17 @@
         Recipe="R1",
         Operator="script",
         Project="814206",
     )
 
 
 @pytest.fixture(name="novaseq_sample_2")
-def fixture_novaseq_sample_2() -> NovaSeqSample:
+def fixture_novaseq_sample_2() -> FlowCellSampleBcl2Fastq:
     """Return a NovaSeq sample."""
-    return NovaSeqSample(
+    return FlowCellSampleBcl2Fastq(
         FCID="HWHMWDMXX",
         Lane=2,
         SampleID="ACC7628A1",
         SampleRef="hg19",
         index="ATTCCACACT",
         index2="TGGTCTTGTT",
         SampleName="814206",
```

### Comparing `cg-32.2.5/tests/apps/demultiplex/test_convert_to_sample_sheet.py` & `cg-32.2.7/tests/apps/demultiplex/test_convert_to_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/demultiplex/test_demultiplex_api.py` & `cg-32.2.7/tests/apps/demultiplex/test_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/demultiplex/test_sample_sheet.py` & `cg-32.2.7/tests/apps/demultiplex/test_sample_sheet.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List
 
 from cg.apps.demultiplex.sample_sheet import dummy_sample, index
 from cg.apps.demultiplex.sample_sheet.index import Index
-from cg.apps.lims.samplesheet import LimsFlowcellSample
+from cg.apps.demultiplex.sample_sheet.models import FlowCellSampleBcl2Fastq
 
 
 def test_get_valid_indexes():
     # GIVEN a sample sheet api
 
     # WHEN fetching the indexes
     indexes: List[Index] = index.get_valid_indexes()
@@ -26,18 +26,18 @@
     # THEN assert the correct name was created
     assert dummy_sample_name == "D10---D710-D504--TCCGCGAA-GGCTCTGA-"
 
 
 def test_get_dummy_sample(bcl2fastq_flow_cell_id: str, index_obj: Index):
     # GIVEN some dummy sample data
 
-    # WHEN creating the dummy sample for a bcl2fastq samplesheet
-    dummy_sample_obj: LimsFlowcellSample = dummy_sample.dummy_sample(
-        flowcell=bcl2fastq_flow_cell_id,
+    # WHEN creating the dummy sample for a bcl2fastq sample sheet
+    dummy_flow_cell_sample: FlowCellSampleBcl2Fastq = dummy_sample.dummy_sample(
+        flow_cell_id=bcl2fastq_flow_cell_id,
         dummy_index=index_obj.sequence,
         lane=1,
         name=index_obj.name,
         bcl_converter="bcl2fastq",
     )
 
     # THEN assert the sample id was correct
-    assert dummy_sample_obj.sample_id == dummy_sample.dummy_sample_name(index_obj.name)
+    assert dummy_flow_cell_sample.sample_id == dummy_sample.dummy_sample_name(index_obj.name)
```

### Comparing `cg-32.2.5/tests/apps/demultiplex/test_validate_sample_sheet.py` & `cg-32.2.7/tests/apps/demultiplex/test_validate_sample_sheet.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import logging
 from typing import List, Dict
 
 import pytest
 
-from cg.apps.demultiplex.sample_sheet.models import SampleSheet, NovaSeqSample
+from cg.apps.demultiplex.sample_sheet.models import SampleSheet, FlowCellSampleBcl2Fastq
 from cg.apps.demultiplex.sample_sheet.validate import (
     get_raw_samples,
     validate_sample_sheet,
     get_samples_by_lane,
     validate_samples_are_unique,
 )
 from cg.constants.demultiplexing import BclConverter
 from cg.exc import SampleSheetError
 
 
 def test_validate_samples_are_unique(
-    novaseq_sample_1: NovaSeqSample,
-    novaseq_sample_2: NovaSeqSample,
+    novaseq_sample_1: FlowCellSampleBcl2Fastq,
+    novaseq_sample_2: FlowCellSampleBcl2Fastq,
 ):
     """Test that validating two different samples finishes successfully."""
     # GIVEN two different NovaSeq samples
     assert novaseq_sample_1 != novaseq_sample_2
 
     # WHEN validating the samples
     validate_samples_are_unique(samples=[novaseq_sample_1, novaseq_sample_2])
 
     # THEN no error is raised
 
 
-def test_validate_samples_are_unique_not_unique(novaseq_sample_1: NovaSeqSample, caplog):
+def test_validate_samples_are_unique_not_unique(novaseq_sample_1: FlowCellSampleBcl2Fastq, caplog):
     """Test that validating two identical samples fails."""
     # GIVEN two identical NovaSeq samples
     caplog.set_level(logging.INFO)
 
     # WHEN validating the samples
     with pytest.raises(SampleSheetError):
         validate_samples_are_unique(samples=[novaseq_sample_1, novaseq_sample_1])
@@ -40,22 +40,22 @@
     # THEN a sample sheet error is raised due to the samples being identical
     assert (
         f"Sample {novaseq_sample_1.sample_id} exists multiple times in sample sheet" in caplog.text
     )
 
 
 def test_get_samples_by_lane(
-    novaseq_sample_1: NovaSeqSample,
-    novaseq_sample_2: NovaSeqSample,
+    novaseq_sample_1: FlowCellSampleBcl2Fastq,
+    novaseq_sample_2: FlowCellSampleBcl2Fastq,
 ):
     """Test that grouping two samples with different lanes returns two groups."""
     # GIVEN two samples on two different lanes
 
     # WHEN getting the samples per lane
-    samples_per_lane: Dict[int, List[NovaSeqSample]] = get_samples_by_lane(
+    samples_per_lane: Dict[int, List[FlowCellSampleBcl2Fastq]] = get_samples_by_lane(
         samples=[novaseq_sample_1, novaseq_sample_2]
     )
 
     # THEN the returned value is a dictionary
     assert isinstance(samples_per_lane, Dict)
     # THEN the dictionary has two entries
     assert len(samples_per_lane) == 2
```

### Comparing `cg-32.2.5/tests/apps/gens/test_gens_api.py` & `cg-32.2.7/tests/apps/gens/test_gens_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/gt/conftest.py` & `cg-32.2.7/tests/apps/gt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/gt/test_gt_api.py` & `cg-32.2.7/tests/apps/gt/test_gt_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/hk/conftest.py` & `cg-32.2.7/tests/apps/hk/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/hk/test__getattr__.py` & `cg-32.2.7/tests/apps/hk/test__getattr__.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/hk/test_add_file.py` & `cg-32.2.7/tests/apps/hk/test_add_file.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/hk/test_bundles.py` & `cg-32.2.7/tests/apps/hk/test_bundles.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/hk/test_core.py` & `cg-32.2.7/tests/apps/hk/test_core.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/hk/test_file.py` & `cg-32.2.7/tests/apps/hk/test_file.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/hk/test_version.py` & `cg-32.2.7/tests/apps/hk/test_version.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/lims/test_api.py` & `cg-32.2.7/tests/apps/lims/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Test the Lims api"""
 import datetime as dt
 
 from requests.exceptions import HTTPError
 
 
-def test_get_received_date(lims_api, mocker):
+def test_get_received_date(lims_mock, mocker):
     """Test to get the received date"""
     # GIVEN a lims api and a mocked sample that returns a received at date
     mocked_sample = mocker.patch("cg.apps.lims.api.Sample")
     mock_instance = mocked_sample.return_value
     date = dt.datetime.today()
     mock_instance.udf = {"Received at": date}
 
     # WHEN fetching the date
-    res = lims_api.get_received_date(123)
+    res = lims_mock.get_received_date(123)
 
-    # THEN asserrt the correct date is fetched
+    # THEN assert the correct date is fetched
     assert res == date
 
 
 def test_get_received_date_no_sample(lims_api, mocker):
     """Test to get the received date when sample not exists"""
     # GIVEN a lims api and a mocked sample that raises exception when fething date
     mocked_sample = mocker.patch("cg.apps.lims.api.Sample")
@@ -40,15 +40,15 @@
     mock_instance = mocked_sample.return_value
     date = dt.datetime.today()
     mock_instance.udf = {"Library Prep Finished": date}
 
     # WHEN fetching the date
     res = lims_api.get_prepared_date(123)
 
-    # THEN asserrt the correct date is fetched
+    # THEN assert the correct date is fetched
     assert res == date
 
 
 def test_get_prepared_date_no_sample(lims_api, mocker):
     """Test to get the prepared date when sample not exists"""
     # GIVEN a lims api and a mocked sample that raises exception when fething date
     mocked_sample = mocker.patch("cg.apps.lims.api.Sample")
@@ -69,15 +69,15 @@
     mock_instance = mocked_sample.return_value
     date = dt.datetime.today()
     mock_instance.udf = {"Delivered at": date}
 
     # WHEN fetching the date
     res = lims_api.get_delivery_date(123)
 
-    # THEN asserrt the correct date is fetched
+    # THEN assert the correct date is fetched
     assert res == date
 
 
 def test_get_delivery_date_no_sample(lims_api, mocker):
     """Test to get the delivery date when sample not exists"""
     # GIVEN a lims api and a mocked sample that raises exception when fething date
     mocked_sample = mocker.patch("cg.apps.lims.api.Sample")
```

### Comparing `cg-32.2.5/tests/apps/loqus/conftest.py` & `cg-32.2.7/tests/apps/loqus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/loqus/test_loqusdb_api.py` & `cg-32.2.7/tests/apps/loqus/test_loqusdb_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/madeline/conftest.py` & `cg-32.2.7/tests/apps/madeline/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/madeline/test_madeline.py` & `cg-32.2.7/tests/apps/madeline/test_madeline.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/mip/conftest.py` & `cg-32.2.7/tests/apps/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/mip/test_config_mip.py` & `cg-32.2.7/tests/apps/mip/test_config_mip.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/mutacc_auto/conftest.py` & `cg-32.2.7/tests/apps/mutacc_auto/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/mutacc_auto/test_mutacc_auto.py` & `cg-32.2.7/tests/apps/mutacc_auto/test_mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/orderform/conftest.py` & `cg-32.2.7/tests/apps/orderform/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/orderform/test_excel_orderform_parser.py` & `cg-32.2.7/tests/apps/orderform/test_excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/orderform/test_excel_sample_schema.py` & `cg-32.2.7/tests/apps/orderform/test_excel_sample_schema.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/orderform/test_json_orderform_parser.py` & `cg-32.2.7/tests/apps/orderform/test_json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/orderform/test_orderform_parser.py` & `cg-32.2.7/tests/apps/orderform/test_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/scout/conftest.py` & `cg-32.2.7/tests/apps/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/scout/test_get_causative_variants.py` & `cg-32.2.7/tests/apps/scout/test_get_causative_variants.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/scout/test_get_scout_cases.py` & `cg-32.2.7/tests/apps/scout/test_get_scout_cases.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/scout/test_scout_load_config.py` & `cg-32.2.7/tests/apps/scout/test_scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/scout/test_scout_models.py` & `cg-32.2.7/tests/apps/scout/test_scout_models.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/sequencing_metrics_parser/conftest.py` & `cg-32.2.7/tests/apps/sequencing_metrics_parser/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/sequencing_metrics_parser/parsers/conftest.py` & `cg-32.2.7/tests/apps/sequencing_metrics_parser/parsers/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py` & `cg-32.2.7/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_to_sequencing_statistics.py` & `cg-32.2.7/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py` & `cg-32.2.7/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py` & `cg-32.2.7/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py` & `cg-32.2.7/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/slurm/conftest.py` & `cg-32.2.7/tests/apps/slurm/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/slurm/test_slurm_api.py` & `cg-32.2.7/tests/apps/slurm/test_slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/test_apps_environ.py` & `cg-32.2.7/tests/apps/test_apps_environ.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/test_osticket.py` & `cg-32.2.7/tests/apps/test_osticket.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/vogue/conftest.py` & `cg-32.2.7/tests/apps/vogue/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/apps/vogue/test_vogue_api.py` & `cg-32.2.7/tests/apps/vogue/test_vogue_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/add/test_cli_add.py` & `cg-32.2.7/tests/cli/add/test_cli_add.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/add/test_cli_add_customer.py` & `cg-32.2.7/tests/cli/add/test_cli_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/add/test_cli_add_family.py` & `cg-32.2.7/tests/cli/add/test_cli_add_family.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/add/test_cli_add_relationship.py` & `cg-32.2.7/tests/cli/add/test_cli_add_relationship.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/add/test_cli_add_sample.py` & `cg-32.2.7/tests/cli/add/test_cli_add_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/backup/conftest.py` & `cg-32.2.7/tests/cli/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/backup/test_backup_command.py` & `cg-32.2.7/tests/cli/backup/test_backup_command.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/clean/conftest.py` & `cg-32.2.7/tests/cli/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/clean/test_balsamic_clean.py` & `cg-32.2.7/tests/cli/clean/test_balsamic_clean.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/clean/test_clean_hk_bundle_files.py` & `cg-32.2.7/tests/cli/clean/test_clean_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/clean/test_hk_bundle_files.py` & `cg-32.2.7/tests/cli/clean/test_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/clean/test_hk_case_bundle_files.py` & `cg-32.2.7/tests/cli/clean/test_hk_case_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/clean/test_microbial_clean.py` & `cg-32.2.7/tests/cli/clean/test_microbial_clean.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/clean/test_rsync_past_run_dirs.py` & `cg-32.2.7/tests/cli/clean/test_rsync_past_run_dirs.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/compress/conftest.py` & `cg-32.2.7/tests/cli/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/compress/test_cli_compress_fastq.py` & `cg-32.2.7/tests/cli/compress/test_cli_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/compress/test_cli_decompress_spring.py` & `cg-32.2.7/tests/cli/compress/test_cli_decompress_spring.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/compress/test_compress_helpers.py` & `cg-32.2.7/tests/cli/compress/test_compress_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/compress/test_store_fastq.py` & `cg-32.2.7/tests/cli/compress/test_store_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/conftest.py` & `cg-32.2.7/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/delete/test_cli_delete_case.py` & `cg-32.2.7/tests/cli/delete/test_cli_delete_case.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/delete/test_cli_delete_cases.py` & `cg-32.2.7/tests/cli/delete/test_cli_delete_cases.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/deliver/conftest.py` & `cg-32.2.7/tests/cli/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/deliver/test_deliver_base.py` & `cg-32.2.7/tests/cli/deliver/test_deliver_base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/deliver/test_rsync_base.py` & `cg-32.2.7/tests/cli/deliver/test_rsync_base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/deliver/test_run_deliver_cmd.py` & `cg-32.2.7/tests/cli/deliver/test_run_deliver_cmd.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/demultiplex/conftest.py` & `cg-32.2.7/tests/cli/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/demultiplex/test_add_flowcell.py` & `cg-32.2.7/tests/cli/demultiplex/test_add_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/demultiplex/test_create_sample_sheet.py` & `cg-32.2.7/tests/cli/demultiplex/test_create_sample_sheet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from pathlib import Path
 from typing import List
 
 from click import testing
 
 from cg.apps.demultiplex.demultiplex_api import DemultiplexingAPI
-from cg.apps.lims.samplesheet import (
-    LimsFlowcellSampleBcl2Fastq,
-    LimsFlowcellSampleDragen,
+from cg.apps.demultiplex.sample_sheet.models import (
+    FlowCellSampleBcl2Fastq,
+    FlowCellSampleDragen,
 )
 from cg.cli.demultiplex.sample_sheet import create_sheet
 from cg.constants.demultiplexing import BclConverter
 from cg.constants.process import EXIT_SUCCESS
 from cg.models.cg_config import CGConfig
 from cg.models.demultiplex.flow_cell import FlowCell
 
-FLOW_CELL_FUNCTION_NAME: str = "cg.cli.demultiplex.sample_sheet.flowcell_samples"
+FLOW_CELL_FUNCTION_NAME: str = "cg.cli.demultiplex.sample_sheet.flow_cell_samples"
 
 
 def test_create_sample_sheet_no_run_parameters(
     cli_runner: testing.CliRunner,
     flow_cell_working_directory_no_run_parameters: Path,
     sample_sheet_context: CGConfig,
-    lims_novaseq_bcl2fastq_samples: List[LimsFlowcellSampleBcl2Fastq],
+    lims_novaseq_bcl2fastq_samples: List[FlowCellSampleBcl2Fastq],
     caplog,
     mocker,
 ):
     # GIVEN a folder with a non-existing sample sheet
     flowcell_object: FlowCell = FlowCell(flow_cell_working_directory_no_run_parameters)
     assert flowcell_object.run_parameters_path.exists() is False
 
@@ -52,15 +52,15 @@
     assert "Could not find run parameters file" in caplog.text
 
 
 def test_create_bcl2fastq_sample_sheet(
     cli_runner: testing.CliRunner,
     flow_cell_working_directory: Path,
     sample_sheet_context: CGConfig,
-    lims_novaseq_bcl2fastq_samples: List[LimsFlowcellSampleBcl2Fastq],
+    lims_novaseq_bcl2fastq_samples: List[FlowCellSampleBcl2Fastq],
     mocker,
 ):
     # GIVEN a flowcell directory with some run parameters
     flowcell: FlowCell = FlowCell(flow_cell_working_directory)
     assert flowcell.run_parameters_path.exists()
 
     # GIVEN that there is no sample sheet present
@@ -88,15 +88,15 @@
     assert flowcell.validate_sample_sheet()
 
 
 def test_create_dragen_sample_sheet(
     cli_runner: testing.CliRunner,
     flow_cell_working_directory: Path,
     sample_sheet_context: CGConfig,
-    lims_novaseq_dragen_samples: List[LimsFlowcellSampleDragen],
+    lims_novaseq_dragen_samples: List[FlowCellSampleDragen],
     mocker,
 ):
     # GIVEN a flowcell directory with some run parameters
     flowcell: FlowCell = FlowCell(flow_cell_working_directory, bcl_converter=BclConverter.DRAGEN)
     assert flowcell.run_parameters_path.exists()
 
     # GIVEN that there is no sample sheet present
```

### Comparing `cg-32.2.5/tests/cli/demultiplex/test_demultiplex_flowcell.py` & `cg-32.2.7/tests/cli/demultiplex/test_demultiplex_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/demultiplex/test_finish_demux.py` & `cg-32.2.7/tests/cli/demultiplex/test_finish_demux.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/demultiplex/test_stats_command.py` & `cg-32.2.7/tests/cli/demultiplex/test_stats_command.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/demultiplex/test_validate_sample_sheet.py` & `cg-32.2.7/tests/cli/demultiplex/test_validate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/generate/report/conftest.py` & `cg-32.2.7/tests/cli/generate/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/generate/report/test_cli_delivery_report.py` & `cg-32.2.7/tests/cli/generate/report/test_cli_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/generate/report/test_utils.py` & `cg-32.2.7/tests/cli/generate/report/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/generate/test_cli_base.py` & `cg-32.2.7/tests/cli/generate/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/get/test_cli_get.py` & `cg-32.2.7/tests/cli/get/test_cli_get.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/get/test_cli_get_analysis.py` & `cg-32.2.7/tests/cli/get/test_cli_get_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/get/test_cli_get_case.py` & `cg-32.2.7/tests/cli/get/test_cli_get_case.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/get/test_cli_get_flow_cell.py` & `cg-32.2.7/tests/cli/get/test_cli_get_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/get/test_cli_get_sample.py` & `cg-32.2.7/tests/cli/get/test_cli_get_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/set/conftest.py` & `cg-32.2.7/tests/cli/set/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/set/test_cli_set_case.py` & `cg-32.2.7/tests/cli/set/test_cli_set_case.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/set/test_cli_set_cases.py` & `cg-32.2.7/tests/cli/set/test_cli_set_cases.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/set/test_cli_set_flowcell.py` & `cg-32.2.7/tests/cli/set/test_cli_set_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/set/test_cli_set_list_keys.py` & `cg-32.2.7/tests/cli/set/test_cli_set_list_keys.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/set/test_cli_set_sample.py` & `cg-32.2.7/tests/cli/set/test_cli_set_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/set/test_cli_set_samples.py` & `cg-32.2.7/tests/cli/set/test_cli_set_samples.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/store/test_fastq.py` & `cg-32.2.7/tests/cli/store/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/test_base.py` & `cg-32.2.7/tests/cli/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/test_clean.py` & `cg-32.2.7/tests/cli/test_clean.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/upload/conftest.py` & `cg-32.2.7/tests/cli/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/upload/test_cli_scout.py` & `cg-32.2.7/tests/cli/upload/test_cli_scout.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/upload/test_cli_upload.py` & `cg-32.2.7/tests/cli/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/upload/test_cli_upload_auto.py` & `cg-32.2.7/tests/cli/upload/test_cli_upload_auto.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/upload/test_cli_upload_delivery_report.py` & `cg-32.2.7/tests/cli/upload/test_cli_upload_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/upload/test_cli_upload_fastq.py` & `cg-32.2.7/tests/cli/upload/test_cli_upload_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/upload/test_cli_upload_genotype.py` & `cg-32.2.7/tests/cli/upload/test_cli_upload_genotype.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/upload/test_cli_upload_gens.py` & `cg-32.2.7/tests/cli/upload/test_cli_upload_gens.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/upload/test_cli_upload_nipt.py` & `cg-32.2.7/tests/cli/upload/test_cli_upload_nipt.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/upload/test_cli_upload_nipt_ftp.py` & `cg-32.2.7/tests/cli/upload/test_cli_upload_nipt_ftp.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/upload/test_cli_upload_nipt_statina.py` & `cg-32.2.7/tests/cli/upload/test_cli_upload_nipt_statina.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/upload/test_cli_upload_observations.py` & `cg-32.2.7/tests/cli/upload/test_cli_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/upload/test_cli_upload_vogue.py` & `cg-32.2.7/tests/cli/upload/test_cli_upload_vogue.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/balsamic/conftest.py` & `cg-32.2.7/tests/cli/workflow/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py` & `cg-32.2.7/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/balsamic/test_compound_commands.py` & `cg-32.2.7/tests/cli/workflow/balsamic/test_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/balsamic/test_link.py` & `cg-32.2.7/tests/cli/workflow/balsamic/test_link.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/balsamic/test_report_deliver.py` & `cg-32.2.7/tests/cli/workflow/balsamic/test_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/balsamic/test_run.py` & `cg-32.2.7/tests/cli/workflow/balsamic/test_run.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/balsamic/test_store_housekeeper.py` & `cg-32.2.7/tests/cli/workflow/balsamic/test_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/conftest.py` & `cg-32.2.7/tests/cli/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/fastq/test_fastq_base.py` & `cg-32.2.7/tests/cli/workflow/fastq/test_fastq_base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/fluffy/conftest.py` & `cg-32.2.7/tests/cli/workflow/fluffy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py` & `cg-32.2.7/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/fluffy/test_cli_link.py` & `cg-32.2.7/tests/cli/workflow/fluffy/test_cli_link.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/fluffy/test_cli_run.py` & `cg-32.2.7/tests/cli/workflow/fluffy/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/fluffy/test_cli_start.py` & `cg-32.2.7/tests/cli/workflow/fluffy/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/fluffy/test_cli_store.py` & `cg-32.2.7/tests/cli/workflow/fluffy/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/microsalt/conftest.py` & `cg-32.2.7/tests/cli/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py` & `cg-32.2.7/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/microsalt/test_microsalt_case_config.py` & `cg-32.2.7/tests/cli/workflow/microsalt/test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/microsalt/test_microsalt_run.py` & `cg-32.2.7/tests/cli/workflow/microsalt/test_microsalt_run.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/mip/conftest.py` & `cg-32.2.7/tests/cli/workflow/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_base.py` & `cg-32.2.7/tests/cli/workflow/mip/test_cli_mip_base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py` & `cg-32.2.7/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_dna_run.py` & `cg-32.2.7/tests/cli/workflow/mip/test_cli_mip_dna_run.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_dna_start.py` & `cg-32.2.7/tests/cli/workflow/mip/test_cli_mip_dna_start.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py` & `cg-32.2.7/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_rna_link.py` & `cg-32.2.7/tests/cli/workflow/mip/test_cli_mip_rna_link.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_rna_run.py` & `cg-32.2.7/tests/cli/workflow/mip/test_cli_mip_rna_run.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_store.py` & `cg-32.2.7/tests/cli/workflow/mip/test_cli_mip_store.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/rnafusion/conftest.py` & `cg-32.2.7/tests/cli/workflow/rnafusion/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py` & `cg-32.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py` & `cg-32.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py` & `cg-32.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py` & `cg-32.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py` & `cg-32.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py` & `cg-32.2.7/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py` & `cg-32.2.7/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/test_cli_workflow.py` & `cg-32.2.7/tests/cli/workflow/test_cli_workflow.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/cli/workflow/test_cli_workflow_clean.py` & `cg-32.2.7/tests/cli/workflow/test_cli_workflow_clean.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/conftest.py` & `cg-32.2.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml` & `cg-32.2.7/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json` & `cg-32.2.7/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json` & `cg-32.2.7/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/analysis/rnafusion/multiqc_data.json` & `cg-32.2.7/tests/fixtures/analysis/rnafusion/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/analysis/sample_coverage.bed` & `cg-32.2.7/tests/fixtures/analysis/sample_coverage.bed`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/balsamic/case/config.json` & `cg-32.2.7/tests/fixtures/apps/balsamic/case/config.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/balsamic/case/metadata.yml` & `cg-32.2.7/tests/fixtures/apps/balsamic/case/metadata.yml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml` & `cg-32.2.7/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/crunchy/spring_metadata.json` & `cg-32.2.7/tests/fixtures/apps/crunchy/spring_metadata.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/RunParameters_different_index_cycles.xml` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/RunParameters_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml` & `cg-32.2.7/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/fluffy/SampleSheet.csv` & `cg-32.2.7/tests/fixtures/apps/fluffy/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/fluffy/deliverables.yaml` & `cg-32.2.7/tests/fixtures/apps/fluffy/deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/madeline/madeline.xml` & `cg-32.2.7/tests/fixtures/apps/madeline/madeline.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/mip/case_metrics_deliverables.yaml` & `cg-32.2.7/tests/fixtures/apps/mip/case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/mip/dna/store/case_config.yaml` & `cg-32.2.7/tests/fixtures/apps/mip/dna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml` & `cg-32.2.7/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml` & `cg-32.2.7/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf` & `cg-32.2.7/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/mip/rna/case_config.yaml` & `cg-32.2.7/tests/fixtures/apps/mip/rna/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml` & `cg-32.2.7/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/mip/rna/store/bundle_data.yaml` & `cg-32.2.7/tests/fixtures/apps/mip/rna/store/bundle_data.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/mip/rna/store/case_config.yaml` & `cg-32.2.7/tests/fixtures/apps/mip/rna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml` & `cg-32.2.7/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml` & `cg-32.2.7/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/scout/643594.config.yaml` & `cg-32.2.7/tests/fixtures/apps/scout/643594.config.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/scout/case_export.json` & `cg-32.2.7/tests/fixtures/apps/scout/case_export.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/scout/export_causatives.json` & `cg-32.2.7/tests/fixtures/apps/scout/export_causatives.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/scout/none_case_export.json` & `cg-32.2.7/tests/fixtures/apps/scout/none_case_export.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/scout/other_sex_case.json` & `cg-32.2.7/tests/fixtures/apps/scout/other_sex_case.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/scout/panel_export.bed` & `cg-32.2.7/tests/fixtures/apps/scout/panel_export.bed`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/scout/panel_export.csv` & `cg-32.2.7/tests/fixtures/apps/scout/panel_export.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/sequencing_metrics_parser/Adapter_Metrics.csv` & `cg-32.2.7/tests/fixtures/apps/sequencing_metrics_parser/Adapter_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/sequencing_metrics_parser/Demultiplex_Stats.csv` & `cg-32.2.7/tests/fixtures/apps/sequencing_metrics_parser/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/sequencing_metrics_parser/Quality_Metrics.csv` & `cg-32.2.7/tests/fixtures/apps/sequencing_metrics_parser/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/sequencing_metrics_parser/RunInfo.xml` & `cg-32.2.7/tests/fixtures/apps/sequencing_metrics_parser/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/apps/sequencing_metrics_parser/SampleSheet.csv` & `cg-32.2.7/tests/fixtures/apps/sequencing_metrics_parser/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/cgweb_orders/balsamic.json` & `cg-32.2.7/tests/fixtures/cgweb_orders/balsamic.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/cgweb_orders/fastq.json` & `cg-32.2.7/tests/fixtures/cgweb_orders/fastq.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/cgweb_orders/metagenome.json` & `cg-32.2.7/tests/fixtures/cgweb_orders/metagenome.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/cgweb_orders/microsalt.json` & `cg-32.2.7/tests/fixtures/cgweb_orders/microsalt.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/cgweb_orders/mip.json` & `cg-32.2.7/tests/fixtures/cgweb_orders/mip.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/cgweb_orders/mip_rna.json` & `cg-32.2.7/tests/fixtures/cgweb_orders/mip_rna.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/cgweb_orders/rml.json` & `cg-32.2.7/tests/fixtures/cgweb_orders/rml.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/cgweb_orders/sarscov2.json` & `cg-32.2.7/tests/fixtures/cgweb_orders/sarscov2.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/data/SampleSheet.csv` & `cg-32.2.7/tests/fixtures/data/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/data/cgfixture.db` & `cg-32.2.7/tests/fixtures/data/cgfixture.db`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/data/hkstore.db` & `cg-32.2.7/tests/fixtures/data/hkstore.db`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/io/example_json.json` & `cg-32.2.7/tests/fixtures/io/example_json.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/orderforms/1508.27.balsamic.xlsx` & `cg-32.2.7/tests/fixtures/orderforms/1508.27.balsamic.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx` & `cg-32.2.7/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx` & `cg-32.2.7/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/orderforms/1508.27.fastq.xlsx` & `cg-32.2.7/tests/fixtures/orderforms/1508.27.fastq.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/orderforms/1508.27.mip.xlsx` & `cg-32.2.7/tests/fixtures/orderforms/1508.27.mip.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/orderforms/1508.27.mip_rna.xlsx` & `cg-32.2.7/tests/fixtures/orderforms/1508.27.mip_rna.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/orderforms/1603.11.microbial.xlsx` & `cg-32.2.7/tests/fixtures/orderforms/1603.11.microbial.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/orderforms/1604.15.rml.xlsx` & `cg-32.2.7/tests/fixtures/orderforms/1604.15.rml.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/orderforms/1605.10.metagenome.xlsx` & `cg-32.2.7/tests/fixtures/orderforms/1605.10.metagenome.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/orderforms/2184.7.sarscov2.xlsx` & `cg-32.2.7/tests/fixtures/orderforms/2184.7.sarscov2.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/orderforms/NIPT-json.json` & `cg-32.2.7/tests/fixtures/orderforms/NIPT-json.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json` & `cg-32.2.7/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/orderforms/mip_uploaded_json_orderform.json` & `cg-32.2.7/tests/fixtures/orderforms/mip_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/report/case_data.json` & `cg-32.2.7/tests/fixtures/report/case_data.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/report/lims_exported_samples.json` & `cg-32.2.7/tests/fixtures/report/lims_exported_samples.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/fixtures/report/lims_family.json` & `cg-32.2.7/tests/fixtures/report/lims_family.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/io/conftest.py` & `cg-32.2.7/tests/io/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,7 +45,19 @@
     return """Lorem,ipsum,sit,amet"""
 
 
 @pytest.fixture(name="csv_temp_path")
 def fixture_csv_temp_path(cg_dir: Path) -> Path:
     """Return a temp file path to use when writing csv."""
     return Path(cg_dir, "write_csv.csv")
+
+
+@pytest.fixture(name="xml_file_path")
+def fixture_xml_file_path(fixtures_dir: Path) -> Path:
+    """Return a file path to example XML file."""
+    return Path(fixtures_dir, "io", "example_xml.xml")
+
+
+@pytest.fixture(name="xml_temp_path")
+def fixture_xml_temp_path(cg_dir: Path) -> Path:
+    """Return a temp file path to use when writing xml."""
+    return Path(cg_dir, "write_xml.xml")
```

### Comparing `cg-32.2.5/tests/io/test_io_controller.py` & `cg-32.2.7/tests/io/test_io_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-
+from typing import List
 from cg.constants.constants import FileFormat
 from cg.io.controller import ReadFile, WriteFile, ReadStream, WriteStream
 from cg.models.mip.mip_sample_info import MipBaseSampleInfo
 
 
 def test_get_content_from_file(case_qc_sample_info_path: Path):
     """
```

### Comparing `cg-32.2.5/tests/io/test_io_csv.py` & `cg-32.2.7/tests/io/test_io_csv.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/io/test_io_json.py` & `cg-32.2.7/tests/io/test_io_json.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/io/test_io_yaml.py` & `cg-32.2.7/tests/io/test_io_yaml.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/io/test_validate_path.py` & `cg-32.2.7/tests/io/test_validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/archive/conftest.py` & `cg-32.2.7/tests/meta/archive/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/archive/test_archiving.py` & `cg-32.2.7/tests/meta/archive/test_archiving.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/backup/conftest.py` & `cg-32.2.7/tests/meta/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/backup/test_meta_backup.py` & `cg-32.2.7/tests/meta/backup/test_meta_backup.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/backup/test_meta_pdc.py` & `cg-32.2.7/tests/meta/backup/test_meta_pdc.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/clean/conftest.py` & `cg-32.2.7/tests/meta/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/clean/test_clean_demultiplexed_runs.py` & `cg-32.2.7/tests/meta/clean/test_clean_demultiplexed_runs.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/clean/test_clean_flow_cell_run_directories.py` & `cg-32.2.7/tests/meta/clean/test_clean_flow_cell_run_directories.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/compress/conftest.py` & `cg-32.2.7/tests/meta/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/compress/test_clean_fastq.py` & `cg-32.2.7/tests/meta/compress/test_clean_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/compress/test_compress_files.py` & `cg-32.2.7/tests/meta/compress/test_compress_files.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/compress/test_compress_meta_fastq.py` & `cg-32.2.7/tests/meta/compress/test_compress_meta_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/compress/test_decompress_spring_meta.py` & `cg-32.2.7/tests/meta/compress/test_decompress_spring_meta.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/compress/test_meta_compress_update_hk.py` & `cg-32.2.7/tests/meta/compress/test_meta_compress_update_hk.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/conftest.py` & `cg-32.2.7/tests/meta/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/deliver/conftest.py` & `cg-32.2.7/tests/meta/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/deliver/test_deliver_ticket.py` & `cg-32.2.7/tests/meta/deliver/test_deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/deliver/test_delivery_api.py` & `cg-32.2.7/tests/meta/deliver/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/demultiplex/conftest.py` & `cg-32.2.7/tests/meta/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/demultiplex/test_delete_demultiplex_api.py` & `cg-32.2.7/tests/meta/demultiplex/test_delete_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/demultiplex/test_demux_post_processing.py` & `cg-32.2.7/tests/meta/demultiplex/test_demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/demultiplex/test_rename_files.py` & `cg-32.2.7/tests/meta/demultiplex/test_rename_files.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/encryption/conftest.py` & `cg-32.2.7/tests/meta/encryption/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/encryption/test_encryption.py` & `cg-32.2.7/tests/meta/encryption/test_encryption.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/observations/conftest.py` & `cg-32.2.7/tests/meta/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/observations/test_meta_upload_observations.py` & `cg-32.2.7/tests/meta/observations/test_meta_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/orders/conftest.py` & `cg-32.2.7/tests/meta/orders/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/orders/test_PoolSubmitter_validate_order.py` & `cg-32.2.7/tests/meta/orders/test_PoolSubmitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py` & `cg-32.2.7/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/orders/test_SarsCov2Submitter_store_order.py` & `cg-32.2.7/tests/meta/orders/test_SarsCov2Submitter_store_order.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/orders/test_SarsCov2Submitter_validate_order.py` & `cg-32.2.7/tests/meta/orders/test_SarsCov2Submitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/orders/test_meta_orders_api.py` & `cg-32.2.7/tests/meta/orders/test_meta_orders_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/orders/test_meta_orders_lims.py` & `cg-32.2.7/tests/meta/orders/test_meta_orders_lims.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/orders/test_meta_orders_status.py` & `cg-32.2.7/tests/meta/orders/test_meta_orders_status.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/orders/test_ticket_handler.py` & `cg-32.2.7/tests/meta/orders/test_ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/report/conftest.py` & `cg-32.2.7/tests/meta/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/report/test_balsamic_api.py` & `cg-32.2.7/tests/meta/report/test_balsamic_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/report/test_field_validators.py` & `cg-32.2.7/tests/meta/report/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/report/test_mip_dna_api.py` & `cg-32.2.7/tests/meta/report/test_mip_dna_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/report/test_report_api.py` & `cg-32.2.7/tests/meta/report/test_report_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/rsync/conftest.py` & `cg-32.2.7/tests/meta/rsync/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/rsync/test_rsync.py` & `cg-32.2.7/tests/meta/rsync/test_rsync.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/test_invoice.py` & `cg-32.2.7/tests/meta/test_invoice.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/transfer/conftest.py` & `cg-32.2.7/tests/meta/transfer/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/transfer/test_external_data.py` & `cg-32.2.7/tests/meta/transfer/test_external_data.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/transfer/test_meta_transfer_flowcell.py` & `cg-32.2.7/tests/meta/transfer/test_meta_transfer_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/transfer/test_meta_transfer_lims.py` & `cg-32.2.7/tests/meta/transfer/test_meta_transfer_lims.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/upload/balsamic/test_balsamic.py` & `cg-32.2.7/tests/meta/upload/balsamic/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/upload/conftest.py` & `cg-32.2.7/tests/meta/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/upload/gisaid/fixtures/four_samples.csv` & `cg-32.2.7/tests/meta/upload/gisaid/fixtures/four_samples.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/upload/mutacc/conftest.py` & `cg-32.2.7/tests/meta/upload/mutacc/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/upload/mutacc/test_meta_upload_mutacc.py` & `cg-32.2.7/tests/meta/upload/mutacc/test_meta_upload_mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/upload/nipt/conftest.py` & `cg-32.2.7/tests/meta/upload/nipt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/upload/nipt/test_nipt_upload_api.py` & `cg-32.2.7/tests/meta/upload/nipt/test_nipt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/upload/scout/conftest.py` & `cg-32.2.7/tests/meta/upload/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/upload/scout/test_generate_load_config.py` & `cg-32.2.7/tests/meta/upload/scout/test_generate_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/upload/scout/test_meta_upload_scoutapi.py` & `cg-32.2.7/tests/meta/upload/scout/test_meta_upload_scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py` & `cg-32.2.7/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/upload/scout/test_scout_config_builder.py` & `cg-32.2.7/tests/meta/upload/scout/test_scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/upload/test_meta_upload_coverage.py` & `cg-32.2.7/tests/meta/upload/test_meta_upload_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/upload/test_upload_api.py` & `cg-32.2.7/tests/meta/upload/test_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/upload/test_upload_genotypes_api.py` & `cg-32.2.7/tests/meta/upload/test_upload_genotypes_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/upload/vogue/conftest.py` & `cg-32.2.7/tests/meta/upload/vogue/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/upload/vogue/test_upload_vogue.py` & `cg-32.2.7/tests/meta/upload/vogue/test_upload_vogue.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/workflow/conftest.py` & `cg-32.2.7/tests/meta/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/workflow/test_analysis.py` & `cg-32.2.7/tests/meta/workflow/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/workflow/test_balsamic.py` & `cg-32.2.7/tests/meta/workflow/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/workflow/test_microsalt.py` & `cg-32.2.7/tests/meta/workflow/test_microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/meta/workflow/test_prepare_fastq_api.py` & `cg-32.2.7/tests/meta/workflow/test_prepare_fastq_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/mocks/balsamic_analysis_mock.py` & `cg-32.2.7/tests/mocks/balsamic_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/mocks/crunchy.py` & `cg-32.2.7/tests/mocks/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/mocks/hk_mock.py` & `cg-32.2.7/tests/mocks/hk_mock.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/mocks/limsmock.py` & `cg-32.2.7/tests/mocks/limsmock.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,22 @@
 from typing_extensions import Literal
 
 
 class LimsProject(BaseModel):
     id: str = "1"
 
 
+class MockReagentType:
+    """Mock class for reagent type."""
+
+    def __init__(self, label: str, sequence: str):
+        self.label: str = label
+        self.sequence: str = sequence
+
+
 class LimsSample(BaseModel):
     id: str
     name: str = None
     customer: str = None
     sex: Literal["male", "female", "unknown"] = None
     father: str = None
     mother: str = None
```

### Comparing `cg-32.2.5/tests/mocks/madeline.py` & `cg-32.2.7/tests/mocks/madeline.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/mocks/mip_analysis_mock.py` & `cg-32.2.7/tests/mocks/mip_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/mocks/osticket.py` & `cg-32.2.7/tests/mocks/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/mocks/process_mock.py` & `cg-32.2.7/tests/mocks/process_mock.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/mocks/report.py` & `cg-32.2.7/tests/mocks/report.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/mocks/scout.py` & `cg-32.2.7/tests/mocks/scout.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/mocks/store_model.py` & `cg-32.2.7/tests/mocks/store_model.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/mocks/tb_mock.py` & `cg-32.2.7/tests/mocks/tb_mock.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/balsamic/conftest.py` & `cg-32.2.7/tests/models/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/balsamic/test_balsamic_analysis.py` & `cg-32.2.7/tests/models/balsamic/test_balsamic_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/conftest.py` & `cg-32.2.7/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/demultiplexing/conftest.py` & `cg-32.2.7/tests/models/demultiplexing/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/demultiplexing/test_demux_results.py` & `cg-32.2.7/tests/models/demultiplexing/test_demux_results.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/demultiplexing/test_flowcell_model.py` & `cg-32.2.7/tests/models/demultiplexing/test_flowcell_model.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/demultiplexing/test_run_parameters.py` & `cg-32.2.7/tests/models/demultiplexing/test_run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/mip/conftest.py` & `cg-32.2.7/tests/models/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/mip/test_mip_analysis.py` & `cg-32.2.7/tests/models/mip/test_mip_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/mip/test_mip_config.py` & `cg-32.2.7/tests/models/mip/test_mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/mip/test_mip_metrics_deliverables.py` & `cg-32.2.7/tests/models/mip/test_mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/mip/test_mip_sample_info.py` & `cg-32.2.7/tests/models/mip/test_mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/nextflow/conftest.py` & `cg-32.2.7/tests/models/nextflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/nextflow/test_nextflow_deliver.py` & `cg-32.2.7/tests/models/nextflow/test_nextflow_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/observations/conftest.py` & `cg-32.2.7/tests/models/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/observations/test_observations_input_files.py` & `cg-32.2.7/tests/models/observations/test_observations_input_files.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/report/test_validators.py` & `cg-32.2.7/tests/models/report/test_validators.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/rnafusion/conftest.py` & `cg-32.2.7/tests/models/rnafusion/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/rnafusion/test_rnafusion_sample.py` & `cg-32.2.7/tests/models/rnafusion/test_rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/test_cg_models.py` & `cg-32.2.7/tests/models/test_cg_models.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/test_compression_data.py` & `cg-32.2.7/tests/models/test_compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/test_file_data.py` & `cg-32.2.7/tests/models/test_file_data.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/models/test_flowcell_class.py` & `cg-32.2.7/tests/models/test_flowcell_class.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/server/conftest.py` & `cg-32.2.7/tests/server/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/api/add/test_store_add_application_version.py` & `cg-32.2.7/tests/store/api/add/test_store_add_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/api/add/test_store_add_base.py` & `cg-32.2.7/tests/store/api/add/test_store_add_base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/api/add/test_store_add_customer.py` & `cg-32.2.7/tests/store/api/add/test_store_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/api/add/test_store_add_flow_celll.py` & `cg-32.2.7/tests/store/api/add/test_store_add_flow_celll.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/api/conftest.py` & `cg-32.2.7/tests/store/api/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/api/delete/test_store_api_delete.py` & `cg-32.2.7/tests/store/api/delete/test_store_api_delete.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/api/find/test_find_basic_data.py` & `cg-32.2.7/tests/store/api/find/test_find_basic_data.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/api/find/test_find_basic_data_application_version.py` & `cg-32.2.7/tests/store/api/find/test_find_basic_data_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/api/find/test_find_business_data.py` & `cg-32.2.7/tests/store/api/find/test_find_business_data.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/api/find/test_find_business_data_analysis.py` & `cg-32.2.7/tests/store/api/find/test_find_business_data_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/api/find/test_find_business_data_case.py` & `cg-32.2.7/tests/store/api/find/test_find_business_data_case.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/api/find/test_find_business_data_sample.py` & `cg-32.2.7/tests/store/api/find/test_find_business_data_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/api/status/test_analyses_to_clean.py` & `cg-32.2.7/tests/store/api/status/test_analyses_to_clean.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/api/status/test_analyses_to_delivery_report.py` & `cg-32.2.7/tests/store/api/status/test_analyses_to_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/api/status/test_store_api_status.py` & `cg-32.2.7/tests/store/api/status/test_store_api_status.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/api/status/test_store_api_status_analysis.py` & `cg-32.2.7/tests/store/api/status/test_store_api_status_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/api/status/test_store_api_status_cases.py` & `cg-32.2.7/tests/store/api/status/test_store_api_status_cases.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/api/status/test_store_api_status_customer.py` & `cg-32.2.7/tests/store/api/status/test_store_api_status_customer.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/api/status/test_store_api_status_pool.py` & `cg-32.2.7/tests/store/api/status/test_store_api_status_pool.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/api/status/test_store_api_status_sample.py` & `cg-32.2.7/tests/store/api/status/test_store_api_status_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/api/test_base.py` & `cg-32.2.7/tests/store/api/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/conftest.py` & `cg-32.2.7/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/filters/test_status_analyses_filters.py` & `cg-32.2.7/tests/store/filters/test_status_analyses_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/filters/test_status_application_filters.py` & `cg-32.2.7/tests/store/filters/test_status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/filters/test_status_application_version_filters.py` & `cg-32.2.7/tests/store/filters/test_status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/filters/test_status_bed_filters.py` & `cg-32.2.7/tests/store/filters/test_status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/filters/test_status_bed_version_filters.py` & `cg-32.2.7/tests/store/filters/test_status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/filters/test_status_case_sample_filters.py` & `cg-32.2.7/tests/store/filters/test_status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/filters/test_status_cases_filters.py` & `cg-32.2.7/tests/store/filters/test_status_cases_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/filters/test_status_collaboration_filters.py` & `cg-32.2.7/tests/store/filters/test_status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/filters/test_status_customer_filters.py` & `cg-32.2.7/tests/store/filters/test_status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/filters/test_status_flow_cell_filters.py` & `cg-32.2.7/tests/store/filters/test_status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/filters/test_status_invoice_filters.py` & `cg-32.2.7/tests/store/filters/test_status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/filters/test_status_organism_filters.py` & `cg-32.2.7/tests/store/filters/test_status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/filters/test_status_panel_filters.py` & `cg-32.2.7/tests/store/filters/test_status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/filters/test_status_pool_filters.py` & `cg-32.2.7/tests/store/filters/test_status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/filters/test_status_samples_filters.py` & `cg-32.2.7/tests/store/filters/test_status_samples_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/filters/test_status_user_filters.py` & `cg-32.2.7/tests/store/filters/test_status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/test_delivery.py` & `cg-32.2.7/tests/store/test_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store/test_store_models.py` & `cg-32.2.7/tests/store/test_store_models.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/store_helpers.py` & `cg-32.2.7/tests/store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/test_store_helpers.py` & `cg-32.2.7/tests/test_store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/utils/conftest.py` & `cg-32.2.7/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/utils/test_commands.py` & `cg-32.2.7/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/utils/test_date.py` & `cg-32.2.7/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/utils/test_dict.py` & `cg-32.2.7/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/utils/test_dispatcher.py` & `cg-32.2.7/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.5/tests/utils/test_utils.py` & `cg-32.2.7/tests/utils/test_utils.py`

 * *Files identical despite different names*

