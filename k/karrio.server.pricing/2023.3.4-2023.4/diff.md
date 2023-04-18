# Comparing `tmp/karrio.server.pricing-2023.3.4-py3-none-any.whl.zip` & `tmp/karrio.server.pricing-2023.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 216211 bytes, number of entries: 45
+Zip file size: 227187 bytes, number of entries: 46
 -rw-rw-r--  2.0 unx       64 b- defN 22-Nov-15 19:21 karrio/server/pricing/__init__.py
 -rw-rw-r--  2.0 unx     1683 b- defN 23-Mar-03 13:50 karrio/server/pricing/admin.py
 -rw-rw-r--  2.0 unx      341 b- defN 23-Mar-03 13:50 karrio/server/pricing/apps.py
 -rw-rw-r--  2.0 unx     4851 b- defN 23-Mar-03 13:50 karrio/server/pricing/models.py
 -rw-rw-r--  2.0 unx      974 b- defN 22-Nov-15 19:21 karrio/server/pricing/signals.py
 -rw-rw-r--  2.0 unx    11192 b- defN 23-Mar-03 13:50 karrio/server/pricing/tests.py
 -rw-rw-r--  2.0 unx       63 b- defN 22-Nov-15 19:21 karrio/server/pricing/views.py
@@ -29,19 +29,20 @@
 -rw-rw-r--  2.0 unx   148996 b- defN 23-Mar-03 13:50 karrio/server/pricing/migrations/0021_auto_20220413_0959.py
 -rw-rw-r--  2.0 unx   147327 b- defN 23-Mar-03 13:50 karrio/server/pricing/migrations/0022_alter_surcharge_services.py
 -rw-rw-r--  2.0 unx   148652 b- defN 23-Mar-03 13:50 karrio/server/pricing/migrations/0023_auto_20220504_1335.py
 -rw-rw-r--  2.0 unx   148964 b- defN 23-Mar-03 13:50 karrio/server/pricing/migrations/0024_auto_20220808_0803.py
 -rw-rw-r--  2.0 unx     1956 b- defN 23-Mar-03 13:50 karrio/server/pricing/migrations/0025_alter_surcharge_carriers.py
 -rw-rw-r--  2.0 unx   149879 b- defN 23-Mar-03 13:50 karrio/server/pricing/migrations/0026_auto_20220828_0158.py
 -rw-rw-r--  2.0 unx   148613 b- defN 23-Mar-03 13:50 karrio/server/pricing/migrations/0027_alter_surcharge_services.py
--rw-rw-r--  2.0 unx   146202 b- defN 23-Mar-03 13:50 karrio/server/pricing/migrations/0028_surcharge_markup_carriers_surcharge_markup_services.py
+-rw-rw-r--  2.0 unx   146271 b- defN 23-Apr-18 09:52 karrio/server/pricing/migrations/0028_surcharge_markup_carriers_surcharge_markup_services.py
 -rw-rw-r--  2.0 unx   143815 b- defN 23-Mar-03 13:50 karrio/server/pricing/migrations/0029_alter_surcharge_services.py
 -rw-rw-r--  2.0 unx   143844 b- defN 23-Mar-18 11:05 karrio/server/pricing/migrations/0030_alter_surcharge_services.py
 -rw-rw-r--  2.0 unx     2038 b- defN 23-Mar-27 07:55 karrio/server/pricing/migrations/0031_alter_surcharge_carriers.py
 -rw-rw-r--  2.0 unx   145524 b- defN 23-Mar-27 07:55 karrio/server/pricing/migrations/0032_alter_surcharge_services.py
--rw-rw-r--  2.0 unx   145580 b- defN 23-Mar-29 13:29 karrio/server/pricing/migrations/0033_alter_surcharge_services.py
+-rw-rw-r--  2.0 unx   145580 b- defN 23-Mar-29 20:04 karrio/server/pricing/migrations/0033_alter_surcharge_services.py
+-rw-rw-r--  2.0 unx   147914 b- defN 23-Apr-04 12:53 karrio/server/pricing/migrations/0034_alter_surcharge_carriers_alter_surcharge_services.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-15 19:21 karrio/server/pricing/migrations/__init__.py
--rw-rw-r--  2.0 unx      664 b- defN 23-Mar-29 13:38 karrio.server.pricing-2023.3.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-29 13:38 karrio.server.pricing-2023.3.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Mar-29 13:38 karrio.server.pricing-2023.3.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     5040 b- defN 23-Mar-29 13:38 karrio.server.pricing-2023.3.4.dist-info/RECORD
-45 files, 2662543 bytes uncompressed, 207761 bytes compressed:  92.2%
+-rw-rw-r--  2.0 unx      662 b- defN 23-Apr-18 10:32 karrio.server.pricing-2023.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 10:32 karrio.server.pricing-2023.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 10:32 karrio.server.pricing-2023.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     5181 b- defN 23-Apr-18 10:32 karrio.server.pricing-2023.4.dist-info/RECORD
+46 files, 2810665 bytes uncompressed, 218497 bytes compressed:  92.2%
```

## zipnote {}

```diff
@@ -114,23 +114,26 @@
 
 Filename: karrio/server/pricing/migrations/0032_alter_surcharge_services.py
 Comment: 
 
 Filename: karrio/server/pricing/migrations/0033_alter_surcharge_services.py
 Comment: 
 
+Filename: karrio/server/pricing/migrations/0034_alter_surcharge_carriers_alter_surcharge_services.py
+Comment: 
+
 Filename: karrio/server/pricing/migrations/__init__.py
 Comment: 
 
-Filename: karrio.server.pricing-2023.3.4.dist-info/METADATA
+Filename: karrio.server.pricing-2023.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.server.pricing-2023.3.4.dist-info/WHEEL
+Filename: karrio.server.pricing-2023.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.server.pricing-2023.3.4.dist-info/top_level.txt
+Filename: karrio.server.pricing-2023.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.server.pricing-2023.3.4.dist-info/RECORD
+Filename: karrio.server.pricing-2023.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/server/pricing/migrations/0028_surcharge_markup_carriers_surcharge_markup_services.py

```diff
@@ -7,42 +7,44 @@
 
 
 def forwards_func(apps, schema_editor):
     db_alias = schema_editor.connection.alias
     Markup = apps.get_model("pricing", "Surcharge")
     _charges = []
 
-    for markup in Markup.objects.using(db_alias).all():
+    for markup in Markup.objects.using(db_alias).all().iterator():
         markup.markup_carriers = lib.to_dict(markup.carriers)
         markup.markup_services = lib.to_dict(markup.services)
         _charges.append(markup)
 
     Markup.objects.using(db_alias).bulk_update(
         _charges, ["markup_carriers", "markup_services"]
     )
 
 
 def reverse_func(apps, schema_editor):
     pass
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("pricing", "0027_alter_surcharge_services"),
     ]
     operations = []
 
     if "postgres" in settings.DB_ENGINE:
         operations += [
-            migrations.RunSQL('ALTER TABLE "surcharge" ALTER COLUMN "carriers" TYPE jsonb USING to_jsonb(carriers)'),
-            migrations.RunSQL('ALTER TABLE "surcharge" ALTER COLUMN "services" TYPE jsonb USING to_jsonb(services)'),
+            migrations.RunSQL(
+                'ALTER TABLE "surcharge" ALTER COLUMN "carriers" TYPE jsonb USING to_jsonb(carriers)'
+            ),
+            migrations.RunSQL(
+                'ALTER TABLE "surcharge" ALTER COLUMN "services" TYPE jsonb USING to_jsonb(services)'
+            ),
         ]
 
-
     operations += [
         migrations.AddField(
             model_name="surcharge",
             name="markup_carriers",
             field=karrio.server.core.fields.MultiChoiceField(
                 blank=True,
                 choices=[
```

## Comparing `karrio.server.pricing-2023.3.4.dist-info/METADATA` & `karrio.server.pricing-2023.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.server.pricing
-Version: 2023.3.4
+Version: 2023.4
 Summary: Multi-carrier shipping API Pricing panel
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `karrio.server.pricing-2023.3.4.dist-info/RECORD` & `karrio.server.pricing-2023.4.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,19 @@
 karrio/server/pricing/migrations/0021_auto_20220413_0959.py,sha256=s6Aa5d_JPfW0EnhR8orqesEG0oxnbR6qvZSzxuWZBmY,148996
 karrio/server/pricing/migrations/0022_alter_surcharge_services.py,sha256=xYT-lXPpWy5GuKBPN50fl_jNmXZ_4S8KkZbHRZeezRc,147327
 karrio/server/pricing/migrations/0023_auto_20220504_1335.py,sha256=QZ4cu3ZkAe7osAq63GIkuvvfVYjrYi2H3_rhT11heCk,148652
 karrio/server/pricing/migrations/0024_auto_20220808_0803.py,sha256=BKRvV7XAbDF6krnvQ7paHFmWnjCBHTizdlK7D34LkjI,148964
 karrio/server/pricing/migrations/0025_alter_surcharge_carriers.py,sha256=xdbs4YjH0JMTlVG8X1Bk4Ge7Zwa8Oy2t-A5PlZH9ZzY,1956
 karrio/server/pricing/migrations/0026_auto_20220828_0158.py,sha256=9HQrd1Rn2_UpOciXQpEdUuXQ0PCs0rIIS7Sugmy_QpY,149879
 karrio/server/pricing/migrations/0027_alter_surcharge_services.py,sha256=3RdA8DfSM-IIP1fN16oTW2EERNm404mrTPvu1rn5F6M,148613
-karrio/server/pricing/migrations/0028_surcharge_markup_carriers_surcharge_markup_services.py,sha256=8P7fPSXVIu8SZPhZ-YS9ajOOHLfOgqo_sB1WMBVkG28,146202
+karrio/server/pricing/migrations/0028_surcharge_markup_carriers_surcharge_markup_services.py,sha256=ROgSx45w2OQUNZGCt3hJJ_beLW_cdDFcOAlSR-bJrtY,146271
 karrio/server/pricing/migrations/0029_alter_surcharge_services.py,sha256=XpVrqiMLQCCu4ypS0VYtsmzx7t2doXwlqWWG8ehG588,143815
 karrio/server/pricing/migrations/0030_alter_surcharge_services.py,sha256=5lJDxemu6bIqjmGnl3wDNlRJEtvqRd2s2KSfTCg6Fec,143844
 karrio/server/pricing/migrations/0031_alter_surcharge_carriers.py,sha256=Bpxcg8XThUWnFzFyNhnCqq9fKE6-lXm-fm-3benFuDY,2038
 karrio/server/pricing/migrations/0032_alter_surcharge_services.py,sha256=F1wDXYEWVAou7oEf3UP8JP5-PN-715K2hTV4ZbLVgG8,145524
 karrio/server/pricing/migrations/0033_alter_surcharge_services.py,sha256=-LHjLXjRDZ1gYKGypoMnHDEB5cYfvNlo5no8aNS8wYQ,145580
+karrio/server/pricing/migrations/0034_alter_surcharge_carriers_alter_surcharge_services.py,sha256=SWYcOsmN47OW0A9aOyR8V7-WNxHyOcO05u5owjjVKyI,147914
 karrio/server/pricing/migrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-karrio.server.pricing-2023.3.4.dist-info/METADATA,sha256=Oe5sk9G-JLYU1xZZTiZi4jKSsaj-B0XvA17KzZUlbyQ,664
-karrio.server.pricing-2023.3.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.server.pricing-2023.3.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.server.pricing-2023.3.4.dist-info/RECORD,,
+karrio.server.pricing-2023.4.dist-info/METADATA,sha256=RhN-chr0YpfkpJzoe2LsomqTMLDkeyza_7cEfADXyh8,662
+karrio.server.pricing-2023.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.server.pricing-2023.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.server.pricing-2023.4.dist-info/RECORD,,
```

