# Comparing `tmp/mimseq-1.3.2.tar.gz` & `tmp/mimseq-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mimseq-1.3.2.tar", last modified: Tue Mar 14 11:23:29 2023, max compression
+gzip compressed data, was "dist/mimseq-1.3.3.tar", last modified: Tue Apr 18 09:35:23 2023, max compression
```

## Comparing `mimseq-1.3.2.tar` & `mimseq-1.3.3.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:29.000000 mimseq-1.3.2/
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:27.000000 mimseq-1.3.2/mimseq/
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:27.000000 mimseq-1.3.2/mimseq/data/
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:28.000000 mimseq-1.3.2/mimseq/data/araTha1-eColitK/
--rwxr-xr-x   0 drew      (1000) users      (100)     1593 2023-03-14 10:33:16.000000 mimseq-1.3.2/mimseq/data/araTha1-eColitK/FastaHeadersforMimseq.py
--rw-r--r--   0 drew      (1000) users      (100)     1191 2023-03-14 10:34:44.000000 mimseq-1.3.2/mimseq/data/araTha1-eColitK/README.txt
--rw-r--r--   0 drew      (1000) users      (100)    18749 2022-05-27 08:41:38.000000 mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-mito-searchResults.txt
--rw-r--r--   0 drew      (1000) users      (100)    17539 2022-03-07 09:38:20.000000 mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-plastid-searchResults.txt
--rw-r--r--   0 drew      (1000) users      (100)    13643 2019-02-21 17:02:30.000000 mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-filtered-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   124283 2019-02-21 17:02:30.000000 mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-mature-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)     4384 2022-05-27 09:19:19.000000 mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)     4120 2022-05-27 09:19:19.000000 mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-plastidtRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   126268 2023-03-14 10:34:39.000000 mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-tRNAs-all.fa
--rw-r--r--   0 drew      (1000) users      (100)    52698 2018-04-18 00:58:34.000000 mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.out
--rw-r--r--   0 drew      (1000) users      (100)   230054 2018-04-18 00:58:34.000000 mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.ss
--rw-r--r--   0 drew      (1000) users      (100)    64333 2022-02-25 14:22:30.000000 mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.out
--rw-r--r--   0 drew      (1000) users      (100)   253880 2018-04-18 00:58:33.000000 mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.ss
--rw-r--r--   0 drew      (1000) users      (100)    48286 2023-03-14 10:25:34.000000 mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)   116013 2022-03-08 15:21:29.000000 mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    18895 2019-02-21 16:51:34.000000 mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-tRNAs_name_map.txt
--rwxr-xr-x   0 drew      (1000) users      (100)      596 2022-05-27 09:19:14.000000 mimseq-1.3.2/mimseq/data/araTha1-eColitK/convertPtRNAdbSearch.py
--rw-r--r--   0 drew      (1000) users      (100)     3325 2023-03-14 09:57:56.000000 mimseq-1.3.2/mimseq/data/araTha1-eColitK/hg38README.txt
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:28.000000 mimseq-1.3.2/mimseq/data/ce11-tRNAs/
--rw-r--r--   0 drew      (1000) users      (100)     2387 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/ce11-tRNAs/ce11-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    64329 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/ce11-tRNAs/ce11-tRNAs-detailed.out
--rw-r--r--   0 drew      (1000) users      (100)    53802 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/ce11-tRNAs/ce11-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)   116662 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/ce11-tRNAs/ce11-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    21452 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/ce11-tRNAs/ce11-tRNAs_name_map.txt
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:28.000000 mimseq-1.3.2/mimseq/data/danRer11-eColitK/
--rw-r--r--   0 drew      (1000) users      (100)      361 2020-10-13 15:34:52.000000 mimseq-1.3.2/mimseq/data/danRer11-eColitK/README.txt
--rw-r--r--   0 drew      (1000) users      (100)     2460 2020-07-14 08:21:01.000000 mimseq-1.3.2/mimseq/data/danRer11-eColitK/danRer11-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   820216 2020-07-14 08:18:14.000000 mimseq-1.3.2/mimseq/data/danRer11-eColitK/danRer11-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)  1748099 2020-07-14 08:15:10.000000 mimseq-1.3.2/mimseq/data/danRer11-eColitK/danRer11_eColitK.fa
--rw-r--r--   0 drew      (1000) users      (100)  1699762 2020-10-13 15:33:53.000000 mimseq-1.3.2/mimseq/data/danRer11-eColitK/danRer11_eColitK_filtered.fa
--rw-r--r--   0 drew      (1000) users      (100)  2070516 2020-07-14 08:17:34.000000 mimseq-1.3.2/mimseq/data/danRer11-eColitK/danRer11_eschColi-tRNAs.out
--rw-r--r--   0 drew      (1000) users      (100)     3196 2020-10-07 14:47:35.000000 mimseq-1.3.2/mimseq/data/danRer11-eColitK/filterList.txt
--rwxr-xr-x   0 drew      (1000) users      (100)      603 2020-10-13 15:34:55.000000 mimseq-1.3.2/mimseq/data/danRer11-eColitK/filtertRNAs.py
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:28.000000 mimseq-1.3.2/mimseq/data/dm6-eColitK/
--rw-r--r--   0 drew      (1000) users      (100)     2630 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/dm6-eColitK/dm6-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    22311 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/dm6-eColitK/dm6-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    56907 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/dm6-eColitK/dm6_eColitK-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    31271 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/dm6-eColitK/dm6_eschColi-tRNAs.out
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:28.000000 mimseq-1.3.2/mimseq/data/dm6-tRNAs/
--rw-r--r--   0 drew      (1000) users      (100)     2630 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/dm6-tRNAs/dm6-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    22311 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/dm6-tRNAs/dm6-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    57209 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/dm6-tRNAs/dm6-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    24907 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/dm6-tRNAs/dm6-tRNAs.out
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:28.000000 mimseq-1.3.2/mimseq/data/eschColi-K_12_MG1655-tRNAs/
--rw-r--r--   0 drew      (1000) users      (100)     6233 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    19253 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)     6364 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.out
--rw-r--r--   0 drew      (1000) users      (100)    35045 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.ss.sort
--rw-r--r--   0 drew      (1000) users      (100)     2515 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs_name_map.txt
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:28.000000 mimseq-1.3.2/mimseq/data/eschColi-tRNA_Lys/
--rw-r--r--   0 drew      (1000) users      (100)     6364 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/eschColi-tRNA_Lys/eschColi_K_12_MG1655-tRNAs.out
--rw-r--r--   0 drew      (1000) users      (100)     6884 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/eschColi-tRNA_Lys/eschColi_modomics.fa
--rw-r--r--   0 drew      (1000) users      (100)      211 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/eschColi-tRNA_Lys/eschColi_tRNA_Lys.fa
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:28.000000 mimseq-1.3.2/mimseq/data/gorGor4-eColitK/
--rwxr-xr-x   0 drew      (1000) users      (100)     1588 2021-07-05 08:53:55.000000 mimseq-1.3.2/mimseq/data/gorGor4-eColitK/FastaHeadersforMimseq.py
--rw-r--r--   0 drew      (1000) users      (100)     3012 2021-07-09 13:07:40.000000 mimseq-1.3.2/mimseq/data/gorGor4-eColitK/README.txt
--rw-r--r--   0 drew      (1000) users      (100)     2502 2021-07-07 13:15:36.000000 mimseq-1.3.2/mimseq/data/gorGor4-eColitK/gorGor4-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   108501 2021-07-05 09:02:35.000000 mimseq-1.3.2/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.fa
--rw-r--r--   0 drew      (1000) users      (100)    67892 2021-07-05 08:48:49.000000 mimseq-1.3.2/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.tmp.fa
--rw-r--r--   0 drew      (1000) users      (100)    63236 2021-07-05 09:01:36.000000 mimseq-1.3.2/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-detailed.out
--rw-r--r--   0 drew      (1000) users      (100)   107333 2021-07-09 13:08:29.000000 mimseq-1.3.2/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered.fa
--rw-r--r--   0 drew      (1000) users      (100)   107126 2021-07-09 13:07:44.000000 mimseq-1.3.2/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered2.fa
--rw-r--r--   0 drew      (1000) users      (100)    44065 2021-07-05 08:34:36.000000 mimseq-1.3.2/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    80347 2021-07-05 08:35:51.000000 mimseq-1.3.2/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    16883 2021-07-05 08:35:37.000000 mimseq-1.3.2/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_name_map.txt
--rw-r--r--   0 drew      (1000) users      (100)    42271 2021-07-05 08:48:46.000000 mimseq-1.3.2/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_noChr.bed
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:28.000000 mimseq-1.3.2/mimseq/data/hg19-eColitK/
--rwxr-xr-x   0 drew      (1000) users      (100)     1585 2022-04-27 14:50:02.000000 mimseq-1.3.2/mimseq/data/hg19-eColitK/FastaHeadersforMimseq.py
--rw-r--r--   0 drew      (1000) users      (100)      540 2022-04-27 14:52:24.000000 mimseq-1.3.2/mimseq/data/hg19-eColitK/README.txt
--rw-r--r--   0 drew      (1000) users      (100)     2436 2021-07-08 09:56:41.000000 mimseq-1.3.2/mimseq/data/hg19-eColitK/hg19-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   113031 2022-04-27 14:53:02.000000 mimseq-1.3.2/mimseq/data/hg19-eColitK/hg19-tRNAs-all.fa
--rw-r--r--   0 drew      (1000) users      (100)    59255 2018-03-06 03:17:41.000000 mimseq-1.3.2/mimseq/data/hg19-eColitK/hg19-tRNAs-detailed.out
--rw-r--r--   0 drew      (1000) users      (100)    46331 2019-07-29 22:32:21.000000 mimseq-1.3.2/mimseq/data/hg19-eColitK/hg19-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    17526 2019-07-29 22:32:21.000000 mimseq-1.3.2/mimseq/data/hg19-eColitK/hg19-tRNAs_name_map.txt
--rw-r--r--   0 drew      (1000) users      (100)    65619 2022-04-27 14:53:56.000000 mimseq-1.3.2/mimseq/data/hg19-eColitK/hg19_eschColi-tRNAs.out
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:28.000000 mimseq-1.3.2/mimseq/data/hg19-eColitK-highConf-tRNAs/
--rw-r--r--   0 drew      (1000) users      (100)     2435 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    46331 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    80399 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    48831 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19_eschColi-tRNAs.out
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:28.000000 mimseq-1.3.2/mimseq/data/hg38-eColitK/
--rwxr-xr-x   0 drew      (1000) users      (100)     1585 2020-10-19 12:52:59.000000 mimseq-1.3.2/mimseq/data/hg38-eColitK/FastaHeadersforMimseq.py
--rw-r--r--   0 drew      (1000) users      (100)     3325 2022-07-20 11:41:08.000000 mimseq-1.3.2/mimseq/data/hg38-eColitK/README.txt
--rw-r--r--   0 drew      (1000) users      (100)     2436 2022-04-26 11:17:07.000000 mimseq-1.3.2/mimseq/data/hg38-eColitK/hg38-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   117384 2021-01-22 10:06:35.000000 mimseq-1.3.2/mimseq/data/hg38-eColitK/hg38-tRNAs-all.fa
--rw-r--r--   0 drew      (1000) users      (100)    67912 2020-10-05 13:31:33.000000 mimseq-1.3.2/mimseq/data/hg38-eColitK/hg38-tRNAs-detailed.out
--rw-r--r--   0 drew      (1000) users      (100)   115259 2022-09-07 13:10:51.000000 mimseq-1.3.2/mimseq/data/hg38-eColitK/hg38-tRNAs-filtered.fa
--rw-r--r--   0 drew      (1000) users      (100)    48137 2020-10-06 09:27:32.000000 mimseq-1.3.2/mimseq/data/hg38-eColitK/hg38-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    82347 2020-10-05 11:41:27.000000 mimseq-1.3.2/mimseq/data/hg38-eColitK/hg38-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    18218 2020-10-05 12:36:55.000000 mimseq-1.3.2/mimseq/data/hg38-eColitK/hg38-tRNAs_name_map.txt
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:28.000000 mimseq-1.3.2/mimseq/data/hg38-eColitK_GlyTCCmutant/
--rwxr-xr-x   0 drew      (1000) users      (100)     1585 2022-03-30 09:22:21.000000 mimseq-1.3.2/mimseq/data/hg38-eColitK_GlyTCCmutant/FastaHeadersforMimseq.py
--rw-r--r--   0 drew      (1000) users      (100)      931 2022-03-30 09:32:29.000000 mimseq-1.3.2/mimseq/data/hg38-eColitK_GlyTCCmutant/README.txt
--rw-r--r--   0 drew      (1000) users      (100)     2436 2022-03-30 09:22:21.000000 mimseq-1.3.2/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   117384 2022-03-30 09:22:21.000000 mimseq-1.3.2/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-all.fa
--rw-r--r--   0 drew      (1000) users      (100)    67912 2022-03-30 09:22:21.000000 mimseq-1.3.2/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-detailed.out
--rw-r--r--   0 drew      (1000) users      (100)   115376 2022-03-30 09:26:15.000000 mimseq-1.3.2/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-filtered.fa
--rw-r--r--   0 drew      (1000) users      (100)    48137 2022-03-30 09:22:21.000000 mimseq-1.3.2/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    82347 2022-03-30 09:22:21.000000 mimseq-1.3.2/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    18218 2022-03-30 09:22:21.000000 mimseq-1.3.2/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs_name_map.txt
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:28.000000 mimseq-1.3.2/mimseq/data/mm10-eColitK/
--rw-r--r--   0 drew      (1000) users      (100)     2452 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/mm10-eColitK/mm10-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    84788 2020-01-31 16:59:36.000000 mimseq-1.3.2/mimseq/data/mm10-eColitK/mm10_eColitK-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    47202 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/mm10-eColitK/mm10_eschColi-tRNAs.out
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:28.000000 mimseq-1.3.2/mimseq/data/mm10-tRNAs/
--rw-r--r--   0 drew      (1000) users      (100)     2452 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/mm10-tRNAs/mm10-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    84575 2020-01-31 17:01:17.000000 mimseq-1.3.2/mimseq/data/mm10-tRNAs/mm10-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    40838 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/mm10-tRNAs/mm10-tRNAs.out.filtered-noPseudo-noChrM
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:28.000000 mimseq-1.3.2/mimseq/data/mm39-eColitK/
--rwxr-xr-x   0 drew      (1000) users      (100)     1585 2022-04-27 08:57:47.000000 mimseq-1.3.2/mimseq/data/mm39-eColitK/FastaHeadersforMimseq.py
--rw-r--r--   0 drew      (1000) users      (100)      758 2022-04-26 15:03:49.000000 mimseq-1.3.2/mimseq/data/mm39-eColitK/README.txt
--rw-r--r--   0 drew      (1000) users      (100)     2452 2022-04-27 08:22:42.000000 mimseq-1.3.2/mimseq/data/mm39-eColitK/mm39-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)   218566 2022-04-27 08:59:25.000000 mimseq-1.3.2/mimseq/data/mm39-eColitK/mm39-tRNAs-all.fa
--rw-r--r--   0 drew      (1000) users      (100)  4027115 2022-04-26 15:02:32.000000 mimseq-1.3.2/mimseq/data/mm39-eColitK/mm39-tRNAs-detailed.out
--rw-r--r--   0 drew      (1000) users      (100)   218353 2022-10-27 11:20:21.000000 mimseq-1.3.2/mimseq/data/mm39-eColitK/mm39-tRNAs-noeColi.fa
--rw-r--r--   0 drew      (1000) users      (100)    89234 2021-05-11 08:57:13.000000 mimseq-1.3.2/mimseq/data/mm39-eColitK/mm39-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)  1352197 2021-05-16 08:53:54.000000 mimseq-1.3.2/mimseq/data/mm39-eColitK/mm39-tRNAs_name_map.txt
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:28.000000 mimseq-1.3.2/mimseq/data/rn7-eColitK/
--rw-r--r--   0 drew      (1000) users      (100)      585 2021-11-03 07:29:18.000000 mimseq-1.3.2/mimseq/data/rn7-eColitK/README.txt
--rw-r--r--   0 drew      (1000) users      (100)     2560 2021-11-02 09:01:00.000000 mimseq-1.3.2/mimseq/data/rn7-eColitK/rn7-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    43272 2021-05-10 08:04:02.000000 mimseq-1.3.2/mimseq/data/rn7-eColitK/rn7-tRNAs-confidence-set.out
--rw-r--r--   0 drew      (1000) users      (100)    92538 2021-05-20 20:42:36.000000 mimseq-1.3.2/mimseq/data/rn7-eColitK/rn7-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    83026 2021-11-03 07:29:35.000000 mimseq-1.3.2/mimseq/data/rn7-eColitK/rn7-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    49636 2021-11-02 08:58:59.000000 mimseq-1.3.2/mimseq/data/rn7-eColitK/rn7_eColitK-tRNAs-confidence-set.out
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:28.000000 mimseq-1.3.2/mimseq/data/sacCer3-Phe_SynVsPur/
--rw-r--r--   0 drew      (1000) users      (100)      429 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-Phe.fa
--rw-r--r--   0 drew      (1000) users      (100)    56689 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    20382 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.out-noChrM
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:28.000000 mimseq-1.3.2/mimseq/data/sacCer3-eColitK/
--rw-r--r--   0 drew      (1000) users      (100)      816 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/sacCer3-eColitK/Turk_2013_mitotRNAbounds_Tab1.bed
--rw-r--r--   0 drew      (1000) users      (100)     2821 2020-07-07 08:03:00.000000 mimseq-1.3.2/mimseq/data/sacCer3-eColitK/sacCer3-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    19475 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/sacCer3-eColitK/sacCer3-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    26478 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/sacCer3-eColitK/sacCer3_eschColi-tRNAs.out
--rw-r--r--   0 drew      (1000) users      (100)    56686 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/sacCer3-eColitK/sacCer3_eschColitK.fa
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:28.000000 mimseq-1.3.2/mimseq/data/sacCer3-tRNAs/
--rw-r--r--   0 drew      (1000) users      (100)     2821 2020-07-07 08:03:30.000000 mimseq-1.3.2/mimseq/data/sacCer3-tRNAs/sacCer3-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    19475 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    56473 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    20382 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.out-noChrM
--rw-r--r--   0 drew      (1000) users      (100)   111081 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.ss.sort
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:28.000000 mimseq-1.3.2/mimseq/data/sacCer3-tRNAs_mutant/
--rw-r--r--   0 drew      (1000) users      (100)     1107 2021-09-23 14:11:39.000000 mimseq-1.3.2/mimseq/data/sacCer3-tRNAs_mutant/README.txt
--rw-r--r--   0 drew      (1000) users      (100)      816 2021-09-24 12:57:51.000000 mimseq-1.3.2/mimseq/data/sacCer3-tRNAs_mutant/Turk_2013_mitotRNAbounds_Tab1.bed
--rw-r--r--   0 drew      (1000) users      (100)     2821 2021-09-24 12:57:51.000000 mimseq-1.3.2/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    19475 2021-09-24 12:57:51.000000 mimseq-1.3.2/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    26478 2021-09-24 12:57:51.000000 mimseq-1.3.2/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColi-tRNAs.out
--rw-r--r--   0 drew      (1000) users      (100)    57096 2021-09-24 12:59:06.000000 mimseq-1.3.2/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColitK.fa
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:29.000000 mimseq-1.3.2/mimseq/data/sacCer3_modOligos/
--rw-r--r--   0 drew      (1000) users      (100)    26595 2020-03-26 14:57:08.000000 mimseq-1.3.2/mimseq/data/sacCer3_modOligos/sacCer3_eschColi-tRNAs.out
--rw-r--r--   0 drew      (1000) users      (100)    56987 2020-03-26 14:51:11.000000 mimseq-1.3.2/mimseq/data/sacCer3_modOligos/sacCer3_eschColitK.fa
--rw-r--r--   0 drew      (1000) users      (100)      320 2020-03-27 13:55:28.000000 mimseq-1.3.2/mimseq/data/sacCer3_modOligos/sacCer3_oligoRefsOnly.fa
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:29.000000 mimseq-1.3.2/mimseq/data/schiPomb-972H/
--rw-r--r--   0 drew      (1000) users      (100)     3385 2020-03-11 16:27:56.000000 mimseq-1.3.2/mimseq/data/schiPomb-972H/schiPomb-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    12387 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.bed
--rw-r--r--   0 drew      (1000) users      (100)    33731 2020-03-11 16:25:12.000000 mimseq-1.3.2/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    14240 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.out.noChrM
--rw-r--r--   0 drew      (1000) users      (100)    67540 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.ss.sort
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:29.000000 mimseq-1.3.2/mimseq/data/schiPomb-eColitK/
--rw-r--r--   0 drew      (1000) users      (100)     3385 2020-03-11 16:28:18.000000 mimseq-1.3.2/mimseq/data/schiPomb-eColitK/schiPomb-mitotRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    33944 2020-03-11 16:24:55.000000 mimseq-1.3.2/mimseq/data/schiPomb-eColitK/schiPomb_972H-tRNAs.fa
--rw-r--r--   0 drew      (1000) users      (100)    20604 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/schiPomb-eColitK/schiPomb_eschColi-tRNAs.out
--rw-r--r--   0 drew      (1000) users      (100)     1397 2021-11-02 13:17:22.000000 mimseq-1.3.2/mimseq/data/additionalMods.txt
--rw-r--r--   0 drew      (1000) users      (100)     2762 2020-06-01 14:20:50.000000 mimseq-1.3.2/mimseq/data/additionalMods_all.txt
--rw-r--r--   0 drew      (1000) users      (100)     1452 2020-06-02 15:55:40.000000 mimseq-1.3.2/mimseq/data/additionalMods_original.txt
--rwxr-xr-x   0 drew      (1000) users      (100)   112128 2020-09-10 10:00:52.000000 mimseq-1.3.2/mimseq/data/modomics
--rwxr-xr-x   0 drew      (1000) users      (100)   112128 2020-06-10 14:49:20.000000 mimseq-1.3.2/mimseq/data/modomics_orig
--rwxr-xr-x   0 drew      (1000) users      (100)    67935 2020-01-30 14:46:45.000000 mimseq-1.3.2/mimseq/data/tRNAmatureseq.cm
--rw-r--r--   0 drew      (1000) users      (100)        0 2020-03-19 10:56:10.000000 mimseq-1.3.2/mimseq/__init__.py
--rw-r--r--   0 drew      (1000) users      (100)     8451 2023-03-09 11:17:02.000000 mimseq-1.3.2/mimseq/ccaPlots.R
--rw-r--r--   0 drew      (1000) users      (100)     7683 2022-05-27 09:54:54.000000 mimseq-1.3.2/mimseq/coveragePlot.R
--rw-r--r--   0 drew      (1000) users      (100)     3793 2023-02-08 10:12:49.000000 mimseq-1.3.2/mimseq/crosstalks.py
--rw-r--r--   0 drew      (1000) users      (100)    32195 2022-09-23 11:55:49.000000 mimseq-1.3.2/mimseq/deseq.R
--rwxr-xr-x   0 drew      (1000) users      (100)     7883 2022-06-22 09:54:11.000000 mimseq-1.3.2/mimseq/getCoverage.py
--rwxr-xr-x   0 drew      (1000) users      (100)    28210 2023-03-14 10:38:15.000000 mimseq-1.3.2/mimseq/mimseq.py
--rw-r--r--   0 drew      (1000) users      (100)    52637 2023-02-08 10:12:49.000000 mimseq-1.3.2/mimseq/mmQuant.py
--rw-r--r--   0 drew      (1000) users      (100)    38088 2023-01-17 10:59:49.000000 mimseq-1.3.2/mimseq/modPlot.R
--rw-r--r--   0 drew      (1000) users      (100)     6580 2020-03-17 16:13:32.000000 mimseq-1.3.2/mimseq/modifications
--rw-r--r--   0 drew      (1000) users      (100)    31508 2022-09-02 08:07:33.000000 mimseq-1.3.2/mimseq/splitClusters.py
--rwxr-xr-x   0 drew      (1000) users      (100)    11714 2022-09-07 07:29:29.000000 mimseq-1.3.2/mimseq/ssAlign.py
--rwxr-xr-x   0 drew      (1000) users      (100)     7272 2022-03-08 14:29:47.000000 mimseq-1.3.2/mimseq/tRNAmap.py
--rwxr-xr-x   0 drew      (1000) users      (100)    48869 2023-03-10 13:59:11.000000 mimseq-1.3.2/mimseq/tRNAtools.py
--rw-r--r--   0 drew      (1000) users      (100)       23 2023-03-14 11:23:01.000000 mimseq-1.3.2/mimseq/version.py
-drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-03-14 11:23:27.000000 mimseq-1.3.2/mimseq.egg-info/
--rw-r--r--   0 drew      (1000) users      (100)      725 2023-03-14 11:23:26.000000 mimseq-1.3.2/mimseq.egg-info/PKG-INFO
--rw-r--r--   0 drew      (1000) users      (100)     7719 2023-03-14 11:23:26.000000 mimseq-1.3.2/mimseq.egg-info/SOURCES.txt
--rw-r--r--   0 drew      (1000) users      (100)        1 2023-03-14 11:23:26.000000 mimseq-1.3.2/mimseq.egg-info/dependency_links.txt
--rw-r--r--   0 drew      (1000) users      (100)       47 2023-03-14 11:23:26.000000 mimseq-1.3.2/mimseq.egg-info/entry_points.txt
--rw-r--r--   0 drew      (1000) users      (100)        1 2023-03-14 11:23:26.000000 mimseq-1.3.2/mimseq.egg-info/not-zip-safe
--rw-r--r--   0 drew      (1000) users      (100)       80 2023-03-14 11:23:26.000000 mimseq-1.3.2/mimseq.egg-info/requires.txt
--rw-r--r--   0 drew      (1000) users      (100)        7 2023-03-14 11:23:26.000000 mimseq-1.3.2/mimseq.egg-info/top_level.txt
--rw-r--r--   0 drew      (1000) users      (100)    35147 2020-01-30 14:46:45.000000 mimseq-1.3.2/LICENSE.txt
--rw-r--r--   0 drew      (1000) users      (100)      264 2021-09-24 14:42:07.000000 mimseq-1.3.2/MANIFEST.in
--rw-r--r--   0 drew      (1000) users      (100)     5091 2023-02-08 15:18:34.000000 mimseq-1.3.2/README.md
--rw-r--r--   0 drew      (1000) users      (100)      124 2023-01-17 11:01:06.000000 mimseq-1.3.2/sampleData_HEKvsK562.txt
--rwxr-xr-x   0 drew      (1000) users      (100)     1913 2023-02-08 10:12:49.000000 mimseq-1.3.2/setup.py
--rw-r--r--   0 drew      (1000) users      (100)      725 2023-03-14 11:23:29.000000 mimseq-1.3.2/PKG-INFO
--rw-r--r--   0 drew      (1000) users      (100)       38 2023-03-14 11:23:29.000000 mimseq-1.3.2/setup.cfg
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:23.000000 mimseq-1.3.3/
+-rw-r--r--   0 drew      (1000) users      (100)    35147 2020-01-30 14:46:45.000000 mimseq-1.3.3/LICENSE.txt
+-rw-r--r--   0 drew      (1000) users      (100)      264 2021-09-24 14:42:07.000000 mimseq-1.3.3/MANIFEST.in
+-rw-r--r--   0 drew      (1000) users      (100)      740 2023-04-18 09:35:23.000000 mimseq-1.3.3/PKG-INFO
+-rw-r--r--   0 drew      (1000) users      (100)     5091 2023-02-08 15:18:34.000000 mimseq-1.3.3/README.md
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/
+-rw-r--r--   0 drew      (1000) users      (100)        0 2020-03-19 10:56:10.000000 mimseq-1.3.3/mimseq/__init__.py
+-rw-r--r--   0 drew      (1000) users      (100)     8451 2023-03-09 11:17:02.000000 mimseq-1.3.3/mimseq/ccaPlots.R
+-rw-r--r--   0 drew      (1000) users      (100)     7683 2022-05-27 09:54:54.000000 mimseq-1.3.3/mimseq/coveragePlot.R
+-rw-r--r--   0 drew      (1000) users      (100)     3793 2023-02-08 10:12:49.000000 mimseq-1.3.3/mimseq/crosstalks.py
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/
+-rw-r--r--   0 drew      (1000) users      (100)     1397 2021-11-02 13:17:22.000000 mimseq-1.3.3/mimseq/data/additionalMods.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2762 2020-06-01 14:20:50.000000 mimseq-1.3.3/mimseq/data/additionalMods_all.txt
+-rw-r--r--   0 drew      (1000) users      (100)     1452 2020-06-02 15:55:40.000000 mimseq-1.3.3/mimseq/data/additionalMods_original.txt
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/
+-rwxr-xr-x   0 drew      (1000) users      (100)     1593 2023-03-14 10:33:16.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/FastaHeadersforMimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)     1191 2023-03-14 10:34:44.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)    18749 2022-05-27 08:41:38.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-mito-searchResults.txt
+-rw-r--r--   0 drew      (1000) users      (100)    17539 2022-03-07 09:38:20.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-plastid-searchResults.txt
+-rw-r--r--   0 drew      (1000) users      (100)    13643 2019-02-21 17:02:30.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-filtered-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   124283 2019-02-21 17:02:30.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-mature-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)     4384 2022-05-27 09:19:19.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)     4120 2022-05-27 09:19:19.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-plastidtRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   126268 2023-03-14 10:34:39.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs-all.fa
+-rw-r--r--   0 drew      (1000) users      (100)    52698 2018-04-18 00:58:34.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.out
+-rw-r--r--   0 drew      (1000) users      (100)   230054 2018-04-18 00:58:34.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.ss
+-rw-r--r--   0 drew      (1000) users      (100)    64333 2022-02-25 14:22:30.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.out
+-rw-r--r--   0 drew      (1000) users      (100)   253880 2018-04-18 00:58:33.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.ss
+-rw-r--r--   0 drew      (1000) users      (100)    48286 2023-03-14 10:25:34.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)   116013 2022-03-08 15:21:29.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    18895 2019-02-21 16:51:34.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs_name_map.txt
+-rwxr-xr-x   0 drew      (1000) users      (100)      596 2022-05-27 09:19:14.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/convertPtRNAdbSearch.py
+-rw-r--r--   0 drew      (1000) users      (100)     3325 2023-03-14 09:57:56.000000 mimseq-1.3.3/mimseq/data/araTha1-eColitK/hg38README.txt
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/ce11-tRNAs/
+-rw-r--r--   0 drew      (1000) users      (100)     2387 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/ce11-tRNAs/ce11-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    64329 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/ce11-tRNAs/ce11-tRNAs-detailed.out
+-rw-r--r--   0 drew      (1000) users      (100)    53802 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/ce11-tRNAs/ce11-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)   116662 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/ce11-tRNAs/ce11-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    21452 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/ce11-tRNAs/ce11-tRNAs_name_map.txt
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/danRer11-eColitK/
+-rw-r--r--   0 drew      (1000) users      (100)      361 2020-10-13 15:34:52.000000 mimseq-1.3.3/mimseq/data/danRer11-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2460 2020-07-14 08:21:01.000000 mimseq-1.3.3/mimseq/data/danRer11-eColitK/danRer11-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   820216 2020-07-14 08:18:14.000000 mimseq-1.3.3/mimseq/data/danRer11-eColitK/danRer11-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)  1748099 2020-07-14 08:15:10.000000 mimseq-1.3.3/mimseq/data/danRer11-eColitK/danRer11_eColitK.fa
+-rw-r--r--   0 drew      (1000) users      (100)  1699762 2020-10-13 15:33:53.000000 mimseq-1.3.3/mimseq/data/danRer11-eColitK/danRer11_eColitK_filtered.fa
+-rw-r--r--   0 drew      (1000) users      (100)  2070516 2020-07-14 08:17:34.000000 mimseq-1.3.3/mimseq/data/danRer11-eColitK/danRer11_eschColi-tRNAs.out
+-rw-r--r--   0 drew      (1000) users      (100)     3196 2020-10-07 14:47:35.000000 mimseq-1.3.3/mimseq/data/danRer11-eColitK/filterList.txt
+-rwxr-xr-x   0 drew      (1000) users      (100)      603 2020-10-13 15:34:55.000000 mimseq-1.3.3/mimseq/data/danRer11-eColitK/filtertRNAs.py
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/dm6-eColitK/
+-rw-r--r--   0 drew      (1000) users      (100)     2630 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/dm6-eColitK/dm6-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    22311 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/dm6-eColitK/dm6-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    56907 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/dm6-eColitK/dm6_eColitK-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    31271 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/dm6-eColitK/dm6_eschColi-tRNAs.out
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/dm6-tRNAs/
+-rw-r--r--   0 drew      (1000) users      (100)     2630 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/dm6-tRNAs/dm6-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    22311 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/dm6-tRNAs/dm6-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    57209 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/dm6-tRNAs/dm6-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    24907 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/dm6-tRNAs/dm6-tRNAs.out
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/eschColi-K_12_MG1655-tRNAs/
+-rw-r--r--   0 drew      (1000) users      (100)     6233 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    19253 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)     6364 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.out
+-rw-r--r--   0 drew      (1000) users      (100)    35045 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.ss.sort
+-rw-r--r--   0 drew      (1000) users      (100)     2515 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs_name_map.txt
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/eschColi-tRNA_Lys/
+-rw-r--r--   0 drew      (1000) users      (100)     6364 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/eschColi-tRNA_Lys/eschColi_K_12_MG1655-tRNAs.out
+-rw-r--r--   0 drew      (1000) users      (100)     6884 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/eschColi-tRNA_Lys/eschColi_modomics.fa
+-rw-r--r--   0 drew      (1000) users      (100)      211 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/eschColi-tRNA_Lys/eschColi_tRNA_Lys.fa
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/
+-rwxr-xr-x   0 drew      (1000) users      (100)     1588 2021-07-05 08:53:55.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/FastaHeadersforMimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)     3012 2021-07-09 13:07:40.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2502 2021-07-07 13:15:36.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   108501 2021-07-05 09:02:35.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.fa
+-rw-r--r--   0 drew      (1000) users      (100)    67892 2021-07-05 08:48:49.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.tmp.fa
+-rw-r--r--   0 drew      (1000) users      (100)    63236 2021-07-05 09:01:36.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-detailed.out
+-rw-r--r--   0 drew      (1000) users      (100)   107333 2021-07-09 13:08:29.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered.fa
+-rw-r--r--   0 drew      (1000) users      (100)   107126 2021-07-09 13:07:44.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered2.fa
+-rw-r--r--   0 drew      (1000) users      (100)    44065 2021-07-05 08:34:36.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    80347 2021-07-05 08:35:51.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    16883 2021-07-05 08:35:37.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_name_map.txt
+-rw-r--r--   0 drew      (1000) users      (100)    42271 2021-07-05 08:48:46.000000 mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_noChr.bed
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK/
+-rwxr-xr-x   0 drew      (1000) users      (100)     1585 2022-04-27 14:50:02.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK/FastaHeadersforMimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)      540 2022-04-27 14:52:24.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2436 2021-07-08 09:56:41.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   113031 2022-04-27 14:53:02.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19-tRNAs-all.fa
+-rw-r--r--   0 drew      (1000) users      (100)    59255 2018-03-06 03:17:41.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19-tRNAs-detailed.out
+-rw-r--r--   0 drew      (1000) users      (100)    46331 2019-07-29 22:32:21.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    17526 2019-07-29 22:32:21.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19-tRNAs_name_map.txt
+-rw-r--r--   0 drew      (1000) users      (100)    65619 2022-04-27 14:53:56.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19_eschColi-tRNAs.out
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK-highConf-tRNAs/
+-rw-r--r--   0 drew      (1000) users      (100)     2435 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    46331 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    80399 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    48831 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19_eschColi-tRNAs.out
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK/
+-rwxr-xr-x   0 drew      (1000) users      (100)     1585 2020-10-19 12:52:59.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK/FastaHeadersforMimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)     3325 2022-07-20 11:41:08.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2436 2022-04-26 11:17:07.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   117384 2021-01-22 10:06:35.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs-all.fa
+-rw-r--r--   0 drew      (1000) users      (100)    67912 2020-10-05 13:31:33.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs-detailed.out
+-rw-r--r--   0 drew      (1000) users      (100)   115259 2022-09-07 13:10:51.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs-filtered.fa
+-rw-r--r--   0 drew      (1000) users      (100)    48137 2020-10-06 09:27:32.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    82347 2020-10-05 11:41:27.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    18218 2020-10-05 12:36:55.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs_name_map.txt
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/
+-rwxr-xr-x   0 drew      (1000) users      (100)     1585 2022-03-30 09:22:21.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/FastaHeadersforMimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)      931 2022-03-30 09:32:29.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2436 2022-03-30 09:22:21.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   117384 2022-03-30 09:22:21.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-all.fa
+-rw-r--r--   0 drew      (1000) users      (100)    67912 2022-03-30 09:22:21.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-detailed.out
+-rw-r--r--   0 drew      (1000) users      (100)   115376 2022-03-30 09:26:15.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-filtered.fa
+-rw-r--r--   0 drew      (1000) users      (100)    48137 2022-03-30 09:22:21.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    82347 2022-03-30 09:22:21.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    18218 2022-03-30 09:22:21.000000 mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs_name_map.txt
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/mm10-eColitK/
+-rw-r--r--   0 drew      (1000) users      (100)     2452 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/mm10-eColitK/mm10-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    84788 2020-01-31 16:59:36.000000 mimseq-1.3.3/mimseq/data/mm10-eColitK/mm10_eColitK-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    47202 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/mm10-eColitK/mm10_eschColi-tRNAs.out
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq/data/mm10-tRNAs/
+-rw-r--r--   0 drew      (1000) users      (100)     2452 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/mm10-tRNAs/mm10-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    84575 2020-01-31 17:01:17.000000 mimseq-1.3.3/mimseq/data/mm10-tRNAs/mm10-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    40838 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/mm10-tRNAs/mm10-tRNAs.out.filtered-noPseudo-noChrM
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:23.000000 mimseq-1.3.3/mimseq/data/mm39-eColitK/
+-rwxr-xr-x   0 drew      (1000) users      (100)     1585 2022-04-27 08:57:47.000000 mimseq-1.3.3/mimseq/data/mm39-eColitK/FastaHeadersforMimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)      758 2022-04-26 15:03:49.000000 mimseq-1.3.3/mimseq/data/mm39-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2452 2022-04-27 08:22:42.000000 mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)   218566 2022-04-27 08:59:25.000000 mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-tRNAs-all.fa
+-rw-r--r--   0 drew      (1000) users      (100)  4027115 2022-04-26 15:02:32.000000 mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-tRNAs-detailed.out
+-rw-r--r--   0 drew      (1000) users      (100)   218353 2022-10-27 11:20:21.000000 mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-tRNAs-noeColi.fa
+-rw-r--r--   0 drew      (1000) users      (100)    89234 2021-05-11 08:57:13.000000 mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)  1352197 2021-05-16 08:53:54.000000 mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-tRNAs_name_map.txt
+-rwxr-xr-x   0 drew      (1000) users      (100)   112128 2020-09-10 10:00:52.000000 mimseq-1.3.3/mimseq/data/modomics
+-rwxr-xr-x   0 drew      (1000) users      (100)   112128 2020-06-10 14:49:20.000000 mimseq-1.3.3/mimseq/data/modomics_orig
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:23.000000 mimseq-1.3.3/mimseq/data/rn7-eColitK/
+-rw-r--r--   0 drew      (1000) users      (100)      585 2021-11-03 07:29:18.000000 mimseq-1.3.3/mimseq/data/rn7-eColitK/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)     2560 2021-11-02 09:01:00.000000 mimseq-1.3.3/mimseq/data/rn7-eColitK/rn7-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    43272 2021-05-10 08:04:02.000000 mimseq-1.3.3/mimseq/data/rn7-eColitK/rn7-tRNAs-confidence-set.out
+-rw-r--r--   0 drew      (1000) users      (100)    92538 2021-05-20 20:42:36.000000 mimseq-1.3.3/mimseq/data/rn7-eColitK/rn7-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    83026 2021-11-03 07:29:35.000000 mimseq-1.3.3/mimseq/data/rn7-eColitK/rn7-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    49636 2021-11-02 08:58:59.000000 mimseq-1.3.3/mimseq/data/rn7-eColitK/rn7_eColitK-tRNAs-confidence-set.out
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:23.000000 mimseq-1.3.3/mimseq/data/sacCer3-Phe_SynVsPur/
+-rw-r--r--   0 drew      (1000) users      (100)      429 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-Phe.fa
+-rw-r--r--   0 drew      (1000) users      (100)    56689 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    20382 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.out-noChrM
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:23.000000 mimseq-1.3.3/mimseq/data/sacCer3-eColitK/
+-rw-r--r--   0 drew      (1000) users      (100)      816 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/sacCer3-eColitK/Turk_2013_mitotRNAbounds_Tab1.bed
+-rw-r--r--   0 drew      (1000) users      (100)     2821 2020-07-07 08:03:00.000000 mimseq-1.3.3/mimseq/data/sacCer3-eColitK/sacCer3-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    19475 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/sacCer3-eColitK/sacCer3-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    26478 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/sacCer3-eColitK/sacCer3_eschColi-tRNAs.out
+-rw-r--r--   0 drew      (1000) users      (100)    56686 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/sacCer3-eColitK/sacCer3_eschColitK.fa
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:23.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs/
+-rw-r--r--   0 drew      (1000) users      (100)     2821 2020-07-07 08:03:30.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs/sacCer3-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    19475 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    56473 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    20382 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.out-noChrM
+-rw-r--r--   0 drew      (1000) users      (100)   111081 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.ss.sort
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:23.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/
+-rw-r--r--   0 drew      (1000) users      (100)     1107 2021-09-23 14:11:39.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/README.txt
+-rw-r--r--   0 drew      (1000) users      (100)      816 2021-09-24 12:57:51.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/Turk_2013_mitotRNAbounds_Tab1.bed
+-rw-r--r--   0 drew      (1000) users      (100)     2821 2021-09-24 12:57:51.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    19475 2021-09-24 12:57:51.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    26478 2021-09-24 12:57:51.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColi-tRNAs.out
+-rw-r--r--   0 drew      (1000) users      (100)    57096 2021-09-24 12:59:06.000000 mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColitK.fa
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:23.000000 mimseq-1.3.3/mimseq/data/sacCer3_modOligos/
+-rw-r--r--   0 drew      (1000) users      (100)    26595 2020-03-26 14:57:08.000000 mimseq-1.3.3/mimseq/data/sacCer3_modOligos/sacCer3_eschColi-tRNAs.out
+-rw-r--r--   0 drew      (1000) users      (100)    56987 2020-03-26 14:51:11.000000 mimseq-1.3.3/mimseq/data/sacCer3_modOligos/sacCer3_eschColitK.fa
+-rw-r--r--   0 drew      (1000) users      (100)      320 2020-03-27 13:55:28.000000 mimseq-1.3.3/mimseq/data/sacCer3_modOligos/sacCer3_oligoRefsOnly.fa
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:23.000000 mimseq-1.3.3/mimseq/data/schiPomb-972H/
+-rw-r--r--   0 drew      (1000) users      (100)     3385 2020-03-11 16:27:56.000000 mimseq-1.3.3/mimseq/data/schiPomb-972H/schiPomb-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    12387 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.bed
+-rw-r--r--   0 drew      (1000) users      (100)    33731 2020-03-11 16:25:12.000000 mimseq-1.3.3/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    14240 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.out.noChrM
+-rw-r--r--   0 drew      (1000) users      (100)    67540 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.ss.sort
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:23.000000 mimseq-1.3.3/mimseq/data/schiPomb-eColitK/
+-rw-r--r--   0 drew      (1000) users      (100)     3385 2020-03-11 16:28:18.000000 mimseq-1.3.3/mimseq/data/schiPomb-eColitK/schiPomb-mitotRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    33944 2020-03-11 16:24:55.000000 mimseq-1.3.3/mimseq/data/schiPomb-eColitK/schiPomb_972H-tRNAs.fa
+-rw-r--r--   0 drew      (1000) users      (100)    20604 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/schiPomb-eColitK/schiPomb_eschColi-tRNAs.out
+-rwxr-xr-x   0 drew      (1000) users      (100)    67935 2020-01-30 14:46:45.000000 mimseq-1.3.3/mimseq/data/tRNAmatureseq.cm
+-rw-r--r--   0 drew      (1000) users      (100)    32195 2022-09-23 11:55:49.000000 mimseq-1.3.3/mimseq/deseq.R
+-rwxr-xr-x   0 drew      (1000) users      (100)     7883 2022-06-22 09:54:11.000000 mimseq-1.3.3/mimseq/getCoverage.py
+-rwxr-xr-x   0 drew      (1000) users      (100)    28210 2023-03-14 10:38:15.000000 mimseq-1.3.3/mimseq/mimseq.py
+-rw-r--r--   0 drew      (1000) users      (100)    52638 2023-04-18 08:46:34.000000 mimseq-1.3.3/mimseq/mmQuant.py
+-rw-r--r--   0 drew      (1000) users      (100)    38088 2023-01-17 10:59:49.000000 mimseq-1.3.3/mimseq/modPlot.R
+-rw-r--r--   0 drew      (1000) users      (100)     6580 2020-03-17 16:13:32.000000 mimseq-1.3.3/mimseq/modifications
+-rw-r--r--   0 drew      (1000) users      (100)    31520 2023-04-18 08:45:46.000000 mimseq-1.3.3/mimseq/splitClusters.py
+-rwxr-xr-x   0 drew      (1000) users      (100)    11682 2023-04-18 08:47:35.000000 mimseq-1.3.3/mimseq/ssAlign.py
+-rwxr-xr-x   0 drew      (1000) users      (100)     7272 2022-03-08 14:29:47.000000 mimseq-1.3.3/mimseq/tRNAmap.py
+-rwxr-xr-x   0 drew      (1000) users      (100)    48869 2023-03-10 13:59:11.000000 mimseq-1.3.3/mimseq/tRNAtools.py
+-rw-r--r--   0 drew      (1000) users      (100)       23 2023-04-18 09:33:02.000000 mimseq-1.3.3/mimseq/version.py
+drwxr-xr-x   0 drew      (1000) users      (100)        0 2023-04-18 09:35:22.000000 mimseq-1.3.3/mimseq.egg-info/
+-rw-r--r--   0 drew      (1000) users      (100)      740 2023-04-18 09:35:21.000000 mimseq-1.3.3/mimseq.egg-info/PKG-INFO
+-rw-r--r--   0 drew      (1000) users      (100)     7719 2023-04-18 09:35:21.000000 mimseq-1.3.3/mimseq.egg-info/SOURCES.txt
+-rw-r--r--   0 drew      (1000) users      (100)        1 2023-04-18 09:35:21.000000 mimseq-1.3.3/mimseq.egg-info/dependency_links.txt
+-rw-r--r--   0 drew      (1000) users      (100)       47 2023-04-18 09:35:21.000000 mimseq-1.3.3/mimseq.egg-info/entry_points.txt
+-rw-r--r--   0 drew      (1000) users      (100)        1 2023-04-18 09:35:21.000000 mimseq-1.3.3/mimseq.egg-info/not-zip-safe
+-rw-r--r--   0 drew      (1000) users      (100)       80 2023-04-18 09:35:21.000000 mimseq-1.3.3/mimseq.egg-info/requires.txt
+-rw-r--r--   0 drew      (1000) users      (100)        7 2023-04-18 09:35:21.000000 mimseq-1.3.3/mimseq.egg-info/top_level.txt
+-rw-r--r--   0 drew      (1000) users      (100)      124 2023-01-17 11:01:06.000000 mimseq-1.3.3/sampleData_HEKvsK562.txt
+-rw-r--r--   0 drew      (1000) users      (100)       38 2023-04-18 09:35:23.000000 mimseq-1.3.3/setup.cfg
+-rwxr-xr-x   0 drew      (1000) users      (100)     1913 2023-02-08 10:12:49.000000 mimseq-1.3.3/setup.py
```

### Comparing `mimseq-1.3.2/mimseq/data/araTha1-eColitK/FastaHeadersforMimseq.py` & `mimseq-1.3.3/mimseq/data/araTha1-eColitK/FastaHeadersforMimseq.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/araTha1-eColitK/README.txt` & `mimseq-1.3.3/mimseq/data/araTha1-eColitK/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-mito-searchResults.txt` & `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-mito-searchResults.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-plastid-searchResults.txt` & `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-PtRNAdb-plastid-searchResults.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-filtered-tRNAs.fa` & `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-filtered-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-mature-tRNAs.fa` & `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-mature-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-mitotRNAs.fa` & `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-plastidtRNAs.fa` & `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-plastidtRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-tRNAs-all.fa` & `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs-all.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.out` & `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.ss` & `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs-confidence-set.ss`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.out` & `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.ss` & `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs-detailed.ss`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-tRNAs.bed` & `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-tRNAs.fa` & `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/araTha1-eColitK/araTha1-tRNAs_name_map.txt` & `mimseq-1.3.3/mimseq/data/araTha1-eColitK/araTha1-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/araTha1-eColitK/convertPtRNAdbSearch.py` & `mimseq-1.3.3/mimseq/data/araTha1-eColitK/convertPtRNAdbSearch.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/araTha1-eColitK/hg38README.txt` & `mimseq-1.3.3/mimseq/data/araTha1-eColitK/hg38README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/ce11-tRNAs/ce11-mitotRNAs.fa` & `mimseq-1.3.3/mimseq/data/ce11-tRNAs/ce11-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/ce11-tRNAs/ce11-tRNAs-detailed.out` & `mimseq-1.3.3/mimseq/data/ce11-tRNAs/ce11-tRNAs-detailed.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/ce11-tRNAs/ce11-tRNAs.bed` & `mimseq-1.3.3/mimseq/data/ce11-tRNAs/ce11-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/ce11-tRNAs/ce11-tRNAs.fa` & `mimseq-1.3.3/mimseq/data/ce11-tRNAs/ce11-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/ce11-tRNAs/ce11-tRNAs_name_map.txt` & `mimseq-1.3.3/mimseq/data/ce11-tRNAs/ce11-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/danRer11-eColitK/danRer11-mitotRNAs.fa` & `mimseq-1.3.3/mimseq/data/danRer11-eColitK/danRer11-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/danRer11-eColitK/danRer11-tRNAs.bed` & `mimseq-1.3.3/mimseq/data/danRer11-eColitK/danRer11-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/danRer11-eColitK/danRer11_eColitK.fa` & `mimseq-1.3.3/mimseq/data/danRer11-eColitK/danRer11_eColitK.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/danRer11-eColitK/danRer11_eColitK_filtered.fa` & `mimseq-1.3.3/mimseq/data/danRer11-eColitK/danRer11_eColitK_filtered.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/danRer11-eColitK/danRer11_eschColi-tRNAs.out` & `mimseq-1.3.3/mimseq/data/danRer11-eColitK/danRer11_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/danRer11-eColitK/filterList.txt` & `mimseq-1.3.3/mimseq/data/danRer11-eColitK/filterList.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/danRer11-eColitK/filtertRNAs.py` & `mimseq-1.3.3/mimseq/data/danRer11-eColitK/filtertRNAs.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/dm6-eColitK/dm6-mitotRNAs.fa` & `mimseq-1.3.3/mimseq/data/dm6-eColitK/dm6-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/dm6-eColitK/dm6-tRNAs.bed` & `mimseq-1.3.3/mimseq/data/dm6-eColitK/dm6-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/dm6-eColitK/dm6_eColitK-tRNAs.fa` & `mimseq-1.3.3/mimseq/data/dm6-eColitK/dm6_eColitK-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/dm6-eColitK/dm6_eschColi-tRNAs.out` & `mimseq-1.3.3/mimseq/data/dm6-eColitK/dm6_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/dm6-tRNAs/dm6-mitotRNAs.fa` & `mimseq-1.3.3/mimseq/data/dm6-tRNAs/dm6-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/dm6-tRNAs/dm6-tRNAs.bed` & `mimseq-1.3.3/mimseq/data/dm6-tRNAs/dm6-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/dm6-tRNAs/dm6-tRNAs.fa` & `mimseq-1.3.3/mimseq/data/dm6-tRNAs/dm6-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/dm6-tRNAs/dm6-tRNAs.out` & `mimseq-1.3.3/mimseq/data/dm6-tRNAs/dm6-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.bed` & `mimseq-1.3.3/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.fa` & `mimseq-1.3.3/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.out` & `mimseq-1.3.3/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.ss.sort` & `mimseq-1.3.3/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs.ss.sort`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs_name_map.txt` & `mimseq-1.3.3/mimseq/data/eschColi-K_12_MG1655-tRNAs/eschColi_K_12_MG1655-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/eschColi-tRNA_Lys/eschColi_K_12_MG1655-tRNAs.out` & `mimseq-1.3.3/mimseq/data/eschColi-tRNA_Lys/eschColi_K_12_MG1655-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/eschColi-tRNA_Lys/eschColi_modomics.fa` & `mimseq-1.3.3/mimseq/data/eschColi-tRNA_Lys/eschColi_modomics.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/gorGor4-eColitK/FastaHeadersforMimseq.py` & `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/FastaHeadersforMimseq.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/gorGor4-eColitK/README.txt` & `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/gorGor4-eColitK/gorGor4-mitotRNAs.fa` & `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.fa` & `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.tmp.fa` & `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-all.tmp.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-detailed.out` & `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-detailed.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered.fa` & `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered2.fa` & `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs-filtered2.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.bed` & `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.fa` & `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_name_map.txt` & `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_noChr.bed` & `mimseq-1.3.3/mimseq/data/gorGor4-eColitK/gorGor4-tRNAs_noChr.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg19-eColitK/FastaHeadersforMimseq.py` & `mimseq-1.3.3/mimseq/data/hg19-eColitK/FastaHeadersforMimseq.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg19-eColitK/README.txt` & `mimseq-1.3.3/mimseq/data/hg19-eColitK/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg19-eColitK/hg19-mitotRNAs.fa` & `mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg19-eColitK/hg19-tRNAs-all.fa` & `mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19-tRNAs-all.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg19-eColitK/hg19-tRNAs-detailed.out` & `mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19-tRNAs-detailed.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg19-eColitK/hg19-tRNAs.bed` & `mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg19-eColitK/hg19-tRNAs_name_map.txt` & `mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg19-eColitK/hg19_eschColi-tRNAs.out` & `mimseq-1.3.3/mimseq/data/hg19-eColitK/hg19_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-mitotRNAs.fa` & `mimseq-1.3.3/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.bed` & `mimseq-1.3.3/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.fa` & `mimseq-1.3.3/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19_eschColi-tRNAs.out` & `mimseq-1.3.3/mimseq/data/hg19-eColitK-highConf-tRNAs/hg19_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg38-eColitK/FastaHeadersforMimseq.py` & `mimseq-1.3.3/mimseq/data/hg38-eColitK/FastaHeadersforMimseq.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg38-eColitK/README.txt` & `mimseq-1.3.3/mimseq/data/hg38-eColitK/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg38-eColitK/hg38-mitotRNAs.fa` & `mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg38-eColitK/hg38-tRNAs-all.fa` & `mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs-all.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg38-eColitK/hg38-tRNAs-detailed.out` & `mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs-detailed.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg38-eColitK/hg38-tRNAs-filtered.fa` & `mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs-filtered.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg38-eColitK/hg38-tRNAs.bed` & `mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg38-eColitK/hg38-tRNAs.fa` & `mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg38-eColitK/hg38-tRNAs_name_map.txt` & `mimseq-1.3.3/mimseq/data/hg38-eColitK/hg38-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg38-eColitK_GlyTCCmutant/FastaHeadersforMimseq.py` & `mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/FastaHeadersforMimseq.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg38-eColitK_GlyTCCmutant/README.txt` & `mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-mitotRNAs.fa` & `mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-all.fa` & `mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-all.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-detailed.out` & `mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-detailed.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-filtered.fa` & `mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs-filtered.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.bed` & `mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.fa` & `mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs_name_map.txt` & `mimseq-1.3.3/mimseq/data/hg38-eColitK_GlyTCCmutant/hg38-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/mm10-eColitK/mm10-mitotRNAs.fa` & `mimseq-1.3.3/mimseq/data/mm10-eColitK/mm10-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/mm10-eColitK/mm10_eColitK-tRNAs.fa` & `mimseq-1.3.3/mimseq/data/mm10-eColitK/mm10_eColitK-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/mm10-eColitK/mm10_eschColi-tRNAs.out` & `mimseq-1.3.3/mimseq/data/mm10-eColitK/mm10_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/mm10-tRNAs/mm10-mitotRNAs.fa` & `mimseq-1.3.3/mimseq/data/mm10-tRNAs/mm10-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/mm10-tRNAs/mm10-tRNAs.fa` & `mimseq-1.3.3/mimseq/data/mm10-tRNAs/mm10-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/mm10-tRNAs/mm10-tRNAs.out.filtered-noPseudo-noChrM` & `mimseq-1.3.3/mimseq/data/mm10-tRNAs/mm10-tRNAs.out.filtered-noPseudo-noChrM`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/mm39-eColitK/FastaHeadersforMimseq.py` & `mimseq-1.3.3/mimseq/data/mm39-eColitK/FastaHeadersforMimseq.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/mm39-eColitK/README.txt` & `mimseq-1.3.3/mimseq/data/mm39-eColitK/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/mm39-eColitK/mm39-mitotRNAs.fa` & `mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/mm39-eColitK/mm39-tRNAs-all.fa` & `mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-tRNAs-all.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/mm39-eColitK/mm39-tRNAs-detailed.out` & `mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-tRNAs-detailed.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/mm39-eColitK/mm39-tRNAs-noeColi.fa` & `mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-tRNAs-noeColi.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/mm39-eColitK/mm39-tRNAs.bed` & `mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/mm39-eColitK/mm39-tRNAs_name_map.txt` & `mimseq-1.3.3/mimseq/data/mm39-eColitK/mm39-tRNAs_name_map.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/rn7-eColitK/README.txt` & `mimseq-1.3.3/mimseq/data/rn7-eColitK/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/rn7-eColitK/rn7-mitotRNAs.fa` & `mimseq-1.3.3/mimseq/data/rn7-eColitK/rn7-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/rn7-eColitK/rn7-tRNAs-confidence-set.out` & `mimseq-1.3.3/mimseq/data/rn7-eColitK/rn7-tRNAs-confidence-set.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/rn7-eColitK/rn7-tRNAs.bed` & `mimseq-1.3.3/mimseq/data/rn7-eColitK/rn7-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/rn7-eColitK/rn7-tRNAs.fa` & `mimseq-1.3.3/mimseq/data/rn7-eColitK/rn7-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/rn7-eColitK/rn7_eColitK-tRNAs-confidence-set.out` & `mimseq-1.3.3/mimseq/data/rn7-eColitK/rn7_eColitK-tRNAs-confidence-set.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.fa` & `mimseq-1.3.3/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.out-noChrM` & `mimseq-1.3.3/mimseq/data/sacCer3-Phe_SynVsPur/sacCer3-tRNAs.out-noChrM`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/sacCer3-eColitK/Turk_2013_mitotRNAbounds_Tab1.bed` & `mimseq-1.3.3/mimseq/data/sacCer3-eColitK/Turk_2013_mitotRNAbounds_Tab1.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/sacCer3-eColitK/sacCer3-mitotRNAs.fa` & `mimseq-1.3.3/mimseq/data/sacCer3-eColitK/sacCer3-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/sacCer3-eColitK/sacCer3-tRNAs.bed` & `mimseq-1.3.3/mimseq/data/sacCer3-eColitK/sacCer3-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/sacCer3-eColitK/sacCer3_eschColi-tRNAs.out` & `mimseq-1.3.3/mimseq/data/sacCer3-eColitK/sacCer3_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/sacCer3-eColitK/sacCer3_eschColitK.fa` & `mimseq-1.3.3/mimseq/data/sacCer3-eColitK/sacCer3_eschColitK.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/sacCer3-tRNAs/sacCer3-mitotRNAs.fa` & `mimseq-1.3.3/mimseq/data/sacCer3-tRNAs/sacCer3-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.bed` & `mimseq-1.3.3/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.fa` & `mimseq-1.3.3/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.out-noChrM` & `mimseq-1.3.3/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.out-noChrM`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.ss.sort` & `mimseq-1.3.3/mimseq/data/sacCer3-tRNAs/sacCer3-tRNAs.ss.sort`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/sacCer3-tRNAs_mutant/README.txt` & `mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/README.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/sacCer3-tRNAs_mutant/Turk_2013_mitotRNAbounds_Tab1.bed` & `mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/Turk_2013_mitotRNAbounds_Tab1.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-mitotRNAs.fa` & `mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-tRNAs.bed` & `mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/sacCer3-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColi-tRNAs.out` & `mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColitK.fa` & `mimseq-1.3.3/mimseq/data/sacCer3-tRNAs_mutant/sacCer3_eschColitK.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/sacCer3_modOligos/sacCer3_eschColi-tRNAs.out` & `mimseq-1.3.3/mimseq/data/sacCer3_modOligos/sacCer3_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/sacCer3_modOligos/sacCer3_eschColitK.fa` & `mimseq-1.3.3/mimseq/data/sacCer3_modOligos/sacCer3_eschColitK.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/schiPomb-972H/schiPomb-mitotRNAs.fa` & `mimseq-1.3.3/mimseq/data/schiPomb-972H/schiPomb-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.bed` & `mimseq-1.3.3/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.bed`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.fa` & `mimseq-1.3.3/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.out.noChrM` & `mimseq-1.3.3/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.out.noChrM`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.ss.sort` & `mimseq-1.3.3/mimseq/data/schiPomb-972H/schiPomb_972H-tRNAs.ss.sort`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/schiPomb-eColitK/schiPomb-mitotRNAs.fa` & `mimseq-1.3.3/mimseq/data/schiPomb-eColitK/schiPomb-mitotRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/schiPomb-eColitK/schiPomb_972H-tRNAs.fa` & `mimseq-1.3.3/mimseq/data/schiPomb-eColitK/schiPomb_972H-tRNAs.fa`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/schiPomb-eColitK/schiPomb_eschColi-tRNAs.out` & `mimseq-1.3.3/mimseq/data/schiPomb-eColitK/schiPomb_eschColi-tRNAs.out`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/additionalMods.txt` & `mimseq-1.3.3/mimseq/data/additionalMods.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/additionalMods_all.txt` & `mimseq-1.3.3/mimseq/data/additionalMods_all.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/additionalMods_original.txt` & `mimseq-1.3.3/mimseq/data/additionalMods_original.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/modomics` & `mimseq-1.3.3/mimseq/data/modomics`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/modomics_orig` & `mimseq-1.3.3/mimseq/data/modomics_orig`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/data/tRNAmatureseq.cm` & `mimseq-1.3.3/mimseq/data/tRNAmatureseq.cm`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/ccaPlots.R` & `mimseq-1.3.3/mimseq/ccaPlots.R`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/coveragePlot.R` & `mimseq-1.3.3/mimseq/coveragePlot.R`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/crosstalks.py` & `mimseq-1.3.3/mimseq/crosstalks.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/deseq.R` & `mimseq-1.3.3/mimseq/deseq.R`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/getCoverage.py` & `mimseq-1.3.3/mimseq/getCoverage.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/mimseq.py` & `mimseq-1.3.3/mimseq/mimseq.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/mmQuant.py` & `mimseq-1.3.3/mimseq/mmQuant.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,21 +80,21 @@
 		else:
 			cluster = isodecoder
 			short_isodecoder = isodecoder
 		anticodon = clusterAnticodon(cons_anticodon, short_isodecoder)
 		for pos in data.keys():
 			cov = cov_table.loc[(cov_table.isodecoder == isodecoder) & (cov_table.pos == pos), 'cov']
 			if (sum(modTable[isodecoder][pos].values()) >= misinc_thresh and (any(cov >= min_cov) or 'mito' in isodecoder) and pos-1 not in knownTable[isodecoder]): # misinc above threshold, cov above threshold and not previously known
-				# if one nucleotide dominates misinc. pattern (i.e. >= 0.9 of all misinc, likely a true SNP or misalignment)
-				if (max(modTable[isodecoder][pos].values()) / sum(modTable[isodecoder][pos].values()) > 0.95):
+				# if one nucleotide dominates misinc. pattern (i.e. >= 0.97 of all misinc, likely a true SNP or misalignment)
+				if (max(modTable[isodecoder][pos].values()) / sum(modTable[isodecoder][pos].values()) > 0.97):
 					# if mod seems to be an inosine (i.e. A with G misinc at 34) add to list and modification SNPs file (see tRNAtools.ModsParser())
 					if (tRNA_dict[isodecoder]['sequence'][pos-1] == 'A' and list(modTable[isodecoder][pos].keys())[list(modTable[isodecoder][pos].values()).index(max(modTable[isodecoder][pos].values()))] == 'G' and pos-1 == min(anticodon)):
 						new_inosines_cluster[cluster].append(pos-1)
 						new_inosines_isodecoder[isodecoder].append(pos-1)
-				elif (max(modTable[isodecoder][pos].values()) / sum(modTable[isodecoder][pos].values()) <= 0.95 and not (pos-1 == min(anticodon))):
+				elif (max(modTable[isodecoder][pos].values()) / sum(modTable[isodecoder][pos].values()) <= 0.97 and not (pos-1 == min(anticodon))):
 					new_mods_cluster[cluster].append(pos-1) #modTable has 1 based values - convert back to 0 based for mod_lists
 					new_mods_isodecoder[isodecoder].append(pos-1)
 
 	with open(inputs + "_predictedModstemp.csv", "w") as predMods:
 		#predMods.write("isodecoder\tpos\tidentity\tbam\n")
 		for isodecoder, data in new_mods_isodecoder.items():
 			for pos in data:
```

### Comparing `mimseq-1.3.2/mimseq/modPlot.R` & `mimseq-1.3.3/mimseq/modPlot.R`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/modifications` & `mimseq-1.3.3/mimseq/modifications`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/splitClusters.py` & `mimseq-1.3.3/mimseq/splitClusters.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,15 @@
     unsplit_isosOnly = set()
     notSplit_cov_posInfo = defaultdict(list)
 
     log.info("Calculating nucleotide coverage for {}".format(input))
     bam = pybedtools.BedTool(input)
     # generate a temporary 2 column file with the chromosome names in the bam file
     temp_chrom = input + "_chrom.txt"
-    cmd = "samtools view -H " + input + " | grep @SQ|sed 's/@SQ\tSN:\|LN://g' > " + temp_chrom
+    cmd = "samtools view -H " + input + " | grep @SQ | sed 's/@SQ\tSN:\|@sq\tSN:\|LN://g' > " + temp_chrom
     subprocess.call(cmd, shell = True)
     ### each bam file might have a reduced set of chromosomes compared to the bedTool object and so sorting on all doesn't always work
     # instead, filter bedTool to have those chromosomes present in the bam
     # first create list of chromosome names in bam from temp_chrom above
     temp_chrom_l = list()
     with open(temp_chrom, "r") as temp_chrom_f:
         for line in temp_chrom_f:
@@ -442,18 +442,18 @@
 def writeDeconvTranscripts(out_dir, experiment_name, tRNA_dict, isodecoder_sizes, clustering):
 
 	# write isodecoder fasta for alignment and context analysis
     with open(out_dir + experiment_name + '_isodecoderTranscripts.fa', 'w') as tempSeqs:
         for seq in isodecoder_sizes.keys():
             # new seq to match unsplit cluster parent to tRNA_dict
             if "/" in seq:
-                tempSeq = seq.split("/")[0]
+                tempSeq = seq.split("/")[0] + "-"
                 isodecoder_list = [x for x in tRNA_dict.keys() if tempSeq in x and not "chr" in x]
                 iso_min = min([x.split("-")[-1] for x in isodecoder_list])
-                newSeq = tempSeq + "-" + str(iso_min)
+                newSeq = tempSeq + str(iso_min)
             else:
                 newSeq = seq
             # make shortnames for fa file
             if clustering:
                 shortname = "-".join(seq.split("-")[:-1]) if not re.search("chr|/", seq) else seq.split("/")[0]
             else:
                 shortname = seq
```

### Comparing `mimseq-1.3.2/mimseq/ssAlign.py` & `mimseq-1.3.3/mimseq/ssAlign.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 	struct_dict = structureParser()
 	stk = AlignIO.read(stkname, "stockholm")
 
 	# Get canonical tRNA position numbering (cons_pos_list). Useful to retain cononical numbering of tRNA positions (i.e. anticodon at 34 - 36, m1A 58 etc...)
 	# Return list of characters with pos or '-'. To be used in all plots with positional data such as heatmaps for stops or modifications.
 	# cons_pos_dict is a dictionary of 1 based positions and canonical positions to create extra column in mods tables (mismatchTable and RTstopTable) mapping ungapped positions to canonical ones
-	ss_cons = "".join([line.split()[-1] for line in open(stkname) if line.startswith("#=GC SS_cons")])
+	ss_cons = stk.column_annotations['secondary_structure']
 	if ungapped:
 		ss_cons_orig = ss_cons
 		ss_cons = ss_cons.replace(".", "")
 	cons_pos = 0
 	cons_pos_list = list()
 	cons_pos_dict = defaultdict()
 	openstem_count = 0
@@ -68,15 +68,15 @@
 					cons_pos_dict[pos+1] = '17'
 					cons_pos_list.append('17')
 				elif (cons_pos == 17) and ('17' in cons_pos_list):
 					cons_pos_dict[pos+1] = '17a'
 					cons_pos_list.append('17a')
 					cons_pos += 1
 
-				elif cons_pos == 20:
+				elif cons_pos == 20: 
 					if not '20' in cons_pos_list:
 						cons_pos_dict[pos+1] = '20'
 						cons_pos_list.append('20')
 					elif not '20a' in cons_pos_list:
 						cons_pos_dict[pos+1] = '20a'
 						cons_pos_list.append('20a')
 					elif not '20b' in cons_pos_list:
@@ -180,20 +180,21 @@
 
 	return(tRNA_struct)
 
 def getAnticodon():
 	# return anticodon position from conserved alignment
 
 	anticodon = list()
-	rf_cons = "".join([line.split()[-1] for line in open(stkname) if line.startswith("#=GC RF")])
+	stk = AlignIO.read(stkname, "stockholm")
+	rf_cons = stk.column_annotations['reference_annotation']
 	# use '*' in rf_cons from stk to delimit the anticodon positions
 	for pos, char in enumerate(rf_cons):
 		if char == "*":
 			anticodon.append(pos)
-
+	
 	return(anticodon)
 
 def clusterAnticodon(cons_anticodon, cluster):
 	# return anticodon position without gaps for specific cluster
 
 	bases = ["A", "C", "G", "U"]
 	stk = AlignIO.read(stkname, "stockholm")
@@ -214,35 +215,35 @@
 
 	cons_pos_list, cons_pos_dict = tRNAclassifier()[2:4]
 	#anticodon = getAnticodon_1base()
 
 	# Define positions of conserved mod sites in gapped alignment for each tRNA
 	sites_dict = defaultdict()
 	mod_sites = ['9', '20', '26', '32', '34', '37', '58']
-
+	
 	for mod in mod_sites:
 		sites_dict[mod] = list(cons_pos_dict.keys())[list(cons_pos_dict.values()).index(mod)]
 
 	upstream_dict = defaultdict(lambda: defaultdict(list))
 
-	stk = AlignIO.read(stkname, "stockholm")
+	stk = AlignIO.read(stkname, "stockholm") 
 	for record in stk:
 		gene = record.id
 		seq = record.seq
 		for pos in sites_dict.values():
 			identity = seq[pos-1] # identity of base at modification position
 			if identity in ['A','C','G','U','T']:
 				up = pos - 2 # pos is 1 based from struct, therefore -1 to make 0 based and -1 to get upstream nucl
 				down = pos
 				while seq[up].upper() not in ['A','C','G','U','T']:
 					up -= 1
 				while seq[down].upper() not in ['A','C','G','U','T']:
 					down += 1
 				canon_pos = cons_pos_dict[pos]
-				upstream_dict[gene][canon_pos].append(identity)
+				upstream_dict[gene][canon_pos].append(identity) 
 				upstream_dict[gene][canon_pos].append(seq[up]) # upstream base
 				upstream_dict[gene][canon_pos].append(seq[down]) # downstream base
 
 	try:
 		os.mkdir(out + "mods")
 	except FileExistsError:
 		pass
@@ -260,15 +261,15 @@
 	# mod_sites are canonical numberings of these positions
 	# cons_pos_list is the full list of tRNA positions numbered according to canonical numbering scheme obtained from multiple seq alignments
 	# cons_pos_dict is the same as list but a dictionary with matching gapped tRNA positions to each canonically numbered position
 	return(mod_sites, cons_pos_list)
 
 def structureParser():
 # read in stk file generated above and define structural regions for each tRNA input
-
+	
 	struct_dict = dict()
 	# get conserved tRNA structure from alignment
 	ss_cons = "".join([line.split()[-1] for line in open(stkname) if line.startswith("#=GC SS_cons")])
 
 	acc = defaultdict()
 
 	term = defaultdict()
```

### Comparing `mimseq-1.3.2/mimseq/tRNAmap.py` & `mimseq-1.3.3/mimseq/tRNAmap.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq/tRNAtools.py` & `mimseq-1.3.3/mimseq/tRNAtools.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/mimseq.egg-info/PKG-INFO` & `mimseq-1.3.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: mimseq
-Version: 1.3.2
+Version: 1.3.3
 Summary: Custom high-throughput tRNA sequencing alignment and quantification pipeline based on modification induced misincorporation cDNA synthesis.
 Home-page: https://github.com/nedialkova-lab/mim-tRNAseq
 Author: Drew Behrens
 Author-email: abehrens@biochem.mpg.de
 License: GPLv3
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+License-File: LICENSE.txt
+
+UNKNOWN
+
```

### Comparing `mimseq-1.3.2/mimseq.egg-info/SOURCES.txt` & `mimseq-1.3.3/mimseq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/LICENSE.txt` & `mimseq-1.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/README.md` & `mimseq-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/setup.py` & `mimseq-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `mimseq-1.3.2/PKG-INFO` & `mimseq-1.3.3/mimseq.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: mimseq
-Version: 1.3.2
+Version: 1.3.3
 Summary: Custom high-throughput tRNA sequencing alignment and quantification pipeline based on modification induced misincorporation cDNA synthesis.
 Home-page: https://github.com/nedialkova-lab/mim-tRNAseq
 Author: Drew Behrens
 Author-email: abehrens@biochem.mpg.de
 License: GPLv3
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+License-File: LICENSE.txt
+
+UNKNOWN
+
```

