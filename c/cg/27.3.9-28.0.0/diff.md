# Comparing `tmp/cg-27.3.9.tar.gz` & `tmp/cg-28.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cg-27.3.9.tar", last modified: Mon Apr 17 14:41:21 2023, max compression
+gzip compressed data, was "dist/cg-28.0.0.tar", last modified: Tue Apr 18 11:57:46 2023, max compression
```

## Comparing `cg-27.3.9.tar` & `cg-28.0.0.tar`

### file list

```diff
@@ -1,1237 +1,1237 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-17 14:41:07.000000 cg-27.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-17 14:41:21.000000 cg-27.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-17 14:41:07.000000 cg-27.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-17 14:41:07.000000 cg-27.3.9/cg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14071 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/crud/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/crud/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/crud/find.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/apps/cgstats/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/apps/cgstats/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/db/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/db/models/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/db/models/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/db/models/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/db/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/db/models/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/db/models/support_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/db/models/unaligned.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/db/models/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/demux_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/dragen_demux_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/parsers/adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/parsers/conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/parsers/demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/parsers/quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/parsers/run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/cgstats/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/coverage/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/crunchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/crunchy/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/crunchy/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/crunchy/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/demultiplex/demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/demultiplex/demux_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/apps/demultiplex/sample_sheet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/demultiplex/sample_sheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/demultiplex/sample_sheet/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/demultiplex/sample_sheet/dummy_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/demultiplex/sample_sheet/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/apps/hermes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/hermes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/hermes/hermes_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/hermes/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/apps/housekeeper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/housekeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17462 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/housekeeper/hk.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/housekeeper/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/apps/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/invoice/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/apps/invoice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/invoice/templates/KI_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/invoice/templates/KI_sample_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/lims/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/lims/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/lims/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/lims/samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/loqus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/madeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/madeline/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/mip/confighandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/orderform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/orderform/excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/orderform/json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/orderform/orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/scout/scout_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/scout/scoutapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/slurm/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/slurm/slurm_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/apps/tb/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/tb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/tb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/tb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-17 14:41:07.000000 cg-27.3.9/cg/apps/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19645 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/compress/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/compress/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/compress/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/delete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/delete/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/delete/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/delete/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/delete/observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/deliver/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/demultiplex/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/demultiplex/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/demultiplex/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/demultiplex/finish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/demultiplex/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/demultiplex/sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/generate/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/generate/report/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/generate/report/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/generate/report/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/import_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/set/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/set/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/set/families.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/set/family.py
--rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/store/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/store/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/upload/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/upload/clinical_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/upload/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/upload/delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/upload/fohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/upload/genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/upload/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/upload/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/upload/nipt/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/upload/nipt/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/upload/nipt/statina.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/upload/observations/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/upload/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/upload/observations/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/upload/observations/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/upload/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/upload/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/upload/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/upload/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/balsamic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/balsamic/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/balsamic/pon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/balsamic/qc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/balsamic/umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/fastq/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/fluffy/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/microsalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/microsalt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/mip/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/mip/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/workflow/mip_dna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/mip_dna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/mip_dna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/workflow/mip_rna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/mip_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/mip_rna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/workflow/mutant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/mutant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/mutant/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/workflow/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/nextflow/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/rnafusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/rnafusion/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/cli/workflow/tower/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/tower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-17 14:41:07.000000 cg-27.3.9/cg/cli/workflow/tower/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-17 14:41:07.000000 cg-27.3.9/cg/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-17 14:41:07.000000 cg-27.3.9/cg/constants/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-17 14:41:07.000000 cg-27.3.9/cg/constants/cgstats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-17 14:41:07.000000 cg-27.3.9/cg/constants/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-04-17 14:41:07.000000 cg-27.3.9/cg/constants/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-17 14:41:07.000000 cg-27.3.9/cg/constants/delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-17 14:41:07.000000 cg-27.3.9/cg/constants/demultiplexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-17 14:41:07.000000 cg-27.3.9/cg/constants/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-17 14:41:07.000000 cg-27.3.9/cg/constants/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-17 14:41:07.000000 cg-27.3.9/cg/constants/gene_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-17 14:41:07.000000 cg-27.3.9/cg/constants/housekeeper_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-17 14:41:07.000000 cg-27.3.9/cg/constants/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-17 14:41:07.000000 cg-27.3.9/cg/constants/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-04-17 14:41:07.000000 cg-27.3.9/cg/constants/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-17 14:41:07.000000 cg-27.3.9/cg/constants/nextflow.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 14:41:07.000000 cg-27.3.9/cg/constants/nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-17 14:41:07.000000 cg-27.3.9/cg/constants/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-17 14:41:07.000000 cg-27.3.9/cg/constants/orderforms.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-17 14:41:07.000000 cg-27.3.9/cg/constants/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-17 14:41:07.000000 cg-27.3.9/cg/constants/pdc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 14:41:07.000000 cg-27.3.9/cg/constants/pedigree.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-17 14:41:07.000000 cg-27.3.9/cg/constants/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-17 14:41:08.000000 cg-27.3.9/cg/constants/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-17 14:41:08.000000 cg-27.3.9/cg/constants/report.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-17 14:41:08.000000 cg-27.3.9/cg/constants/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-17 14:41:08.000000 cg-27.3.9/cg/constants/sample_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-17 14:41:08.000000 cg-27.3.9/cg/constants/scout_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-17 14:41:08.000000 cg-27.3.9/cg/constants/sequencing.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-17 14:41:08.000000 cg-27.3.9/cg/constants/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-17 14:41:08.000000 cg-27.3.9/cg/constants/subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-17 14:41:08.000000 cg-27.3.9/cg/constants/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-17 14:41:08.000000 cg-27.3.9/cg/constants/tb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-04-17 14:41:08.000000 cg-27.3.9/cg/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-17 14:41:08.000000 cg-27.3.9/cg/io/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-17 14:41:08.000000 cg-27.3.9/cg/io/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-17 14:41:08.000000 cg-27.3.9/cg/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-17 14:41:08.000000 cg-27.3.9/cg/io/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-17 14:41:08.000000 cg-27.3.9/cg/io/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/archive/ddn_dataflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18846 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/backup/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/backup/pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/clean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/clean/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/clean/demultiplexed_flow_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/clean/flow_cell_run_directories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/compress/compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/compress/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/deliver_ticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/demultiplex/delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/demultiplex/demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/demultiplex/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/encryption/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/observations/balsamic_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/observations/mip_dna_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/observations/observations_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/orders/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/orders/balsamic_qc_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/orders/balsamic_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/orders/balsamic_umi_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/orders/case_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/orders/fastq_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/orders/fluffy_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/orders/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/orders/metagenome_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/orders/microbial_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/orders/microsalt_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/orders/mip_dna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/orders/mip_rna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/orders/pool_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/orders/rml_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/orders/sars_cov_2_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/orders/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/orders/ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/report/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/report/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/report/field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/report/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)    17804 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/report/report_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/report/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/report/templates/balsamic_report.html
--rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/report/templates/bootstrap.html
--rw-r--r--   0 runner    (1001) docker     (123)    77831 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/report/templates/mip-dna_report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/rsync/rsync_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/rsync/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/tar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/tar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/tar/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/transfer/external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/transfer/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/transfer/lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/balsamic/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/upload/fohm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/fohm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/fohm/fohm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/gisaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/gisaid/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/gisaid/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/gisaid/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/upload/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/mip/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/mip/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/nipt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/nipt/nipt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/upload/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/rnafusion/rnafusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/scout/balsamic_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/scout/balsamic_umi_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/scout/hk_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/scout/mip_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/scout/rnafusion_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/scout/scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    19581 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/scout/uploadscoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/upload/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19851 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/workflow/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    28514 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/workflow/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/workflow/balsamic_pon.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/workflow/balsamic_qc.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/workflow/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/workflow/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/workflow/fluffy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18187 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/workflow/microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)    14337 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/workflow/mip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/workflow/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/workflow/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/workflow/mutant.py
--rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/workflow/nextflow_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/workflow/prepare_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/workflow/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-17 14:41:08.000000 cg-27.3.9/cg/meta/workflow/tower_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/balsamic/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/balsamic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/balsamic/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12885 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/cg_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/models/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/cgstats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/cgstats/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/cgstats/stats_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/compression_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/models/deliverables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/deliverables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/deliverables/metric_deliverables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/models/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/demultiplex/demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/demultiplex/flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/demultiplex/run_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/file_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/models/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/invoice/invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/models/lims/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/lims/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/mip/mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/mip/mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/mip/mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/mip/mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/nextflow/deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/nextflow/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/observations/input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/models/orders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/orders/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/orders/excel_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/orders/json_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/orders/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/orders/orderform_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/orders/sample_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/orders/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/report/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/report/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/report/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/report/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/rnafusion/rnafusion_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/models/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/scout/scout_load_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/models/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/slurm/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/models/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-17 14:41:08.000000 cg-27.3.9/cg/models/workflow/mutant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-04-17 14:41:08.000000 cg-27.3.9/cg/resources/20181012_Indices.csv
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-17 14:41:08.000000 cg-27.3.9/cg/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-17 14:41:08.000000 cg-27.3.9/cg/resources/rnafusion_bundle_filenames.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16689 2023-04-17 14:41:08.000000 cg-27.3.9/cg/server/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    17951 2023-04-17 14:41:08.000000 cg-27.3.9/cg/server/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-04-17 14:41:08.000000 cg-27.3.9/cg/server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-17 14:41:08.000000 cg-27.3.9/cg/server/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-17 14:41:08.000000 cg-27.3.9/cg/server/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-17 14:41:08.000000 cg-27.3.9/cg/server/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/server/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-17 14:41:08.000000 cg-27.3.9/cg/server/invoices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/server/invoices/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/server/invoices/templates/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-17 14:41:08.000000 cg-27.3.9/cg/server/invoices/templates/invoices/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-04-17 14:41:08.000000 cg-27.3.9/cg/server/invoices/templates/invoices/invoice.html
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-17 14:41:08.000000 cg-27.3.9/cg/server/invoices/templates/invoices/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-04-17 14:41:08.000000 cg-27.3.9/cg/server/invoices/templates/invoices/new.html
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-17 14:41:08.000000 cg-27.3.9/cg/server/invoices/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/server/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/server/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-17 14:41:08.000000 cg-27.3.9/cg/server/templates/admin/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/store/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/api/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/api/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/api/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     9114 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/api/find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    31043 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/api/find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12822 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/api/import_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/api/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    41557 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/api/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/filters/status_analysis_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/filters/status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/filters/status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/filters/status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/filters/status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/filters/status_case_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/filters/status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/filters/status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/filters/status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/filters/status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/filters/status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/filters/status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/filters/status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/filters/status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/filters/status_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/filters/status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    27648 2023-04-17 14:41:08.000000 cg-27.3.9/cg/store/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-17 14:41:08.000000 cg-27.3.9/cg/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/utils/checksum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/utils/checksum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-17 14:41:08.000000 cg-27.3.9/cg/utils/checksum/checksum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/utils/click/
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-17 14:41:08.000000 cg-27.3.9/cg/utils/click/EnumChoice.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/utils/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-17 14:41:08.000000 cg-27.3.9/cg/utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-17 14:41:08.000000 cg-27.3.9/cg/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-17 14:41:08.000000 cg-27.3.9/cg/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-17 14:41:08.000000 cg-27.3.9/cg/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-17 14:41:08.000000 cg-27.3.9/cg/utils/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-17 14:41:08.000000 cg-27.3.9/cg/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-17 14:41:08.000000 cg-27.3.9/cg/utils/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg/utils/flask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/cg/utils/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-17 14:41:08.000000 cg-27.3.9/cg/utils/flask/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-17 14:41:08.000000 cg-27.3.9/cg/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-17 14:41:08.000000 cg-27.3.9/cg/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/cg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-17 14:41:20.000000 cg-27.3.9/cg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39296 2023-04-17 14:41:21.000000 cg-27.3.9/cg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:41:20.000000 cg-27.3.9/cg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 14:41:20.000000 cg-27.3.9/cg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:41:20.000000 cg-27.3.9/cg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-17 14:41:20.000000 cg-27.3.9/cg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-17 14:41:20.000000 cg-27.3.9/cg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-17 14:41:08.000000 cg-27.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-17 14:41:08.000000 cg-27.3.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 14:41:21.000000 cg-27.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-17 14:41:08.000000 cg-27.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/cgstats/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/cgstats/crud/test_create_novaseq.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/cgstats/crud/test_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/cgstats/parsers/test_adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/cgstats/parsers/test_conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/cgstats/parsers/test_demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/cgstats/parsers/test_quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/cgstats/parsers/test_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/cgstats/test_cgstats_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/cgstats/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/coverage/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/coverage/test_coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/crunchy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/crunchy/test_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/crunchy/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/crunchy/test_crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/crunchy/test_spring_decompression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/demultiplex/test_convert_to_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/demultiplex/test_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/demultiplex/test_parse_run_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/demultiplex/test_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/apps/gens/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/gens/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/gens/test_gens_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/gt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/gt/test_gt_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/apps/hk/
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/hk/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/hk/test__getattr__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/hk/test_add_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/hk/test_bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/hk/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/hk/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/hk/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/lims/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/lims/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/apps/loqus/
--rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/loqus/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/loqus/test_loqusdb_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/madeline/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/madeline/test_madeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/mip/test_config_mip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/apps/mutacc_auto/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/mutacc_auto/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/mutacc_auto/test_mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/orderform/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/orderform/test_excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/orderform/test_excel_sample_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/orderform/test_json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/orderform/test_orderform_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/scout/test_get_causative_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/scout/test_get_scout_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/scout/test_scout_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/scout/test_scout_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/slurm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/slurm/test_slurm_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/test_apps_environ.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/test_osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/apps/vogue/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/vogue/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-17 14:41:08.000000 cg-27.3.9/tests/apps/vogue/test_vogue_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/add/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/add/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/add/test_cli_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/add/test_cli_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/add/test_cli_add_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/add/test_cli_add_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/add/test_cli_add_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/backup/test_backup_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/clean/test_balsamic_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/clean/test_clean_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/clean/test_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/clean/test_hk_case_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/clean/test_microbial_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/clean/test_rsync_past_run_dirs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/compress/test_cli_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/compress/test_cli_decompress_spring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/compress/test_compress_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/compress/test_store_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/delete/test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/delete/test_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/deliver/test_deliver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/deliver/test_rsync_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/deliver/test_run_deliver_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/demultiplex/test_add_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/demultiplex/test_demultiplex_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/demultiplex/test_finish_demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/demultiplex/test_stats_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/demultiplex/test_validate_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/generate/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/generate/report/test_cli_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/generate/report/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/generate/test_cli_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/get/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/get/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/get/test_cli_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/get/test_cli_get_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/get/test_cli_get_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/get/test_cli_get_flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/get/test_cli_get_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/set/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/set/test_families.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/set/test_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/set/test_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/set/test_list_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/set/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/set/test_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/store/test_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/test_cli_status_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/upload/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/upload/test_cli_scout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/upload/test_cli_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/upload/test_cli_upload_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/upload/test_cli_upload_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/upload/test_cli_upload_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/upload/test_cli_upload_genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/upload/test_cli_upload_gens.py
--rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/upload/test_cli_upload_nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/upload/test_cli_upload_nipt_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/upload/test_cli_upload_nipt_statina.py
--rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/upload/test_cli_upload_observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/upload/test_cli_upload_vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)    30975 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/balsamic/test_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/balsamic/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/balsamic/test_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/balsamic/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/balsamic/test_store_housekeeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/fastq/test_fastq_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/fluffy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/fluffy/test_cli_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/fluffy/test_cli_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/fluffy/test_cli_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/fluffy/test_cli_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/microsalt/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/workflow/microsalt/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/microsalt/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/microsalt/test_microsalt_case_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/microsalt/test_microsalt_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/mip/test_cli_mip_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/mip/test_cli_mip_dna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/mip/test_cli_mip_dna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/mip/test_cli_mip_dna_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/mip/test_cli_mip_rna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/mip/test_cli_mip_rna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/mip/test_cli_mip_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/rnafusion/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/test_cli_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-04-17 14:41:08.000000 cg-27.3.9/tests/cli/workflow/test_cli_workflow_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    61338 2023-04-17 14:41:08.000000 cg-27.3.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/DEMUX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/analysis/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/analysis/balsamic/tn_wgs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/analysis/microsalt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
--rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/analysis/mip/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/analysis/mip/dna/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/analysis/mip/dna/ADM2.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/analysis/mip/dna/ADM3.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/analysis/mip/dna/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/analysis/mip/dna/adm1.mt.bam
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/analysis/mip/dna/multiqc.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/analysis/mip/dna/report.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/analysis/mip/dna/smn.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/analysis/mip/dna/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/analysis/mip/dna/snv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/analysis/mip/dna/str.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/analysis/mip/dna/sv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/analysis/mip/dna/sv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/analysis/sample_coverage.bed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/balsamic/case/
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/balsamic/case/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/balsamic/case/metadata.yml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/balsamic/case/metadata_directory.yml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/crunchy/spring_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)    53877 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/hiseq_run/
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/raw_lims_samples/
--rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/fluffy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/fluffy/2020-23219-05/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/fluffy/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/fluffy/deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/fluffy/multiqc_report.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/fluffy/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/gt/yellowhog.bcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/madeline/madeline.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/mip/case_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/mip/dna/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/mip/dna/store/
--rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/mip/dna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
--rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/mip/rna/
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/mip/rna/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/mip/rna/store/
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/mip/rna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/mip/sample_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/scout/643594.config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/scout/case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/scout/export_causatives.json
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/scout/none_case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/scout/other_sex_case.json
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/scout/panel_export.bed
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/scout/panel_export.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/apps/shipping/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/apps/shipping/scout-deploy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/cgweb_orders/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/cgweb_orders/balsamic.json
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/cgweb_orders/fastq.json
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/cgweb_orders/metagenome.json
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/cgweb_orders/microsalt.json
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/cgweb_orders/mip.json
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/cgweb_orders/mip_rna.json
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/cgweb_orders/rml.json
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/cgweb_orders/sarscov2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/data/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/data/cgfixture.db
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/data/fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/data/hkstore.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/data/yellowhog/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/data/yellowhog/pedigree.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/io/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/io/example_csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/io/example_json.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/orderforms/
--rw-r--r--   0 runner    (1001) docker     (123)   267284 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/orderforms/1508.27.balsamic.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   258613 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   266876 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   266141 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/orderforms/1508.27.fastq.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   266967 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/orderforms/1508.27.mip.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   266759 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/orderforms/1508.27.mip_rna.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    95878 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/orderforms/1603.11.microbial.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   163548 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/orderforms/1604.15.rml.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    88463 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/orderforms/1605.10.metagenome.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   227684 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/orderforms/NIPT-json.json
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/report/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/report/case_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/report/lims_exported_samples.json
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/report/lims_family.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/store/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/fixtures/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/store/api/application_versions.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-04-17 14:41:08.000000 cg-27.3.9/tests/fixtures/store/api/applications.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-17 14:41:08.000000 cg-27.3.9/tests/io/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-04-17 14:41:08.000000 cg-27.3.9/tests/io/test_io_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-17 14:41:08.000000 cg-27.3.9/tests/io/test_io_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-17 14:41:08.000000 cg-27.3.9/tests/io/test_io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-17 14:41:08.000000 cg-27.3.9/tests/io/test_io_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/archive/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/archive/test_archiving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24823 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/backup/test_meta_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/backup/test_meta_pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/clean/test_clean_demultiplexed_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/clean/test_clean_flow_cell_run_directories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/compress/test_clean_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/compress/test_compress_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/compress/test_compress_meta_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/compress/test_decompress_spring_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/compress/test_meta_compress_update_hk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/meta/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/deliver/test_deliver_ticket.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/deliver/test_delivery_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13319 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/demultiplex/test_delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13707 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/demultiplex/test_demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/demultiplex/test_rename_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/encryption/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/encryption/test_encryption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/observations/test_meta_upload_observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/orders/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/orders/test_PoolSubmitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/orders/test_SarsCov2Submitter_store_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    19702 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/orders/test_meta_orders_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/orders/test_meta_orders_lims.py
--rw-r--r--   0 runner    (1001) docker     (123)    29074 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/orders/test_meta_orders_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/orders/test_ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/report/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/report/test_balsamic_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/report/test_field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/report/test_mip_dna_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/report/test_report_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/rsync/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/rsync/test_rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/test_invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/transfer/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/transfer/test_external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/transfer/test_meta_transfer_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/transfer/test_meta_transfer_lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/balsamic/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/gisaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/gisaid/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/meta/upload/gisaid/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/gisaid/fixtures/four_samples.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/meta/upload/mutacc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/mutacc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/mutacc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/nipt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/nipt/test_nipt_upload_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23340 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/scout/test_generate_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/scout/test_meta_upload_scoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    24928 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/scout/test_scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/test_meta_upload_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/test_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/test_upload_genotypes_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/meta/upload/vogue/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/vogue/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/upload/vogue/test_upload_vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/workflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/workflow/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/workflow/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/workflow/test_microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-17 14:41:08.000000 cg-27.3.9/tests/meta/workflow/test_prepare_fastq_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-17 14:41:08.000000 cg-27.3.9/tests/mocks/balsamic_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-17 14:41:08.000000 cg-27.3.9/tests/mocks/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-04-17 14:41:08.000000 cg-27.3.9/tests/mocks/hk_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-17 14:41:08.000000 cg-27.3.9/tests/mocks/limsmock.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-17 14:41:08.000000 cg-27.3.9/tests/mocks/madeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-17 14:41:08.000000 cg-27.3.9/tests/mocks/mip_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-17 14:41:08.000000 cg-27.3.9/tests/mocks/osticket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-17 14:41:08.000000 cg-27.3.9/tests/mocks/process_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-17 14:41:08.000000 cg-27.3.9/tests/mocks/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-17 14:41:08.000000 cg-27.3.9/tests/mocks/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-17 14:41:08.000000 cg-27.3.9/tests/mocks/store_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-17 14:41:08.000000 cg-27.3.9/tests/mocks/tb_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/balsamic/test_balsamic_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/models/demultiplexing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/demultiplexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/demultiplexing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/demultiplexing/test_demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/demultiplexing/test_flowcell_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/mip/test_mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/mip/test_mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/mip/test_mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/mip/test_mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/nextflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/nextflow/test_nextflow_deliver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/observations/test_observations_input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/report/test_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/rnafusion/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/rnafusion/test_rnafusion_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/test_cg_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/test_compression_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/test_file_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-17 14:41:08.000000 cg-27.3.9/tests/models/test_flowcell_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/server/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-17 14:41:08.000000 cg-27.3.9/tests/server/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-17 14:41:08.000000 cg-27.3.9/tests/server/test_server_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-17 14:41:08.000000 cg-27.3.9/tests/server/test_server_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-17 14:41:08.000000 cg-27.3.9/tests/small_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/store/api/add/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/add/test_store_add_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/add/test_store_add_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/add/test_store_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/add/test_store_add_flow_celll.py
--rw-r--r--   0 runner    (1001) docker     (123)    22495 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/store/api/delete/
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/delete/test_store_api_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/store/api/find/
--rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/find/test_find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/find/test_find_basic_data_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    28729 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/find/test_find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/find/test_find_business_data_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/find/test_find_business_data_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/find/test_find_business_data_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/store/api/status/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/status/test_analyses_to_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/status/test_analyses_to_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/status/test_store_api_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    15264 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/status/test_store_api_status_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    54207 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/status/test_store_api_status_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/status/test_store_api_status_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/status/test_store_api_status_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/status/test_store_api_status_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/api/test_store_import_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    16784 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/filters/test_status_analyses_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/filters/test_status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/filters/test_status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/filters/test_status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/filters/test_status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/filters/test_status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    39472 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/filters/test_status_cases_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/filters/test_status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/filters/test_status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/filters/test_status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/filters/test_status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/filters/test_status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/filters/test_status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/filters/test_status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    26900 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/filters/test_status_samples_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/filters/test_status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/test_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store/test_store_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    29709 2023-04-17 14:41:08.000000 cg-27.3.9/tests/store_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-17 14:41:08.000000 cg-27.3.9/tests/test_store_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:21.000000 cg-27.3.9/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:41:08.000000 cg-27.3.9/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-17 14:41:08.000000 cg-27.3.9/tests/utils/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-17 14:41:08.000000 cg-27.3.9/tests/utils/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-17 14:41:08.000000 cg-27.3.9/tests/utils/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-17 14:41:08.000000 cg-27.3.9/tests/utils/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-04-17 14:41:08.000000 cg-27.3.9/tests/utils/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-17 14:41:08.000000 cg-27.3.9/tests/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-18 11:57:35.000000 cg-28.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-18 11:57:46.000000 cg-28.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-18 11:57:35.000000 cg-28.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-18 11:57:35.000000 cg-28.0.0/cg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14071 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/crud/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/crud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/crud/find.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/apps/cgstats/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/apps/cgstats/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/db/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/db/models/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/db/models/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/db/models/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/db/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/db/models/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/db/models/support_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/db/models/unaligned.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/db/models/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/demux_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/dragen_demux_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/parsers/adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/parsers/conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/parsers/demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/parsers/quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/parsers/run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/cgstats/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/coverage/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/crunchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/crunchy/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/crunchy/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/crunchy/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/demultiplex/demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/demultiplex/demux_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/apps/demultiplex/sample_sheet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/demultiplex/sample_sheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/demultiplex/sample_sheet/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/demultiplex/sample_sheet/dummy_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/demultiplex/sample_sheet/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/apps/hermes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/hermes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/hermes/hermes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/hermes/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/apps/housekeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/housekeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17462 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/housekeeper/hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/housekeeper/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/apps/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/invoice/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/apps/invoice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/invoice/templates/KI_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/invoice/templates/KI_sample_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/lims/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/lims/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/lims/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/lims/samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/loqus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/madeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/madeline/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/mip/confighandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/orderform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/orderform/excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/orderform/json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/orderform/orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/scout/scout_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/scout/scoutapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/slurm/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/slurm/slurm_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/apps/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/tb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/tb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/tb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-18 11:57:35.000000 cg-28.0.0/cg/apps/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/compress/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/compress/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/compress/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/delete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/delete/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/delete/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/delete/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/delete/observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/deliver/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/demultiplex/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/demultiplex/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/demultiplex/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/demultiplex/finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/demultiplex/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/demultiplex/sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/generate/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/generate/report/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/generate/report/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/generate/report/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/import_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/set/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/set/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/set/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/set/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/store/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/store/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/upload/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/upload/clinical_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/upload/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/upload/delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/upload/fohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/upload/genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/upload/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/upload/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/upload/nipt/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/upload/nipt/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/upload/nipt/statina.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/upload/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/upload/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/upload/observations/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/upload/observations/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/upload/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/upload/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/upload/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/upload/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/balsamic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/balsamic/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/balsamic/pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/balsamic/qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/balsamic/umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/fastq/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/fluffy/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/microsalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/microsalt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/mip/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/mip/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/workflow/mip_dna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/mip_dna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/mip_dna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/workflow/mip_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/mip_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/mip_rna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/workflow/mutant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/mutant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/mutant/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/workflow/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/nextflow/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/rnafusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/rnafusion/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/cli/workflow/tower/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/tower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-18 11:57:35.000000 cg-28.0.0/cg/cli/workflow/tower/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/cgstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/demultiplexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/gene_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/housekeeper_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/nextflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/orderforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/pdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/sample_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/scout_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/sequencing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-18 11:57:35.000000 cg-28.0.0/cg/constants/tb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-04-18 11:57:35.000000 cg-28.0.0/cg/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-18 11:57:35.000000 cg-28.0.0/cg/io/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-18 11:57:35.000000 cg-28.0.0/cg/io/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-18 11:57:35.000000 cg-28.0.0/cg/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-18 11:57:35.000000 cg-28.0.0/cg/io/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-18 11:57:35.000000 cg-28.0.0/cg/io/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/archive/ddn_dataflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18853 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/backup/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/backup/pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/clean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/clean/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14387 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/clean/demultiplexed_flow_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/clean/flow_cell_run_directories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/compress/compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/compress/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/deliver_ticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/demultiplex/delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/demultiplex/demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/demultiplex/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/encryption/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/observations/balsamic_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/observations/mip_dna_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/observations/observations_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/orders/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/orders/balsamic_qc_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/orders/balsamic_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/orders/balsamic_umi_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/orders/case_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/orders/fastq_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/orders/fluffy_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/orders/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/orders/metagenome_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/orders/microbial_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/orders/microsalt_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/orders/mip_dna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/orders/mip_rna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/orders/pool_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/orders/rml_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/orders/sars_cov_2_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/orders/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/orders/ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/report/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/report/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/report/field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/report/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17804 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/report/report_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/report/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/report/templates/balsamic_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/report/templates/bootstrap.html
+-rw-r--r--   0 runner    (1001) docker     (123)    77831 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/report/templates/mip-dna_report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/rsync/rsync_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/rsync/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/tar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/tar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/tar/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/transfer/external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/transfer/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/transfer/lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/balsamic/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/upload/fohm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/fohm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/fohm/fohm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/gisaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/gisaid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/gisaid/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/gisaid/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/upload/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/mip/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/mip/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/nipt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/nipt/nipt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/upload/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/rnafusion/rnafusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/scout/balsamic_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/scout/balsamic_umi_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/scout/hk_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/scout/mip_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/scout/rnafusion_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/scout/scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19581 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/scout/uploadscoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/upload/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19851 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/workflow/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28514 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/workflow/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/workflow/balsamic_pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/workflow/balsamic_qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/workflow/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/workflow/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/workflow/fluffy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18187 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/workflow/microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14337 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/workflow/mip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/workflow/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/workflow/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/workflow/mutant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/workflow/nextflow_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/workflow/prepare_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/workflow/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-18 11:57:35.000000 cg-28.0.0/cg/meta/workflow/tower_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/balsamic/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/balsamic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/balsamic/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12885 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/cg_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/models/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/cgstats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/cgstats/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/cgstats/stats_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/compression_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/models/deliverables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/deliverables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/deliverables/metric_deliverables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/models/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/demultiplex/demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/demultiplex/flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/demultiplex/run_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/file_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/models/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/invoice/invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/models/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/lims/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/mip/mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/mip/mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/mip/mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/mip/mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/nextflow/deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/nextflow/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/observations/input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/models/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/orders/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/orders/excel_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/orders/json_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/orders/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/orders/orderform_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/orders/sample_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/orders/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/report/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/report/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/report/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/rnafusion/rnafusion_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/models/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/scout/scout_load_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/models/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/slurm/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/models/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-18 11:57:35.000000 cg-28.0.0/cg/models/workflow/mutant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-04-18 11:57:35.000000 cg-28.0.0/cg/resources/20181012_Indices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-18 11:57:35.000000 cg-28.0.0/cg/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-18 11:57:35.000000 cg-28.0.0/cg/resources/rnafusion_bundle_filenames.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16689 2023-04-18 11:57:35.000000 cg-28.0.0/cg/server/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17974 2023-04-18 11:57:35.000000 cg-28.0.0/cg/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-04-18 11:57:35.000000 cg-28.0.0/cg/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-18 11:57:35.000000 cg-28.0.0/cg/server/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-18 11:57:35.000000 cg-28.0.0/cg/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-18 11:57:35.000000 cg-28.0.0/cg/server/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/server/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-18 11:57:35.000000 cg-28.0.0/cg/server/invoices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/server/invoices/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/server/invoices/templates/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-18 11:57:35.000000 cg-28.0.0/cg/server/invoices/templates/invoices/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-04-18 11:57:35.000000 cg-28.0.0/cg/server/invoices/templates/invoices/invoice.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-18 11:57:35.000000 cg-28.0.0/cg/server/invoices/templates/invoices/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-04-18 11:57:35.000000 cg-28.0.0/cg/server/invoices/templates/invoices/new.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-18 11:57:35.000000 cg-28.0.0/cg/server/invoices/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/server/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/server/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-18 11:57:35.000000 cg-28.0.0/cg/server/templates/admin/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/store/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/api/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/api/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/api/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9114 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/api/find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31073 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/api/find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12822 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/api/import_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39392 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/api/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/filters/status_analysis_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/filters/status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/filters/status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/filters/status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/filters/status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/filters/status_case_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/filters/status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/filters/status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/filters/status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/filters/status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/filters/status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/filters/status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/filters/status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/filters/status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/filters/status_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/filters/status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27648 2023-04-18 11:57:35.000000 cg-28.0.0/cg/store/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-18 11:57:35.000000 cg-28.0.0/cg/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/utils/checksum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/utils/checksum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-18 11:57:35.000000 cg-28.0.0/cg/utils/checksum/checksum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/utils/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-18 11:57:35.000000 cg-28.0.0/cg/utils/click/EnumChoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/utils/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-18 11:57:35.000000 cg-28.0.0/cg/utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-18 11:57:35.000000 cg-28.0.0/cg/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-18 11:57:35.000000 cg-28.0.0/cg/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-18 11:57:35.000000 cg-28.0.0/cg/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-18 11:57:35.000000 cg-28.0.0/cg/utils/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-18 11:57:35.000000 cg-28.0.0/cg/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-18 11:57:35.000000 cg-28.0.0/cg/utils/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg/utils/flask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/cg/utils/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-18 11:57:35.000000 cg-28.0.0/cg/utils/flask/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-18 11:57:35.000000 cg-28.0.0/cg/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-18 11:57:35.000000 cg-28.0.0/cg/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/cg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-18 11:57:46.000000 cg-28.0.0/cg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39356 2023-04-18 11:57:46.000000 cg-28.0.0/cg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 11:57:46.000000 cg-28.0.0/cg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-18 11:57:46.000000 cg-28.0.0/cg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 11:57:46.000000 cg-28.0.0/cg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-18 11:57:46.000000 cg-28.0.0/cg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-18 11:57:46.000000 cg-28.0.0/cg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-18 11:57:35.000000 cg-28.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-18 11:57:35.000000 cg-28.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 11:57:46.000000 cg-28.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-18 11:57:35.000000 cg-28.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/cgstats/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/cgstats/crud/test_create_novaseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/cgstats/crud/test_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/cgstats/parsers/test_adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/cgstats/parsers/test_conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/cgstats/parsers/test_demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/cgstats/parsers/test_quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/cgstats/parsers/test_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/cgstats/test_cgstats_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/cgstats/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/coverage/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/coverage/test_coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/crunchy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/crunchy/test_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/crunchy/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/crunchy/test_crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/crunchy/test_spring_decompression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/demultiplex/test_convert_to_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/demultiplex/test_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/demultiplex/test_parse_run_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/demultiplex/test_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/apps/gens/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/gens/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/gens/test_gens_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/gt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/gt/test_gt_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/apps/hk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/hk/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/hk/test__getattr__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/hk/test_add_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/hk/test_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/hk/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/hk/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/hk/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/lims/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/lims/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/apps/loqus/
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/loqus/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/loqus/test_loqusdb_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/madeline/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/madeline/test_madeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/mip/test_config_mip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/apps/mutacc_auto/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/mutacc_auto/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/mutacc_auto/test_mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/orderform/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/orderform/test_excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/orderform/test_excel_sample_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/orderform/test_json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/orderform/test_orderform_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/scout/test_get_causative_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/scout/test_get_scout_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/scout/test_scout_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/scout/test_scout_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/slurm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/slurm/test_slurm_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/test_apps_environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/test_osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/apps/vogue/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/vogue/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-18 11:57:35.000000 cg-28.0.0/tests/apps/vogue/test_vogue_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/add/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/add/test_cli_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/add/test_cli_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/add/test_cli_add_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/add/test_cli_add_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/add/test_cli_add_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/backup/test_backup_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/clean/test_balsamic_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/clean/test_clean_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/clean/test_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/clean/test_hk_case_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/clean/test_microbial_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/clean/test_rsync_past_run_dirs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/compress/test_cli_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/compress/test_cli_decompress_spring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/compress/test_compress_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/compress/test_store_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/delete/test_cli_delete_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/delete/test_cli_delete_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/deliver/test_deliver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/deliver/test_rsync_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/deliver/test_run_deliver_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/demultiplex/test_add_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/demultiplex/test_demultiplex_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/demultiplex/test_finish_demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/demultiplex/test_stats_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/demultiplex/test_validate_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/generate/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/generate/report/test_cli_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/generate/report/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/generate/test_cli_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/get/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/get/test_cli_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/get/test_cli_get_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/get/test_cli_get_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/get/test_cli_get_flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/get/test_cli_get_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/set/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/set/test_cli_set_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/set/test_cli_set_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/set/test_cli_set_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/set/test_cli_set_list_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/set/test_cli_set_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/set/test_cli_set_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/store/test_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/test_cli_status_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/upload/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/upload/test_cli_scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/upload/test_cli_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/upload/test_cli_upload_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/upload/test_cli_upload_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/upload/test_cli_upload_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/upload/test_cli_upload_genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/upload/test_cli_upload_gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/upload/test_cli_upload_nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/upload/test_cli_upload_nipt_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/upload/test_cli_upload_nipt_statina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/upload/test_cli_upload_observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/upload/test_cli_upload_vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)    30975 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/balsamic/test_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/balsamic/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/balsamic/test_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/balsamic/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/balsamic/test_store_housekeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/fastq/test_fastq_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/fluffy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/fluffy/test_cli_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/fluffy/test_cli_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/fluffy/test_cli_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/fluffy/test_cli_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/microsalt/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/workflow/microsalt/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/microsalt/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/microsalt/test_microsalt_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/microsalt/test_microsalt_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/mip/test_cli_mip_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/mip/test_cli_mip_dna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/mip/test_cli_mip_dna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/mip/test_cli_mip_dna_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/mip/test_cli_mip_rna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/mip/test_cli_mip_rna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/mip/test_cli_mip_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/rnafusion/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/test_cli_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-04-18 11:57:35.000000 cg-28.0.0/tests/cli/workflow/test_cli_workflow_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61338 2023-04-18 11:57:35.000000 cg-28.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/DEMUX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/analysis/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/analysis/balsamic/tn_wgs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/analysis/microsalt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
+-rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/analysis/mip/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/analysis/mip/dna/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/analysis/mip/dna/ADM2.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/analysis/mip/dna/ADM3.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/analysis/mip/dna/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/analysis/mip/dna/adm1.mt.bam
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/analysis/mip/dna/multiqc.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/analysis/mip/dna/report.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/analysis/mip/dna/smn.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/analysis/mip/dna/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/analysis/mip/dna/snv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/analysis/mip/dna/str.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/analysis/mip/dna/sv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/analysis/mip/dna/sv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/analysis/sample_coverage.bed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/balsamic/case/
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/balsamic/case/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/balsamic/case/metadata.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/balsamic/case/metadata_directory.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/crunchy/spring_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    53877 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/hiseq_run/
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/raw_lims_samples/
+-rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/fluffy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/fluffy/2020-23219-05/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/fluffy/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/fluffy/deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/fluffy/multiqc_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/fluffy/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/gt/yellowhog.bcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/madeline/madeline.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/mip/case_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/mip/dna/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/mip/dna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/mip/dna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/mip/rna/
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/mip/rna/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/mip/rna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/mip/rna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/mip/sample_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/scout/643594.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/scout/case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/scout/export_causatives.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/scout/none_case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/scout/other_sex_case.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/scout/panel_export.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/scout/panel_export.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/apps/shipping/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/apps/shipping/scout-deploy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/cgweb_orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/cgweb_orders/balsamic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/cgweb_orders/fastq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/cgweb_orders/metagenome.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/cgweb_orders/microsalt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/cgweb_orders/mip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/cgweb_orders/mip_rna.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/cgweb_orders/rml.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/cgweb_orders/sarscov2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/data/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/data/cgfixture.db
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/data/fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/data/hkstore.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/data/yellowhog/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/data/yellowhog/pedigree.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/io/example_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/io/example_json.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/orderforms/
+-rw-r--r--   0 runner    (1001) docker     (123)   267284 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/orderforms/1508.27.balsamic.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   258613 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   266876 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   266141 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/orderforms/1508.27.fastq.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   266967 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/orderforms/1508.27.mip.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   266759 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/orderforms/1508.27.mip_rna.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    95878 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/orderforms/1603.11.microbial.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   163548 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/orderforms/1604.15.rml.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    88463 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/orderforms/1605.10.metagenome.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   227684 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/orderforms/NIPT-json.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/report/case_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/report/lims_exported_samples.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/report/lims_family.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/store/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/fixtures/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/store/api/application_versions.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-04-18 11:57:35.000000 cg-28.0.0/tests/fixtures/store/api/applications.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-18 11:57:35.000000 cg-28.0.0/tests/io/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-04-18 11:57:35.000000 cg-28.0.0/tests/io/test_io_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-18 11:57:35.000000 cg-28.0.0/tests/io/test_io_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-18 11:57:35.000000 cg-28.0.0/tests/io/test_io_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-18 11:57:35.000000 cg-28.0.0/tests/io/test_io_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/archive/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/archive/test_archiving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24579 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/backup/test_meta_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/backup/test_meta_pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/clean/test_clean_demultiplexed_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/clean/test_clean_flow_cell_run_directories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/compress/test_clean_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/compress/test_compress_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/compress/test_compress_meta_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/compress/test_decompress_spring_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/compress/test_meta_compress_update_hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/meta/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/deliver/test_deliver_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/deliver/test_delivery_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13343 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/demultiplex/test_delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13707 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/demultiplex/test_demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/demultiplex/test_rename_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/encryption/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/encryption/test_encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/observations/test_meta_upload_observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/orders/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/orders/test_PoolSubmitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/orders/test_SarsCov2Submitter_store_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19702 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/orders/test_meta_orders_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/orders/test_meta_orders_lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29074 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/orders/test_meta_orders_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/orders/test_ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/report/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/report/test_balsamic_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/report/test_field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/report/test_mip_dna_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/report/test_report_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/rsync/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/rsync/test_rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/test_invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/transfer/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/transfer/test_external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/transfer/test_meta_transfer_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/transfer/test_meta_transfer_lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/balsamic/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/gisaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/gisaid/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/meta/upload/gisaid/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/gisaid/fixtures/four_samples.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/meta/upload/mutacc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/mutacc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/mutacc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/nipt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/nipt/test_nipt_upload_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23340 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/scout/test_generate_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/scout/test_meta_upload_scoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24928 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/scout/test_scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/test_meta_upload_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/test_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/test_upload_genotypes_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/meta/upload/vogue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/vogue/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/upload/vogue/test_upload_vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/workflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/workflow/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/workflow/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/workflow/test_microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-18 11:57:35.000000 cg-28.0.0/tests/meta/workflow/test_prepare_fastq_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-18 11:57:35.000000 cg-28.0.0/tests/mocks/balsamic_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-18 11:57:35.000000 cg-28.0.0/tests/mocks/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-04-18 11:57:35.000000 cg-28.0.0/tests/mocks/hk_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-18 11:57:35.000000 cg-28.0.0/tests/mocks/limsmock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-18 11:57:35.000000 cg-28.0.0/tests/mocks/madeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-18 11:57:35.000000 cg-28.0.0/tests/mocks/mip_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-18 11:57:35.000000 cg-28.0.0/tests/mocks/osticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-18 11:57:35.000000 cg-28.0.0/tests/mocks/process_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-18 11:57:35.000000 cg-28.0.0/tests/mocks/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-18 11:57:35.000000 cg-28.0.0/tests/mocks/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-18 11:57:35.000000 cg-28.0.0/tests/mocks/store_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-18 11:57:35.000000 cg-28.0.0/tests/mocks/tb_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/balsamic/test_balsamic_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/models/demultiplexing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/demultiplexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/demultiplexing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/demultiplexing/test_demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/demultiplexing/test_flowcell_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/mip/test_mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/mip/test_mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/mip/test_mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/mip/test_mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/nextflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/nextflow/test_nextflow_deliver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/observations/test_observations_input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/report/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/rnafusion/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/rnafusion/test_rnafusion_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/test_cg_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/test_compression_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/test_file_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-18 11:57:35.000000 cg-28.0.0/tests/models/test_flowcell_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-18 11:57:35.000000 cg-28.0.0/tests/server/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-18 11:57:35.000000 cg-28.0.0/tests/server/test_server_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-18 11:57:35.000000 cg-28.0.0/tests/server/test_server_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-18 11:57:35.000000 cg-28.0.0/tests/small_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/store/api/add/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/add/test_store_add_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/add/test_store_add_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/add/test_store_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/add/test_store_add_flow_celll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22499 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/store/api/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/delete/test_store_api_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/store/api/find/
+-rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/find/test_find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/find/test_find_basic_data_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28769 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/find/test_find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/find/test_find_business_data_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/find/test_find_business_data_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/find/test_find_business_data_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/store/api/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/status/test_analyses_to_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/status/test_analyses_to_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/status/test_store_api_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15264 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/status/test_store_api_status_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54207 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/status/test_store_api_status_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/status/test_store_api_status_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/status/test_store_api_status_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/status/test_store_api_status_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/api/test_store_import_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16784 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/filters/test_status_analyses_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/filters/test_status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/filters/test_status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/filters/test_status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/filters/test_status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/filters/test_status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39472 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/filters/test_status_cases_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/filters/test_status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/filters/test_status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/filters/test_status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/filters/test_status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/filters/test_status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/filters/test_status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/filters/test_status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26900 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/filters/test_status_samples_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/filters/test_status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/test_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store/test_store_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29715 2023-04-18 11:57:35.000000 cg-28.0.0/tests/store_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-18 11:57:35.000000 cg-28.0.0/tests/test_store_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:46.000000 cg-28.0.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:57:35.000000 cg-28.0.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-18 11:57:35.000000 cg-28.0.0/tests/utils/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-18 11:57:35.000000 cg-28.0.0/tests/utils/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-18 11:57:35.000000 cg-28.0.0/tests/utils/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-18 11:57:35.000000 cg-28.0.0/tests/utils/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-04-18 11:57:35.000000 cg-28.0.0/tests/utils/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-18 11:57:35.000000 cg-28.0.0/tests/utils/test_utils.py
```

### Comparing `cg-27.3.9/PKG-INFO` & `cg-28.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 27.3.9
+Version: 28.0.0
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-27.3.9/README.md` & `cg-28.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/cgstats/crud/create.py` & `cg-28.0.0/cg/apps/cgstats/crud/create.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/cgstats/crud/delete.py` & `cg-28.0.0/cg/apps/cgstats/crud/delete.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/cgstats/crud/find.py` & `cg-28.0.0/cg/apps/cgstats/crud/find.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/cgstats/db/models/base.py` & `cg-28.0.0/cg/apps/cgstats/db/models/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/cgstats/db/models/datasource.py` & `cg-28.0.0/cg/apps/cgstats/db/models/datasource.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/cgstats/db/models/demux.py` & `cg-28.0.0/cg/apps/cgstats/db/models/demux.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/cgstats/db/models/flowcell.py` & `cg-28.0.0/cg/apps/cgstats/db/models/flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/cgstats/db/models/project.py` & `cg-28.0.0/cg/apps/cgstats/db/models/project.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/cgstats/db/models/sample.py` & `cg-28.0.0/cg/apps/cgstats/db/models/sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/cgstats/db/models/support_params.py` & `cg-28.0.0/cg/apps/cgstats/db/models/support_params.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/cgstats/db/models/unaligned.py` & `cg-28.0.0/cg/apps/cgstats/db/models/unaligned.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/cgstats/db/models/version.py` & `cg-28.0.0/cg/apps/cgstats/db/models/version.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/cgstats/demux_sample.py` & `cg-28.0.0/cg/apps/cgstats/demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/cgstats/dragen_demux_sample.py` & `cg-28.0.0/cg/apps/cgstats/dragen_demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/cgstats/parsers/adapter_metrics.py` & `cg-28.0.0/cg/apps/cgstats/parsers/adapter_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/cgstats/parsers/conversion_stats.py` & `cg-28.0.0/cg/apps/cgstats/parsers/conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/cgstats/parsers/demux_stats.py` & `cg-28.0.0/cg/apps/cgstats/parsers/demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py` & `cg-28.0.0/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/cgstats/parsers/quality_metrics.py` & `cg-28.0.0/cg/apps/cgstats/parsers/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/cgstats/parsers/run_info.py` & `cg-28.0.0/cg/apps/cgstats/parsers/run_info.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/cgstats/stats.py` & `cg-28.0.0/cg/apps/cgstats/stats.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/coverage/api.py` & `cg-28.0.0/cg/apps/coverage/api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/crunchy/crunchy.py` & `cg-28.0.0/cg/apps/crunchy/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/crunchy/files.py` & `cg-28.0.0/cg/apps/crunchy/files.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/crunchy/sbatch.py` & `cg-28.0.0/cg/apps/crunchy/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/demultiplex/demultiplex_api.py` & `cg-28.0.0/cg/apps/demultiplex/demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/demultiplex/demux_report.py` & `cg-28.0.0/cg/apps/demultiplex/demux_report.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/demultiplex/sample_sheet/create.py` & `cg-28.0.0/cg/apps/demultiplex/sample_sheet/create.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/demultiplex/sample_sheet/dummy_sample.py` & `cg-28.0.0/cg/apps/demultiplex/sample_sheet/dummy_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/demultiplex/sample_sheet/index.py` & `cg-28.0.0/cg/apps/demultiplex/sample_sheet/index.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py` & `cg-28.0.0/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/demultiplex/sbatch.py` & `cg-28.0.0/cg/apps/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/gens.py` & `cg-28.0.0/cg/apps/gens.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/gt.py` & `cg-28.0.0/cg/apps/gt.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/hermes/hermes_api.py` & `cg-28.0.0/cg/apps/hermes/hermes_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/hermes/models.py` & `cg-28.0.0/cg/apps/hermes/models.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/housekeeper/hk.py` & `cg-28.0.0/cg/apps/housekeeper/hk.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/invoice/render.py` & `cg-28.0.0/cg/apps/invoice/render.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/invoice/templates/KI_pool_invoice.xlsx` & `cg-28.0.0/cg/apps/invoice/templates/KI_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/invoice/templates/KI_sample_invoice.xlsx` & `cg-28.0.0/cg/apps/invoice/templates/KI_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/invoice/templates/KTH_pool_invoice.xlsx` & `cg-28.0.0/cg/apps/invoice/templates/KTH_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/invoice/templates/KTH_sample_invoice.xlsx` & `cg-28.0.0/cg/apps/invoice/templates/KTH_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/lims/api.py` & `cg-28.0.0/cg/apps/lims/api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/lims/batch.py` & `cg-28.0.0/cg/apps/lims/batch.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/lims/order.py` & `cg-28.0.0/cg/apps/lims/order.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/lims/samplesheet.py` & `cg-28.0.0/cg/apps/lims/samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/loqus.py` & `cg-28.0.0/cg/apps/loqus.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/madeline/api.py` & `cg-28.0.0/cg/apps/madeline/api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/mip/confighandler.py` & `cg-28.0.0/cg/apps/mip/confighandler.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/mutacc_auto.py` & `cg-28.0.0/cg/apps/mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/orderform/excel_orderform_parser.py` & `cg-28.0.0/cg/apps/orderform/excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/orderform/json_orderform_parser.py` & `cg-28.0.0/cg/apps/orderform/json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/orderform/orderform_parser.py` & `cg-28.0.0/cg/apps/orderform/orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/osticket.py` & `cg-28.0.0/cg/apps/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/scout/scout_export.py` & `cg-28.0.0/cg/apps/scout/scout_export.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/scout/scoutapi.py` & `cg-28.0.0/cg/apps/scout/scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/slurm/sbatch.py` & `cg-28.0.0/cg/apps/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/slurm/slurm_api.py` & `cg-28.0.0/cg/apps/slurm/slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/tb/api.py` & `cg-28.0.0/cg/apps/tb/api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/tb/models.py` & `cg-28.0.0/cg/apps/tb/models.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/apps/vogue.py` & `cg-28.0.0/cg/apps/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/add.py` & `cg-28.0.0/cg/cli/add.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/backup.py` & `cg-28.0.0/cg/cli/backup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         root_dir=context.backup.root.dict(),
         dry_run=dry_run,
     )
     backup_api: BackupAPI = context.meta_apis["backup_api"]
 
     status_api: Store = context.status_db
     flow_cell: Optional[Flowcell] = (
-        status_api.get_flow_cell(flow_cell_id=flow_cell_id) if flow_cell_id else None
+        status_api.get_flow_cell_by_name(flow_cell_name=flow_cell_id) if flow_cell_id else None
     )
 
     if not flow_cell and flow_cell_id:
         LOG.error(f"{flow_cell_id}: not found in database")
         raise click.Abort
 
     if not flow_cell_id:
```

### Comparing `cg-27.3.9/cg/cli/base.py` & `cg-28.0.0/cg/cli/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/clean.py` & `cg-28.0.0/cg/cli/clean.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,18 +333,16 @@
 @DRY_RUN
 @click.pass_obj
 def fix_flow_cell_status(context: CGConfig, dry_run: bool):
     """Set correct flow cell statuses in Statusdb."""
     status_db: Store = context.status_db
     housekeeper_api: HousekeeperAPI = context.housekeeper_api
 
-    flow_cells_in_statusdb: List[Flowcell] = list(
-        status_db.get_flow_cells_by_statuses(
-            flow_cell_statuses=[FlowCellStatus.ON_DISK, FlowCellStatus.REMOVED]
-        )
+    flow_cells_in_statusdb: List[Flowcell] = status_db.get_flow_cells_by_statuses(
+        flow_cell_statuses=[FlowCellStatus.ON_DISK, FlowCellStatus.REMOVED]
     )
 
     LOG.info(
         f"Number of flow cells with status {FlowCellStatus.ON_DISK.value} or {FlowCellStatus.REMOVED} in Statusdb: {len(flow_cells_in_statusdb)}"
     )
 
     for flow_cell in flow_cells_in_statusdb:
```

### Comparing `cg-27.3.9/cg/cli/compress/base.py` & `cg-28.0.0/cg/cli/compress/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/compress/fastq.py` & `cg-28.0.0/cg/cli/compress/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/compress/helpers.py` & `cg-28.0.0/cg/cli/compress/helpers.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/delete/case.py` & `cg-28.0.0/cg/cli/delete/case.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/delete/cases.py` & `cg-28.0.0/cg/cli/delete/cases.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/delete/observations.py` & `cg-28.0.0/cg/cli/delete/observations.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/deliver/base.py` & `cg-28.0.0/cg/cli/deliver/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/demultiplex/add.py` & `cg-28.0.0/cg/cli/demultiplex/add.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/demultiplex/base.py` & `cg-28.0.0/cg/cli/demultiplex/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/demultiplex/demux.py` & `cg-28.0.0/cg/cli/demultiplex/demux.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/demultiplex/finish.py` & `cg-28.0.0/cg/cli/demultiplex/finish.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/demultiplex/report.py` & `cg-28.0.0/cg/cli/demultiplex/report.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/demultiplex/sample_sheet.py` & `cg-28.0.0/cg/cli/demultiplex/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/export.py` & `cg-28.0.0/cg/cli/export.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/generate/report/base.py` & `cg-28.0.0/cg/cli/generate/report/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/generate/report/options.py` & `cg-28.0.0/cg/cli/generate/report/options.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/generate/report/utils.py` & `cg-28.0.0/cg/cli/generate/report/utils.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/get.py` & `cg-28.0.0/cg/cli/get.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 @get.command("flow-cell")
 @click.option("--samples/--no-samples", default=True, help="Display related samples")
 @click.argument("flow-cell-id")
 @click.pass_context
 def flow_cell(context: click.Context, samples: bool, flow_cell_id: str):
     """Get information about a flow cell and the samples on it."""
     status_db: Store = context.obj.status_db
-    existing_flow_cell: Flowcell = status_db.get_flow_cell(flow_cell_id=flow_cell_id)
+    existing_flow_cell: Flowcell = status_db.get_flow_cell_by_name(flow_cell_name=flow_cell_id)
     if not existing_flow_cell:
         LOG.error(f"{flow_cell_id}: flow cell not found")
         raise click.Abort
     row: List[str] = [
         existing_flow_cell.name,
         existing_flow_cell.sequencer_type,
         existing_flow_cell.sequencer_name,
```

### Comparing `cg-27.3.9/cg/cli/import_cmd.py` & `cg-28.0.0/cg/cli/import_cmd.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/set/base.py` & `cg-28.0.0/cg/cli/set/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Set data in the status database and LIMS."""
 import datetime
 import getpass
 import logging
 from typing import Iterable, List, Optional
 
 import click
-from cg.cli.set.families import families
-from cg.cli.set.family import family
+from cg.cli.set.cases import cases
+from cg.cli.set.case import case
 from cg.constants import FLOWCELL_STATUS
 from cg.exc import LimsDataError
 from cg.models.cg_config import CGConfig
 from cg.store import Store
 from cg.store.models import Sample, Customer, ApplicationVersion, Flowcell
 
 CONFIRM = "Continue?"
@@ -279,26 +279,26 @@
             obj.comment = f"{timestamp}-{getpass.getuser()}: {comment}"
         else:
             obj.comment = f"{timestamp}-{getpass.getuser()}: {comment}" + "\n" + obj.comment
 
 
 @set_cmd.command()
 @click.option("-s", "--status", type=click.Choice(FLOWCELL_STATUS))
-@click.argument("flowcell_name")
+@click.argument("flow_cell_name")
 @click.pass_obj
-def flowcell(context: CGConfig, flowcell_name: str, status: Optional[str]):
+def flowcell(context: CGConfig, flow_cell_name: str, status: Optional[str]):
     """Update information about a flow cell."""
     status_db: Store = context.status_db
-    flowcell_obj: Flowcell = status_db.get_flow_cell(flowcell_name)
+    flowcell_obj: Flowcell = status_db.get_flow_cell_by_name(flow_cell_name=flow_cell_name)
 
     if flowcell_obj is None:
-        LOG.warning(f"flow cell not found: {flowcell_name}")
+        LOG.warning(f"flow cell not found: {flow_cell_name}")
         raise click.Abort
     prev_status: str = flowcell_obj.status
     flowcell_obj.status = status
 
     status_db.commit()
-    LOG.info(f"{flowcell_name} set: {prev_status} -> {status}")
+    LOG.info(f"{flow_cell_name} set: {prev_status} -> {status}")
 
 
-set_cmd.add_command(family)
-set_cmd.add_command(families)
+set_cmd.add_command(case)
+set_cmd.add_command(cases)
```

### Comparing `cg-27.3.9/cg/cli/set/families.py` & `cg-28.0.0/cg/cli/set/cases.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import logging
 from typing import List, Optional, Set, Tuple
 
 import click
-from cg.constants import CASE_ACTIONS
+from cg.constants import CASE_ACTIONS, Priority
+from cg.cli.set.case import case
 from cg.store import Store
 from cg.store.models import Family, Sample
-
-from .family import family
-from ...constants import Priority
-from ...utils.click.EnumChoice import EnumChoice
+from cg.utils.click.EnumChoice import EnumChoice
 
 CONFIRM = "Continue?"
 
 LOG = logging.getLogger(__name__)
 
 
 def _get_samples_by_identifiers(identifiers: click.Tuple([str, str]), store: Store) -> List[Sample]:
@@ -38,47 +36,47 @@
     "identifiers",
     nargs=2,
     type=click.Tuple([str, str]),
     multiple=True,
     help="Give an identifier on sample and the value to use it with, e.g. --sample-identifier "
     "name Prov52",
 )
-@click.option("-a", "--action", type=click.Choice(CASE_ACTIONS), help="update family action")
+@click.option("-a", "--action", type=click.Choice(CASE_ACTIONS), help="update case action")
 @click.option("-c", "--customer-id", type=click.STRING, help="update customer")
 @click.option("-g", "--panel", "panel_abbreviations", multiple=True, help="update gene panels")
 @click.option(
     "-p", "--priority", type=EnumChoice(Priority, use_value=False), help="update priority"
 )
 @click.pass_context
-def families(
+def cases(
     context: click.Context,
     action: Optional[str],
     priority: Optional[Priority],
     panel_abbreviations: Optional[Tuple[str]],
     customer_id: Optional[str],
     identifiers: click.Tuple([str, str]),
 ):
     """Set values on many families at the same time"""
     store: Store = context.obj.status_db
-    cases: List[Family] = _get_cases(identifiers, store)
+    cases_to_alter: List[Family] = _get_cases(identifiers, store)
 
-    if not cases:
+    if not cases_to_alter:
         LOG.error("No cases to alter!")
         raise click.Abort
 
     LOG.info("Would alter cases:")
 
-    for case in cases:
-        LOG.info(case)
+    for case_to_alter in cases_to_alter:
+        LOG.info(case_to_alter)
 
     if not (click.confirm(CONFIRM)):
         raise click.Abort
 
-    for case in cases:
+    for case_to_alter in cases_to_alter:
         context.invoke(
-            family,
+            case,
             action=action,
             priority=priority,
             panel_abbreviations=panel_abbreviations,
-            family_id=case.internal_id,
+            case_id=case_to_alter.internal_id,
             customer_id=customer_id,
         )
```

### Comparing `cg-27.3.9/cg/cli/set/family.py` & `cg-28.0.0/cg/cli/set/case.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,24 +31,24 @@
     type=EnumChoice(DataDelivery),
     help="Update case data delivery",
 )
 @click.option("-g", "--panel", "panel_abbreviations", multiple=True, help="update gene panels")
 @click.option(
     "-p", "--priority", type=EnumChoice(Priority, use_value=False), help="update priority"
 )
-@click.argument("family_id")
+@click.argument("case_id")
 @click.pass_obj
-def family(
+def case(
     context: CGConfig,
     action: Optional[str],
     data_analysis: Optional[Pipeline],
     data_delivery: Optional[DataDelivery],
     priority: Optional[Priority],
     panel_abbreviations: Optional[Tuple[str]],
-    family_id: str,
+    case_id: str,
     customer_id: Optional[str],
 ):
     """Update information about a case."""
 
     options: List[str] = [
         action,
         panel_abbreviations,
@@ -56,15 +56,15 @@
         customer_id,
         data_analysis,
         data_delivery,
     ]
     abort_on_empty_options(options=options)
 
     status_db: Store = context.status_db
-    case: Family = get_case(family_id, status_db)
+    case: Family = get_case(case_id=case_id, status_db=status_db)
 
     if action:
         update_action(case=case, action=action)
 
     if customer_id:
         update_customer(case=case, customer_id=customer_id, status_db=status_db)
```

### Comparing `cg-27.3.9/cg/cli/status.py` & `cg-28.0.0/cg/cli/status.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/store/fastq.py` & `cg-28.0.0/cg/cli/store/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/store/store.py` & `cg-28.0.0/cg/cli/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/transfer.py` & `cg-28.0.0/cg/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/upload/base.py` & `cg-28.0.0/cg/cli/upload/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/upload/clinical_delivery.py` & `cg-28.0.0/cg/cli/upload/clinical_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/upload/coverage.py` & `cg-28.0.0/cg/cli/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/upload/delivery_report.py` & `cg-28.0.0/cg/cli/upload/delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/upload/fohm.py` & `cg-28.0.0/cg/cli/upload/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/upload/genotype.py` & `cg-28.0.0/cg/cli/upload/genotype.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/upload/gens.py` & `cg-28.0.0/cg/cli/upload/gens.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/upload/gisaid.py` & `cg-28.0.0/cg/cli/upload/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/upload/mutacc.py` & `cg-28.0.0/cg/cli/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/upload/nipt/base.py` & `cg-28.0.0/cg/cli/upload/nipt/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/upload/nipt/ftp.py` & `cg-28.0.0/cg/cli/upload/nipt/ftp.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/upload/nipt/statina.py` & `cg-28.0.0/cg/cli/upload/nipt/statina.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/upload/observations/observations.py` & `cg-28.0.0/cg/cli/upload/observations/observations.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/upload/observations/utils.py` & `cg-28.0.0/cg/cli/upload/observations/utils.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/upload/scout.py` & `cg-28.0.0/cg/cli/upload/scout.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/upload/utils.py` & `cg-28.0.0/cg/cli/upload/utils.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/upload/validate.py` & `cg-28.0.0/cg/cli/upload/validate.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/upload/vogue.py` & `cg-28.0.0/cg/cli/upload/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/workflow/balsamic/base.py` & `cg-28.0.0/cg/cli/workflow/balsamic/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/workflow/balsamic/options.py` & `cg-28.0.0/cg/cli/workflow/balsamic/options.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/workflow/balsamic/pon.py` & `cg-28.0.0/cg/cli/workflow/balsamic/pon.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/workflow/balsamic/qc.py` & `cg-28.0.0/cg/cli/workflow/balsamic/qc.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/workflow/balsamic/umi.py` & `cg-28.0.0/cg/cli/workflow/balsamic/umi.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/workflow/base.py` & `cg-28.0.0/cg/cli/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/workflow/commands.py` & `cg-28.0.0/cg/cli/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/workflow/fastq/base.py` & `cg-28.0.0/cg/cli/workflow/fastq/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/workflow/fluffy/base.py` & `cg-28.0.0/cg/cli/workflow/fluffy/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/workflow/microsalt/base.py` & `cg-28.0.0/cg/cli/workflow/microsalt/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/workflow/mip/base.py` & `cg-28.0.0/cg/cli/workflow/mip/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/workflow/mip/options.py` & `cg-28.0.0/cg/cli/workflow/mip/options.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/workflow/mip_dna/base.py` & `cg-28.0.0/cg/cli/workflow/mip_dna/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/workflow/mip_rna/base.py` & `cg-28.0.0/cg/cli/workflow/mip_rna/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/workflow/mutant/base.py` & `cg-28.0.0/cg/cli/workflow/mutant/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/workflow/nextflow/options.py` & `cg-28.0.0/cg/cli/workflow/nextflow/options.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/workflow/rnafusion/base.py` & `cg-28.0.0/cg/cli/workflow/rnafusion/base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/cli/workflow/rnafusion/options.py` & `cg-28.0.0/cg/cli/workflow/rnafusion/options.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/constants/__init__.py` & `cg-28.0.0/cg/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/constants/compression.py` & `cg-28.0.0/cg/constants/compression.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/constants/constants.py` & `cg-28.0.0/cg/constants/constants.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/constants/delivery.py` & `cg-28.0.0/cg/constants/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/constants/demultiplexing.py` & `cg-28.0.0/cg/constants/demultiplexing.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/constants/encryption.py` & `cg-28.0.0/cg/constants/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/constants/gene_panel.py` & `cg-28.0.0/cg/constants/gene_panel.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/constants/housekeeper_tags.py` & `cg-28.0.0/cg/constants/housekeeper_tags.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/constants/lims.py` & `cg-28.0.0/cg/constants/lims.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/constants/nextflow.py` & `cg-28.0.0/cg/constants/nextflow.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/constants/observations.py` & `cg-28.0.0/cg/constants/observations.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/constants/orderforms.py` & `cg-28.0.0/cg/constants/orderforms.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/constants/priority.py` & `cg-28.0.0/cg/constants/priority.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/constants/report.py` & `cg-28.0.0/cg/constants/report.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/constants/rnafusion.py` & `cg-28.0.0/cg/constants/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/constants/scout_upload.py` & `cg-28.0.0/cg/constants/scout_upload.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/constants/sequencing.py` & `cg-28.0.0/cg/constants/sequencing.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/constants/subject.py` & `cg-28.0.0/cg/constants/subject.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/exc.py` & `cg-28.0.0/cg/exc.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/io/api.py` & `cg-28.0.0/cg/io/api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/io/controller.py` & `cg-28.0.0/cg/io/controller.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/io/csv.py` & `cg-28.0.0/cg/io/csv.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/io/json.py` & `cg-28.0.0/cg/io/json.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/io/yaml.py` & `cg-28.0.0/cg/io/yaml.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/archive/ddn_dataflow.py` & `cg-28.0.0/cg/meta/archive/ddn_dataflow.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/backup/backup.py` & `cg-28.0.0/cg/meta/backup/backup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,26 +46,26 @@
         self.tar_api: TarAPI = tar_api
         self.pdc: PdcAPI = pdc_api
         self.root_dir: dict = root_dir
         self.dry_run: bool = dry_run
 
     def check_processing(self) -> bool:
         """Check if the processing queue for flow cells is not full."""
-        processing_flow_cells_count: int = self.status.get_flow_cells_by_statuses(
-            flow_cell_statuses=[FlowCellStatus.PROCESSING]
-        ).count()
+        processing_flow_cells_count: int = len(
+            self.status.get_flow_cells_by_statuses(flow_cell_statuses=[FlowCellStatus.PROCESSING])
+        )
         LOG.debug(f"Processing flow cells: {processing_flow_cells_count}")
         return processing_flow_cells_count < MAX_PROCESSING_FLOW_CELLS
 
     def get_first_flow_cell(self) -> Optional[Flowcell]:
         """Get the first flow cell from the requested queue."""
         flow_cell: Optional[Flowcell] = self.status.get_flow_cells_by_statuses(
             flow_cell_statuses=[FlowCellStatus.REQUESTED]
-        ).first()
-        return flow_cell or None
+        )
+        return flow_cell[0] if flow_cell else None
 
     def fetch_flow_cell(self, flow_cell: Optional[Flowcell] = None) -> Optional[float]:
         """Start fetching a flow cell from backup if possible.
 
         1. The processing queue is not full.
         2. The requested queue is not emtpy.
         """
```

### Comparing `cg-27.3.9/cg/meta/backup/pdc.py` & `cg-28.0.0/cg/meta/backup/pdc.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/clean/api.py` & `cg-28.0.0/cg/meta/clean/api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/clean/demultiplexed_flow_cells.py` & `cg-28.0.0/cg/meta/clean/demultiplexed_flow_cells.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,17 @@
                 LOG.warning(f"Flow cell not correctly named!: {self.path}")
         return self._is_correctly_named
 
     @property
     def exists_in_statusdb(self) -> bool:
         """Checks if flow cell exists in Statusdb."""
         if self._exists_in_statusdb is None:
-            self._exists_in_statusdb: bool = self.status_db.get_flow_cell(self.id) is not None
+            self._exists_in_statusdb: bool = (
+                self.status_db.get_flow_cell_by_name(flow_cell_name=self.id) is not None
+            )
             if not self._exists_in_statusdb:
                 LOG.warning(f"Flow cell {self.id} does not exist in Statusdb!")
         return self._exists_in_statusdb
 
     @property
     def fastq_files_exist_in_housekeeper(self) -> bool:
         """Checks if the flow cell has any FASTQ files in Housekeeper."""
@@ -235,15 +237,17 @@
 
     def remove_from_demultiplexed_runs(self) -> None:
         """Removes a flow cell directory completely from demultiplexed-runs."""
         if self.is_correctly_named:
             self.archive_sample_sheet()
         shutil.rmtree(self.path, ignore_errors=True)
         if self.exists_in_statusdb and self.is_correctly_named:
-            self.status_db.get_flow_cell(self.id).status = FlowCellStatus.REMOVED
+            self.status_db.get_flow_cell_by_name(
+                flow_cell_name=self.id
+            ).status = FlowCellStatus.REMOVED
         self.status_db.commit()
 
     def remove_failed_flow_cell(self) -> None:
         """Performs the two removal actions for failed flow cells."""
         self.remove_from_demultiplexed_runs()
         if self.files_exist_in_housekeeper and self.is_correctly_named:
             self.remove_files_from_housekeeper()
```

### Comparing `cg-27.3.9/cg/meta/clean/flow_cell_run_directories.py` & `cg-28.0.0/cg/meta/clean/flow_cell_run_directories.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             self._age: int = (get_timedelta_from_date(date=self.sequenced_date)).days
         return self._age
 
     @property
     def sequenced_date(self) -> datetime:
         """The date on which the flow cell was sequenced."""
         if self._sequenced_date is None:
-            flow_cell: Flowcell = self.status_db.get_flow_cell(flow_cell_id=self.id)
+            flow_cell: Flowcell = self.status_db.get_flow_cell_by_name(flow_cell_name=self.id)
             if flow_cell:
                 LOG.info(f"Found flow cell {self.id} in Statusdb, getting sequenced date.")
                 self._sequenced_date: datetime = flow_cell.sequenced_at
             else:
                 LOG.info(
                     f"Flow cell {self.id} NOT found in Statusdb, deriving sequenced date from run dir name!"
                 )
@@ -73,23 +73,25 @@
             self._is_retrieved_from_pdc = self.flow_cell_status in PDC_RETRIEVAL_STATUSES
         return self._is_retrieved_from_pdc
 
     @property
     def flow_cell_status(self) -> str:
         """Return status of the flow cell."""
         if self._flow_cell_status is None:
-            self._flow_cell_status = self.status_db.get_flow_cell(flow_cell_id=self.id).status
+            self._flow_cell_status = self.status_db.get_flow_cell_by_name(
+                flow_cell_name=self.id
+            ).status
         return self._flow_cell_status
 
     @property
     def exists_in_statusdb(self) -> bool:
         """The flow cell exists in Statusdb."""
         if self._exists_in_statusdb is None:
             self._exists_in_statusdb = (
-                self.status_db.get_flow_cell(flow_cell_id=self.id) is not None
+                self.status_db.get_flow_cell_by_name(flow_cell_name=self.id) is not None
             )
         return self._exists_in_statusdb
 
     def remove_run_directory(self) -> None:
         """Removes the flow cell run directory."""
         LOG.info(f"Removing run directory {self.flow_cell_dir}")
         shutil.rmtree(self.flow_cell_dir, ignore_errors=True)
```

### Comparing `cg-27.3.9/cg/meta/compress/compress.py` & `cg-28.0.0/cg/meta/compress/compress.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/compress/files.py` & `cg-28.0.0/cg/meta/compress/files.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/deliver.py` & `cg-28.0.0/cg/meta/deliver.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/deliver_ticket.py` & `cg-28.0.0/cg/meta/deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/demultiplex/delete_demultiplex_api.py` & `cg-28.0.0/cg/meta/demultiplex/delete_demultiplex_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,32 +45,26 @@
         Example: 201203_A00689_0200_AHVKJCDRXX
         """
         return self.run_path.name.split("_")[-1][1:]
 
     @property
     def status_db_presence(self) -> bool:
         """Update about the presence of given flow cell in status_db"""
-        return bool(
-            self.status_db.query(Flowcell).filter(Flowcell.name == self.flow_cell_name).first()
-        )
+        return bool(self.status_db.get_flow_cell_by_name(flow_cell_name=self.flow_cell_name))
 
     @staticmethod
     def set_dry_run(dry_run: bool) -> bool:
         """Set dry run flag for API"""
         log.debug(f"DeleteDemuxAPI: Setting dry run mode to {dry_run}")
         return dry_run
 
     def _set_samples_on_flow_cell(self) -> None:
         """Set a list of samples related to a flow cell in status-db"""
-        self.samples_on_flow_cell: List[Sample] = (
-            self.status_db.query(Flowcell)
-            .filter(Flowcell.name == self.flow_cell_name)
-            .first()
-            .samples
-        )
+        flow_cell = self.status_db.get_flow_cell_by_name(flow_cell_name=self.flow_cell_name)
+        self.samples_on_flow_cell: List[Sample] = flow_cell.samples
 
     def active_samples_on_flow_cell(self) -> Optional[List[str]]:
         """Check if there are any active cases related to samples of a flow cell"""
         active_samples_on_flow_cell: List[str] = [
             sample.internal_id
             for sample in self.samples_on_flow_cell
             if self.status_db.has_active_cases_for_sample(internal_id=sample.internal_id)
@@ -168,15 +162,17 @@
         if self.dry_run:
             log.info(
                 f"DeleteDemuxAPI-Hasta: Would have removed the following directory: {self.demultiplexing_path}\n"
                 f"DeleteDemuxAPI-Hasta: Would have removed the following directory: {self.run_path}"
             )
             return
         if demultiplexing_dir and run_dir and self.status_db_presence:
-            flow_cell_obj: Flowcell = self.status_db.get_flow_cell(self.flow_cell_name)
+            flow_cell_obj: Flowcell = self.status_db.get_flow_cell_by_name(
+                flow_cell_name=self.flow_cell_name
+            )
             flow_cell_obj.status = "removed"
             self.status_db.commit()
         if demultiplexing_dir and self.demultiplexing_path.exists():
             self._delete_demultiplexing_dir_hasta()
         else:
             log.info(
                 f"DeleteDemuxAPI-Hasta: Skipped demultiplexing directory, or no target: {self.demultiplexing_dir}"
```

### Comparing `cg-27.3.9/cg/meta/demultiplex/demux_post_processing.py` & `cg-28.0.0/cg/meta/demultiplex/demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/demultiplex/files.py` & `cg-28.0.0/cg/meta/demultiplex/files.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/encryption/encryption.py` & `cg-28.0.0/cg/meta/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/invoice.py` & `cg-28.0.0/cg/meta/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/meta.py` & `cg-28.0.0/cg/meta/meta.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/observations/balsamic_observations_api.py` & `cg-28.0.0/cg/meta/observations/balsamic_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/observations/mip_dna_observations_api.py` & `cg-28.0.0/cg/meta/observations/mip_dna_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/observations/observations_api.py` & `cg-28.0.0/cg/meta/observations/observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/orders/api.py` & `cg-28.0.0/cg/meta/orders/api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/orders/case_submitter.py` & `cg-28.0.0/cg/meta/orders/case_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/orders/fastq_submitter.py` & `cg-28.0.0/cg/meta/orders/fastq_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/orders/lims.py` & `cg-28.0.0/cg/meta/orders/lims.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/orders/metagenome_submitter.py` & `cg-28.0.0/cg/meta/orders/metagenome_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/orders/microbial_submitter.py` & `cg-28.0.0/cg/meta/orders/microbial_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/orders/pool_submitter.py` & `cg-28.0.0/cg/meta/orders/pool_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/orders/sars_cov_2_submitter.py` & `cg-28.0.0/cg/meta/orders/sars_cov_2_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/orders/submitter.py` & `cg-28.0.0/cg/meta/orders/submitter.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/orders/ticket_handler.py` & `cg-28.0.0/cg/meta/orders/ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/report/balsamic.py` & `cg-28.0.0/cg/meta/report/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/report/balsamic_umi.py` & `cg-28.0.0/cg/meta/report/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/report/field_validators.py` & `cg-28.0.0/cg/meta/report/field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/report/mip_dna.py` & `cg-28.0.0/cg/meta/report/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/report/report_api.py` & `cg-28.0.0/cg/meta/report/report_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/report/templates/balsamic_report.html` & `cg-28.0.0/cg/meta/report/templates/balsamic_report.html`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/report/templates/bootstrap.html` & `cg-28.0.0/cg/meta/report/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/report/templates/mip-dna_report.html` & `cg-28.0.0/cg/meta/report/templates/mip-dna_report.html`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/rsync/rsync_api.py` & `cg-28.0.0/cg/meta/rsync/rsync_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/tar/tar.py` & `cg-28.0.0/cg/meta/tar/tar.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/transfer/external_data.py` & `cg-28.0.0/cg/meta/transfer/external_data.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/transfer/flowcell.py` & `cg-28.0.0/cg/meta/transfer/flowcell.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                 flow_cell_id,
                 SequencingFileTag.CGSTATS_LOG,
             ],
         )
         cgstats_flow_cell: StatsFlowcell = self.stats.flowcell(flowcell_name=flow_cell_id)
         flow_cell: Flowcell = self._add_flow_cell_to_status_db(
             cgstats_flow_cell=cgstats_flow_cell,
-            flow_cell=self.db.get_flow_cell(flow_cell_id=flow_cell_id),
+            flow_cell=self.db.get_flow_cell_by_name(flow_cell_name=flow_cell_id),
             flow_cell_id=flow_cell_id,
         )
 
         self._include_sample_sheet_to_housekeeper(
             flow_cell_dir=flow_cell_dir, flow_cell_id=flow_cell_id, store=store
         )
         self._include_cgstats_log_to_housekeeper(
@@ -128,15 +128,15 @@
 
     def _add_flow_cell_to_status_db(
         self, cgstats_flow_cell: StatsFlowcell, flow_cell: Optional[Flowcell], flow_cell_id: str
     ) -> Flowcell:
         """Add a flow cell to the status database."""
         if not flow_cell:
             flow_cell: Flowcell = self.db.add_flow_cell(
-                flow_cell_id=flow_cell_id,
+                flow_cell_name=flow_cell_id,
                 sequencer_name=cgstats_flow_cell.sequencer,
                 sequencer_type=cgstats_flow_cell.sequencer_type,
                 date=cgstats_flow_cell.date,
                 flow_cell_status=FlowCellStatus.ON_DISK,
             )
         return flow_cell
```

### Comparing `cg-27.3.9/cg/meta/transfer/lims.py` & `cg-28.0.0/cg/meta/transfer/lims.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/upload/balsamic/balsamic.py` & `cg-28.0.0/cg/meta/upload/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/upload/coverage.py` & `cg-28.0.0/cg/meta/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/upload/fohm/fohm.py` & `cg-28.0.0/cg/meta/upload/fohm/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/upload/gisaid/constants.py` & `cg-28.0.0/cg/meta/upload/gisaid/constants.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/upload/gisaid/gisaid.py` & `cg-28.0.0/cg/meta/upload/gisaid/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/upload/gisaid/models.py` & `cg-28.0.0/cg/meta/upload/gisaid/models.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/upload/gt.py` & `cg-28.0.0/cg/meta/upload/gt.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/upload/mip/mip_dna.py` & `cg-28.0.0/cg/meta/upload/mip/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/upload/mip/mip_rna.py` & `cg-28.0.0/cg/meta/upload/mip/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/upload/mutacc.py` & `cg-28.0.0/cg/meta/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/upload/nipt/nipt.py` & `cg-28.0.0/cg/meta/upload/nipt/nipt.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/upload/rnafusion/rnafusion.py` & `cg-28.0.0/cg/meta/upload/rnafusion/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/upload/scout/balsamic_config_builder.py` & `cg-28.0.0/cg/meta/upload/scout/balsamic_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/upload/scout/balsamic_umi_config_builder.py` & `cg-28.0.0/cg/meta/upload/scout/balsamic_umi_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/upload/scout/hk_tags.py` & `cg-28.0.0/cg/meta/upload/scout/hk_tags.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/upload/scout/mip_config_builder.py` & `cg-28.0.0/cg/meta/upload/scout/mip_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/upload/scout/rnafusion_config_builder.py` & `cg-28.0.0/cg/meta/upload/scout/rnafusion_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/upload/scout/scout_config_builder.py` & `cg-28.0.0/cg/meta/upload/scout/scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/upload/scout/uploadscoutapi.py` & `cg-28.0.0/cg/meta/upload/scout/uploadscoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/upload/upload_api.py` & `cg-28.0.0/cg/meta/upload/upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/upload/vogue.py` & `cg-28.0.0/cg/meta/upload/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/workflow/analysis.py` & `cg-28.0.0/cg/meta/workflow/analysis.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/workflow/balsamic.py` & `cg-28.0.0/cg/meta/workflow/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/workflow/balsamic_pon.py` & `cg-28.0.0/cg/meta/workflow/balsamic_pon.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/workflow/balsamic_qc.py` & `cg-28.0.0/cg/meta/workflow/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/workflow/balsamic_umi.py` & `cg-28.0.0/cg/meta/workflow/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/workflow/fastq.py` & `cg-28.0.0/cg/meta/workflow/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/workflow/fluffy.py` & `cg-28.0.0/cg/meta/workflow/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/workflow/microsalt.py` & `cg-28.0.0/cg/meta/workflow/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/workflow/mip.py` & `cg-28.0.0/cg/meta/workflow/mip.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/workflow/mip_dna.py` & `cg-28.0.0/cg/meta/workflow/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/workflow/mip_rna.py` & `cg-28.0.0/cg/meta/workflow/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/workflow/mutant.py` & `cg-28.0.0/cg/meta/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/workflow/nextflow_common.py` & `cg-28.0.0/cg/meta/workflow/nextflow_common.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/workflow/prepare_fastq.py` & `cg-28.0.0/cg/meta/workflow/prepare_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/workflow/rnafusion.py` & `cg-28.0.0/cg/meta/workflow/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/meta/workflow/tower_common.py` & `cg-28.0.0/cg/meta/workflow/tower_common.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/balsamic/config.py` & `cg-28.0.0/cg/models/balsamic/config.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/balsamic/metrics.py` & `cg-28.0.0/cg/models/balsamic/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/cg_config.py` & `cg-28.0.0/cg/models/cg_config.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/cgstats/stats_sample.py` & `cg-28.0.0/cg/models/cgstats/stats_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/compression_data.py` & `cg-28.0.0/cg/models/compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/deliverables/metric_deliverables.py` & `cg-28.0.0/cg/models/deliverables/metric_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/demultiplex/demux_results.py` & `cg-28.0.0/cg/models/demultiplex/demux_results.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/demultiplex/flow_cell.py` & `cg-28.0.0/cg/models/demultiplex/flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/demultiplex/run_parameters.py` & `cg-28.0.0/cg/models/demultiplex/run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/demultiplex/sbatch.py` & `cg-28.0.0/cg/models/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/file_data.py` & `cg-28.0.0/cg/models/file_data.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/invoice/invoice.py` & `cg-28.0.0/cg/models/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/lims/sample.py` & `cg-28.0.0/cg/models/lims/sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/mip/mip_config.py` & `cg-28.0.0/cg/models/mip/mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/mip/mip_metrics_deliverables.py` & `cg-28.0.0/cg/models/mip/mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/mip/mip_sample_info.py` & `cg-28.0.0/cg/models/mip/mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/nextflow/deliverables.py` & `cg-28.0.0/cg/models/nextflow/deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/nextflow/sample.py` & `cg-28.0.0/cg/models/nextflow/sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/observations/input_files.py` & `cg-28.0.0/cg/models/observations/input_files.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/orders/constants.py` & `cg-28.0.0/cg/models/orders/constants.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/orders/excel_sample.py` & `cg-28.0.0/cg/models/orders/excel_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/orders/json_sample.py` & `cg-28.0.0/cg/models/orders/json_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/orders/order.py` & `cg-28.0.0/cg/models/orders/order.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/orders/orderform_schema.py` & `cg-28.0.0/cg/models/orders/orderform_schema.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/orders/sample_base.py` & `cg-28.0.0/cg/models/orders/sample_base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/orders/samples.py` & `cg-28.0.0/cg/models/orders/samples.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/report/metadata.py` & `cg-28.0.0/cg/models/report/metadata.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/report/report.py` & `cg-28.0.0/cg/models/report/report.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/report/sample.py` & `cg-28.0.0/cg/models/report/sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/report/validators.py` & `cg-28.0.0/cg/models/report/validators.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/rnafusion/rnafusion_sample.py` & `cg-28.0.0/cg/models/rnafusion/rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/scout/scout_load_config.py` & `cg-28.0.0/cg/models/scout/scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/slurm/sbatch.py` & `cg-28.0.0/cg/models/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/models/workflow/mutant.py` & `cg-28.0.0/cg/models/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/resources/20181012_Indices.csv` & `cg-28.0.0/cg/resources/20181012_Indices.csv`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/resources/rnafusion_bundle_filenames.csv` & `cg-28.0.0/cg/resources/rnafusion_bundle_filenames.csv`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/server/admin.py` & `cg-28.0.0/cg/server/admin.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/server/api.py` & `cg-28.0.0/cg/server/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,15 +363,15 @@
     parsed_flow_cells: List[Dict] = [flow_cell.to_dict() for flow_cell in flow_cells[:50]]
     return jsonify(flowcells=parsed_flow_cells, total=len(flow_cells))
 
 
 @BLUEPRINT.route("/flowcells/<flowcell_id>")
 def parse_flow_cell(flowcell_id):
     """Return a single flowcell."""
-    flow_cell: Flowcell = db.get_flow_cell(flowcell_id)
+    flow_cell: Flowcell = db.get_flow_cell_by_name(flow_cell_name=flowcell_id)
     if flow_cell is None:
         return abort(http.HTTPStatus.NOT_FOUND)
     return jsonify(**flow_cell.to_dict(samples=True))
 
 
 @BLUEPRINT.route("/analyses")
 def parse_analyses():
```

### Comparing `cg-27.3.9/cg/server/app.py` & `cg-28.0.0/cg/server/app.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/server/config.py` & `cg-28.0.0/cg/server/config.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/server/ext.py` & `cg-28.0.0/cg/server/ext.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/server/invoices/templates/invoices/index.html` & `cg-28.0.0/cg/server/invoices/templates/invoices/index.html`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/server/invoices/templates/invoices/invoice.html` & `cg-28.0.0/cg/server/invoices/templates/invoices/invoice.html`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/server/invoices/templates/invoices/layout.html` & `cg-28.0.0/cg/server/invoices/templates/invoices/layout.html`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/server/invoices/templates/invoices/new.html` & `cg-28.0.0/cg/server/invoices/templates/invoices/new.html`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/server/invoices/views.py` & `cg-28.0.0/cg/server/invoices/views.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/store/api/add.py` & `cg-28.0.0/cg/store/api/add.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,23 +213,23 @@
         new_record.sample = sample
         new_record.mother = mother
         new_record.father = father
         return new_record
 
     def add_flow_cell(
         self,
-        flow_cell_id: str,
+        flow_cell_name: str,
         sequencer_name: str,
         sequencer_type: str,
         date: dt.datetime,
         flow_cell_status: Optional[str] = FlowCellStatus.ON_DISK,
     ) -> Flowcell:
         """Build a new Flowcell record."""
         return self.Flowcell(
-            name=flow_cell_id,
+            name=flow_cell_name,
             sequencer_name=sequencer_name,
             sequencer_type=sequencer_type,
             sequenced_at=date,
             status=flow_cell_status,
         )
 
     def add_analysis(
```

### Comparing `cg-27.3.9/cg/store/api/core.py` & `cg-28.0.0/cg/store/api/core.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/store/api/delete.py` & `cg-28.0.0/cg/store/api/delete.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 class DeleteDataHandler(BaseHandler):
     """Contains methods to delete business data model instances"""
 
     def delete_flow_cell(self, flow_cell_id: str) -> None:
         """Delete flow cell."""
         flow_cell: Flowcell = apply_flow_cell_filter(
             flow_cells=self._get_query(table=Flowcell),
-            flow_cell_id=flow_cell_id,
-            filter_functions=[FlowCellFilter.GET_BY_ID],
+            flow_cell_name=flow_cell_id,
+            filter_functions=[FlowCellFilter.GET_BY_NAME],
         ).first()
 
         if flow_cell:
             flow_cell.delete()
             flow_cell.flush()
             self.commit()
```

### Comparing `cg-27.3.9/cg/store/api/find_basic_data.py` & `cg-28.0.0/cg/store/api/find_basic_data.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/store/api/find_business_data.py` & `cg-28.0.0/cg/store/api/find_business_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,64 +374,64 @@
         return apply_sample_filter(
             samples=self._get_query(table=Sample),
             filter_functions=filter_functions,
             customer_entry_ids=customer_entry_id,
             name=sample_name,
         ).first()
 
-    def get_flow_cell(self, flow_cell_id: str) -> Flowcell:
-        """Return flow cell by flow cell id."""
+    def get_flow_cell_by_name(self, flow_cell_name: str) -> Flowcell:
+        """Return flow cell by flow cell name."""
         return apply_flow_cell_filter(
             flow_cells=self._get_query(table=Flowcell),
-            flow_cell_id=flow_cell_id,
-            filter_functions=[FlowCellFilter.GET_BY_ID],
+            flow_cell_name=flow_cell_name,
+            filter_functions=[FlowCellFilter.GET_BY_NAME],
         ).first()
 
     def get_flow_cell_by_name_pattern(self, name_pattern: str) -> Flowcell:
         """Return flow cell by name pattern."""
         return apply_flow_cell_filter(
             flow_cells=self._get_query(table=Flowcell),
-            name_pattern=name_pattern,
-            filter_functions=[FlowCellFilter.GET_BY_NAME_PATTERN],
+            name_search=name_pattern,
+            filter_functions=[FlowCellFilter.GET_BY_NAME_SEARCH],
         ).first()
 
     def get_flow_cells_by_statuses(self, flow_cell_statuses: List[str]) -> Optional[List[Flowcell]]:
         """Return flow cells with supplied statuses."""
         return apply_flow_cell_filter(
             flow_cells=self._get_query(table=Flowcell),
             flow_cell_statuses=flow_cell_statuses,
             filter_functions=[FlowCellFilter.GET_WITH_STATUSES],
-        )
+        ).all()
 
     def get_flow_cell_by_name_pattern_and_status(
         self, flow_cell_statuses: List[str], name_pattern: str
     ) -> List[Flowcell]:
         """Return flow cell by name pattern and status."""
         filter_functions: List[FlowCellFilter] = [
             FlowCellFilter.GET_WITH_STATUSES,
-            FlowCellFilter.GET_BY_NAME_PATTERN,
+            FlowCellFilter.GET_BY_NAME_SEARCH,
         ]
         return apply_flow_cell_filter(
             flow_cells=self._get_query(table=Flowcell),
-            name_pattern=name_pattern,
+            name_search=name_pattern,
             flow_cell_statuses=flow_cell_statuses,
             filter_functions=filter_functions,
         ).all()
 
     def get_flow_cells_by_case(self, case: Family) -> Optional[List[Flowcell]]:
         """Return flow cells for case."""
         return apply_flow_cell_filter(
             flow_cells=self._get_join_flow_cell_sample_links_query(),
             filter_functions=[FlowCellFilter.GET_BY_CASE],
             case=case,
         )
 
     def get_samples_from_flow_cell(self, flow_cell_id: str) -> Optional[List[Sample]]:
         """Return samples present on flow cell."""
-        flow_cell: Flowcell = self.get_flow_cell(flow_cell_id=flow_cell_id)
+        flow_cell: Flowcell = self.get_flow_cell_by_name(flow_cell_name=flow_cell_id)
         if flow_cell:
             return flow_cell.samples
 
     def is_all_flow_cells_on_disk(self, case_id: str) -> bool:
         """Check if flow cells are on disk for sample before starting the analysis.
         Flow cells not on disk will be requested.
         """
```

### Comparing `cg-27.3.9/cg/store/api/import_func.py` & `cg-28.0.0/cg/store/api/import_func.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/store/api/models.py` & `cg-28.0.0/cg/store/api/models.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/store/api/status.py` & `cg-28.0.0/cg/store/api/status.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from sqlalchemy.orm import Query
 from typing_extensions import Literal
 
 from cg.constants import CASE_ACTIONS, Pipeline, FlowCellStatus
 from cg.constants.constants import CaseActions
 from cg.constants.invoice import CustomerNames
+from cg.store.filters.status_customer_filters import CustomerFilter, apply_customer_filter
 from cg.store.models import (
     Analysis,
     Application,
     ApplicationVersion,
     Customer,
     Family,
     FamilySample,
@@ -522,76 +523,14 @@
             case_data.analysis_completed_at,
             case_data.analysis_uploaded_at,
             case_data.samples_delivered_at,
         )
         case_data.max_tat = self._get_max_tat(links=case_obj.links)
         return case_data
 
-    def _get_filtered_case_query(
-        self,
-        case_action: Optional[str],
-        customer_id: str,
-        data_analysis: str,
-        days: int,
-        exclude_customer_id: bool,
-        internal_id: str,
-        name: str,
-        priority: str,
-        sample_id: str,
-    ) -> Query:
-        cases_query: Query = self._get_query(table=Family)
-        filter_functions: List[Callable] = []
-
-        filter_case_order_date = None
-        if days != 0:
-            filter_case_order_date = datetime.now() - timedelta(days=days)
-            filter_functions.append(CaseFilter.GET_NEW_BY_ORDER_DATE)
-        if case_action:
-            filter_functions.append(CaseFilter.FILTER_BY_ACTION)
-        if priority:
-            filter_functions.append(CaseFilter.FILTER_BY_PRIORITY)
-        if internal_id:
-            filter_functions.append(CaseFilter.FILTER_BY_INTERNAL_ID_SEARCH)
-        if name:
-            filter_functions.append(CaseFilter.FILTER_BY_NAME_SEARCH)
-        if data_analysis:
-            filter_functions.append(CaseFilter.FILTER_BY_PIPELINE_SEARCH)
-
-        cases_query = apply_case_filter(
-            cases=cases_query,
-            filter_functions=filter_functions,
-            order_date=filter_case_order_date,
-            action=case_action,
-            priority=priority,
-            internal_id_search=internal_id,
-            name_search=name,
-            pipeline_search=data_analysis,
-        )
-
-        # customer filters
-        if customer_id or exclude_customer_id:
-            cases_query = cases_query.join(Family.customer)
-
-        if customer_id:
-            cases_query = cases_query.filter(Customer.internal_id == customer_id)
-
-        if exclude_customer_id:
-            cases_query = cases_query.filter(Customer.internal_id != exclude_customer_id)
-
-        # sample filters
-        if sample_id:
-            cases_query = cases_query.join(Family.links, FamilySample.sample)
-            cases_query = cases_query.filter(Sample.internal_id.ilike(f"%{sample_id}%"))
-        else:
-            cases_query = cases_query.outerjoin(Family.links, FamilySample.sample)
-
-        # other joins
-        cases_query = cases_query.outerjoin(Family.analyses, Sample.invoice, Sample.flowcells)
-        return cases_query
-
     @staticmethod
     def _is_rerun(
         case_obj: Family,
         samples_received_at: datetime,
         samples_prepared_at: datetime,
         samples_sequenced_at: datetime,
     ) -> bool:
```

### Comparing `cg-27.3.9/cg/store/filters/status_analysis_filters.py` & `cg-28.0.0/cg/store/filters/status_analysis_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/store/filters/status_application_filters.py` & `cg-28.0.0/cg/store/filters/status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/store/filters/status_application_version_filters.py` & `cg-28.0.0/cg/store/filters/status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/store/filters/status_bed_filters.py` & `cg-28.0.0/cg/store/filters/status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/store/filters/status_bed_version_filters.py` & `cg-28.0.0/cg/store/filters/status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/store/filters/status_case_filters.py` & `cg-28.0.0/cg/store/filters/status_case_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/store/filters/status_case_sample_filters.py` & `cg-28.0.0/cg/store/filters/status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/store/filters/status_collaboration_filters.py` & `cg-28.0.0/cg/store/filters/status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/store/filters/status_customer_filters.py` & `cg-28.0.0/cg/store/filters/status_customer_filters.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,25 +9,35 @@
 def filter_customer_by_customer_internal_id(
     customers: Query, customer_internal_id: str, **kwargs
 ) -> Query:
     """Return customer by customer internal id."""
     return customers.filter(Customer.internal_id == customer_internal_id)
 
 
+def filter_customer_by_exclude_customer_internal_id(
+    customers: Query, exclude_customer_internal_id: str, **kwargs
+) -> Query:
+    """Return customer excluded by customer internal id."""
+    return customers.filter(Customer.internal_id != exclude_customer_internal_id)
+
+
 class CustomerFilter(Enum):
     """Define customer filter functions."""
 
     FILTER_BY_INTERNAL_ID: Callable = filter_customer_by_customer_internal_id
+    EXCLUDE_INTERNAL_ID: Callable = filter_customer_by_exclude_customer_internal_id
 
 
 def apply_customer_filter(
     customers: Query,
     filter_functions: List[Callable],
     customer_internal_id: Optional[str] = None,
+    exclude_customer_internal_id: Optional[str] = None,
 ) -> Query:
     """Apply filtering functions and return filtered results."""
     for filter_function in filter_functions:
         customers: Query = filter_function(
             customers=customers,
             customer_internal_id=customer_internal_id,
+            exclude_customer_internal_id=exclude_customer_internal_id,
         )
     return customers
```

### Comparing `cg-27.3.9/cg/store/filters/status_flow_cell_filters.py` & `cg-28.0.0/cg/store/filters/status_flow_cell_filters.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,51 +7,51 @@
 
 
 def filter_flow_cells_by_case(case: Family, flow_cells: Query, **kwargs) -> Query:
     """Return flow cells by case id."""
     return flow_cells.filter(FamilySample.family == case)
 
 
-def filter_flow_cell_by_id(flow_cells: Query, flow_cell_id: str, **kwargs) -> Query:
+def get_flow_cell_by_name(flow_cells: Query, flow_cell_name: str, **kwargs) -> Query:
     """Return flow cell by flow cell id."""
-    return flow_cells.filter(Flowcell.name == flow_cell_id)
+    return flow_cells.filter(Flowcell.name == flow_cell_name)
 
 
-def filter_flow_cell_by_name_pattern(flow_cells: Query, name_pattern: str, **kwargs) -> Query:
+def filter_flow_cell_by_name_search(flow_cells: Query, name_search: str, **kwargs) -> Query:
     """Return flow cell by flow cell id enquiry."""
-    return flow_cells.filter(Flowcell.name.like(f"%{name_pattern}%"))
+    return flow_cells.filter(Flowcell.name.like(f"%{name_search}%"))
 
 
 def filter_flow_cells_with_statuses(
     flow_cells: Query, flow_cell_statuses: List[str], **kwargs
 ) -> Query:
     """Return flow cells by flow cell statuses."""
     return flow_cells.filter(Flowcell.status.in_(flow_cell_statuses))
 
 
 def apply_flow_cell_filter(
     flow_cells: Query,
     filter_functions: List[Callable],
     case: Optional[Family] = None,
-    flow_cell_id: Optional[str] = None,
-    name_pattern: Optional[str] = None,
+    flow_cell_name: Optional[str] = None,
+    name_search: Optional[str] = None,
     flow_cell_statuses: Optional[List[str]] = None,
 ) -> Query:
     """Apply filtering functions and return filtered results."""
     for function in filter_functions:
         flow_cells: Query = function(
             flow_cells=flow_cells,
             case=case,
-            flow_cell_id=flow_cell_id,
+            flow_cell_name=flow_cell_name,
             flow_cell_statuses=flow_cell_statuses,
-            name_pattern=name_pattern,
+            name_search=name_search,
         )
     return flow_cells
 
 
 class FlowCellFilter(Enum):
     """Define FlowCell filter functions."""
 
     GET_BY_CASE: Callable = filter_flow_cells_by_case
-    GET_BY_ID: Callable = filter_flow_cell_by_id
-    GET_BY_NAME_PATTERN: Callable = filter_flow_cell_by_name_pattern
+    GET_BY_NAME: Callable = get_flow_cell_by_name
+    GET_BY_NAME_SEARCH: Callable = filter_flow_cell_by_name_search
     GET_WITH_STATUSES: Callable = filter_flow_cells_with_statuses
```

### Comparing `cg-27.3.9/cg/store/filters/status_invoice_filters.py` & `cg-28.0.0/cg/store/filters/status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/store/filters/status_organism_filters.py` & `cg-28.0.0/cg/store/filters/status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/store/filters/status_panel_filters.py` & `cg-28.0.0/cg/store/filters/status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/store/filters/status_pool_filters.py` & `cg-28.0.0/cg/store/filters/status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/store/filters/status_sample_filters.py` & `cg-28.0.0/cg/store/filters/status_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/store/filters/status_user_filters.py` & `cg-28.0.0/cg/store/filters/status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/store/models.py` & `cg-28.0.0/cg/store/models.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/utils/checksum/checksum.py` & `cg-28.0.0/cg/utils/checksum/checksum.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/utils/click/EnumChoice.py` & `cg-28.0.0/cg/utils/click/EnumChoice.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/utils/commands.py` & `cg-28.0.0/cg/utils/commands.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/utils/date.py` & `cg-28.0.0/cg/utils/date.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/utils/dict.py` & `cg-28.0.0/cg/utils/dict.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/utils/dispatcher.py` & `cg-28.0.0/cg/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/utils/email.py` & `cg-28.0.0/cg/utils/email.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/utils/flask/enum.py` & `cg-28.0.0/cg/utils/flask/enum.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg/utils/utils.py` & `cg-28.0.0/cg/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/cg.egg-info/PKG-INFO` & `cg-28.0.0/cg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 27.3.9
+Version: 28.0.0
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-27.3.9/cg.egg-info/SOURCES.txt` & `cg-28.0.0/cg.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -127,16 +127,16 @@
 cg/cli/generate/base.py
 cg/cli/generate/report/__init__.py
 cg/cli/generate/report/base.py
 cg/cli/generate/report/options.py
 cg/cli/generate/report/utils.py
 cg/cli/set/__init__.py
 cg/cli/set/base.py
-cg/cli/set/families.py
-cg/cli/set/family.py
+cg/cli/set/case.py
+cg/cli/set/cases.py
 cg/cli/store/__init__.py
 cg/cli/store/fastq.py
 cg/cli/store/store.py
 cg/cli/upload/__init__.py
 cg/cli/upload/base.py
 cg/cli/upload/clinical_delivery.py
 cg/cli/upload/coverage.py
@@ -542,16 +542,16 @@
 tests/cli/clean/test_microbial_clean.py
 tests/cli/clean/test_rsync_past_run_dirs.py
 tests/cli/compress/conftest.py
 tests/cli/compress/test_cli_compress_fastq.py
 tests/cli/compress/test_cli_decompress_spring.py
 tests/cli/compress/test_compress_helpers.py
 tests/cli/compress/test_store_fastq.py
-tests/cli/delete/test_case.py
-tests/cli/delete/test_cases.py
+tests/cli/delete/test_cli_delete_case.py
+tests/cli/delete/test_cli_delete_cases.py
 tests/cli/deliver/conftest.py
 tests/cli/deliver/test_deliver_base.py
 tests/cli/deliver/test_rsync_base.py
 tests/cli/deliver/test_run_deliver_cmd.py
 tests/cli/demultiplex/__init__.py
 tests/cli/demultiplex/conftest.py
 tests/cli/demultiplex/test_add_flowcell.py
@@ -569,20 +569,20 @@
 tests/cli/get/__init__.py
 tests/cli/get/test_cli_get.py
 tests/cli/get/test_cli_get_analysis.py
 tests/cli/get/test_cli_get_case.py
 tests/cli/get/test_cli_get_flow_cell.py
 tests/cli/get/test_cli_get_sample.py
 tests/cli/set/conftest.py
-tests/cli/set/test_families.py
-tests/cli/set/test_family.py
-tests/cli/set/test_flowcell.py
-tests/cli/set/test_list_keys.py
-tests/cli/set/test_sample.py
-tests/cli/set/test_samples.py
+tests/cli/set/test_cli_set_case.py
+tests/cli/set/test_cli_set_cases.py
+tests/cli/set/test_cli_set_flowcell.py
+tests/cli/set/test_cli_set_list_keys.py
+tests/cli/set/test_cli_set_sample.py
+tests/cli/set/test_cli_set_samples.py
 tests/cli/store/test_fastq.py
 tests/cli/tests/fixtures/data/fastq.fastq.gz
 tests/cli/upload/__init__.py
 tests/cli/upload/conftest.py
 tests/cli/upload/test_cli_scout.py
 tests/cli/upload/test_cli_upload.py
 tests/cli/upload/test_cli_upload_auto.py
```

### Comparing `cg-27.3.9/requirements.txt` & `cg-28.0.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/setup.py` & `cg-28.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     with io.open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
         LONG_DESCRIPTION = "\n" + f.read()
 except FileNotFoundError:
     LONG_DESCRIPTION = DESCRIPTION
 
 setup(
     name=NAME,
-    version="27.3.9",
+    version="28.0.0",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     url=URL,
     include_package_data=True,
```

### Comparing `cg-27.3.9/tests/apps/cgstats/conftest.py` & `cg-28.0.0/tests/apps/cgstats/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/cgstats/crud/test_create_novaseq.py` & `cg-28.0.0/tests/apps/cgstats/crud/test_create_novaseq.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/cgstats/crud/test_delete.py` & `cg-28.0.0/tests/apps/cgstats/crud/test_delete.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/cgstats/parsers/test_conversion_stats.py` & `cg-28.0.0/tests/apps/cgstats/parsers/test_conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/cgstats/parsers/test_demux_stats.py` & `cg-28.0.0/tests/apps/cgstats/parsers/test_demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/cgstats/parsers/test_run_info.py` & `cg-28.0.0/tests/apps/cgstats/parsers/test_run_info.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/cgstats/test_cgstats_create.py` & `cg-28.0.0/tests/apps/cgstats/test_cgstats_create.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/cgstats/test_stats.py` & `cg-28.0.0/tests/apps/cgstats/test_stats.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/conftest.py` & `cg-28.0.0/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/coverage/test_coverage.py` & `cg-28.0.0/tests/apps/coverage/test_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/crunchy/conftest.py` & `cg-28.0.0/tests/apps/crunchy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/crunchy/test_compress_fastq.py` & `cg-28.0.0/tests/apps/crunchy/test_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/crunchy/test_config.py` & `cg-28.0.0/tests/apps/crunchy/test_config.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/crunchy/test_crunchy.py` & `cg-28.0.0/tests/apps/crunchy/test_crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/crunchy/test_spring_decompression.py` & `cg-28.0.0/tests/apps/crunchy/test_spring_decompression.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/demultiplex/conftest.py` & `cg-28.0.0/tests/apps/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/demultiplex/test_convert_to_sample_sheet.py` & `cg-28.0.0/tests/apps/demultiplex/test_convert_to_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/demultiplex/test_demultiplex_api.py` & `cg-28.0.0/tests/apps/demultiplex/test_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/demultiplex/test_parse_run_parameters.py` & `cg-28.0.0/tests/apps/demultiplex/test_parse_run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/demultiplex/test_sample_sheet.py` & `cg-28.0.0/tests/apps/demultiplex/test_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/gens/test_gens_api.py` & `cg-28.0.0/tests/apps/gens/test_gens_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/gt/conftest.py` & `cg-28.0.0/tests/apps/gt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/gt/test_gt_api.py` & `cg-28.0.0/tests/apps/gt/test_gt_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/hk/conftest.py` & `cg-28.0.0/tests/apps/hk/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/hk/test__getattr__.py` & `cg-28.0.0/tests/apps/hk/test__getattr__.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/hk/test_add_file.py` & `cg-28.0.0/tests/apps/hk/test_add_file.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/hk/test_bundles.py` & `cg-28.0.0/tests/apps/hk/test_bundles.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/hk/test_core.py` & `cg-28.0.0/tests/apps/hk/test_core.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/hk/test_file.py` & `cg-28.0.0/tests/apps/hk/test_file.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/hk/test_version.py` & `cg-28.0.0/tests/apps/hk/test_version.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/lims/conftest.py` & `cg-28.0.0/tests/apps/lims/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/lims/test_api.py` & `cg-28.0.0/tests/apps/lims/test_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/loqus/conftest.py` & `cg-28.0.0/tests/apps/loqus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/loqus/test_loqusdb_api.py` & `cg-28.0.0/tests/apps/loqus/test_loqusdb_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/madeline/conftest.py` & `cg-28.0.0/tests/apps/madeline/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/madeline/test_madeline.py` & `cg-28.0.0/tests/apps/madeline/test_madeline.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/mip/conftest.py` & `cg-28.0.0/tests/apps/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/mip/test_config_mip.py` & `cg-28.0.0/tests/apps/mip/test_config_mip.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/mutacc_auto/conftest.py` & `cg-28.0.0/tests/apps/mutacc_auto/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/mutacc_auto/test_mutacc_auto.py` & `cg-28.0.0/tests/apps/mutacc_auto/test_mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/orderform/conftest.py` & `cg-28.0.0/tests/apps/orderform/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/orderform/test_excel_orderform_parser.py` & `cg-28.0.0/tests/apps/orderform/test_excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/orderform/test_excel_sample_schema.py` & `cg-28.0.0/tests/apps/orderform/test_excel_sample_schema.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/orderform/test_json_orderform_parser.py` & `cg-28.0.0/tests/apps/orderform/test_json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/orderform/test_orderform_parser.py` & `cg-28.0.0/tests/apps/orderform/test_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/scout/conftest.py` & `cg-28.0.0/tests/apps/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/scout/test_get_causative_variants.py` & `cg-28.0.0/tests/apps/scout/test_get_causative_variants.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/scout/test_get_scout_cases.py` & `cg-28.0.0/tests/apps/scout/test_get_scout_cases.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/scout/test_scout_load_config.py` & `cg-28.0.0/tests/apps/scout/test_scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/scout/test_scout_models.py` & `cg-28.0.0/tests/apps/scout/test_scout_models.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/slurm/conftest.py` & `cg-28.0.0/tests/apps/slurm/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/slurm/test_slurm_api.py` & `cg-28.0.0/tests/apps/slurm/test_slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/test_apps_environ.py` & `cg-28.0.0/tests/apps/test_apps_environ.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/test_osticket.py` & `cg-28.0.0/tests/apps/test_osticket.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/vogue/conftest.py` & `cg-28.0.0/tests/apps/vogue/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/apps/vogue/test_vogue_api.py` & `cg-28.0.0/tests/apps/vogue/test_vogue_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/add/test_cli_add.py` & `cg-28.0.0/tests/cli/add/test_cli_add.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/add/test_cli_add_customer.py` & `cg-28.0.0/tests/cli/add/test_cli_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/add/test_cli_add_family.py` & `cg-28.0.0/tests/cli/add/test_cli_add_family.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/add/test_cli_add_relationship.py` & `cg-28.0.0/tests/cli/add/test_cli_add_relationship.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/add/test_cli_add_sample.py` & `cg-28.0.0/tests/cli/add/test_cli_add_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/backup/conftest.py` & `cg-28.0.0/tests/cli/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/backup/test_backup_command.py` & `cg-28.0.0/tests/cli/backup/test_backup_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     # GIVEN a context with a backup_api
     assert "backup_api" in backup_context.meta_apis
 
     # GIVEN that there are no flow cells set to "requested" in status_db
     assert not backup_context.status_db.get_flow_cells_by_statuses(
         flow_cell_statuses=[FlowCellStatus.REQUESTED]
-    ).first()
+    )
 
     # WHEN running the fetch flow cell command without specifying any flow cell in dry run mode
     result = cli_runner.invoke(fetch_flow_cell, ["--dry-run"], obj=backup_context)
 
     # THEN assert that it exits without any problems
     assert result.exit_code == EXIT_SUCCESS
 
@@ -39,15 +39,15 @@
 
     # GIVEN a context with a backup_api
     assert "backup_api" in backup_context.meta_apis
 
     # GIVEN that there are no flow cells set to "requested" in status_db
     assert not backup_context.status_db.get_flow_cells_by_statuses(
         flow_cell_statuses=[FlowCellStatus.REQUESTED]
-    ).first()
+    )
 
     # GIVEN that the backup api returns a retrieval time
     expected_time = 60
     mocker.patch("cg.meta.backup.backup.BackupAPI.fetch_flow_cell", return_value=expected_time)
 
     # WHEN running the fetch flow cell command without specifying any flow cell in dry run mode
     result = cli_runner.invoke(fetch_flow_cell, ["--dry-run"], obj=backup_context)
@@ -61,15 +61,15 @@
 
 def test_run_fetch_flow_cell_non_existing_flow_cell(
     cli_runner: CliRunner, backup_context: CGConfig, caplog
 ):
     # GIVEN a context with a backup api
     # GIVEN a non existing flow cell id
     flow_cell_id = "hello"
-    assert backup_context.status_db.get_flow_cell(flow_cell_id) is None
+    assert backup_context.status_db.get_flow_cell_by_name(flow_cell_id) is None
 
     # WHEN running the command with the non existing flow cell id
     result = cli_runner.invoke(
         fetch_flow_cell, ["--flow-cell-id", flow_cell_id], obj=backup_context
     )
 
     # THEN assert that it exits with a non zero exit code
```

### Comparing `cg-27.3.9/tests/cli/clean/conftest.py` & `cg-28.0.0/tests/cli/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/clean/test_balsamic_clean.py` & `cg-28.0.0/tests/cli/clean/test_balsamic_clean.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/clean/test_clean_hk_bundle_files.py` & `cg-28.0.0/tests/cli/clean/test_clean_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/clean/test_hk_bundle_files.py` & `cg-28.0.0/tests/cli/clean/test_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/clean/test_hk_case_bundle_files.py` & `cg-28.0.0/tests/cli/clean/test_hk_case_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/clean/test_microbial_clean.py` & `cg-28.0.0/tests/cli/clean/test_microbial_clean.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/clean/test_rsync_past_run_dirs.py` & `cg-28.0.0/tests/cli/clean/test_rsync_past_run_dirs.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/compress/conftest.py` & `cg-28.0.0/tests/cli/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/compress/test_cli_compress_fastq.py` & `cg-28.0.0/tests/cli/compress/test_cli_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/compress/test_cli_decompress_spring.py` & `cg-28.0.0/tests/cli/compress/test_cli_decompress_spring.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/compress/test_compress_helpers.py` & `cg-28.0.0/tests/cli/compress/test_compress_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/compress/test_store_fastq.py` & `cg-28.0.0/tests/cli/compress/test_store_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/conftest.py` & `cg-28.0.0/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/delete/test_case.py` & `cg-28.0.0/tests/cli/delete/test_cli_delete_case.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/delete/test_cases.py` & `cg-28.0.0/tests/cli/delete/test_cli_delete_cases.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/deliver/conftest.py` & `cg-28.0.0/tests/cli/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/deliver/test_deliver_base.py` & `cg-28.0.0/tests/cli/deliver/test_deliver_base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/deliver/test_rsync_base.py` & `cg-28.0.0/tests/cli/deliver/test_rsync_base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/deliver/test_run_deliver_cmd.py` & `cg-28.0.0/tests/cli/deliver/test_run_deliver_cmd.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/demultiplex/conftest.py` & `cg-28.0.0/tests/cli/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/demultiplex/test_add_flowcell.py` & `cg-28.0.0/tests/cli/demultiplex/test_add_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/demultiplex/test_create_sample_sheet.py` & `cg-28.0.0/tests/cli/demultiplex/test_create_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/demultiplex/test_demultiplex_flowcell.py` & `cg-28.0.0/tests/cli/demultiplex/test_demultiplex_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/demultiplex/test_finish_demux.py` & `cg-28.0.0/tests/cli/demultiplex/test_finish_demux.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/demultiplex/test_stats_command.py` & `cg-28.0.0/tests/cli/demultiplex/test_stats_command.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/demultiplex/test_validate_sample_sheet.py` & `cg-28.0.0/tests/cli/demultiplex/test_validate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/generate/report/conftest.py` & `cg-28.0.0/tests/cli/generate/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/generate/report/test_cli_delivery_report.py` & `cg-28.0.0/tests/cli/generate/report/test_cli_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/generate/report/test_utils.py` & `cg-28.0.0/tests/cli/generate/report/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/generate/test_cli_base.py` & `cg-28.0.0/tests/cli/generate/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/get/test_cli_get.py` & `cg-28.0.0/tests/cli/get/test_cli_get.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/get/test_cli_get_analysis.py` & `cg-28.0.0/tests/cli/get/test_cli_get_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/get/test_cli_get_case.py` & `cg-28.0.0/tests/cli/get/test_cli_get_case.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/get/test_cli_get_flow_cell.py` & `cg-28.0.0/tests/cli/get/test_cli_get_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/get/test_cli_get_sample.py` & `cg-28.0.0/tests/cli/get/test_cli_get_sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
 def test_get_sample_flowcells_with_flowcell(
     cli_runner: CliRunner, base_context: CGConfig, disk_store: Store, helpers: StoreHelpers
 ):
     """Test query samples and hide flow cell, ensuring that no flow cell name is in the output."""
     # GIVEN a database with a sample and a related flow cell
     flow_cell = helpers.add_flowcell(disk_store)
     sample = helpers.add_sample(disk_store, flowcell=flow_cell)
-    returned_flow_cell: Flowcell = disk_store.get_flow_cell(flow_cell_id=flow_cell.name)
+    returned_flow_cell: Flowcell = disk_store.get_flow_cell_by_name(flow_cell_name=flow_cell.name)
     assert sample in returned_flow_cell.samples
 
     # WHEN getting a sample with the --hide-flow-cell flag
     result = cli_runner.invoke(
         get, ["sample", sample.internal_id, "--hide-flow-cell"], obj=base_context
     )
```

### Comparing `cg-27.3.9/tests/cli/set/conftest.py` & `cg-28.0.0/tests/cli/set/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/set/test_families.py` & `cg-28.0.0/tests/cli/set/test_cli_set_cases.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,43 @@
-"""Test methods for cg/cli/set/families"""
+"""This script tests the cli methods to set values of several cases in status-db."""
 import logging
-
+from click.testing import CliRunner
 import pytest
-from cg.cli.set.families import families
+from _pytest.logging import LogCaptureFixture
+
+from cg.cli.set.cases import cases
 from cg.models.cg_config import CGConfig
 from cg.store import Store
 from cg.store.models import Family, Sample
-
-SUCCESS = 0
+from tests.store_helpers import StoreHelpers
 
 
 @pytest.mark.parametrize("identifier_key", ["original_ticket", "order"])
-def test_set_families_by_sample_identifiers(
-    cli_runner, base_context: CGConfig, identifier_key, helpers, caplog, ticket_id
+def test_set_cases_by_sample_identifiers(
+    cli_runner: CliRunner,
+    base_context: CGConfig,
+    identifier_key: str,
+    helpers: StoreHelpers,
+    caplog: LogCaptureFixture,
+    ticket_id: str,
 ):
     # GIVEN a database with a case with a sample
     base_store: Store = base_context.status_db
-    sample_obj: Sample = helpers.add_sample(base_store)
-    sample_obj.original_ticket = ticket_id
-    sample_obj.order = "An order"
+    new_sample: Sample = helpers.add_sample(base_store)
+    new_sample.original_ticket: str = ticket_id
+    new_sample.order: str = "An order"
     case: Family = helpers.add_case(base_store)
-    helpers.add_relationship(base_store, sample=sample_obj, case=case)
-    identifier_value = getattr(sample_obj, identifier_key)
+    helpers.add_relationship(base_store, sample=new_sample, case=case)
+    identifier_value = getattr(new_sample, identifier_key)
 
     caplog.set_level(logging.INFO)
 
     # WHEN calling set families with valid sample identifiers
     cli_runner.invoke(
-        families,
+        cases,
         ["--sample-identifier", identifier_key, identifier_value],
         obj=base_context,
     )
 
     # THEN it should name the case to be changed
     assert case.internal_id in caplog.text
     assert case.name in caplog.text
```

### Comparing `cg-27.3.9/tests/cli/set/test_family.py` & `cg-28.0.0/tests/cli/set/test_cli_set_case.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,188 +1,190 @@
-"""This script tests the cli methods to set values of cases in status-db"""
+"""This script tests the cli methods to set values of a case in status-db."""
 from click.testing import CliRunner
 
-from cg.cli.set.family import family
-from cg.constants import DataDelivery, Pipeline
+from cg.cli.set.case import case
+from cg.constants import DataDelivery, Pipeline, EXIT_SUCCESS
 from cg.models.cg_config import CGConfig
 from cg.store import Store
+from cg.store.models import Family
+from tests.store_helpers import StoreHelpers
 
-SUCCESS = 0
 
-
-def test_set_family_without_options(
-    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers
+def test_set_case_without_options(
+    cli_runner: CliRunner,
+    base_context: CGConfig,
+    base_store: Store,
+    helpers: StoreHelpers,
 ):
-    """Test to set a case using only the required arguments"""
+    """Test to set a case using only the required arguments."""
     # GIVEN a database with a case
-    case_id = helpers.add_case(base_store).internal_id
+    case_id: str = helpers.add_case(store=base_store).internal_id
     assert base_store.Family.query.count() == 1
 
     # WHEN setting a case
-    result = cli_runner.invoke(family, [case_id], obj=base_context)
+    result = cli_runner.invoke(case, [case_id], obj=base_context)
 
     # THEN it should abort
-    assert result.exit_code != SUCCESS
+    assert result.exit_code != EXIT_SUCCESS
 
 
-def test_set_family_bad_family(cli_runner, base_context):
-    """Test to set a case using a non-existing case"""
+def test_set_case_bad_family(
+    cli_runner: CliRunner, base_context: CGConfig, case_id_does_not_exist: str
+):
+    """Test to set a case using a non-existing case id."""
     # GIVEN an empty database
 
     # WHEN setting a case
-    case_id = "dummy_name"
-    result = cli_runner.invoke(family, [case_id], obj=base_context)
+    result = cli_runner.invoke(case, [case_id_does_not_exist], obj=base_context)
 
     # THEN it should complain on missing case
-    assert result.exit_code != SUCCESS
+    assert result.exit_code != EXIT_SUCCESS
 
 
-def test_set_family_bad_panel(
-    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers
+def test_set_case_bad_panel(
+    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers: StoreHelpers
 ):
-    """Test to set a case using a non-existing panel"""
+    """Test to set a case using a non-existing panel."""
     # GIVEN a database with a case
 
     # WHEN setting a case
-    panel_id = "dummy_panel"
-    case_id = helpers.add_case(base_store).internal_id
-    result = cli_runner.invoke(family, [case_id, "--panel", panel_id], obj=base_context)
+    panel_id: str = "dummy_panel"
+    case_id: str = helpers.add_case(store=base_store).internal_id
+    result = cli_runner.invoke(case, [case_id, "--panel", panel_id], obj=base_context)
 
     # THEN it should complain in missing panel instead of setting a value
-    assert result.exit_code != SUCCESS
+    assert result.exit_code != EXIT_SUCCESS
     assert panel_id not in base_store.Family.query.first().panels
 
 
-def test_set_family_panel(
-    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers
+def test_set_case_panel(
+    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers: StoreHelpers
 ):
-    """Test to set a case using an existing panel"""
+    """Test to set a case using an existing panel."""
     # GIVEN a database with a case and a panel not yet added to the case
-    panel_id = helpers.ensure_panel(base_store, "a_panel").name
-    case_id = helpers.add_case(base_store).internal_id
+    panel_id: str = helpers.ensure_panel(store=base_store, panel_abbreviation="a_panel").name
+    case_id: str = helpers.add_case(store=base_store).internal_id
     assert panel_id not in base_store.Family.query.first().panels
 
     # WHEN setting a panel of a case
-    result = cli_runner.invoke(family, [case_id, "--panel", panel_id], obj=base_context)
+    result = cli_runner.invoke(case, [case_id, "--panel", panel_id], obj=base_context)
 
     # THEN it should set panel on the case
-    assert result.exit_code == SUCCESS
+    assert result.exit_code == EXIT_SUCCESS
     assert panel_id in base_store.Family.query.first().panels
 
 
-def test_set_family_priority(
-    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers
+def test_set_case_priority(
+    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers: StoreHelpers
 ):
-    """Test that the added case gets the priority we send in"""
+    """Test that the added case gets the priority we send in."""
     # GIVEN a database with a case
-    case_id = helpers.add_case(base_store).internal_id
-    priority = "priority"
+    case_id: str = helpers.add_case(base_store).internal_id
+    priority: str = "priority"
     assert base_store.Family.query.first().priority_human != priority
 
     # WHEN setting a case
     result = cli_runner.invoke(
-        family, [case_id, "--priority", priority], obj=base_context, catch_exceptions=False
+        case, [case_id, "--priority", priority], obj=base_context, catch_exceptions=False
     )
 
     # THEN it should have been set
-    assert result.exit_code == SUCCESS
+    assert result.exit_code == EXIT_SUCCESS
     assert base_store.Family.query.count() == 1
     assert base_store.Family.query.first().priority_human == priority
 
 
-def test_set_family_customer(
-    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers
+def test_set_case_customer(
+    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers: StoreHelpers
 ):
-    """Test to set a case using an existing customer"""
+    """Test to set a case using an existing customer."""
     # GIVEN a database with a case and a customer not yet on the case
-    customer_id = helpers.ensure_customer(base_store, customer_id="a_customer").internal_id
-    case = helpers.add_case(base_store)
-    assert customer_id != case.customer.internal_id
+    customer_id: str = helpers.ensure_customer(
+        store=base_store, customer_id="a_customer"
+    ).internal_id
+    case_to_alter: Family = helpers.add_case(store=base_store)
+    assert customer_id != case_to_alter.customer.internal_id
 
     # WHEN setting a customer of a case
     result = cli_runner.invoke(
-        family, [case.internal_id, "--customer-id", customer_id], obj=base_context
+        case, [case_to_alter.internal_id, "--customer-id", customer_id], obj=base_context
     )
 
     # THEN it should set customer on the case
-    assert result.exit_code == SUCCESS
-    assert customer_id == case.customer.internal_id
+    assert result.exit_code == EXIT_SUCCESS
+    assert customer_id == case_to_alter.customer.internal_id
 
 
-def test_set_family_bad_data_analysis(
-    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers
+def test_set_case_bad_data_analysis(
+    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers: StoreHelpers
 ):
-    """Test to set a case using a non-existing data_analysis"""
+    """Test to set a case using a non-existing data_analysis."""
     # GIVEN a database with a case
 
     # WHEN setting a data_analysis on a case
-    data_analysis = "dummy_pipeline"
-    case_id = helpers.add_case(base_store).internal_id
-    result = cli_runner.invoke(
-        family, [case_id, "--data-analysis", data_analysis], obj=base_context
-    )
+    data_analysis: str = "dummy_pipeline"
+    case_id: str = helpers.add_case(store=base_store).internal_id
+    result = cli_runner.invoke(case, [case_id, "--data-analysis", data_analysis], obj=base_context)
 
-    # THEN it should complain in non valid data_analysis instead of setting a value
-    assert result.exit_code != SUCCESS
+    # THEN it should complain in invalid data_analysis instead of setting a value
+    assert result.exit_code != EXIT_SUCCESS
     assert str(data_analysis) != base_store.Family.query.first().data_analysis
 
 
-def test_set_family_data_analysis(
-    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers
+def test_set_case_data_analysis(
+    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers: StoreHelpers
 ):
-    """Test to set a case using an existing data_analysis"""
+    """Test to set a case using an existing data_analysis."""
 
     # GIVEN a database with a case and a data_analysis not yet set on the case
-    data_analysis = Pipeline.FASTQ
-    case_obj = helpers.add_case(base_store)
-    assert str(data_analysis) != case_obj.data_analysis
+    data_analysis: str = Pipeline.FASTQ
+    case_to_alter: str = helpers.add_case(base_store)
+    assert str(data_analysis) != case_to_alter.data_analysis
 
     # WHEN setting a data_analysis of a case
     result = cli_runner.invoke(
-        family,
-        [case_obj.internal_id, "--data-analysis", str(data_analysis)],
+        case,
+        [case_to_alter.internal_id, "--data-analysis", str(data_analysis)],
         obj=base_context,
     )
 
     # THEN it should set data_analysis on the case
-    assert result.exit_code == SUCCESS
-    assert str(data_analysis) == case_obj.data_analysis
+    assert result.exit_code == EXIT_SUCCESS
+    assert str(data_analysis) == case_to_alter.data_analysis
 
 
-def test_set_family_bad_data_delivery(
-    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers
+def test_set_case_bad_data_delivery(
+    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers: StoreHelpers
 ):
-    """Test to set a case using a non-existing data_delivery"""
+    """Test to set a case using a non-existing data_delivery."""
     # GIVEN a database with a case
 
     # WHEN setting a data_delivery on a case
-    data_delivery = "dummy_delivery"
-    case_id = helpers.add_case(base_store).internal_id
-    result = cli_runner.invoke(
-        family, [case_id, "--data-delivery", data_delivery], obj=base_context
-    )
+    data_delivery: str = "dummy_delivery"
+    case_id: str = helpers.add_case(base_store).internal_id
+    result = cli_runner.invoke(case, [case_id, "--data-delivery", data_delivery], obj=base_context)
 
-    # THEN it should complain in non valid data_delivery instead of setting a value
-    assert result.exit_code != SUCCESS
+    # THEN it should complain in invalid data_delivery instead of setting a value
+    assert result.exit_code != EXIT_SUCCESS
     assert str(data_delivery) != base_store.Family.query.first().data_delivery
 
 
-def test_set_family_data_delivery(
-    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers
+def test_set_case_data_delivery(
+    cli_runner: CliRunner, base_context: CGConfig, base_store: Store, helpers: StoreHelpers
 ):
-    """Test to set a case using an existing data_delivery"""
+    """Test to set a case using an existing data_delivery."""
 
     # GIVEN a database with a case and a data_delivery not yet set on the case
-    data_delivery = DataDelivery.FASTQ
-    case_obj = helpers.add_case(base_store)
-    assert str(data_delivery) != case_obj.data_delivery
+    data_delivery: str = DataDelivery.FASTQ
+    case_to_alter: str = helpers.add_case(base_store)
+    assert str(data_delivery) != case_to_alter.data_delivery
 
     # WHEN setting a data_delivery of a case
     result = cli_runner.invoke(
-        family,
-        [case_obj.internal_id, "--data-delivery", str(data_delivery)],
+        case,
+        [case_to_alter.internal_id, "--data-delivery", str(data_delivery)],
         obj=base_context,
     )
 
     # THEN it should set data_delivery on the case
-    assert result.exit_code == SUCCESS
-    assert str(data_delivery) == case_obj.data_delivery
+    assert result.exit_code == EXIT_SUCCESS
+    assert str(data_delivery) == case_to_alter.data_delivery
```

### Comparing `cg-27.3.9/tests/cli/set/test_flowcell.py` & `cg-28.0.0/tests/cli/set/test_cli_set_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/set/test_list_keys.py` & `cg-28.0.0/tests/cli/set/test_cli_set_list_keys.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/set/test_sample.py` & `cg-28.0.0/tests/cli/set/test_cli_set_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/set/test_samples.py` & `cg-28.0.0/tests/cli/set/test_cli_set_samples.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/store/test_fastq.py` & `cg-28.0.0/tests/cli/store/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/test_base.py` & `cg-28.0.0/tests/cli/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/test_clean.py` & `cg-28.0.0/tests/cli/test_clean.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/test_cli_status_cases.py` & `cg-28.0.0/tests/cli/test_cli_status_cases.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/upload/conftest.py` & `cg-28.0.0/tests/cli/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/upload/test_cli_scout.py` & `cg-28.0.0/tests/cli/upload/test_cli_scout.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/upload/test_cli_upload.py` & `cg-28.0.0/tests/cli/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/upload/test_cli_upload_auto.py` & `cg-28.0.0/tests/cli/upload/test_cli_upload_auto.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/upload/test_cli_upload_delivery_report.py` & `cg-28.0.0/tests/cli/upload/test_cli_upload_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/upload/test_cli_upload_fastq.py` & `cg-28.0.0/tests/cli/upload/test_cli_upload_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/upload/test_cli_upload_genotype.py` & `cg-28.0.0/tests/cli/upload/test_cli_upload_genotype.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/upload/test_cli_upload_gens.py` & `cg-28.0.0/tests/cli/upload/test_cli_upload_gens.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/upload/test_cli_upload_nipt.py` & `cg-28.0.0/tests/cli/upload/test_cli_upload_nipt.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/upload/test_cli_upload_nipt_ftp.py` & `cg-28.0.0/tests/cli/upload/test_cli_upload_nipt_ftp.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/upload/test_cli_upload_nipt_statina.py` & `cg-28.0.0/tests/cli/upload/test_cli_upload_nipt_statina.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/upload/test_cli_upload_observations.py` & `cg-28.0.0/tests/cli/upload/test_cli_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/upload/test_cli_upload_vogue.py` & `cg-28.0.0/tests/cli/upload/test_cli_upload_vogue.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/balsamic/conftest.py` & `cg-28.0.0/tests/cli/workflow/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py` & `cg-28.0.0/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/balsamic/test_compound_commands.py` & `cg-28.0.0/tests/cli/workflow/balsamic/test_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/balsamic/test_link.py` & `cg-28.0.0/tests/cli/workflow/balsamic/test_link.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/balsamic/test_report_deliver.py` & `cg-28.0.0/tests/cli/workflow/balsamic/test_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/balsamic/test_run.py` & `cg-28.0.0/tests/cli/workflow/balsamic/test_run.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/balsamic/test_store_housekeeper.py` & `cg-28.0.0/tests/cli/workflow/balsamic/test_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/conftest.py` & `cg-28.0.0/tests/cli/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/fastq/test_fastq_base.py` & `cg-28.0.0/tests/cli/workflow/fastq/test_fastq_base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/fluffy/conftest.py` & `cg-28.0.0/tests/cli/workflow/fluffy/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,14 +146,14 @@
         internal_id=fluffy_sample_lims_id,
         is_tumour=False,
         application_type="tgs",
         reads=100,
         sequenced_at=dt.datetime.now(),
     )
     helpers.add_flowcell(
-        fluffy_analysis_api.status_db, flow_cell_id="flowcell", samples=[example_fluffy_sample]
+        fluffy_analysis_api.status_db, flow_cell_name="flowcell", samples=[example_fluffy_sample]
     )
     helpers.add_relationship(
         fluffy_analysis_api.status_db, case=example_fluffy_case, sample=example_fluffy_sample
     )
     cg_context.meta_apis["analysis_api"] = fluffy_analysis_api
     return cg_context
```

### Comparing `cg-27.3.9/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py` & `cg-28.0.0/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/fluffy/test_cli_link.py` & `cg-28.0.0/tests/cli/workflow/fluffy/test_cli_link.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/fluffy/test_cli_run.py` & `cg-28.0.0/tests/cli/workflow/fluffy/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/fluffy/test_cli_start.py` & `cg-28.0.0/tests/cli/workflow/fluffy/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/fluffy/test_cli_store.py` & `cg-28.0.0/tests/cli/workflow/fluffy/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/microsalt/conftest.py` & `cg-28.0.0/tests/cli/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py` & `cg-28.0.0/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/microsalt/test_microsalt_case_config.py` & `cg-28.0.0/tests/cli/workflow/microsalt/test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/microsalt/test_microsalt_run.py` & `cg-28.0.0/tests/cli/workflow/microsalt/test_microsalt_run.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/mip/conftest.py` & `cg-28.0.0/tests/cli/workflow/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/mip/test_cli_mip_base.py` & `cg-28.0.0/tests/cli/workflow/mip/test_cli_mip_base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py` & `cg-28.0.0/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/mip/test_cli_mip_dna_run.py` & `cg-28.0.0/tests/cli/workflow/mip/test_cli_mip_dna_run.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/mip/test_cli_mip_dna_start.py` & `cg-28.0.0/tests/cli/workflow/mip/test_cli_mip_dna_start.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py` & `cg-28.0.0/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/mip/test_cli_mip_rna_link.py` & `cg-28.0.0/tests/cli/workflow/mip/test_cli_mip_rna_link.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/mip/test_cli_mip_rna_run.py` & `cg-28.0.0/tests/cli/workflow/mip/test_cli_mip_rna_run.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/mip/test_cli_mip_store.py` & `cg-28.0.0/tests/cli/workflow/mip/test_cli_mip_store.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/rnafusion/conftest.py` & `cg-28.0.0/tests/cli/workflow/rnafusion/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py` & `cg-28.0.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py` & `cg-28.0.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py` & `cg-28.0.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py` & `cg-28.0.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py` & `cg-28.0.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/test_cli_workflow.py` & `cg-28.0.0/tests/cli/workflow/test_cli_workflow.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/cli/workflow/test_cli_workflow_clean.py` & `cg-28.0.0/tests/cli/workflow/test_cli_workflow_clean.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/conftest.py` & `cg-28.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml` & `cg-28.0.0/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json` & `cg-28.0.0/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json` & `cg-28.0.0/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/analysis/sample_coverage.bed` & `cg-28.0.0/tests/fixtures/analysis/sample_coverage.bed`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/balsamic/case/config.json` & `cg-28.0.0/tests/fixtures/apps/balsamic/case/config.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/balsamic/case/metadata.yml` & `cg-28.0.0/tests/fixtures/apps/balsamic/case/metadata.yml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml` & `cg-28.0.0/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/crunchy/spring_metadata.json` & `cg-28.0.0/tests/fixtures/apps/crunchy/spring_metadata.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml` & `cg-28.0.0/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/fluffy/SampleSheet.csv` & `cg-28.0.0/tests/fixtures/apps/fluffy/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/fluffy/deliverables.yaml` & `cg-28.0.0/tests/fixtures/apps/fluffy/deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/madeline/madeline.xml` & `cg-28.0.0/tests/fixtures/apps/madeline/madeline.xml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/mip/case_metrics_deliverables.yaml` & `cg-28.0.0/tests/fixtures/apps/mip/case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/mip/dna/store/case_config.yaml` & `cg-28.0.0/tests/fixtures/apps/mip/dna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml` & `cg-28.0.0/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml` & `cg-28.0.0/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf` & `cg-28.0.0/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/mip/rna/case_config.yaml` & `cg-28.0.0/tests/fixtures/apps/mip/rna/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml` & `cg-28.0.0/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/mip/rna/store/bundle_data.yaml` & `cg-28.0.0/tests/fixtures/apps/mip/rna/store/bundle_data.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/mip/rna/store/case_config.yaml` & `cg-28.0.0/tests/fixtures/apps/mip/rna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml` & `cg-28.0.0/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml` & `cg-28.0.0/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/scout/643594.config.yaml` & `cg-28.0.0/tests/fixtures/apps/scout/643594.config.yaml`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/scout/case_export.json` & `cg-28.0.0/tests/fixtures/apps/scout/case_export.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/scout/export_causatives.json` & `cg-28.0.0/tests/fixtures/apps/scout/export_causatives.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/scout/none_case_export.json` & `cg-28.0.0/tests/fixtures/apps/scout/none_case_export.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/scout/other_sex_case.json` & `cg-28.0.0/tests/fixtures/apps/scout/other_sex_case.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/scout/panel_export.bed` & `cg-28.0.0/tests/fixtures/apps/scout/panel_export.bed`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/apps/scout/panel_export.csv` & `cg-28.0.0/tests/fixtures/apps/scout/panel_export.csv`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/cgweb_orders/balsamic.json` & `cg-28.0.0/tests/fixtures/cgweb_orders/balsamic.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/cgweb_orders/fastq.json` & `cg-28.0.0/tests/fixtures/cgweb_orders/fastq.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/cgweb_orders/metagenome.json` & `cg-28.0.0/tests/fixtures/cgweb_orders/metagenome.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/cgweb_orders/microsalt.json` & `cg-28.0.0/tests/fixtures/cgweb_orders/microsalt.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/cgweb_orders/mip.json` & `cg-28.0.0/tests/fixtures/cgweb_orders/mip.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/cgweb_orders/mip_rna.json` & `cg-28.0.0/tests/fixtures/cgweb_orders/mip_rna.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/cgweb_orders/rml.json` & `cg-28.0.0/tests/fixtures/cgweb_orders/rml.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/cgweb_orders/sarscov2.json` & `cg-28.0.0/tests/fixtures/cgweb_orders/sarscov2.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/data/SampleSheet.csv` & `cg-28.0.0/tests/fixtures/data/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/data/cgfixture.db` & `cg-28.0.0/tests/fixtures/data/cgfixture.db`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/data/hkstore.db` & `cg-28.0.0/tests/fixtures/data/hkstore.db`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/io/example_json.json` & `cg-28.0.0/tests/fixtures/io/example_json.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/orderforms/1508.27.balsamic.xlsx` & `cg-28.0.0/tests/fixtures/orderforms/1508.27.balsamic.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx` & `cg-28.0.0/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx` & `cg-28.0.0/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/orderforms/1508.27.fastq.xlsx` & `cg-28.0.0/tests/fixtures/orderforms/1508.27.fastq.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/orderforms/1508.27.mip.xlsx` & `cg-28.0.0/tests/fixtures/orderforms/1508.27.mip.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/orderforms/1508.27.mip_rna.xlsx` & `cg-28.0.0/tests/fixtures/orderforms/1508.27.mip_rna.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/orderforms/1603.11.microbial.xlsx` & `cg-28.0.0/tests/fixtures/orderforms/1603.11.microbial.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/orderforms/1604.15.rml.xlsx` & `cg-28.0.0/tests/fixtures/orderforms/1604.15.rml.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/orderforms/1605.10.metagenome.xlsx` & `cg-28.0.0/tests/fixtures/orderforms/1605.10.metagenome.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/orderforms/2184.7.sarscov2.xlsx` & `cg-28.0.0/tests/fixtures/orderforms/2184.7.sarscov2.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/orderforms/NIPT-json.json` & `cg-28.0.0/tests/fixtures/orderforms/NIPT-json.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json` & `cg-28.0.0/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/orderforms/mip_uploaded_json_orderform.json` & `cg-28.0.0/tests/fixtures/orderforms/mip_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/report/case_data.json` & `cg-28.0.0/tests/fixtures/report/case_data.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/report/lims_exported_samples.json` & `cg-28.0.0/tests/fixtures/report/lims_exported_samples.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/report/lims_family.json` & `cg-28.0.0/tests/fixtures/report/lims_family.json`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/store/api/application_versions.xlsx` & `cg-28.0.0/tests/fixtures/store/api/application_versions.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/fixtures/store/api/applications.xlsx` & `cg-28.0.0/tests/fixtures/store/api/applications.xlsx`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/io/conftest.py` & `cg-28.0.0/tests/io/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/io/test_io_controller.py` & `cg-28.0.0/tests/io/test_io_controller.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/io/test_io_csv.py` & `cg-28.0.0/tests/io/test_io_csv.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/io/test_io_json.py` & `cg-28.0.0/tests/io/test_io_json.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/io/test_io_yaml.py` & `cg-28.0.0/tests/io/test_io_yaml.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/archive/conftest.py` & `cg-28.0.0/tests/meta/archive/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/archive/test_archiving.py` & `cg-28.0.0/tests/meta/archive/test_archiving.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/backup/conftest.py` & `cg-28.0.0/tests/meta/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/backup/test_meta_backup.py` & `cg-28.0.0/tests/meta/backup/test_meta_backup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Tests for the meta BackupAPI"""
 
 import logging
 import subprocess
 
 import mock
 import pytest
-from mock import call
+from mock import call, patch
 
 from cg.constants.sequencing import Sequencers
 from tests.mocks.hk_mock import MockFile
 
 from cg.apps.housekeeper.hk import HousekeeperAPI
 from cg.constants import FileExtensions, FlowCellStatus
 from cg.exc import ChecksumFailedError
@@ -28,17 +28,15 @@
         status=mock_store,
         tar_api=mock.Mock(),
         pdc_api=mock.Mock(),
         root_dir=mock.Mock(),
     )
 
     # WHEN there's already a flow cell being retrieved from PDC
-    mock_store.get_flow_cells_by_statuses(
-        flow_cell_statuses=[FlowCellStatus.PROCESSING]
-    ).count.return_value = 1
+    mock_store.get_flow_cells_by_statuses.return_value = [[mock.Mock()]]
 
     # THEN this method should return False
     assert backup_api.check_processing() is False
 
 
 @mock.patch("cg.store")
 def test_maximum_processing_queue_not_full(mock_store):
@@ -49,17 +47,15 @@
         encrypt_dir=mock.Mock(),
         status=mock_store,
         tar_api=mock.Mock(),
         pdc_api=mock.Mock(),
         root_dir=mock.Mock(),
     )
     # WHEN there are no flow cells being retrieved from PDC
-    mock_store.get_flow_cells_by_statuses(
-        flow_cell_statuses=[FlowCellStatus.PROCESSING]
-    ).count.return_value = 0
+    mock_store.get_flow_cells_by_statuses().return_value = []
 
     # THEN this method should return True
     assert backup_api.check_processing() is True
 
 
 @mock.patch("cg.store.models.Flowcell")
 @mock.patch("cg.store")
@@ -72,17 +68,15 @@
         status=mock_store,
         tar_api=mock.Mock(),
         pdc_api=mock.Mock(),
         root_dir=mock.Mock(),
     )
 
     # WHEN a flow cell is requested to be retrieved from PDC
-    mock_store.get_flow_cells_by_statuses(
-        flow_cell_statuses=[FlowCellStatus.REQUESTED]
-    ).first.return_value = mock_flow_cell
+    mock_store.get_flow_cells_by_statuses().return_value = [mock_flow_cell]
 
     popped_flow_cell = backup_api.get_first_flow_cell()
 
     # THEN a flow cell is returned
     assert popped_flow_cell is not None
 
 
@@ -96,17 +90,15 @@
         status=mock_store,
         tar_api=mock.Mock(),
         pdc_api=mock.Mock(),
         root_dir=mock.Mock(),
     )
 
     # WHEN there are no flow cells requested to be retrieved from PDC
-    mock_store.get_flow_cells_by_statuses(
-        flow_cell_statuses=[FlowCellStatus.REQUESTED]
-    ).first.return_value = None
+    mock_store.get_flow_cells_by_statuses.return_value = []
 
     popped_flow_cell = backup_api.get_first_flow_cell()
 
     # THEN no flow cell is returned
     assert popped_flow_cell is None
```

### Comparing `cg-27.3.9/tests/meta/backup/test_meta_pdc.py` & `cg-28.0.0/tests/meta/backup/test_meta_pdc.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/clean/conftest.py` & `cg-28.0.0/tests/meta/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/clean/test_clean_demultiplexed_runs.py` & `cg-28.0.0/tests/meta/clean/test_clean_demultiplexed_runs.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     flow_cell_path: Path,
     statusdb_return_value: Optional[Flowcell],
     result: bool,
     request,
 ):
     # GIVEN a flow cell that exists in statusdb
     flow_cell_path = request.getfixturevalue(flow_cell_path)
-    mock_statusdb.get_flow_cell.return_value = statusdb_return_value
+    mock_statusdb.get_flow_cell_by_name.return_value = statusdb_return_value
     mock_hk.files.return_value.count.return_value = 1
     flow_cell_obj = DemultiplexedRunsFlowCell(
         flow_cell_path=flow_cell_path,
         status_db=mock_statusdb,
         housekeeper_api=mock_hk,
         trailblazer_api=mock_tb,
     )
```

### Comparing `cg-27.3.9/tests/meta/clean/test_clean_flow_cell_run_directories.py` & `cg-28.0.0/tests/meta/clean/test_clean_flow_cell_run_directories.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     mock_statusdb,
     mock_hk,
     flow_cell_path,
     timestamp_yesterday,
 ):
     # GIVEN a flow cell with a sequenced_at date in statusdb
     flow_cell: RunDirFlowCell = RunDirFlowCell(flow_cell_path, mock_statusdb, mock_hk)
-    mock_statusdb.get_flow_cell.return_value.sequenced_at = timestamp_yesterday
+    mock_statusdb.get_flow_cell_by_name.return_value.sequenced_at = timestamp_yesterday
 
     # WHEN determining the age of a flow cell
     result = flow_cell.sequenced_date
 
     # THEN the sequenced_date property of the flow cell should be set to the sequenced_at date in
     # statusdb
     assert result == timestamp_yesterday
@@ -52,15 +52,15 @@
 def test_sequenced_date_from_run_name(
     mock_statusdb,
     mock_hk,
     flow_cell_path,
 ):
     # GIVEN a flow cell that does not exist in statusdb
     flow_cell: RunDirFlowCell = RunDirFlowCell(flow_cell_path, mock_statusdb, mock_hk)
-    mock_statusdb.get_flow_cell.return_value = None
+    mock_statusdb.get_flow_cell_by_name.return_value = None
 
     # WHEN determining the age of a flow cell
     result = flow_cell.sequenced_date
 
     # THEN the sequenced_date property of the flow cell should be derived from the run name of
     # the flow cell
     assert result == flow_cell.derived_date
```

### Comparing `cg-27.3.9/tests/meta/compress/conftest.py` & `cg-28.0.0/tests/meta/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/compress/test_clean_fastq.py` & `cg-28.0.0/tests/meta/compress/test_clean_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/compress/test_compress_files.py` & `cg-28.0.0/tests/meta/compress/test_compress_files.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/compress/test_compress_meta_fastq.py` & `cg-28.0.0/tests/meta/compress/test_compress_meta_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/compress/test_decompress_spring_meta.py` & `cg-28.0.0/tests/meta/compress/test_decompress_spring_meta.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/compress/test_meta_compress_update_hk.py` & `cg-28.0.0/tests/meta/compress/test_meta_compress_update_hk.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/conftest.py` & `cg-28.0.0/tests/meta/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/deliver/conftest.py` & `cg-28.0.0/tests/meta/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/deliver/test_deliver_ticket.py` & `cg-28.0.0/tests/meta/deliver/test_deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/deliver/test_delivery_api.py` & `cg-28.0.0/tests/meta/deliver/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/demultiplex/conftest.py` & `cg-28.0.0/tests/meta/demultiplex/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     helpers.add_relationship(
         store=populated_flow_cell_store,
         sample=sample,
         case=family,
     )
     helpers.add_flowcell(
         store=populated_flow_cell_store,
-        flow_cell_id=flow_cell_id,
+        flow_cell_name=flow_cell_id,
         sequencer_type="novaseq",
         samples=[sample],
     )
     return populated_flow_cell_store
 
 
 @pytest.fixture(name="active_flow_cell_store")
@@ -132,15 +132,15 @@
     helpers.add_relationship(
         store=active_flow_cell_store,
         sample=sample,
         case=family,
     )
     helpers.add_flowcell(
         store=active_flow_cell_store,
-        flow_cell_id=flow_cell_id,
+        flow_cell_name=flow_cell_id,
         sequencer_type="novaseq",
         samples=[sample],
     )
     return active_flow_cell_store
 
 
 @pytest.fixture(name="sample_level_housekeeper_api")
```

### Comparing `cg-27.3.9/tests/meta/demultiplex/test_delete_demultiplex_api.py` & `cg-28.0.0/tests/meta/demultiplex/test_delete_demultiplex_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     empty_presence: bool = wipe_demux_api.status_db_presence
 
     # THEN there should be an appropriate presence in both cases
     assert not empty_presence
 
     # WHEN adding a flowcell into the statusdb and checking its updated presence
     helpers.add_flowcell(
-        store=wipe_demux_api.status_db, flow_cell_id=flow_cell_id, sequencer_type="novaseq"
+        store=wipe_demux_api.status_db, flow_cell_name=flow_cell_id, sequencer_type="novaseq"
     )
     populated_presence: bool = wipe_demux_api.status_db_presence
 
     # THEN the presence should be updated
     assert populated_presence
 
 
@@ -303,15 +303,17 @@
     tmp_demulitplexing_dir: Path,
     tmp_flow_cell_run_path: Path,
 ):
     """Test if function to remove files from the file system is working"""
 
     caplog.set_level(logging.INFO)
     wipe_demux_api: DeleteDemuxAPI = populated_wipe_demultiplex_api
-    flow_cell_obj: Flowcell = wipe_demux_api.status_db.get_flow_cell(wipe_demux_api.flow_cell_name)
+    flow_cell_obj: Flowcell = wipe_demux_api.status_db.get_flow_cell_by_name(
+        wipe_demux_api.flow_cell_name
+    )
     wipe_demux_api.set_dry_run(dry_run=False)
 
     # GIVEN an existing demultiplexing and run directory of a flow cell, with a status "ondisk"
 
     assert tmp_demulitplexing_dir.exists()
     assert tmp_flow_cell_run_path.exists()
     assert flow_cell_obj.status == "ondisk"
```

### Comparing `cg-27.3.9/tests/meta/demultiplex/test_demux_post_processing.py` & `cg-28.0.0/tests/meta/demultiplex/test_demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/demultiplex/test_rename_files.py` & `cg-28.0.0/tests/meta/demultiplex/test_rename_files.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/encryption/conftest.py` & `cg-28.0.0/tests/meta/encryption/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/encryption/test_encryption.py` & `cg-28.0.0/tests/meta/encryption/test_encryption.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/observations/conftest.py` & `cg-28.0.0/tests/meta/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/observations/test_meta_upload_observations.py` & `cg-28.0.0/tests/meta/observations/test_meta_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/orders/conftest.py` & `cg-28.0.0/tests/meta/orders/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/orders/test_PoolSubmitter_validate_order.py` & `cg-28.0.0/tests/meta/orders/test_PoolSubmitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py` & `cg-28.0.0/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/orders/test_SarsCov2Submitter_store_order.py` & `cg-28.0.0/tests/meta/orders/test_SarsCov2Submitter_store_order.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/orders/test_SarsCov2Submitter_validate_order.py` & `cg-28.0.0/tests/meta/orders/test_SarsCov2Submitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/orders/test_meta_orders_api.py` & `cg-28.0.0/tests/meta/orders/test_meta_orders_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/orders/test_meta_orders_lims.py` & `cg-28.0.0/tests/meta/orders/test_meta_orders_lims.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/orders/test_meta_orders_status.py` & `cg-28.0.0/tests/meta/orders/test_meta_orders_status.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/orders/test_ticket_handler.py` & `cg-28.0.0/tests/meta/orders/test_ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/report/conftest.py` & `cg-28.0.0/tests/meta/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/report/test_balsamic_api.py` & `cg-28.0.0/tests/meta/report/test_balsamic_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/report/test_field_validators.py` & `cg-28.0.0/tests/meta/report/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/report/test_mip_dna_api.py` & `cg-28.0.0/tests/meta/report/test_mip_dna_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/report/test_report_api.py` & `cg-28.0.0/tests/meta/report/test_report_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/rsync/conftest.py` & `cg-28.0.0/tests/meta/rsync/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/rsync/test_rsync.py` & `cg-28.0.0/tests/meta/rsync/test_rsync.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/test_invoice.py` & `cg-28.0.0/tests/meta/test_invoice.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/transfer/conftest.py` & `cg-28.0.0/tests/meta/transfer/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/transfer/test_external_data.py` & `cg-28.0.0/tests/meta/transfer/test_external_data.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/transfer/test_meta_transfer_flowcell.py` & `cg-28.0.0/tests/meta/transfer/test_meta_transfer_flowcell.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 def test_add_flow_cell_to_status_db(
     transfer_flow_cell_api: Generator[TransferFlowCell, None, None], yet_another_flow_cell_id: str
 ):
     """Test adding flow cell to Status db."""
     # GIVEN transfer flow cell API
 
     # GIVEN a flow cell that does not exist in status db
-    flow_cell: Flowcell = transfer_flow_cell_api.db.get_flow_cell(
-        flow_cell_id=yet_another_flow_cell_id
+    flow_cell: Flowcell = transfer_flow_cell_api.db.get_flow_cell_by_name(
+        flow_cell_name=yet_another_flow_cell_id
     )
 
     assert flow_cell is None
 
     # GIVEN a cgstats flow cell
     cgstats_flow_cell: StatsFlowcell = transfer_flow_cell_api.stats.flowcell(
         yet_another_flow_cell_id
@@ -71,16 +71,18 @@
     helpers: StoreHelpers,
     transfer_flow_cell_api: Generator[TransferFlowCell, None, None],
 ):
     """Test adding flow cell to Status db, when already present."""
     # GIVEN transfer flow cell API
 
     # GIVEN a flow cell that exist in status db
-    helpers.add_flowcell(store=flowcell_store, flow_cell_id=flow_cell_id)
-    flow_cell: Flowcell = transfer_flow_cell_api.db.get_flow_cell(flow_cell_id=flow_cell_id)
+    helpers.add_flowcell(store=flowcell_store, flow_cell_name=flow_cell_id)
+    flow_cell: Flowcell = transfer_flow_cell_api.db.get_flow_cell_by_name(
+        flow_cell_name=flow_cell_id
+    )
 
     assert flow_cell is not None
 
     # GIVEN a cgstats flow cell
     cgstats_flow_cell: StatsFlowcell = transfer_flow_cell_api.stats.flowcell(flow_cell_id)
 
     # WHEN adding flow cell to status db
@@ -360,15 +362,15 @@
     # GIVEN a cgstats flow cell
     cgstats_flow_cell: StatsFlowcell = transfer_flow_cell_api.stats.flowcell(
         yet_another_flow_cell_id
     )
 
     # GIVEN a flow cell that exist in status db
     flow_cell: Flowcell = helpers.add_flowcell(
-        store=flowcell_store, flow_cell_id=yet_another_flow_cell_id
+        store=flowcell_store, flow_cell_name=yet_another_flow_cell_id
     )
 
     # GIVEN no sample in flow cell
     assert len(flow_cell.samples) == 0
 
     # WHEN parsing the flow cell samples
     transfer_flow_cell_api._parse_flow_cell_samples(
@@ -397,15 +399,15 @@
     )
 
     # GIVEN a sample name that does not exist in cgstats
     cgstats_flow_cell.samples[0].name = "sample_does_not_exist_in_cgstats"
 
     # GIVEN a flow cell that exist in status db
     flow_cell: Flowcell = helpers.add_flowcell(
-        store=flowcell_store, flow_cell_id=yet_another_flow_cell_id
+        store=flowcell_store, flow_cell_name=yet_another_flow_cell_id
     )
 
     # GIVEN no sample in flow cell
     assert len(flow_cell.samples) == 0
 
     # WHEN parsing the flow cell samples
     transfer_flow_cell_api._parse_flow_cell_samples(
```

### Comparing `cg-27.3.9/tests/meta/transfer/test_meta_transfer_lims.py` & `cg-28.0.0/tests/meta/transfer/test_meta_transfer_lims.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/upload/balsamic/test_balsamic.py` & `cg-28.0.0/tests/meta/upload/balsamic/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/upload/conftest.py` & `cg-28.0.0/tests/meta/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/upload/gisaid/conftest.py` & `cg-28.0.0/tests/meta/upload/gisaid/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/upload/gisaid/fixtures/four_samples.csv` & `cg-28.0.0/tests/meta/upload/gisaid/fixtures/four_samples.csv`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/upload/mutacc/conftest.py` & `cg-28.0.0/tests/meta/upload/mutacc/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/upload/mutacc/test_meta_upload_mutacc.py` & `cg-28.0.0/tests/meta/upload/mutacc/test_meta_upload_mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/upload/nipt/conftest.py` & `cg-28.0.0/tests/meta/upload/nipt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/upload/nipt/test_nipt_upload_api.py` & `cg-28.0.0/tests/meta/upload/nipt/test_nipt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/upload/scout/conftest.py` & `cg-28.0.0/tests/meta/upload/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/upload/scout/test_generate_load_config.py` & `cg-28.0.0/tests/meta/upload/scout/test_generate_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/upload/scout/test_meta_upload_scoutapi.py` & `cg-28.0.0/tests/meta/upload/scout/test_meta_upload_scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py` & `cg-28.0.0/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/upload/scout/test_scout_config_builder.py` & `cg-28.0.0/tests/meta/upload/scout/test_scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/upload/test_meta_upload_coverage.py` & `cg-28.0.0/tests/meta/upload/test_meta_upload_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/upload/test_upload_api.py` & `cg-28.0.0/tests/meta/upload/test_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/upload/test_upload_genotypes_api.py` & `cg-28.0.0/tests/meta/upload/test_upload_genotypes_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/upload/vogue/conftest.py` & `cg-28.0.0/tests/meta/upload/vogue/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/upload/vogue/test_upload_vogue.py` & `cg-28.0.0/tests/meta/upload/vogue/test_upload_vogue.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/workflow/conftest.py` & `cg-28.0.0/tests/meta/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/workflow/test_analysis.py` & `cg-28.0.0/tests/meta/workflow/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/workflow/test_balsamic.py` & `cg-28.0.0/tests/meta/workflow/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/workflow/test_microsalt.py` & `cg-28.0.0/tests/meta/workflow/test_microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/meta/workflow/test_prepare_fastq_api.py` & `cg-28.0.0/tests/meta/workflow/test_prepare_fastq_api.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/mocks/balsamic_analysis_mock.py` & `cg-28.0.0/tests/mocks/balsamic_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/mocks/crunchy.py` & `cg-28.0.0/tests/mocks/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/mocks/hk_mock.py` & `cg-28.0.0/tests/mocks/hk_mock.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/mocks/limsmock.py` & `cg-28.0.0/tests/mocks/limsmock.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/mocks/madeline.py` & `cg-28.0.0/tests/mocks/madeline.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/mocks/mip_analysis_mock.py` & `cg-28.0.0/tests/mocks/mip_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/mocks/osticket.py` & `cg-28.0.0/tests/mocks/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/mocks/process_mock.py` & `cg-28.0.0/tests/mocks/process_mock.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/mocks/report.py` & `cg-28.0.0/tests/mocks/report.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/mocks/scout.py` & `cg-28.0.0/tests/mocks/scout.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/mocks/store_model.py` & `cg-28.0.0/tests/mocks/store_model.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/mocks/tb_mock.py` & `cg-28.0.0/tests/mocks/tb_mock.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/models/balsamic/conftest.py` & `cg-28.0.0/tests/models/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/models/balsamic/test_balsamic_analysis.py` & `cg-28.0.0/tests/models/balsamic/test_balsamic_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/models/conftest.py` & `cg-28.0.0/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/models/demultiplexing/conftest.py` & `cg-28.0.0/tests/models/demultiplexing/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/models/demultiplexing/test_demux_results.py` & `cg-28.0.0/tests/models/demultiplexing/test_demux_results.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/models/demultiplexing/test_flowcell_model.py` & `cg-28.0.0/tests/models/demultiplexing/test_flowcell_model.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/models/mip/conftest.py` & `cg-28.0.0/tests/models/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/models/mip/test_mip_analysis.py` & `cg-28.0.0/tests/models/mip/test_mip_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/models/mip/test_mip_config.py` & `cg-28.0.0/tests/models/mip/test_mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/models/mip/test_mip_metrics_deliverables.py` & `cg-28.0.0/tests/models/mip/test_mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/models/mip/test_mip_sample_info.py` & `cg-28.0.0/tests/models/mip/test_mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/models/nextflow/conftest.py` & `cg-28.0.0/tests/models/nextflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/models/nextflow/test_nextflow_deliver.py` & `cg-28.0.0/tests/models/nextflow/test_nextflow_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/models/observations/conftest.py` & `cg-28.0.0/tests/models/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/models/observations/test_observations_input_files.py` & `cg-28.0.0/tests/models/observations/test_observations_input_files.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/models/report/test_validators.py` & `cg-28.0.0/tests/models/report/test_validators.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/models/rnafusion/conftest.py` & `cg-28.0.0/tests/models/rnafusion/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/models/rnafusion/test_rnafusion_sample.py` & `cg-28.0.0/tests/models/rnafusion/test_rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/models/test_cg_models.py` & `cg-28.0.0/tests/models/test_cg_models.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/models/test_compression_data.py` & `cg-28.0.0/tests/models/test_compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/models/test_file_data.py` & `cg-28.0.0/tests/models/test_file_data.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/models/test_flowcell_class.py` & `cg-28.0.0/tests/models/test_flowcell_class.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/server/conftest.py` & `cg-28.0.0/tests/server/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/api/add/test_store_add_application_version.py` & `cg-28.0.0/tests/store/api/add/test_store_add_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/api/add/test_store_add_base.py` & `cg-28.0.0/tests/store/api/add/test_store_add_base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/api/add/test_store_add_customer.py` & `cg-28.0.0/tests/store/api/add/test_store_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/api/add/test_store_add_flow_celll.py` & `cg-28.0.0/tests/store/api/add/test_store_add_flow_celll.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ):
     """Test adding a flow cell to the database."""
 
     # GIVEN a database with no flow cell
 
     # WHEN adding flow cell
     flow_cell: Flowcell = base_store.add_flow_cell(
-        flow_cell_id=flow_cell_id,
+        flow_cell_name=flow_cell_id,
         sequencer_name=sequencer_name,
         sequencer_type=Sequencers.NOVASEQ,
         date=timestamp_now,
         flow_cell_status=FlowCellStatus.ON_DISK,
     )
 
     # THEN flow cell should be returned
@@ -43,15 +43,15 @@
 ):
     """Test adding a flow cell with a status to the database."""
 
     # GIVEN a database with no flow cell
 
     # WHEN adding flow cell
     flow_cell: Flowcell = base_store.add_flow_cell(
-        flow_cell_id=flow_cell_id,
+        flow_cell_name=flow_cell_id,
         sequencer_name=sequencer_name,
         sequencer_type=Sequencers.NOVASEQ,
         date=timestamp_now,
         flow_cell_status=FlowCellStatus.PROCESSING,
     )
 
     # THEN the flow cell status should be "processing"
```

### Comparing `cg-27.3.9/tests/store/api/conftest.py` & `cg-28.0.0/tests/store/api/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,22 +273,22 @@
         sequenced_at=timestamp_now,
     )
 
     one_day_ahead_of_now = timestamp_now + dt.timedelta(days=1)
 
     helpers.add_flowcell(
         store=re_sequenced_sample_store,
-        flow_cell_id=another_flow_cell_id,
+        flow_cell_name=another_flow_cell_id,
         samples=[store_sample],
         date=timestamp_now,
     )
 
     helpers.add_flowcell(
         store=re_sequenced_sample_store,
-        flow_cell_id=flow_cell_id,
+        flow_cell_name=flow_cell_id,
         samples=[store_sample],
         date=one_day_ahead_of_now,
     )
 
     helpers.add_relationship(store=re_sequenced_sample_store, case=store_case, sample=store_sample)
 
     return re_sequenced_sample_store
```

### Comparing `cg-27.3.9/tests/store/api/delete/test_store_api_delete.py` & `cg-28.0.0/tests/store/api/delete/test_store_api_delete.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 from cg.store.models import Flowcell, Family, FamilySample, Sample
 
 
 def test_delete_flow_cell(flow_cell_id: str, populated_flow_cell_store: Store):
     """Test deleting a flow cell in Store."""
 
     # GIVEN a database containing a flow cell
-    flow_cell: Flowcell = populated_flow_cell_store.get_flow_cell(flow_cell_id=flow_cell_id)
+    flow_cell: Flowcell = populated_flow_cell_store.get_flow_cell_by_name(
+        flow_cell_name=flow_cell_id
+    )
 
     assert flow_cell
 
     # WHEN removing flow cell
     populated_flow_cell_store.delete_flow_cell(flow_cell_id=flow_cell_id)
 
     # THEN no entry should be found for the flow cell
-    results: Flowcell = populated_flow_cell_store.get_flow_cell(flow_cell_id=flow_cell_id)
+    results: Flowcell = populated_flow_cell_store.get_flow_cell_by_name(flow_cell_name=flow_cell_id)
 
     assert not results
 
 
 def test_store_api_delete_relationships_between_sample_and_cases(
     sample_id_in_single_case: str,
     sample_id_in_multiple_cases: str,
```

### Comparing `cg-27.3.9/tests/store/api/find/test_find_basic_data.py` & `cg-28.0.0/tests/store/api/find/test_find_basic_data.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/api/find/test_find_basic_data_application_version.py` & `cg-28.0.0/tests/store/api/find/test_find_basic_data_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/api/find/test_find_business_data.py` & `cg-28.0.0/tests/store/api/find/test_find_business_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,15 +71,17 @@
 
 def test_get_flow_cell(flow_cell_id: str, re_sequenced_sample_store: Store):
     """Test returning the latest flow cell from the database."""
 
     # GIVEN a store with two flow cells
 
     # WHEN fetching the latest flow cell
-    flow_cell: Flowcell = re_sequenced_sample_store.get_flow_cell(flow_cell_id=flow_cell_id)
+    flow_cell: Flowcell = re_sequenced_sample_store.get_flow_cell_by_name(
+        flow_cell_name=flow_cell_id
+    )
 
     # THEN the returned flow cell should have the same name as the one in the database
     assert flow_cell.name == flow_cell_id
 
 
 def test_get_flow_cell_by_name_pattern(flow_cell_id: str, re_sequenced_sample_store: Store):
     """Test returning the latest flow cell from the database by enquiry."""
@@ -102,17 +104,17 @@
     case_obj: Family,
     helpers: StoreHelpers,
     sample_obj: Sample,
 ):
     """Test returning the latest flow cell from the database by case."""
 
     # GIVEN a store with two flow cell
-    helpers.add_flowcell(store=base_store, flow_cell_id=flow_cell_id, samples=[sample_obj])
+    helpers.add_flowcell(store=base_store, flow_cell_name=flow_cell_id, samples=[sample_obj])
 
-    helpers.add_flowcell(store=base_store, flow_cell_id=another_flow_cell_id)
+    helpers.add_flowcell(store=base_store, flow_cell_name=another_flow_cell_id)
 
     # WHEN fetching the latest flow cell
     flow_cells: List[Flowcell] = base_store.get_flow_cells_by_case(case=case_obj)
 
     # THEN the flow cell samples for the case should be returned
     for flow_cell in flow_cells:
         for sample in flow_cell.samples:
@@ -261,22 +263,22 @@
     sample_obj: Sample,
 ):
     """Test check if all flow cells for samples on a case is on disk when not on disk."""
     caplog.set_level(logging.DEBUG)
     # GIVEN a store with two flow cell
     flow_cell = helpers.add_flowcell(
         store=base_store,
-        flow_cell_id=flow_cell_id,
+        flow_cell_name=flow_cell_id,
         samples=[sample_obj],
         status=FlowCellStatus.PROCESSING,
     )
 
     another_flow_cell = helpers.add_flowcell(
         store=base_store,
-        flow_cell_id=another_flow_cell_id,
+        flow_cell_name=another_flow_cell_id,
         samples=[sample_obj],
         status=FlowCellStatus.RETRIEVED,
     )
 
     # WHEN fetching the latest flow cell
     is_on_disk = base_store.is_all_flow_cells_on_disk(case_id=case_id)
 
@@ -298,22 +300,22 @@
     sample_obj: Sample,
 ):
     """Test check if all flow cells for samples on a case is on disk when requested."""
     caplog.set_level(logging.DEBUG)
     # GIVEN a store with two flow cell
     flow_cell = helpers.add_flowcell(
         store=base_store,
-        flow_cell_id=flow_cell_id,
+        flow_cell_name=flow_cell_id,
         samples=[sample_obj],
         status=FlowCellStatus.REMOVED,
     )
 
     another_flow_cell = helpers.add_flowcell(
         store=base_store,
-        flow_cell_id=another_flow_cell_id,
+        flow_cell_name=another_flow_cell_id,
         samples=[sample_obj],
         status=FlowCellStatus.REQUESTED,
     )
 
     # WHEN fetching the latest flow cell
     is_on_disk = base_store.is_all_flow_cells_on_disk(case_id=case_id)
 
@@ -336,18 +338,18 @@
     helpers: StoreHelpers,
     sample_obj: Sample,
 ):
     """Test check if all flow cells for samples on a case is on disk."""
     caplog.set_level(logging.DEBUG)
     # GIVEN a store with two flow cell
     flow_cell = helpers.add_flowcell(
-        store=base_store, flow_cell_id=flow_cell_id, samples=[sample_obj]
+        store=base_store, flow_cell_name=flow_cell_id, samples=[sample_obj]
     )
 
-    helpers.add_flowcell(store=base_store, flow_cell_id=another_flow_cell_id)
+    helpers.add_flowcell(store=base_store, flow_cell_name=another_flow_cell_id)
 
     # WHEN fetching the latest flow cell
     is_on_disk = base_store.is_all_flow_cells_on_disk(case_id=case_id)
 
     # THEN return true
     assert is_on_disk is True
```

### Comparing `cg-27.3.9/tests/store/api/find/test_find_business_data_analysis.py` & `cg-28.0.0/tests/store/api/find/test_find_business_data_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/api/find/test_find_business_data_case.py` & `cg-28.0.0/tests/store/api/find/test_find_business_data_case.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/api/find/test_find_business_data_sample.py` & `cg-28.0.0/tests/store/api/find/test_find_business_data_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/api/status/test_analyses_to_clean.py` & `cg-28.0.0/tests/store/api/status/test_analyses_to_clean.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/api/status/test_analyses_to_delivery_report.py` & `cg-28.0.0/tests/store/api/status/test_analyses_to_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/api/status/test_store_api_status.py` & `cg-28.0.0/tests/store/api/status/test_store_api_status.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/api/status/test_store_api_status_analysis.py` & `cg-28.0.0/tests/store/api/status/test_store_api_status_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/api/status/test_store_api_status_cases.py` & `cg-28.0.0/tests/store/api/status/test_store_api_status_cases.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/api/status/test_store_api_status_customer.py` & `cg-28.0.0/tests/store/api/status/test_store_api_status_customer.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/api/status/test_store_api_status_pool.py` & `cg-28.0.0/tests/store/api/status/test_store_api_status_pool.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/api/status/test_store_api_status_sample.py` & `cg-28.0.0/tests/store/api/status/test_store_api_status_sample.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/api/test_base.py` & `cg-28.0.0/tests/store/api/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/api/test_store_import_func.py` & `cg-28.0.0/tests/store/api/test_store_import_func.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/conftest.py` & `cg-28.0.0/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/filters/test_status_analyses_filters.py` & `cg-28.0.0/tests/store/filters/test_status_analyses_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/filters/test_status_application_filters.py` & `cg-28.0.0/tests/store/filters/test_status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/filters/test_status_application_version_filters.py` & `cg-28.0.0/tests/store/filters/test_status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/filters/test_status_bed_filters.py` & `cg-28.0.0/tests/store/filters/test_status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/filters/test_status_bed_version_filters.py` & `cg-28.0.0/tests/store/filters/test_status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/filters/test_status_case_sample_filters.py` & `cg-28.0.0/tests/store/filters/test_status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/filters/test_status_cases_filters.py` & `cg-28.0.0/tests/store/filters/test_status_cases_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/filters/test_status_collaboration_filters.py` & `cg-28.0.0/tests/store/filters/test_status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/filters/test_status_flow_cell_filters.py` & `cg-28.0.0/tests/store/filters/test_status_flow_cell_filters.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from sqlalchemy.orm import Query
 
 from cg.constants import FlowCellStatus
 from cg.store import Store
 from cg.store.models import Flowcell, Family, Sample
 from cg.store.filters.status_flow_cell_filters import (
-    filter_flow_cell_by_id,
     filter_flow_cells_with_statuses,
+    get_flow_cell_by_name,
     filter_flow_cells_by_case,
-    filter_flow_cell_by_name_pattern,
+    filter_flow_cell_by_name_search,
 )
 from tests.store_helpers import StoreHelpers
 
 
 def test_get_flow_cells_by_case(
     base_store: Store,
     case_id: str,
@@ -21,15 +21,15 @@
     flow_cell_id: str,
     helpers: StoreHelpers,
     sample_obj: Sample,
 ):
     """Test that a flow cell is returned when there is a flow cell with matching flow cell case."""
 
     # GIVEN a flow cell that exist in status db
-    helpers.add_flowcell(store=base_store, flow_cell_id=flow_cell_id, samples=[sample_obj])
+    helpers.add_flowcell(store=base_store, flow_cell_name=flow_cell_id, samples=[sample_obj])
 
     # GIVEN a flow cell Query
 
     # WHEN getting flow cell
     returned_flow_cell: Optional[List[Flowcell]] = filter_flow_cells_by_case(
         flow_cells=base_store._get_join_flow_cell_sample_links_query(), case=case_obj
     )
@@ -62,55 +62,55 @@
     assert not list(returned_flow_cell)
 
 
 def test_get_flow_cell_by_id(base_store: Store, helpers: StoreHelpers, flow_cell_id: str):
     """Test that a flow cell is returned when there is a flow cell with matching flow cell id."""
 
     # GIVEN a flow cell that exist in status db
-    flow_cell: Flowcell = helpers.add_flowcell(store=base_store, flow_cell_id=flow_cell_id)
+    flow_cell: Flowcell = helpers.add_flowcell(store=base_store, flow_cell_name=flow_cell_id)
 
     # GIVEN a flow cell Query
 
     # WHEN getting flow cell
-    returned_flow_cell: Flowcell = filter_flow_cell_by_id(
-        flow_cells=base_store._get_query(table=Flowcell), flow_cell_id=flow_cell_id
+    returned_flow_cell: Flowcell = get_flow_cell_by_name(
+        flow_cells=base_store._get_query(table=Flowcell), flow_cell_name=flow_cell_id
     )
 
     # THEN returned flow cell should be the original flow cell
     assert isinstance(returned_flow_cell, Query)
 
     assert flow_cell is returned_flow_cell.first()
 
 
 def test_get_flow_cell_by_id_and_by_enquiry(
     base_store: Store, helpers: StoreHelpers, flow_cell_id: str
 ):
     """Test that a flow cell is returned when there is a flow cell with enquiry flow cell id."""
 
     # GIVEN a flow cell that exist in status db
-    flow_cell: Flowcell = helpers.add_flowcell(store=base_store, flow_cell_id=flow_cell_id)
+    flow_cell: Flowcell = helpers.add_flowcell(store=base_store, flow_cell_name=flow_cell_id)
 
     # GIVEN a flow cell Query
 
     # WHEN getting flow cell
-    returned_flow_cell: List[Flowcell] = filter_flow_cell_by_name_pattern(
-        flow_cells=base_store._get_query(table=Flowcell), name_pattern=flow_cell_id[:4]
+    returned_flow_cell: List[Flowcell] = filter_flow_cell_by_name_search(
+        flow_cells=base_store._get_query(table=Flowcell), name_search=flow_cell_id[:4]
     )
 
     # THEN a list of flow cells should be returned
     assert isinstance(returned_flow_cell[0], Flowcell)
 
     assert flow_cell is returned_flow_cell[0]
 
 
 def test_get_flow_cells_with_statuses(base_store: Store, helpers: StoreHelpers, flow_cell_id: str):
     """Test that a flow cell is returned when there is a flow cell with matching flow cell id."""
 
     # GIVEN a flow cell that exist in status db
-    helpers.add_flowcell(store=base_store, flow_cell_id=flow_cell_id)
+    helpers.add_flowcell(store=base_store, flow_cell_name=flow_cell_id)
 
     # GIVEN a flow cell Query
 
     # WHEN getting flow cell
     returned_flow_cell_query: Query = filter_flow_cells_with_statuses(
         flow_cells=base_store._get_query(table=Flowcell),
         flow_cell_statuses=[FlowCellStatus.ON_DISK, FlowCellStatus.PROCESSING],
```

### Comparing `cg-27.3.9/tests/store/filters/test_status_invoice_filters.py` & `cg-28.0.0/tests/store/filters/test_status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/filters/test_status_organism_filters.py` & `cg-28.0.0/tests/store/filters/test_status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/filters/test_status_panel_filters.py` & `cg-28.0.0/tests/store/filters/test_status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/filters/test_status_pool_filters.py` & `cg-28.0.0/tests/store/filters/test_status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/filters/test_status_samples_filters.py` & `cg-28.0.0/tests/store/filters/test_status_samples_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/filters/test_status_user_filters.py` & `cg-28.0.0/tests/store/filters/test_status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/test_delivery.py` & `cg-28.0.0/tests/store/test_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store/test_store_models.py` & `cg-28.0.0/tests/store/test_store_models.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/store_helpers.py` & `cg-28.0.0/tests/store_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -578,24 +578,24 @@
         return [
             StoreHelpers.add_sample(store, str(sample_id)) for sample_id in range(1, nr_samples)
         ]
 
     @staticmethod
     def add_flowcell(
         store: Store,
-        flow_cell_id: str = "flowcell_test",
+        flow_cell_name: str = "flowcell_test",
         archived_at: datetime = None,
         sequencer_type: str = Sequencers.HISEQX,
         samples: List[Sample] = None,
         status: str = None,
         date: datetime = datetime.now(),
     ) -> Flowcell:
         """Utility function to add a flow cell to the store and return an object."""
         flow_cell = store.add_flow_cell(
-            flow_cell_id=flow_cell_id,
+            flow_cell_name=flow_cell_name,
             sequencer_name="dummy_sequencer",
             sequencer_type=sequencer_type,
             date=date,
         )
         flow_cell.archived_at = archived_at
         if samples:
             flow_cell.samples = samples
```

### Comparing `cg-27.3.9/tests/test_store_helpers.py` & `cg-28.0.0/tests/test_store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/utils/conftest.py` & `cg-28.0.0/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/utils/test_commands.py` & `cg-28.0.0/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/utils/test_date.py` & `cg-28.0.0/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/utils/test_dict.py` & `cg-28.0.0/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/utils/test_dispatcher.py` & `cg-28.0.0/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-27.3.9/tests/utils/test_utils.py` & `cg-28.0.0/tests/utils/test_utils.py`

 * *Files identical despite different names*

