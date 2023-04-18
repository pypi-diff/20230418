# Comparing `tmp/pymodelio-1.0.2-py3-none-any.whl.zip` & `tmp/pymodelio-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 26849 bytes, number of entries: 40
--rw-r--r--  2.0 unx      374 b- defN 23-Apr-18 20:36 pymodelio/__init__.py
+Zip file size: 26843 bytes, number of entries: 40
+-rw-r--r--  2.0 unx      374 b- defN 23-Apr-18 20:44 pymodelio/__init__.py
 -rw-r--r--  2.0 unx     1882 b- defN 23-Apr-18 12:32 pymodelio/attribute.py
 -rw-r--r--  2.0 unx       67 b- defN 22-Sep-06 22:04 pymodelio/constants.py
 -rw-r--r--  2.0 unx      845 b- defN 23-Apr-18 13:35 pymodelio/model_serializer.py
 -rw-r--r--  2.0 unx      408 b- defN 23-Apr-17 16:04 pymodelio/pymodelio_cache.py
 -rw-r--r--  2.0 unx    10788 b- defN 23-Apr-18 20:37 pymodelio/pymodelio_model.py
 -rw-r--r--  2.0 unx       44 b- defN 23-Apr-18 14:09 pymodelio/shared_vars.py
 -rw-r--r--  2.0 unx       88 b- defN 23-Apr-13 15:15 pymodelio/undefined.py
@@ -18,25 +18,25 @@
 -rw-r--r--  2.0 unx      398 b- defN 23-Apr-15 22:13 pymodelio/settings/pymodelio_setting.py
 -rw-r--r--  2.0 unx     1040 b- defN 23-Apr-15 22:13 pymodelio/settings/pymodelio_settings.py
 -rw-r--r--  2.0 unx      635 b- defN 23-Apr-18 14:19 pymodelio/validators/__init__.py
 -rw-r--r--  2.0 unx      285 b- defN 22-Sep-06 22:04 pymodelio/validators/bool_validator.py
 -rw-r--r--  2.0 unx      323 b- defN 22-Sep-06 22:04 pymodelio/validators/datetime_validator.py
 -rw-r--r--  2.0 unx     5539 b- defN 23-Apr-18 19:48 pymodelio/validators/default_validators_builder.py
 -rw-r--r--  2.0 unx      285 b- defN 22-Sep-06 22:04 pymodelio/validators/dict_validator.py
--rw-r--r--  2.0 unx      756 b- defN 23-Apr-18 19:51 pymodelio/validators/email_validator.py
+-rw-r--r--  2.0 unx      752 b- defN 23-Apr-18 20:42 pymodelio/validators/email_validator.py
 -rw-r--r--  2.0 unx      463 b- defN 22-Sep-06 22:04 pymodelio/validators/float_validator.py
 -rw-r--r--  2.0 unx      961 b- defN 23-Apr-18 16:31 pymodelio/validators/forward_ref_validator.py
 -rw-r--r--  2.0 unx      455 b- defN 22-Sep-06 22:04 pymodelio/validators/int_validator.py
 -rw-r--r--  2.0 unx     1331 b- defN 23-Apr-18 19:51 pymodelio/validators/iterable_validator.py
 -rw-r--r--  2.0 unx      473 b- defN 22-Sep-06 22:04 pymodelio/validators/list_validator.py
 -rw-r--r--  2.0 unx     1010 b- defN 23-Apr-15 15:13 pymodelio/validators/numeric_validator.py
 -rw-r--r--  2.0 unx      471 b- defN 23-Apr-16 21:48 pymodelio/validators/set_validator.py
 -rw-r--r--  2.0 unx     1341 b- defN 23-Apr-15 15:14 pymodelio/validators/string_validator.py
 -rw-r--r--  2.0 unx      475 b- defN 23-Apr-16 21:48 pymodelio/validators/tuple_validator.py
 -rw-r--r--  2.0 unx      274 b- defN 22-Sep-06 22:04 pymodelio/validators/validation_patterns.py
 -rw-r--r--  2.0 unx     1372 b- defN 23-Apr-18 19:50 pymodelio/validators/validator.py
--rw-r--r--  2.0 unx     1070 b- defN 23-Apr-18 20:38 pymodelio-1.0.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    24491 b- defN 23-Apr-18 20:38 pymodelio-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 20:38 pymodelio-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-18 20:38 pymodelio-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3608 b- defN 23-Apr-18 20:38 pymodelio-1.0.2.dist-info/RECORD
-40 files, 63577 bytes uncompressed, 20947 bytes compressed:  67.1%
+-rw-r--r--  2.0 unx     1070 b- defN 23-Apr-18 20:45 pymodelio-1.0.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    24491 b- defN 23-Apr-18 20:45 pymodelio-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 20:45 pymodelio-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-18 20:45 pymodelio-1.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3608 b- defN 23-Apr-18 20:45 pymodelio-1.0.3.dist-info/RECORD
+40 files, 63573 bytes uncompressed, 20941 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -99,23 +99,23 @@
 
 Filename: pymodelio/validators/validation_patterns.py
 Comment: 
 
 Filename: pymodelio/validators/validator.py
 Comment: 
 
-Filename: pymodelio-1.0.2.dist-info/LICENSE.txt
+Filename: pymodelio-1.0.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pymodelio-1.0.2.dist-info/METADATA
+Filename: pymodelio-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: pymodelio-1.0.2.dist-info/WHEEL
+Filename: pymodelio-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: pymodelio-1.0.2.dist-info/top_level.txt
+Filename: pymodelio-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pymodelio-1.0.2.dist-info/RECORD
+Filename: pymodelio-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pymodelio/__init__.py

```diff
@@ -1,10 +1,10 @@
 # flake8: noqa
 
-__version__ = '1.0.2'
+__version__ = '1.0.3'
 
 # constants
 from .constants import UNDEFINED
 
 # Settings
 from .settings.pymodelio_setting import PymodelioSetting
 from .settings.pymodelio_settings import PymodelioSettings
```

## pymodelio/validators/email_validator.py

```diff
@@ -12,8 +12,8 @@
 
     def validate(self, value: Any, path: str = None) -> None:
         super().validate(value, path)
         if value is None:
             return
         # Is override for adding a custom message and validating the string as lowercase
         if re.compile(EMAIL_VALIDATION_PATTERN).match(value.lower()) is None:
-            self.raise_validation_error(path, 'is not instance of email address')
+            self.raise_validation_error(path, 'is not a valid email address')
```

## Comparing `pymodelio-1.0.2.dist-info/LICENSE.txt` & `pymodelio-1.0.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pymodelio-1.0.2.dist-info/METADATA` & `pymodelio-1.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodelio
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple Python module for defining domain models, serializing, deserializing and validating them
 Home-page: https://github.com/GabrielMartinMoran/pymodelio
 Author: Gabriel Martín Moran
 Author-email: moran.gabriel.95@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: ciso8601
```

## Comparing `pymodelio-1.0.2.dist-info/RECORD` & `pymodelio-1.0.3.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pymodelio/__init__.py,sha256=oDNDOWdI9D783BqShOc669fnHCfQv3F-IVZ1ytQJmYo,374
+pymodelio/__init__.py,sha256=SRItuevLvz-A8BUpZdujEDmTXPJ5fb6Z8rNdqQQrl7k,374
 pymodelio/attribute.py,sha256=W9z_mZg6892XqqQ_t1fvwHJG-cJ7UyrGNUHdvcSwlQU,1882
 pymodelio/constants.py,sha256=qDMrr5LAO8nm9yVfWJbCJ6MV9WenSypNm4GBVopNgwY,67
 pymodelio/model_serializer.py,sha256=S3Ywak4tdorwSYsI4mvUMRXlA7d8H0_fC6wvHOl5YU0,845
 pymodelio/pymodelio_cache.py,sha256=BQ9tWj8oIcTBIqlwI_-XR3Nm4DAadLy6OVZSgmr-W84,408
 pymodelio/pymodelio_model.py,sha256=v9WK8rkZIaxoCJp0P7zyXIjUGjyilKEL4pHcQ5UMjdA,10788
 pymodelio/shared_vars.py,sha256=grXRCAaGUhOG1-tENkcZgJEndtZJSQvF_QU7qbRjycc,44
 pymodelio/undefined.py,sha256=dvmNY7_3EmfidEGomJNzWXkOdbg8VfJski1t05mniH0,88
@@ -17,24 +17,24 @@
 pymodelio/settings/pymodelio_setting.py,sha256=iaG5QqJHLqWJcbV2KPVOnu40qU8pmrRJ2pOGTpn6_p0,398
 pymodelio/settings/pymodelio_settings.py,sha256=4BqMNG9Rx9PNRk1aOV2G4aWKyHH5eVPtFUEfblKjXXE,1040
 pymodelio/validators/__init__.py,sha256=D2ACgRBgX97IRmKurhDZNegxtW_6ZYnUioqocYMRQkc,635
 pymodelio/validators/bool_validator.py,sha256=KHTd2I0QRUX-8Lcrxvtg1wqLZvsMotlwv1VpCiZi-cc,285
 pymodelio/validators/datetime_validator.py,sha256=TZ9Pt_zJZT49OIhAZyf7U37bKWesHQXpJoy6bg6mCjc,323
 pymodelio/validators/default_validators_builder.py,sha256=hQtRE9DkXxSQsamfr5_1Lovk_ohEUJBMXjQpHjS7l88,5539
 pymodelio/validators/dict_validator.py,sha256=Y_NmLEFdySBbuDcEdbPCVRF3Sf_mrnyUbdROA8zwSTk,285
-pymodelio/validators/email_validator.py,sha256=nxABnmeYvxdUNf4HKBDJZdPwNhaGm6r_1zk5ESWSA7E,756
+pymodelio/validators/email_validator.py,sha256=xFHPHRNoznLWnd8QVuEbH9BSJxnoszR1RgdkOVCXwN0,752
 pymodelio/validators/float_validator.py,sha256=LOy0OEYn7_7FxILFVngYd24gYEeUF6D5IFJCc44PVXI,463
 pymodelio/validators/forward_ref_validator.py,sha256=8uk-vdrX9TPmg7CnNEhAxPm_mlt1D3o8SCqymddoJyo,961
 pymodelio/validators/int_validator.py,sha256=_3TJIKZN9G8wprtizbV4JgBiNX2rvsiZmugHjRcno54,455
 pymodelio/validators/iterable_validator.py,sha256=jgtBWEjO54lzDYD_X14aai6qkR301303w4YNOxC8CZw,1331
 pymodelio/validators/list_validator.py,sha256=T5-7KDGyLsg8o7WFAO7djOkKLGrmqzb9Q8Pv2TcvuvY,473
 pymodelio/validators/numeric_validator.py,sha256=M6TpOVg69P460AvBPeu32_sGv9xE_TedmC9nXl7peaA,1010
 pymodelio/validators/set_validator.py,sha256=X7XcbS6Az4E9snK4g_Vr6jXEnGJTY4qGBOQ8HC8ycUQ,471
 pymodelio/validators/string_validator.py,sha256=HidLUkuIYmDhDIZuWa5LYVX6w1rm2XupYhzQY_G9rZM,1341
 pymodelio/validators/tuple_validator.py,sha256=GLva3HKUmGWTfohgfC1mW2q7DfPl_qIQ5RAH6V8KWt4,475
 pymodelio/validators/validation_patterns.py,sha256=-gSYH0dt_J-K2A10VeAv6bEIi4TRV8x8OWLkYuLZrk4,274
 pymodelio/validators/validator.py,sha256=JvkMDxCpGre4oIJARzF1D7ZED3xsbI1kUmkdp7t0CcE,1372
-pymodelio-1.0.2.dist-info/LICENSE.txt,sha256=sL92kzk5LocRUegJuJvjbS-U5nceM2IAKHEUIavtJ90,1070
-pymodelio-1.0.2.dist-info/METADATA,sha256=gD0pGxTNTs8pS7SXYVghRLTSDBvzdT-3cWcM3_KBYIc,24491
-pymodelio-1.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pymodelio-1.0.2.dist-info/top_level.txt,sha256=XrPsEjrAMkBQoxcrC6tFQs-EiY6TbHuDV5I68o5ZZyE,10
-pymodelio-1.0.2.dist-info/RECORD,,
+pymodelio-1.0.3.dist-info/LICENSE.txt,sha256=sL92kzk5LocRUegJuJvjbS-U5nceM2IAKHEUIavtJ90,1070
+pymodelio-1.0.3.dist-info/METADATA,sha256=3rrRNzAMYFiLyDbpbIIkCita0DOuHO09mje4QFPcD-0,24491
+pymodelio-1.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pymodelio-1.0.3.dist-info/top_level.txt,sha256=XrPsEjrAMkBQoxcrC6tFQs-EiY6TbHuDV5I68o5ZZyE,10
+pymodelio-1.0.3.dist-info/RECORD,,
```

