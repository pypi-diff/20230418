# Comparing `tmp/phc-ingestion-0.3.5.tar.gz` & `tmp/phc-ingestion-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.3.5.tar", last modified: Tue Apr 18 12:19:30 2023, max compression
+gzip compressed data, was "phc-ingestion-0.3.6.tar", last modified: Tue Apr 18 14:55:00 2023, max compression
```

## Comparing `phc-ingestion-0.3.5.tar` & `phc-ingestion-0.3.6.tar`

### file list

```diff
@@ -1,55 +1,57 @@
--rw-r--r--   0        0        0       16 2023-04-18 12:19:04.497902 phc-ingestion-0.3.5/PYPI.md
--rw-r--r--   0        0        0        0 2023-04-18 12:19:04.497902 phc-ingestion-0.3.5/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2023-04-18 12:19:04.497902 phc-ingestion-0.3.5/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1441 2023-04-18 12:19:04.497902 phc-ingestion-0.3.5/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2023-04-18 12:19:04.497902 phc-ingestion-0.3.5/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4468 2023-04-18 12:19:04.497902 phc-ingestion-0.3.5/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0      629 2023-04-18 12:19:04.497902 phc-ingestion-0.3.5/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      555 2023-04-18 12:19:04.497902 phc-ingestion-0.3.5/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4142 2023-04-18 12:19:04.497902 phc-ingestion-0.3.5/ingestion/caris/util/json.py
--rw-r--r--   0        0        0    21500 2023-04-18 12:19:04.497902 phc-ingestion-0.3.5/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     4783 2023-04-18 12:19:04.497902 phc-ingestion-0.3.5/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      500 2023-04-18 12:19:04.497902 phc-ingestion-0.3.5/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0     1443 2023-04-18 12:19:04.497902 phc-ingestion-0.3.5/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     4848 2023-04-18 12:19:04.497902 phc-ingestion-0.3.5/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2023-04-18 12:19:04.497902 phc-ingestion-0.3.5/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     2748 2023-04-18 12:19:04.497902 phc-ingestion-0.3.5/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2023-04-18 12:19:04.497902 phc-ingestion-0.3.5/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5908 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0     8641 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     3188 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0      406 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/ingestion/nextgen/process_cnv.py
--rw-r--r--   0        0        0      401 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/ingestion/nextgen/process_manifest.py
--rw-r--r--   0        0        0      497 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/ingestion/nextgen/process_structural.py
--rw-r--r--   0        0        0      279 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/ingestion/nextgen/process_vcf.py
--rw-r--r--   0        0        0      240 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/ingestion/nextgen/types.py
--rw-r--r--   0        0        0      951 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/pyproject.toml
--rw-r--r--   0        0        0    31504 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/tests/caris/resources/TN20-779441.json
--rw-r--r--   0        0        0    31986 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/tests/caris/resources/TN20-779441_IHC.json
--rw-r--r--   0        0        0     3696 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/tests/caris/resources/TN20-779441_empty_test.json
--rw-r--r--   0        0        0    27666 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/tests/caris/resources/TN20-779441_equivocal.json
--rw-r--r--   0        0        0    26976 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/tests/caris/resources/TN20-779441_equivocal_status.json
--rw-r--r--   0        0        0    26971 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/tests/caris/resources/TN20-779441_high.json
--rw-r--r--   0        0        0    27662 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/tests/caris/resources/TN20-779441_msi_foo.json
--rw-r--r--   0        0        0    27090 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/tests/caris/resources/TN20-779441_no_phys.json
--rw-r--r--   0        0        0    26970 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/tests/caris/resources/TN20-779441_qns.json
--rw-r--r--   0        0        0    26989 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/tests/caris/resources/TN20-779441_qns_long.json
--rw-r--r--   0        0        0   292815 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/tests/caris/resources/carisSample.tar.gz
--rw-r--r--   0        0        0    67481 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/tests/caris/test_caris.py
--rw-r--r--   0        0        0      973 2023-04-18 12:19:04.505902 phc-ingestion-0.3.5/tests/foundation/data/sample/sample.copynumber.csv
--rw-r--r--   0        0        0      667 2023-04-18 12:19:04.505902 phc-ingestion-0.3.5/tests/foundation/data/sample/sample.structural.csv
--rw-r--r--   0        0        0     3038 2023-04-18 12:19:04.505902 phc-ingestion-0.3.5/tests/foundation/data/sample/sample.vcf
--rw-r--r--   0        0        0     2524 2023-04-18 12:19:04.501902 phc-ingestion-0.3.5/tests/foundation/data/sample.vcf
--rw-r--r--   0        0        0   393383 2023-04-18 12:19:04.505902 phc-ingestion-0.3.5/tests/foundation/data/sample.xml
--rw-r--r--   0        0        0   396026 2023-04-18 12:19:04.509902 phc-ingestion-0.3.5/tests/foundation/data/sample_missing_mrn.xml
--rw-r--r--   0        0        0   396053 2023-04-18 12:19:04.513902 phc-ingestion-0.3.5/tests/foundation/data/sample_namespace.xml
--rw-r--r--   0        0        0   395401 2023-04-18 12:19:04.513902 phc-ingestion-0.3.5/tests/foundation/data/sample_no_biomarkers.xml
--rw-r--r--   0        0        0     3249 2023-04-18 12:19:04.513902 phc-ingestion-0.3.5/tests/foundation/data/sample_scientific_notation/sample_scientific_notation.vcf
--rw-r--r--   0        0        0     2712 2023-04-18 12:19:04.513902 phc-ingestion-0.3.5/tests/foundation/data/sample_scientific_notation.vcf
--rw-r--r--   0        0        0   389679 2023-04-18 12:19:04.517902 phc-ingestion-0.3.5/tests/foundation/data/sample_with_multiple_non_human_content.xml
--rw-r--r--   0        0        0     3038 2023-04-18 12:19:04.517902 phc-ingestion-0.3.5/tests/foundation/data/vcf_expected.vcf
--rw-r--r--   0        0        0     3249 2023-04-18 12:19:04.517902 phc-ingestion-0.3.5/tests/foundation/data/vcf_expected_scientific_notation.vcf
--rw-r--r--   0        0        0    31475 2023-04-18 12:19:04.517902 phc-ingestion-0.3.5/tests/foundation/test_util.py
--rw-r--r--   0        0        0      268 1970-01-01 00:00:00.000000 phc-ingestion-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0       16 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/PYPI.md
+-rw-r--r--   0        0        0        0 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1441 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4468 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0      629 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      555 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     4142 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0    21500 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     4783 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      500 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0     1443 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     4848 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     2748 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5908 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0     8641 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     3188 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0       46 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     1788 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0      406 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0      401 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0      497 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0      279 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0      951 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0    31504 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/tests/caris/resources/TN20-779441.json
+-rw-r--r--   0        0        0    31986 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/tests/caris/resources/TN20-779441_IHC.json
+-rw-r--r--   0        0        0     3696 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/tests/caris/resources/TN20-779441_empty_test.json
+-rw-r--r--   0        0        0    27666 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/tests/caris/resources/TN20-779441_equivocal.json
+-rw-r--r--   0        0        0    26976 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/tests/caris/resources/TN20-779441_equivocal_status.json
+-rw-r--r--   0        0        0    26971 2023-04-18 14:54:39.951794 phc-ingestion-0.3.6/tests/caris/resources/TN20-779441_high.json
+-rw-r--r--   0        0        0    27662 2023-04-18 14:54:39.955793 phc-ingestion-0.3.6/tests/caris/resources/TN20-779441_msi_foo.json
+-rw-r--r--   0        0        0    27090 2023-04-18 14:54:39.955793 phc-ingestion-0.3.6/tests/caris/resources/TN20-779441_no_phys.json
+-rw-r--r--   0        0        0    26970 2023-04-18 14:54:39.955793 phc-ingestion-0.3.6/tests/caris/resources/TN20-779441_qns.json
+-rw-r--r--   0        0        0    26989 2023-04-18 14:54:39.955793 phc-ingestion-0.3.6/tests/caris/resources/TN20-779441_qns_long.json
+-rw-r--r--   0        0        0   292815 2023-04-18 14:54:39.955793 phc-ingestion-0.3.6/tests/caris/resources/carisSample.tar.gz
+-rw-r--r--   0        0        0    67481 2023-04-18 14:54:39.955793 phc-ingestion-0.3.6/tests/caris/test_caris.py
+-rw-r--r--   0        0        0      973 2023-04-18 14:54:39.959793 phc-ingestion-0.3.6/tests/foundation/data/sample/sample.copynumber.csv
+-rw-r--r--   0        0        0      667 2023-04-18 14:54:39.959793 phc-ingestion-0.3.6/tests/foundation/data/sample/sample.structural.csv
+-rw-r--r--   0        0        0     3038 2023-04-18 14:54:39.959793 phc-ingestion-0.3.6/tests/foundation/data/sample/sample.vcf
+-rw-r--r--   0        0        0     2524 2023-04-18 14:54:39.955793 phc-ingestion-0.3.6/tests/foundation/data/sample.vcf
+-rw-r--r--   0        0        0   393383 2023-04-18 14:54:39.959793 phc-ingestion-0.3.6/tests/foundation/data/sample.xml
+-rw-r--r--   0        0        0   396026 2023-04-18 14:54:39.959793 phc-ingestion-0.3.6/tests/foundation/data/sample_missing_mrn.xml
+-rw-r--r--   0        0        0   396053 2023-04-18 14:54:39.963794 phc-ingestion-0.3.6/tests/foundation/data/sample_namespace.xml
+-rw-r--r--   0        0        0   395401 2023-04-18 14:54:39.967794 phc-ingestion-0.3.6/tests/foundation/data/sample_no_biomarkers.xml
+-rw-r--r--   0        0        0     3249 2023-04-18 14:54:39.967794 phc-ingestion-0.3.6/tests/foundation/data/sample_scientific_notation/sample_scientific_notation.vcf
+-rw-r--r--   0        0        0     2712 2023-04-18 14:54:39.967794 phc-ingestion-0.3.6/tests/foundation/data/sample_scientific_notation.vcf
+-rw-r--r--   0        0        0   389679 2023-04-18 14:54:39.971794 phc-ingestion-0.3.6/tests/foundation/data/sample_with_multiple_non_human_content.xml
+-rw-r--r--   0        0        0     3038 2023-04-18 14:54:39.971794 phc-ingestion-0.3.6/tests/foundation/data/vcf_expected.vcf
+-rw-r--r--   0        0        0     3249 2023-04-18 14:54:39.971794 phc-ingestion-0.3.6/tests/foundation/data/vcf_expected_scientific_notation.vcf
+-rw-r--r--   0        0        0    31475 2023-04-18 14:54:39.971794 phc-ingestion-0.3.6/tests/foundation/test_util.py
+-rw-r--r--   0        0        0      268 1970-01-01 00:00:00.000000 phc-ingestion-0.3.6/PKG-INFO
```

### Comparing `phc-ingestion-0.3.5/ingestion/caris/process.py` & `phc-ingestion-0.3.6/ingestion/caris/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/ingestion/caris/util/cnv.py` & `phc-ingestion-0.3.6/ingestion/caris/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/ingestion/caris/util/ga4gh.py` & `phc-ingestion-0.3.6/ingestion/caris/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.3.6/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/ingestion/caris/util/json.py` & `phc-ingestion-0.3.6/ingestion/caris/util/json.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/ingestion/caris/util/metadata.py` & `phc-ingestion-0.3.6/ingestion/caris/util/metadata.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/ingestion/caris/util/structural.py` & `phc-ingestion-0.3.6/ingestion/caris/util/structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/ingestion/caris/util/tsv.py` & `phc-ingestion-0.3.6/ingestion/caris/util/tsv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/ingestion/caris/util/vcf.py` & `phc-ingestion-0.3.6/ingestion/caris/util/vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/ingestion/foundation/process.py` & `phc-ingestion-0.3.6/ingestion/foundation/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.3.6/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.3.6/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.3.6/ingestion/foundation/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.3.6/ingestion/foundation/util/vcf_etl.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/pyproject.toml` & `phc-ingestion-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phc-ingestion"
-version = "0.3.5"
+version = "0.3.6"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
```

### Comparing `phc-ingestion-0.3.5/tests/caris/resources/TN20-779441.json` & `phc-ingestion-0.3.6/tests/caris/resources/TN20-779441.json`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/caris/resources/TN20-779441_IHC.json` & `phc-ingestion-0.3.6/tests/caris/resources/TN20-779441_IHC.json`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/caris/resources/TN20-779441_empty_test.json` & `phc-ingestion-0.3.6/tests/caris/resources/TN20-779441_empty_test.json`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/caris/resources/TN20-779441_equivocal.json` & `phc-ingestion-0.3.6/tests/caris/resources/TN20-779441_equivocal.json`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/caris/resources/TN20-779441_equivocal_status.json` & `phc-ingestion-0.3.6/tests/caris/resources/TN20-779441_equivocal_status.json`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/caris/resources/TN20-779441_high.json` & `phc-ingestion-0.3.6/tests/caris/resources/TN20-779441_high.json`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/caris/resources/TN20-779441_msi_foo.json` & `phc-ingestion-0.3.6/tests/caris/resources/TN20-779441_msi_foo.json`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/caris/resources/TN20-779441_no_phys.json` & `phc-ingestion-0.3.6/tests/caris/resources/TN20-779441_no_phys.json`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/caris/resources/TN20-779441_qns.json` & `phc-ingestion-0.3.6/tests/caris/resources/TN20-779441_qns.json`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/caris/resources/TN20-779441_qns_long.json` & `phc-ingestion-0.3.6/tests/caris/resources/TN20-779441_qns_long.json`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/caris/resources/carisSample.tar.gz` & `phc-ingestion-0.3.6/tests/caris/resources/carisSample.tar.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/caris/test_caris.py` & `phc-ingestion-0.3.6/tests/caris/test_caris.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/foundation/data/sample/sample.copynumber.csv` & `phc-ingestion-0.3.6/tests/foundation/data/sample/sample.copynumber.csv`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/foundation/data/sample/sample.structural.csv` & `phc-ingestion-0.3.6/tests/foundation/data/sample/sample.structural.csv`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/foundation/data/sample/sample.vcf` & `phc-ingestion-0.3.6/tests/foundation/data/sample/sample.vcf`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/foundation/data/sample.vcf` & `phc-ingestion-0.3.6/tests/foundation/data/sample.vcf`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/foundation/data/sample.xml` & `phc-ingestion-0.3.6/tests/foundation/data/sample.xml`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/foundation/data/sample_missing_mrn.xml` & `phc-ingestion-0.3.6/tests/foundation/data/sample_missing_mrn.xml`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/foundation/data/sample_namespace.xml` & `phc-ingestion-0.3.6/tests/foundation/data/sample_namespace.xml`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/foundation/data/sample_no_biomarkers.xml` & `phc-ingestion-0.3.6/tests/foundation/data/sample_no_biomarkers.xml`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/foundation/data/sample_scientific_notation/sample_scientific_notation.vcf` & `phc-ingestion-0.3.6/tests/foundation/data/sample_scientific_notation/sample_scientific_notation.vcf`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/foundation/data/sample_scientific_notation.vcf` & `phc-ingestion-0.3.6/tests/foundation/data/sample_scientific_notation.vcf`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/foundation/data/sample_with_multiple_non_human_content.xml` & `phc-ingestion-0.3.6/tests/foundation/data/sample_with_multiple_non_human_content.xml`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/foundation/data/vcf_expected.vcf` & `phc-ingestion-0.3.6/tests/foundation/data/vcf_expected.vcf`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/foundation/data/vcf_expected_scientific_notation.vcf` & `phc-ingestion-0.3.6/tests/foundation/data/vcf_expected_scientific_notation.vcf`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.5/tests/foundation/test_util.py` & `phc-ingestion-0.3.6/tests/foundation/test_util.py`

 * *Files identical despite different names*

