# Comparing `tmp/ilus-1.3.1.tar.gz` & `tmp/ilus-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ilus-1.3.1.tar", last modified: Mon Feb 27 16:13:52 2023, max compression
+gzip compressed data, was "dist/ilus-1.3.2.tar", last modified: Tue Apr 18 07:21:33 2023, max compression
```

## Comparing `ilus-1.3.1.tar` & `ilus-1.3.2.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-02-27 16:13:52.282384 ilus-1.3.1/
--rw-r--r--   0 huangshujia   (501) staff       (20)    35137 2023-02-06 08:38:34.000000 ilus-1.3.1/LICENSE
--rw-r--r--   0 huangshujia   (501) staff       (20)    33281 2023-02-27 16:13:52.281365 ilus-1.3.1/PKG-INFO
--rw-r--r--   0 huangshujia   (501) staff       (20)    32397 2023-02-08 06:59:40.000000 ilus-1.3.1/README.md
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-02-27 16:13:52.226884 ilus-1.3.1/ilus/
--rw-r--r--   0 huangshujia   (501) staff       (20)        0 2018-11-29 10:13:48.000000 ilus-1.3.1/ilus/__init__.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-02-27 16:13:52.234516 ilus-1.3.1/ilus/launch/
--rw-r--r--   0 huangshujia   (501) staff       (20)        0 2018-11-29 10:13:48.000000 ilus-1.3.1/ilus/launch/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)     3307 2022-07-20 03:59:17.000000 ilus-1.3.1/ilus/launch/do.py
--rw-r--r--   0 huangshujia   (501) staff       (20)    23084 2023-02-27 15:51:49.000000 ilus-1.3.1/ilus/launch/runfunction.py
--rw-r--r--   0 huangshujia   (501) staff       (20)     5512 2023-02-27 16:13:13.000000 ilus-1.3.1/ilus/main.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-02-27 16:13:52.236489 ilus-1.3.1/ilus/modules/
--rw-r--r--   0 huangshujia   (501) staff       (20)        0 2018-11-29 10:13:48.000000 ilus-1.3.1/ilus/modules/__init__.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-02-27 16:13:52.237532 ilus-1.3.1/ilus/modules/ngsaligner/
--rw-r--r--   0 huangshujia   (501) staff       (20)        0 2018-11-29 10:13:48.000000 ilus-1.3.1/ilus/modules/ngsaligner/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)     1541 2023-02-16 03:32:18.000000 ilus-1.3.1/ilus/modules/ngsaligner/bwa.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-02-27 16:13:52.239433 ilus-1.3.1/ilus/modules/summary/
--rw-r--r--   0 huangshujia   (501) staff       (20)        0 2020-04-29 06:48:45.000000 ilus-1.3.1/ilus/modules/summary/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)     1643 2023-02-22 01:03:58.000000 ilus-1.3.1/ilus/modules/summary/bam.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-02-27 16:13:52.257660 ilus-1.3.1/ilus/modules/utils/
--rw-r--r--   0 huangshujia   (501) staff       (20)      175 2023-02-21 08:25:02.000000 ilus-1.3.1/ilus/modules/utils/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)      976 2023-02-24 01:22:28.000000 ilus-1.3.1/ilus/modules/utils/_check_jobs.py
--rw-r--r--   0 huangshujia   (501) staff       (20)     4069 2023-02-21 09:01:14.000000 ilus-1.3.1/ilus/modules/utils/_check_samplesheet.py
--rw-r--r--   0 huangshujia   (501) staff       (20)     2778 2023-02-21 05:55:33.000000 ilus-1.3.1/ilus/modules/utils/_split_jobs.py
--rw-r--r--   0 huangshujia   (501) staff       (20)      891 2023-02-21 03:35:30.000000 ilus-1.3.1/ilus/modules/utils/_utils.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-02-27 16:13:52.261947 ilus-1.3.1/ilus/modules/variants/
--rw-r--r--   0 huangshujia   (501) staff       (20)        0 2020-04-19 07:17:36.000000 ilus-1.3.1/ilus/modules/variants/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)    10948 2023-02-27 00:10:49.000000 ilus-1.3.1/ilus/modules/variants/gatk.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-02-27 16:13:52.265868 ilus-1.3.1/ilus/modules/vcf/
--rw-r--r--   0 huangshujia   (501) staff       (20)        0 2020-04-28 10:06:56.000000 ilus-1.3.1/ilus/modules/vcf/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)      667 2023-02-20 08:48:18.000000 ilus-1.3.1/ilus/modules/vcf/bcftools.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-02-27 16:13:52.276340 ilus-1.3.1/ilus/pipeline/
--rw-r--r--   0 huangshujia   (501) staff       (20)      173 2023-02-16 04:10:30.000000 ilus-1.3.1/ilus/pipeline/__init__.py
--rw-r--r--   0 huangshujia   (501) staff       (20)     3746 2023-02-20 08:09:44.000000 ilus-1.3.1/ilus/pipeline/_command_args.py
--rw-r--r--   0 huangshujia   (501) staff       (20)    10545 2023-02-24 08:45:49.000000 ilus-1.3.1/ilus/pipeline/_wgs.py
-drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-02-27 16:13:52.232197 ilus-1.3.1/ilus.egg-info/
--rw-r--r--   0 huangshujia   (501) staff       (20)    33281 2023-02-27 16:13:51.000000 ilus-1.3.1/ilus.egg-info/PKG-INFO
--rw-r--r--   0 huangshujia   (501) staff       (20)      818 2023-02-27 16:13:51.000000 ilus-1.3.1/ilus.egg-info/SOURCES.txt
--rw-r--r--   0 huangshujia   (501) staff       (20)        1 2023-02-27 16:13:51.000000 ilus-1.3.1/ilus.egg-info/dependency_links.txt
--rw-r--r--   0 huangshujia   (501) staff       (20)       41 2023-02-27 16:13:51.000000 ilus-1.3.1/ilus.egg-info/entry_points.txt
--rw-r--r--   0 huangshujia   (501) staff       (20)       14 2023-02-27 16:13:51.000000 ilus-1.3.1/ilus.egg-info/requires.txt
--rw-r--r--   0 huangshujia   (501) staff       (20)        5 2023-02-27 16:13:51.000000 ilus-1.3.1/ilus.egg-info/top_level.txt
--rw-r--r--   0 huangshujia   (501) staff       (20)       38 2023-02-27 16:13:52.282765 ilus-1.3.1/setup.cfg
--rw-r--r--   0 huangshujia   (501) staff       (20)     2137 2023-02-27 16:13:23.000000 ilus-1.3.1/setup.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-04-18 07:21:33.975458 ilus-1.3.2/
+-rw-r--r--   0 huangshujia   (501) staff       (20)    35137 2023-02-06 08:38:34.000000 ilus-1.3.2/LICENSE
+-rw-r--r--   0 huangshujia   (501) staff       (20)    33456 2023-04-18 07:21:33.974546 ilus-1.3.2/PKG-INFO
+-rw-r--r--   0 huangshujia   (501) staff       (20)    32397 2023-02-08 06:59:40.000000 ilus-1.3.2/README.md
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-04-18 07:21:33.900805 ilus-1.3.2/ilus/
+-rw-r--r--   0 huangshujia   (501) staff       (20)        0 2018-11-29 10:13:48.000000 ilus-1.3.2/ilus/__init__.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-04-18 07:21:33.920161 ilus-1.3.2/ilus/launch/
+-rw-r--r--   0 huangshujia   (501) staff       (20)        0 2018-11-29 10:13:48.000000 ilus-1.3.2/ilus/launch/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)     3307 2022-07-20 03:59:17.000000 ilus-1.3.2/ilus/launch/do.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)    23124 2023-03-14 04:19:47.000000 ilus-1.3.2/ilus/launch/runfunction.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)     5552 2023-04-18 07:21:04.000000 ilus-1.3.2/ilus/main.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-04-18 07:21:33.924643 ilus-1.3.2/ilus/modules/
+-rw-r--r--   0 huangshujia   (501) staff       (20)        0 2018-11-29 10:13:48.000000 ilus-1.3.2/ilus/modules/__init__.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-04-18 07:21:33.926094 ilus-1.3.2/ilus/modules/ngsaligner/
+-rw-r--r--   0 huangshujia   (501) staff       (20)        0 2018-11-29 10:13:48.000000 ilus-1.3.2/ilus/modules/ngsaligner/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)     1541 2023-02-16 03:32:18.000000 ilus-1.3.2/ilus/modules/ngsaligner/bwa.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-04-18 07:21:33.930632 ilus-1.3.2/ilus/modules/summary/
+-rw-r--r--   0 huangshujia   (501) staff       (20)        0 2020-04-29 06:48:45.000000 ilus-1.3.2/ilus/modules/summary/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)     1643 2023-02-22 01:03:58.000000 ilus-1.3.2/ilus/modules/summary/bam.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-04-18 07:21:33.950537 ilus-1.3.2/ilus/modules/utils/
+-rw-r--r--   0 huangshujia   (501) staff       (20)      175 2023-02-21 08:25:02.000000 ilus-1.3.2/ilus/modules/utils/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)      182 2023-03-14 04:15:47.000000 ilus-1.3.2/ilus/modules/utils/_check_config.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)     1001 2023-03-06 07:47:44.000000 ilus-1.3.2/ilus/modules/utils/_check_jobs.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)     4029 2023-03-05 12:02:52.000000 ilus-1.3.2/ilus/modules/utils/_check_samplesheet.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)     2778 2023-02-21 05:55:33.000000 ilus-1.3.2/ilus/modules/utils/_split_jobs.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)      891 2023-02-21 03:35:30.000000 ilus-1.3.2/ilus/modules/utils/_utils.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-04-18 07:21:33.953710 ilus-1.3.2/ilus/modules/variants/
+-rw-r--r--   0 huangshujia   (501) staff       (20)        0 2020-04-19 07:17:36.000000 ilus-1.3.2/ilus/modules/variants/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)    10948 2023-02-27 00:10:49.000000 ilus-1.3.2/ilus/modules/variants/gatk.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-04-18 07:21:33.958123 ilus-1.3.2/ilus/modules/vcf/
+-rw-r--r--   0 huangshujia   (501) staff       (20)        0 2020-04-28 10:06:56.000000 ilus-1.3.2/ilus/modules/vcf/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)      667 2023-02-20 08:48:18.000000 ilus-1.3.2/ilus/modules/vcf/bcftools.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-04-18 07:21:33.969824 ilus-1.3.2/ilus/pipeline/
+-rw-r--r--   0 huangshujia   (501) staff       (20)      173 2023-02-16 04:10:30.000000 ilus-1.3.2/ilus/pipeline/__init__.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)     3746 2023-02-20 08:09:44.000000 ilus-1.3.2/ilus/pipeline/_command_args.py
+-rw-r--r--   0 huangshujia   (501) staff       (20)    10545 2023-02-24 08:45:49.000000 ilus-1.3.2/ilus/pipeline/_wgs.py
+drwxr-xr-x   0 huangshujia   (501) staff       (20)        0 2023-04-18 07:21:33.912240 ilus-1.3.2/ilus.egg-info/
+-rw-r--r--   0 huangshujia   (501) staff       (20)    33456 2023-04-18 07:21:32.000000 ilus-1.3.2/ilus.egg-info/PKG-INFO
+-rw-r--r--   0 huangshujia   (501) staff       (20)      854 2023-04-18 07:21:33.000000 ilus-1.3.2/ilus.egg-info/SOURCES.txt
+-rw-r--r--   0 huangshujia   (501) staff       (20)        1 2023-04-18 07:21:32.000000 ilus-1.3.2/ilus.egg-info/dependency_links.txt
+-rw-r--r--   0 huangshujia   (501) staff       (20)       41 2023-04-18 07:21:32.000000 ilus-1.3.2/ilus.egg-info/entry_points.txt
+-rw-r--r--   0 huangshujia   (501) staff       (20)       14 2023-04-18 07:21:32.000000 ilus-1.3.2/ilus.egg-info/requires.txt
+-rw-r--r--   0 huangshujia   (501) staff       (20)        5 2023-04-18 07:21:32.000000 ilus-1.3.2/ilus.egg-info/top_level.txt
+-rw-r--r--   0 huangshujia   (501) staff       (20)       38 2023-04-18 07:21:33.975776 ilus-1.3.2/setup.cfg
+-rw-r--r--   0 huangshujia   (501) staff       (20)     2339 2023-04-18 07:20:52.000000 ilus-1.3.2/setup.py
```

### Comparing `ilus-1.3.1/LICENSE` & `ilus-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ilus-1.3.1/PKG-INFO` & `ilus-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: ilus
-Version: 1.3.1
+Version: 1.3.2
 Summary: ilus: A handy tools for generating WGS/WES analysis pipeline.
 Home-page: https://github.com/ShujiaHuang/ilus
 Author: Shujia Huang
 Author-email: huangshujia9@gmail.com
 Maintainer: Shujia Huang
 Maintainer-email: huangshujia9@gmail.com
 License: BSD (3-clause)
 Download-URL: https://github.com/ShujiaHuang/ilus
 Platform: UNKNOWN
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Ilus
 ====
 
 [![DOI](https://zenodo.org/badge/254013599.svg)](https://zenodo.org/badge/latestdoi/254013599)
```

### Comparing `ilus-1.3.1/README.md` & `ilus-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ilus-1.3.1/ilus/launch/do.py` & `ilus-1.3.2/ilus/launch/do.py`

 * *Files identical despite different names*

### Comparing `ilus-1.3.1/ilus/launch/runfunction.py` & `ilus-1.3.2/ilus/launch/runfunction.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,17 +147,20 @@
 
         if not is_dry_run and (not sample_shell_fname.exists() or kwargs.overwrite):
             _create_cmd_file(sample_shell_fname, cmd)
 
     return markdup_shell_files_list  # [[sample, sample_shell_fname], ...]
 
 
-def gatk_baserecalibrator(kwargs, out_folder_name: str, aione: dict = None,
+def gatk_baserecalibrator(kwargs,
+                          out_folder_name: str,
+                          aione: dict = None,
                           is_calculate_summary: bool = True,
                           is_dry_run: bool = False):
+
     shell_dirtory = Path(kwargs.outdir).joinpath(out_folder_name, "shell", "bqsr")
     if not is_dry_run:
         safe_makedir(shell_dirtory)
 
     aione["sample_final_bqsr_bam"] = []
     bqsr_shell_files_list = []
 
@@ -315,21 +318,20 @@
 
         if not sample_gvcf_list:
             sys.stderr.write("[Error] Interval parameters in configuration file may be different "
                              "from that input gvcf file list in ``gatk_combineGVCFs`` function.")
             sys.exit(1)
 
         interval_n = "_".join(interval) if type(interval) is list else interval.replace(":", "_")  # chr:s -> chr_s
-
         sub_shell_fname = shell_dirtory.joinpath(f"{project_name}.{interval_n}.combineGVCFs.sh")
         combineGVCF_fname = output_dirtory.joinpath(f"{project_name}.{interval_n}.genomics_db") \
             if is_use_gDBI else output_dirtory.joinpath(f"{project_name}.{interval_n}.g.vcf.gz")
 
         # Create commandline for combining GVCFs
-        calling_interval = "%s:%s-%s" % (interval[0], interval[1], interval[2]) \
+        calling_interval = f"{interval[0]}:{interval[1]}-{interval[2]}" \
             if type(interval) is list else interval
 
         combineGVCFs_cmd = gatk.combineGVCFs(aione["config"],
                                              sample_gvcf_list,
                                              combineGVCF_fname,
                                              interval=calling_interval)
 
@@ -372,16 +374,16 @@
 
 
 def gatk_genotypeGVCFs(kwargs, out_folder_name: str, aione: dict = None, is_dry_run: bool = False):
     """Create shell for genotypeGVCFs.
     """
     output_dirtory, shell_dirtory = _md(Path(kwargs.outdir).joinpath(out_folder_name),
                                         is_dry_run=is_dry_run)
-    is_use_gDBI = aione["config"]["gatk"]["use_genomicsDBImport"] \
-        if "use_genomicsDBImport" in aione["config"]["gatk"] else False
+    # is_use_gDBI = aione["config"]["gatk"]["use_genomicsDBImport"] \
+    #     if "use_genomicsDBImport" in aione["config"]["gatk"] else False
 
     genotype_vcf_shell_files_list = []
     aione["genotype_vcf_list"] = []
 
     variant_calling_intervals = aione["config"]["gatk"]["variant_calling_interval"]
     for interval in variant_calling_intervals:
         interval_n = "_".join(interval) if type(interval) is list else interval.replace(":", "_")  # chr:s -> chr_s
@@ -390,15 +392,15 @@
             continue
 
         sub_shell_fname = shell_dirtory.joinpath(f"{kwargs.project_name}.{interval_n}.genotype.sh")
         genotype_vcf_fname = str(output_dirtory.joinpath(f"{kwargs.project_name}.{interval_n}.vcf.gz"))
         genotype_vcf_shell_files_list.append([kwargs.project_name + "." + interval_n, sub_shell_fname])
         aione["genotype_vcf_list"].append(genotype_vcf_fname)
 
-        calling_interval = "%s:%s-%s" % (interval[0], interval[1], interval[2]) \
+        calling_interval = f"{interval[0]}:{interval[1]}-{interval[2]}" \
             if type(interval) is list else interval
 
         # Create commandline for genotype joint-calling process
         combineGVCF_fname = aione["combineGVCFs"][interval_n]
         genotype_cmd = gatk.genotypeGVCFs(aione["config"],
                                           combineGVCF_fname,
                                           genotype_vcf_fname,
```

### Comparing `ilus-1.3.1/ilus/main.py` & `ilus-1.3.2/ilus/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     WGS, create_wgs_pipeline_command,
     genotypeGVCFs, create_genotype_joint_calling_command,
     variantrecalibrator, create_vqsr_command
 )
 from ilus.modules.utils import split_jobs, check_jobs_status
 
 PROG_NAME = "ilus"
-VERSION = "1.3.1"
+VERSION = "1.3.2"
 
 
 def create_split_job_command(commands):
     # Create subparser for the "split-jobs" command
     split_job_cmd = commands.add_parser("split-jobs", help="Split the whole shell into multiple jobs.")
     split_job_cmd.add_argument(
         "-I", "--input",
@@ -84,15 +84,15 @@
 
     cmdparser.add_argument(
         "-v", "--version",
         action="store_true",
         help=f"show the version of {PROG_NAME} and exit."
     )
 
-    commands = cmdparser.add_subparsers(dest="command", title="ilus commands")
+    commands = cmdparser.add_subparsers(dest="command", title=f"{PROG_NAME} commands")
 
     # The arguments for the whole pipeline of WGS.
     create_wgs_pipeline_command(commands)
 
     # The arguments for joint-calling process
     create_genotype_joint_calling_command(commands)
 
@@ -179,11 +179,11 @@
 def main():
     START_TIME = datetime.now()
 
     args = parse_commandline_args()
     run_command(args)
 
     elapsed_time = datetime.now() - START_TIME
-    print(f"\nCreating pipeline for '{args.command}' done, "
-          f"{elapsed_time.seconds} seconds elapsed.")
+    print(f"\n{PROG_NAME} (version: {VERSION}) for '{args.command}' done, "
+          f"{elapsed_time.seconds} seconds elapsed.", file=sys.stderr)
 
     return
```

### Comparing `ilus-1.3.1/ilus/modules/ngsaligner/bwa.py` & `ilus-1.3.2/ilus/modules/ngsaligner/bwa.py`

 * *Files identical despite different names*

### Comparing `ilus-1.3.1/ilus/modules/summary/bam.py` & `ilus-1.3.2/ilus/modules/summary/bam.py`

 * *Files identical despite different names*

### Comparing `ilus-1.3.1/ilus/modules/utils/_check_jobs.py` & `ilus-1.3.2/ilus/modules/utils/_check_jobs.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,17 @@
     # Match anything looks like: "[xx] xxx done" or "[xx] xx xxx ... done"
     pattern = re.compile(r'^\[\S+\].*?\s+done$')
 
     def check_job(input_fname):
         if not Path(input_fname).exists():
             return False
 
-        with open(input_fname) as f:
-            for last_line in f:
+        last_line = ""
+        with open(input_fname) as _f:
+            for last_line in _f:
                 pass
 
         return pattern.match(last_line.strip()) is not None
 
     all_done = True
     with open(task_log_file) as f:
         for line in f:
```

### Comparing `ilus-1.3.1/ilus/modules/utils/_check_samplesheet.py` & `ilus-1.3.2/ilus/modules/utils/_check_samplesheet.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     sys.exit(1)
 
 
 def check_samplesheet(input_fname):
     """This function checks that the samplesheet follows the following structure:
 
     #SAMPLE	RGID	FASTQ1	FASTQ2	LANE
-    HL003   "@RG\tID:HL003_HL003_L01_65\tPL:COMPLETE\tPU:HL003_L01_65_HL003\tLB:HL003_L01\tSM:HL003"        HL003_L01_65_1.fq.gz     HL003_L01_65_2.fq.gz     HL003_L01_65
-    HL003   "@RG\tID:HL003_HL003_L01_67\tPL:COMPLETE\tPU:HL003_L01_67_HL003\tLB:HL003_L01\tSM:HL003"        HL003_L01_67_1.fq.gz     .       HL003_L01_67
-    HL003   "@RG\tID:HL003_HL003_L01_68\tPL:COMPLETE\tPU:HL003_L01_68_HL003\tLB:HL003_L01\tSM:HL003"        HL003_L01_68_1.fq.gz     HL003_L01_68_2.fq.gz     HL003_L01_68
+    HL003  "@RG\tID:HL003_HL003_L01_65\tPL:COMPLETE\tPU:HL003_L01_65_HL003\tLB:HL003_L01\tSM:HL003"  HL003_L01_65_1.fq.gz  HL003_L01_65_2.fq.gz  HL003_L01_65
+    HL003  "@RG\tID:HL003_HL003_L01_67\tPL:COMPLETE\tPU:HL003_L01_67_HL003\tLB:HL003_L01\tSM:HL003"  HL003_L01_67_1.fq.gz  .   HL003_L01_67
+    HL003  "@RG\tID:HL003_HL003_L01_68\tPL:COMPLETE\tPU:HL003_L01_68_HL003\tLB:HL003_L01\tSM:HL003"  HL003_L01_68_1.fq.gz  HL003_L01_68_2.fq.gz  HL003_L01_68
     """
 
     with gzip.open(input_fname) if input_fname.endswith(".gz") else open(input_fname) as f:
         HEADER = ["#SAMPLE", "RGID", "FASTQ1", "FASTQ2", "LANE"]
         header = f.readline().strip().split()
         if header[:len(HEADER)] != HEADER:
             if header[: len(HEADER)] != HEADER:
```

### Comparing `ilus-1.3.1/ilus/modules/utils/_split_jobs.py` & `ilus-1.3.2/ilus/modules/utils/_split_jobs.py`

 * *Files identical despite different names*

### Comparing `ilus-1.3.1/ilus/modules/utils/_utils.py` & `ilus-1.3.2/ilus/modules/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `ilus-1.3.1/ilus/modules/variants/gatk.py` & `ilus-1.3.2/ilus/modules/variants/gatk.py`

 * *Files identical despite different names*

### Comparing `ilus-1.3.1/ilus/modules/vcf/bcftools.py` & `ilus-1.3.2/ilus/modules/vcf/bcftools.py`

 * *Files identical despite different names*

### Comparing `ilus-1.3.1/ilus/pipeline/_command_args.py` & `ilus-1.3.2/ilus/pipeline/_command_args.py`

 * *Files identical despite different names*

### Comparing `ilus-1.3.1/ilus/pipeline/_wgs.py` & `ilus-1.3.2/ilus/pipeline/_wgs.py`

 * *Files identical despite different names*

### Comparing `ilus-1.3.1/ilus.egg-info/PKG-INFO` & `ilus-1.3.2/ilus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: ilus
-Version: 1.3.1
+Version: 1.3.2
 Summary: ilus: A handy tools for generating WGS/WES analysis pipeline.
 Home-page: https://github.com/ShujiaHuang/ilus
 Author: Shujia Huang
 Author-email: huangshujia9@gmail.com
 Maintainer: Shujia Huang
 Maintainer-email: huangshujia9@gmail.com
 License: BSD (3-clause)
 Download-URL: https://github.com/ShujiaHuang/ilus
 Platform: UNKNOWN
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Ilus
 ====
 
 [![DOI](https://zenodo.org/badge/254013599.svg)](https://zenodo.org/badge/latestdoi/254013599)
```

### Comparing `ilus-1.3.1/ilus.egg-info/SOURCES.txt` & `ilus-1.3.2/ilus.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 ilus/launch/runfunction.py
 ilus/modules/__init__.py
 ilus/modules/ngsaligner/__init__.py
 ilus/modules/ngsaligner/bwa.py
 ilus/modules/summary/__init__.py
 ilus/modules/summary/bam.py
 ilus/modules/utils/__init__.py
+ilus/modules/utils/_check_config.py
 ilus/modules/utils/_check_jobs.py
 ilus/modules/utils/_check_samplesheet.py
 ilus/modules/utils/_split_jobs.py
 ilus/modules/utils/_utils.py
 ilus/modules/variants/__init__.py
 ilus/modules/variants/gatk.py
 ilus/modules/vcf/__init__.py
```

### Comparing `ilus-1.3.1/setup.py` & `ilus-1.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 meta = Namespace(
     __DISTNAME__="ilus",
     __AUTHOR__="Shujia Huang",
     __AUTHOR_EMAIL__="huangshujia9@gmail.com",
     __URL__="https://github.com/ShujiaHuang/ilus",
     __LICENSE__="BSD (3-clause)",
     __DOWNLOAD_URL__="https://github.com/ShujiaHuang/ilus",
-    __VERSION__="1.3.1",
+    __VERSION__="1.3.2",
 )
 
 if __name__ == "__main__":
     this_path = Path(__file__).resolve().parent
     long_description = this_path.joinpath("README.md")
 
     setup(name=meta.__DISTNAME__,
@@ -37,28 +37,32 @@
           long_description=(open(long_description).read()),
           long_description_content_type="text/markdown",
           license=meta.__LICENSE__,
           url=meta.__URL__,
           version=meta.__VERSION__,
           download_url=meta.__DOWNLOAD_URL__,
           packages=find_packages(),
+          python_requires=">=3.5",
           install_requires=[
               'PyYAML>=5.1.2',
           ],
           include_package_data=True,
           # scripts = [],
           entry_points={
               "console_scripts": [
                   'ilus = ilus.main:main'
               ]
           },
           classifiers=[
+              'License :: OSI Approved :: BSD License',
               'Intended Audience :: Science/Research',
+              'Programming Language :: Python :: 3.6',
               'Programming Language :: Python :: 3.7',
               'Programming Language :: Python :: 3.8',
               'Programming Language :: Python :: 3.9',
-              'License :: OSI Approved :: BSD License',
+              'Programming Language :: Python :: 3.10',
+              'Programming Language :: Python :: 3.11',
               'Topic :: Scientific/Engineering :: Bio-Informatics',
               'Operating System :: POSIX',
               'Operating System :: POSIX :: Linux',
               'Operating System :: MacOS'],
           )
```

