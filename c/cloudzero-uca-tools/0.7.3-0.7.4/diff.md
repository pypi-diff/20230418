# Comparing `tmp/cloudzero_uca_tools-0.7.3.tar.gz` & `tmp/cloudzero_uca_tools-0.7.4.tar.gz`

## Comparing `cloudzero_uca_tools-0.7.3.tar` & `cloudzero_uca_tools-0.7.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/__version__.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/constants.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/exceptions.py
--rwxr-xr-x   0        0        0     9092 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/main.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/commands/__init__.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/commands/convert.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/common/__init__.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/common/aws.py
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/common/cli.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/common/custom_types.py
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/common/files.py
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/common/formatters.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/common/standards.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/data/alb_configuration.json
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/data/configuration.json
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/data/csv_configuration.json
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/data/data.csv
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/data/example_alb_logs
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/data/sample_uca_data.json
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/data/test_configuration.json
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/data/test_data.csv
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/data/transform.jq
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/features/__init__.py
--rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/features/convert.py
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/features/generate.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/features/transform.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/features/transmit.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/interfaces/__init__.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/interfaces/uca_api.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/vendored/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/vendored/aws_log_parser/__init__.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/vendored/aws_log_parser/exceptions.py
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/vendored/aws_log_parser/interface.py
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/vendored/aws_log_parser/models.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/vendored/aws_log_parser/parser.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/vendored/aws_log_parser/util.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/vendored/aws_log_parser/aws/__init__.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/vendored/aws_log_parser/aws/client.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/vendored/aws_log_parser/aws/plugin.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/vendored/aws_log_parser/aws/s3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/vendored/aws_log_parser/cli/__init__.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/uca/vendored/aws_log_parser/cli/main.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/.gitignore
--rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/LICENSE
--rw-r--r--   0        0        0    13634 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/README.md
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/pyproject.toml
--rw-r--r--   0        0        0    14654 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/__init__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/__version__.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/constants.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/exceptions.py
+-rwxr-xr-x   0        0        0     9081 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/main.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/commands/__init__.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/commands/convert.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/common/__init__.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/common/aws.py
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/common/cli.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/common/custom_types.py
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/common/files.py
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/common/formatters.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/common/standards.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/data/alb_configuration.json
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/data/configuration.json
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/data/csv_configuration.json
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/data/data.csv
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/data/example_alb_logs
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/data/sample_uca_data.json
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/data/test_configuration.json
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/data/test_data.csv
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/data/transform.jq
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/features/__init__.py
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/features/convert.py
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/features/generate.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/features/transform.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/features/transmit.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/interfaces/__init__.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/interfaces/uca_api.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/vendored/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/vendored/aws_log_parser/__init__.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/vendored/aws_log_parser/exceptions.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/vendored/aws_log_parser/interface.py
+-rw-r--r--   0        0        0     5354 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/vendored/aws_log_parser/models.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/vendored/aws_log_parser/parser.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/vendored/aws_log_parser/util.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/vendored/aws_log_parser/aws/__init__.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/vendored/aws_log_parser/aws/client.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/vendored/aws_log_parser/aws/plugin.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/vendored/aws_log_parser/aws/s3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/vendored/aws_log_parser/cli/__init__.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/uca/vendored/aws_log_parser/cli/main.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/.gitignore
+-rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/LICENSE
+-rw-r--r--   0        0        0    13634 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/README.md
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0    14769 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.4/PKG-INFO
```

### Comparing `cloudzero_uca_tools-0.7.3/uca/constants.py` & `cloudzero_uca_tools-0.7.4/uca/constants.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.3/uca/main.py` & `cloudzero_uca_tools-0.7.4/uca/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #  Copyright (c) 2021-2023 CloudZero, Inc. or its affiliates. All Rights Reserved.
 #  SPDX-License-Identifier: Apache-2.0
 #  Direct all questions to support@cloudzero.com
 
-import csv
 import os
 import sys
 from datetime import datetime, timedelta
 
 import click
 import simplejson as json
```

### Comparing `cloudzero_uca_tools-0.7.3/uca/commands/convert.py` & `cloudzero_uca_tools-0.7.4/uca/commands/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 @click.option("--data", "-d", help="Data to convert")
 def cli(ctx, data):
     """Convert Command"""
     # Step 3: ctx.parent to access root scope
     print(ctx.parent.params)
     print(data)
 
-
 # @cli.group()
 # @click.option("--data", "-d", help="Data to convert")
 # def convert(data):
 #     print(data)
 
 #
 #
```

### Comparing `cloudzero_uca_tools-0.7.3/uca/common/aws.py` & `cloudzero_uca_tools-0.7.4/uca/common/aws.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.3/uca/common/cli.py` & `cloudzero_uca_tools-0.7.4/uca/common/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,14 @@
         if ans == 'n' or ans == 'N':
             return False
 
 
 def print_uca_sample(uca_to_send, record_count=5):
     sample_count = min(record_count, len(uca_to_send))
     sample_events = []
-    print(f" - Sample of UCA records post-processing:")
+    print(" - Sample of UCA records post-processing:")
     # refactor
     for x in sorted({*range(0, sample_count),
                      *[random.randint(sample_count, len(uca_to_send) - sample_count) for x in range(0, sample_count)],
                      *range(len(uca_to_send) - sample_count, len(uca_to_send))}):
         sample_events.append([x, json.dumps(uca_to_send[x])])
     print(tabulate(sample_events, headers=["#", "Record"], tablefmt="simple", maxcolwidths=[None, 240]))
```

### Comparing `cloudzero_uca_tools-0.7.3/uca/common/custom_types.py` & `cloudzero_uca_tools-0.7.4/uca/common/custom_types.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.3/uca/common/files.py` & `cloudzero_uca_tools-0.7.4/uca/common/files.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.3/uca/common/formatters.py` & `cloudzero_uca_tools-0.7.4/uca/common/formatters.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.3/uca/common/standards.py` & `cloudzero_uca_tools-0.7.4/uca/common/standards.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.3/uca/data/alb_configuration.json` & `cloudzero_uca_tools-0.7.4/uca/data/alb_configuration.json`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.3/uca/data/example_alb_logs` & `cloudzero_uca_tools-0.7.4/uca/data/example_alb_logs`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.3/uca/features/convert.py` & `cloudzero_uca_tools-0.7.4/uca/features/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 #  Copyright (c) 2021-2023 CloudZero, Inc. or its affiliates. All Rights Reserved.
 #  SPDX-License-Identifier: Apache-2.0
 #  Direct all questions to support@cloudzero.com
 
+import re
 import sys
 from collections import defaultdict, Counter
-import re
 from decimal import Decimal
-
-import simplejson as json
 from string import Template
 
-from uca.vendored.aws_log_parser import AwsLogParser, LogType
+import simplejson as json
 
 from uca.common.cli import eprint
 from uca.common.formatters import rgetattr
 from uca.common.standards import get_seconds_from_time, utc_datetime_from_anything
+from uca.vendored.aws_log_parser import AwsLogParser, LogType
 
 AWS_FORMAT_TYPE = "AWS"
 CSV_FORMAT_TYPE = "CSV"
 
 
 def transform_csv_record(record, configuration):
     schema = configuration.settings['convert']['schema']['columns']
```

### Comparing `cloudzero_uca_tools-0.7.3/uca/features/generate.py` & `cloudzero_uca_tools-0.7.4/uca/features/generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,17 +80,19 @@
                 round_decimal(max(Decimal(abs(Decimal(row[unit_value_header]) + randint(-jitter, jitter))), Decimal(1)),
                               PRECISION))
         elif settings['mode'] == 'allocation':
             jitter = int(settings.get('jitter'))
             try:
                 if jitter:
                     row[unit_value_header] = round_decimal((Decimal(settings['allocation']) *
-                                                            Decimal(row['unit_allocation'])) + randint(0, jitter), PRECISION)
+                                                            Decimal(row['unit_allocation'])) + randint(0, jitter),
+                                                           PRECISION)
                 else:
-                    row[unit_value_header] = round_decimal(Decimal(settings['allocation']) * Decimal(row[unit_value_header]), PRECISION)
+                    row[unit_value_header] = round_decimal(
+                        Decimal(settings['allocation']) * Decimal(row[unit_value_header]), PRECISION)
 
             except KeyError:
                 print('ERROR: Must add "unit_allocation" column to CSV')
                 sys.exit(-1)
             except Exception as error:
                 print(f'ERROR: {error}')
                 sys.exit(-1)
```

### Comparing `cloudzero_uca_tools-0.7.3/uca/features/transform.py` & `cloudzero_uca_tools-0.7.4/uca/features/transform.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.3/uca/features/transmit.py` & `cloudzero_uca_tools-0.7.4/uca/features/transmit.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,9 +17,7 @@
         write_to_file(uca_to_send, output_file)
         print(f'\nWrote results to {output_file}')
     elif api_key:
         print('\nSending to API')
         send_uca_events(api_key, uca_to_send)
     else:
         print('\nFinished, nothing to do')
-
-
```

### Comparing `cloudzero_uca_tools-0.7.3/uca/interfaces/uca_api.py` & `cloudzero_uca_tools-0.7.4/uca/interfaces/uca_api.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.3/uca/vendored/aws_log_parser/interface.py` & `cloudzero_uca_tools-0.7.4/uca/vendored/aws_log_parser/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 import csv
-import typing
 import importlib
 import importlib.util
 import sys
-
+import typing
 from dataclasses import dataclass, fields, field
 from pathlib import Path
 from urllib.parse import urlparse
 
 from .aws import AwsClient
 from .models import (
     LogFormat,
 )
-from .util import batcher
-
 from .parser import to_python
+from .util import batcher
 
 
 @dataclass
 class AwsLogParser:
-
     log_type: LogFormat
 
     # Optional
     region: typing.Optional[str] = None
     profile: typing.Optional[str] = None
     file_suffix: str = ".log"
     verbose: bool = False
```

### Comparing `cloudzero_uca_tools-0.7.3/uca/vendored/aws_log_parser/models.py` & `cloudzero_uca_tools-0.7.4/uca/vendored/aws_log_parser/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import datetime
 import typing
-
+from dataclasses import dataclass
 from enum import (
     Enum,
     auto,
 )
-
-from dataclasses import dataclass, field
 from http import cookies
 
 
 class HttpType(Enum):
     Grpc = "grpc"
     Grpcs = "grpcs"
     Http = "http"
```

### Comparing `cloudzero_uca_tools-0.7.3/uca/vendored/aws_log_parser/parser.py` & `cloudzero_uca_tools-0.7.4/uca/vendored/aws_log_parser/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import datetime
 import logging
 import typing
 import urllib.parse
-
 from http import cookies
 
 from .exceptions import UnknownHttpType
 from .models import (
     HttpType,
     Host,
     HttpRequest,
```

### Comparing `cloudzero_uca_tools-0.7.3/uca/vendored/aws_log_parser/aws/client.py` & `cloudzero_uca_tools-0.7.4/uca/vendored/aws_log_parser/aws/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-import boto3
-import boto3.session
-import typing
-
 import importlib
-
+import typing
 from dataclasses import dataclass
 
+import boto3
+import boto3.session
+
 
 @dataclass
 class AwsClient:
-
     region: typing.Optional[str] = None
     profile: typing.Optional[str] = None
     verbose: bool = False
 
     @property
     def aws_session(self):
         return boto3.session.Session(region_name=self.region, profile_name=self.profile)
@@ -52,14 +50,13 @@
         for tag in tags:
             if tag["Key"] == name:
                 return tag["Value"]
 
 
 @dataclass
 class AwsService:
-
     aws_client: AwsClient
 
     def get_tag(self, tags, name):
         for tag in tags:
             if tag["Key"] == name:
                 return tag["Value"]
```

### Comparing `cloudzero_uca_tools-0.7.3/uca/vendored/aws_log_parser/aws/plugin.py` & `cloudzero_uca_tools-0.7.4/uca/vendored/aws_log_parser/aws/plugin.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing
 from dataclasses import dataclass, field
 
-from aws_log_parser.aws import AwsClient
+from uca.vendored.aws_log_parser.aws import AwsClient
 
 
 @dataclass
 class AwsPluginBase:
     """
     Resolve the instance_id from its private ip address.
     """
@@ -16,15 +16,14 @@
     _cache: typing.Dict[str, str] = field(default_factory=dict)
 
     @property
     def ec2_client(self):
         return self.aws_client.ec2_client
 
     def lookup(self, ips):
-
         unknown = ips - self._cache.keys()
 
         if unknown:
             self.query(list(unknown))
 
         return self._cache
```

### Comparing `cloudzero_uca_tools-0.7.3/uca/vendored/aws_log_parser/aws/s3.py` & `cloudzero_uca_tools-0.7.4/uca/vendored/aws_log_parser/aws/s3.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import gzip
-
 from dataclasses import dataclass
 
 from .client import (
     AwsClient,
     AwsService,
 )
 
 
 @dataclass
 class S3Service(AwsService):
-
     aws_client: AwsClient
 
     @property
     def client(self):
         return self.aws_client.aws_client("s3")
 
     def list_files(self, bucket, prefix, sort_key, reverse=True):
@@ -33,15 +31,14 @@
             print(f"Reading s3://{bucket}/{key}")
         contents = self.client.get_object(Bucket=bucket, Key=key)
         if endswith == ".gz":
             with gzip.GzipFile(fileobj=contents["Body"]) as _gz:
                 yield from [line for line in _gz.read().decode("utf-8").splitlines()]
         else:
             yield from [line.decode("utf-8") for line in contents["Body"].iter_lines()]
-        
 
     def read_keys(self, bucket, prefix, endswith=None):
 
         for file in self.list_files(bucket, prefix, "LastModified"):
             if endswith and not file["Key"].endswith(endswith):
                 continue
```

### Comparing `cloudzero_uca_tools-0.7.3/uca/vendored/aws_log_parser/cli/main.py` & `cloudzero_uca_tools-0.7.4/uca/vendored/aws_log_parser/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import argparse
 import logging
-
 from collections import Counter
 from pathlib import Path
 
 from rich.console import Console
 from rich.table import Table
 
-
 from ..interface import AwsLogParser
 from ..models import LogType
 
 console = Console()
 logger = logging.getLogger(__name__)
 
 
@@ -33,25 +31,24 @@
     total = counter.total()
     for i, pair in enumerate(sorted(counter.items(), key=lambda t: t[1]), 1):
         instance_name, count = pair
         table.add_row(
             str(i),
             instance_name,
             f"{count:,}",
-            f"({(count/total) * 100:.2f}%)",
+            f"({(count / total) * 100:.2f}%)",
             end_section=i == len(counter),
         )
 
     table.add_row("", "Total", f"{total:,}", "")
 
     console.print(table)
 
 
 def main():
-
     parser = argparse.ArgumentParser(description="Parse AWS log data.")
     parser.add_argument(
         "url",
         help="Url to the file to parse",
     )
 
     parser.add_argument(
```

### Comparing `cloudzero_uca_tools-0.7.3/.gitignore` & `cloudzero_uca_tools-0.7.4/.gitignore`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.3/LICENSE` & `cloudzero_uca_tools-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.3/README.md` & `cloudzero_uca_tools-0.7.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ## Features
 * Transmit UCA data to CloudZero (using the CloudZero UCA API)
 * Generate UCA data
 * Convert raw data in CSV form to UCA JSON format
 
 ## prerequisites
 * Tested on MacOS, should probably run on Linux in general
-* Python 3.8 or newer
+* Python 3.9 or newer
 * `pipx` or your favorite method of installing packages from PyPi. Have you considered [pipx](https://pypa.github.io/pipx/)?
 
 ## Installation
       $ pipx install cloudzero-uca-tools
 
 ## General Usage
 CloudZero UCA tools exist to produce UCA events that can then be transmitted to the CloudZero API
```

### Comparing `cloudzero_uca_tools-0.7.3/PKG-INFO` & `cloudzero_uca_tools-0.7.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 Metadata-Version: 2.1
 Name: cloudzero-uca-tools
-Version: 0.7.3
+Version: 0.7.4
 Summary: CloudZero UCA Toolkit
 Project-URL: Homepage, https://github.com/Cloudzero/cloudzero-uca-tools
 Author-email: CloudZero <support@cloudzero.com>
-License-Expression: Apache-2.0
+License: Apache-2.0
 License-File: LICENSE
 Keywords: CloudZero,Toolkit,UCA,analysis,cost,economics,unit
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Requires-Dist: beautifulsoup4>=4.11.2
-Requires-Dist: boto3==1.26.66
+Requires-Dist: boto3==1.26.69
 Requires-Dist: click>=8.1.3
 Requires-Dist: colored>=1.4.4
+Requires-Dist: geoip2==4.6.0
 Requires-Dist: jq>=1.4.0
 Requires-Dist: progressbar>=2.5
+Requires-Dist: python-whois==0.8.0
 Requires-Dist: requests>=2.28.2
+Requires-Dist: rich==13.3.1
 Requires-Dist: simplejson>=3.18.3
 Requires-Dist: stringcase>=1.2.0
 Requires-Dist: tabulate>=0.9.0
+Requires-Dist: user-agents==2.2.0
 Description-Content-Type: text/markdown
 
 # CloudZero UCA Toolkit
 Utilities for generating, transforming and transmitting unit cost analytics (UCA) data to the CloudZero API.
 Visit our [UCA documentation](https://docs.cloudzero.com/docs/enhanced-unit-cost-analytics) to learn more about
 [CloudZero](https://www.cloudzero.com) and our enhanced unit cost analytics capabilities.
 
 ## Features
 * Transmit UCA data to CloudZero (using the CloudZero UCA API)
 * Generate UCA data
 * Convert raw data in CSV form to UCA JSON format
 
 ## prerequisites
 * Tested on MacOS, should probably run on Linux in general
-* Python 3.8 or newer
+* Python 3.9 or newer
 * `pipx` or your favorite method of installing packages from PyPi. Have you considered [pipx](https://pypa.github.io/pipx/)?
 
 ## Installation
       $ pipx install cloudzero-uca-tools
 
 ## General Usage
 CloudZero UCA tools exist to produce UCA events that can then be transmitted to the CloudZero API
```

