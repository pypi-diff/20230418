# Comparing `tmp/telus_bulk-1.3.5.tar.gz` & `tmp/telus_bulk-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telus_bulk-1.3.5.tar", last modified: Thu Apr 13 21:40:52 2023, max compression
+gzip compressed data, was "telus_bulk-1.3.6.tar", last modified: Tue Apr 18 16:41:18 2023, max compression
```

## Comparing `telus_bulk-1.3.5.tar` & `telus_bulk-1.3.6.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 21:40:52.303653 telus_bulk-1.3.5/
--rw-rw-rw-   0        0        0     1091 2022-09-21 18:35:35.000000 telus_bulk-1.3.5/LICENSE
--rw-rw-rw-   0        0        0     5312 2023-04-13 21:40:52.301154 telus_bulk-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     3431 2023-04-13 21:39:06.000000 telus_bulk-1.3.5/README.md
--rw-rw-rw-   0        0        0     1013 2023-04-13 21:38:04.000000 telus_bulk-1.3.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 21:40:52.305152 telus_bulk-1.3.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 21:40:51.671585 telus_bulk-1.3.5/src/
--rw-rw-rw-   0        0        0        0 2022-09-29 17:24:33.000000 telus_bulk-1.3.5/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 21:40:51.676086 telus_bulk-1.3.5/src/telus_bulk/
--rw-rw-rw-   0        0        0       72 2022-09-29 16:01:50.000000 telus_bulk-1.3.5/src/telus_bulk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 21:40:51.703114 telus_bulk-1.3.5/src/telus_bulk/helpers/
-drwxrwxrwx   0        0        0        0 2023-04-13 21:40:51.713090 telus_bulk-1.3.5/src/telus_bulk/helpers/cron_job/
--rw-rw-rw-   0        0        0       62 2022-11-30 18:14:51.000000 telus_bulk-1.3.5/src/telus_bulk/helpers/cron_job/__init__.py
--rw-rw-rw-   0        0        0      709 2022-11-30 18:14:22.000000 telus_bulk-1.3.5/src/telus_bulk/helpers/cron_job/thread_job.py
--rw-rw-rw-   0        0        0       82 2022-10-05 22:39:52.000000 telus_bulk-1.3.5/src/telus_bulk/helpers/mutiple_spaces.py
-drwxrwxrwx   0        0        0        0 2023-04-13 21:40:51.728589 telus_bulk-1.3.5/src/telus_bulk/helpers/web_methods/
--rw-rw-rw-   0        0        0      200 2022-12-20 23:56:52.000000 telus_bulk-1.3.5/src/telus_bulk/helpers/web_methods/__init__.py
--rw-rw-rw-   0        0        0     2569 2022-12-20 23:56:35.000000 telus_bulk-1.3.5/src/telus_bulk/helpers/web_methods/async_web_methods_helper.py
--rw-rw-rw-   0        0        0     2447 2022-10-25 17:08:26.000000 telus_bulk-1.3.5/src/telus_bulk/helpers/web_methods/web_methods_helper.py
-drwxrwxrwx   0        0        0        0 2023-04-13 21:40:51.738585 telus_bulk-1.3.5/src/telus_bulk/models/
--rw-rw-rw-   0        0        0       65 2022-09-14 17:56:07.000000 telus_bulk-1.3.5/src/telus_bulk/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 21:40:51.796086 telus_bulk-1.3.5/src/telus_bulk/models/ams/
--rw-rw-rw-   0        0        0       75 2022-09-14 17:37:58.000000 telus_bulk-1.3.5/src/telus_bulk/models/ams/__init__.py
--rw-rw-rw-   0        0        0     2788 2022-10-05 23:54:12.000000 telus_bulk-1.3.5/src/telus_bulk/models/ams/address_detail_model.py
--rw-rw-rw-   0        0        0      470 2022-11-29 22:57:32.000000 telus_bulk-1.3.5/src/telus_bulk/models/ams/city_alias.py
--rw-rw-rw-   0        0        0      519 2022-09-26 23:03:35.000000 telus_bulk-1.3.5/src/telus_bulk/models/ams/coordinate.py
--rw-rw-rw-   0        0        0      230 2022-08-09 18:59:43.000000 telus_bulk-1.3.5/src/telus_bulk/models/ams/credentials_response.py
--rw-rw-rw-   0        0        0      506 2022-09-12 17:32:45.000000 telus_bulk-1.3.5/src/telus_bulk/models/ams/e911_address.py
--rw-rw-rw-   0        0        0      856 2022-10-05 23:50:04.000000 telus_bulk-1.3.5/src/telus_bulk/models/ams/fms_address.py
--rw-rw-rw-   0        0        0      392 2022-10-05 23:46:20.000000 telus_bulk-1.3.5/src/telus_bulk/models/ams/reference_id.py
--rw-rw-rw-   0        0        0      302 2022-10-05 23:52:28.000000 telus_bulk-1.3.5/src/telus_bulk/models/ams/reference_ids.py
--rw-rw-rw-   0        0        0      657 2022-08-15 17:21:00.000000 telus_bulk-1.3.5/src/telus_bulk/models/ams/zone_attribute.py
--rw-rw-rw-   0        0        0      464 2022-10-05 23:47:15.000000 telus_bulk-1.3.5/src/telus_bulk/models/ams/zone_info_item.py
-drwxrwxrwx   0        0        0        0 2023-04-13 21:40:51.805586 telus_bulk-1.3.5/src/telus_bulk/models/available_partners/
--rw-rw-rw-   0        0        0      118 2022-09-29 17:42:55.000000 telus_bulk-1.3.5/src/telus_bulk/models/available_partners/__init__.py
--rw-rw-rw-   0        0        0      352 2022-09-29 17:42:42.000000 telus_bulk-1.3.5/src/telus_bulk/models/available_partners/partners_enum.py
-drwxrwxrwx   0        0        0        0 2023-04-13 21:40:51.815085 telus_bulk-1.3.5/src/telus_bulk/models/clli/
--rw-rw-rw-   0        0        0       50 2022-11-08 00:11:09.000000 telus_bulk-1.3.5/src/telus_bulk/models/clli/__init__.py
--rw-rw-rw-   0        0        0      448 2022-11-18 22:55:35.000000 telus_bulk-1.3.5/src/telus_bulk/models/clli/clli_dto.py
-drwxrwxrwx   0        0        0        0 2023-04-13 21:40:51.820586 telus_bulk-1.3.5/src/telus_bulk/models/firestore/
--rw-rw-rw-   0        0        0      821 2022-10-21 18:53:27.000000 telus_bulk-1.3.5/src/telus_bulk/models/firestore/firestore_reference.py
--rw-rw-rw-   0        0        0       92 2022-10-18 17:59:41.000000 telus_bulk-1.3.5/src/telus_bulk/models/product_type.py
-drwxrwxrwx   0        0        0        0 2023-04-13 21:40:51.835089 telus_bulk-1.3.5/src/telus_bulk/models/reports/
--rw-rw-rw-   0        0        0      155 2022-11-11 21:28:00.000000 telus_bulk-1.3.5/src/telus_bulk/models/reports/__init__.py
--rw-rw-rw-   0        0        0     1208 2023-04-13 21:10:46.000000 telus_bulk-1.3.5/src/telus_bulk/models/reports/report_address.py
--rw-rw-rw-   0        0        0      395 2022-11-17 17:58:06.000000 telus_bulk-1.3.5/src/telus_bulk/models/reports/report_qualification_detail.py
-drwxrwxrwx   0        0        0        0 2023-04-13 21:40:51.844586 telus_bulk-1.3.5/src/telus_bulk/models/tmf_620/
--rw-rw-rw-   0        0        0       58 2022-12-30 21:59:38.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_620/__init__.py
--rw-rw-rw-   0        0        0      109 2022-12-30 21:58:25.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_620/status_enum.py
-drwxrwxrwx   0        0        0        0 2023-04-13 21:40:52.223152 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/
--rw-rw-rw-   0        0        0        0 2022-07-20 23:06:53.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/__init__.py
--rw-rw-rw-   0        0        0     1078 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/addressable.py
--rw-rw-rw-   0        0        0     1511 2022-09-14 17:54:30.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/alternate_service_proposal.py
--rw-rw-rw-   0        0        0     1539 2022-09-14 17:54:33.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/characteristic.py
--rw-rw-rw-   0        0        0     1220 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/characteristic_relationship.py
--rw-rw-rw-   0        0        0     3724 2022-10-25 17:09:23.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification.py
--rw-rw-rw-   0        0        0     2442 2022-09-14 17:54:33.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_attribute_value_change_event.py
--rw-rw-rw-   0        0        0      993 2022-09-14 17:54:33.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_attribute_value_change_event_payload.py
--rw-rw-rw-   0        0        0     2666 2022-11-09 14:29:21.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_create.py
--rw-rw-rw-   0        0        0     2071 2022-09-14 17:54:33.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_create_event.py
--rw-rw-rw-   0        0        0      937 2022-09-14 17:54:33.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_create_event_payload.py
--rw-rw-rw-   0        0        0     2071 2022-09-14 17:54:33.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_delete_event.py
--rw-rw-rw-   0        0        0      937 2022-09-14 17:54:33.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_delete_event_payload.py
--rw-rw-rw-   0        0        0     2424 2022-09-14 17:54:33.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_information_required_event.py
--rw-rw-rw-   0        0        0      989 2022-09-14 17:54:33.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_information_required_event_payload.py
--rw-rw-rw-   0        0        0     4516 2022-10-31 17:35:23.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_item.py
--rw-rw-rw-   0        0        0     2905 2022-09-14 17:54:33.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_queue_item.py
--rw-rw-rw-   0        0        0     2152 2022-09-14 17:54:32.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_state_change_event.py
--rw-rw-rw-   0        0        0      957 2022-09-14 17:54:32.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_state_change_event_payload.py
--rw-rw-rw-   0        0        0     3362 2022-09-14 17:54:32.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_update.py
--rw-rw-rw-   0        0        0     1407 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/constraint_ref.py
--rw-rw-rw-   0        0        0     1271 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/entity_ref.py
--rw-rw-rw-   0        0        0     1075 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/entity_value.py
--rw-rw-rw-   0        0        0     1280 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/error.py
--rw-rw-rw-   0        0        0      777 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/event_subscription.py
--rw-rw-rw-   0        0        0      742 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/event_subscription_input.py
--rw-rw-rw-   0        0        0      214 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/example.py
--rw-rw-rw-   0        0        0      899 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/extensible.py
--rw-rw-rw-   0        0        0      146 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/extra_models.py
--rw-rw-rw-   0        0        0     1836 2022-09-14 17:54:32.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/feature.py
--rw-rw-rw-   0        0        0     1400 2022-09-14 17:54:31.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/feature_relationship.py
--rw-rw-rw-   0        0        0     1192 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/note.py
--rw-rw-rw-   0        0        0      546 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/order_item_action_type.py
--rw-rw-rw-   0        0        0     1659 2022-10-25 17:10:03.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/overall_process.py
--rw-rw-rw-   0        0        0     1109 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/place.py
--rw-rw-rw-   0        0        0     1261 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/place_ref.py
--rw-rw-rw-   0        0        0     3301 2022-09-14 17:54:31.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/query_service_qualification.py
--rw-rw-rw-   0        0        0     2094 2022-09-14 17:54:31.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/query_service_qualification_create.py
--rw-rw-rw-   0        0        0     2071 2022-09-14 17:54:31.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/query_service_qualification_create_event.py
--rw-rw-rw-   0        0        0      937 2022-09-14 17:54:31.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/query_service_qualification_create_event_payload.py
--rw-rw-rw-   0        0        0     2071 2022-09-14 17:54:31.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/query_service_qualification_delete_event.py
--rw-rw-rw-   0        0        0      937 2022-09-14 17:54:31.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/query_service_qualification_delete_event_payload.py
--rw-rw-rw-   0        0        0     2152 2022-09-14 17:54:30.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/query_service_qualification_state_change_event.py
--rw-rw-rw-   0        0        0      957 2022-09-14 17:54:30.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/query_service_qualification_state_change_event_payload.py
--rw-rw-rw-   0        0        0     3014 2022-09-14 17:54:30.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/query_service_qualification_update.py
--rw-rw-rw-   0        0        0     1494 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/related_entity_ref_or_value.py
--rw-rw-rw-   0        0        0     1526 2022-12-12 21:11:57.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/related_party.py
--rw-rw-rw-   0        0        0     1645 2023-01-26 22:32:07.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/related_place_ref_or_value.py
--rw-rw-rw-   0        0        0     1780 2022-09-14 17:54:30.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/related_service_order_item.py
--rw-rw-rw-   0        0        0     1277 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/resource_ref.py
--rw-rw-rw-   0        0        0     4778 2022-09-14 17:54:30.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/service.py
--rw-rw-rw-   0        0        0     1451 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/service_category_ref.py
--rw-rw-rw-   0        0        0     1371 2022-10-24 21:26:56.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/service_eligibility_unavailability_reason.py
--rw-rw-rw-   0        0        0     2572 2022-09-14 17:54:32.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/service_qualification.py
--rw-rw-rw-   0        0        0     1990 2022-09-14 17:54:32.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/service_qualification_item.py
--rw-rw-rw-   0        0        0     1314 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/service_qualification_item_relationship.py
--rw-rw-rw-   0        0        0     1282 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/service_qualification_relationship.py
--rw-rw-rw-   0        0        0     1281 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/service_ref.py
--rw-rw-rw-   0        0        0     6545 2022-10-21 21:16:52.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/service_ref_or_value.py
--rw-rw-rw-   0        0        0     1520 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/service_specification_ref.py
--rw-rw-rw-   0        0        0      537 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/service_state_type.py
--rw-rw-rw-   0        0        0      528 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/task_state_type.py
--rw-rw-rw-   0        0        0     1118 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/termination_error.py
--rw-rw-rw-   0        0        0     1143 2022-08-02 18:19:44.000000 telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/time_period.py
-drwxrwxrwx   0        0        0        0 2023-04-13 21:40:52.253153 telus_bulk-1.3.5/src/telus_bulk/models/worker_job/
--rw-rw-rw-   0        0        0      173 2022-09-26 22:38:16.000000 telus_bulk-1.3.5/src/telus_bulk/models/worker_job/__init__.py
--rw-rw-rw-   0        0        0     1169 2022-09-14 20:38:25.000000 telus_bulk-1.3.5/src/telus_bulk/models/worker_job/address_processing_job.py
--rw-rw-rw-   0        0        0      426 2023-03-27 23:18:27.000000 telus_bulk-1.3.5/src/telus_bulk/models/worker_job/city_coverage_processed_job.py
--rw-rw-rw-   0        0        0     1306 2023-01-26 22:56:40.000000 telus_bulk-1.3.5/src/telus_bulk/models/worker_job/place.py
--rw-rw-rw-   0        0        0      418 2022-09-12 18:55:49.000000 telus_bulk-1.3.5/src/telus_bulk/models/worker_job/service_specification.py
-drwxrwxrwx   0        0        0        0 2023-04-13 21:40:52.277157 telus_bulk-1.3.5/src/telus_bulk/pagination/
--rw-rw-rw-   0        0        0      113 2022-10-13 18:10:36.000000 telus_bulk-1.3.5/src/telus_bulk/pagination/__init__.py
--rw-rw-rw-   0        0        0      349 2022-10-13 21:12:04.000000 telus_bulk-1.3.5/src/telus_bulk/pagination/page_dto.py
--rw-rw-rw-   0        0        0      641 2022-10-13 21:39:09.000000 telus_bulk-1.3.5/src/telus_bulk/pagination/page_meta_dto.py
-drwxrwxrwx   0        0        0        0 2023-04-13 21:40:51.698091 telus_bulk-1.3.5/src/telus_bulk.egg-info/
--rw-rw-rw-   0        0        0     5312 2023-04-13 21:40:51.000000 telus_bulk-1.3.5/src/telus_bulk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5932 2023-04-13 21:40:51.000000 telus_bulk-1.3.5/src/telus_bulk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 21:40:51.000000 telus_bulk-1.3.5/src/telus_bulk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-13 21:40:51.000000 telus_bulk-1.3.5/src/telus_bulk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 21:40:52.291653 telus_bulk-1.3.5/tests/
--rw-rw-rw-   0        0        0      358 2022-09-29 18:01:51.000000 telus_bulk-1.3.5/tests/test_available_partner.py
--rw-rw-rw-   0        0        0      325 2022-10-05 22:35:35.000000 telus_bulk-1.3.5/tests/test_helpers.py
--rw-rw-rw-   0        0        0     1141 2022-11-09 14:32:32.000000 telus_bulk-1.3.5/tests/test_svc_create.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:41:18.378934 telus_bulk-1.3.6/
+-rw-rw-rw-   0        0        0     1091 2022-09-21 18:35:35.000000 telus_bulk-1.3.6/LICENSE
+-rw-rw-rw-   0        0        0     5417 2023-04-18 16:41:18.375930 telus_bulk-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3536 2023-04-18 16:38:35.000000 telus_bulk-1.3.6/README.md
+-rw-rw-rw-   0        0        0     1013 2023-04-18 16:37:04.000000 telus_bulk-1.3.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 16:41:18.379933 telus_bulk-1.3.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 16:41:17.753494 telus_bulk-1.3.6/src/
+-rw-rw-rw-   0        0        0        0 2022-09-29 17:24:33.000000 telus_bulk-1.3.6/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:41:17.756489 telus_bulk-1.3.6/src/telus_bulk/
+-rw-rw-rw-   0        0        0       72 2022-09-29 16:01:50.000000 telus_bulk-1.3.6/src/telus_bulk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:41:17.780105 telus_bulk-1.3.6/src/telus_bulk/helpers/
+drwxrwxrwx   0        0        0        0 2023-04-18 16:41:17.790105 telus_bulk-1.3.6/src/telus_bulk/helpers/cron_job/
+-rw-rw-rw-   0        0        0       62 2022-11-30 18:14:51.000000 telus_bulk-1.3.6/src/telus_bulk/helpers/cron_job/__init__.py
+-rw-rw-rw-   0        0        0      709 2022-11-30 18:14:22.000000 telus_bulk-1.3.6/src/telus_bulk/helpers/cron_job/thread_job.py
+-rw-rw-rw-   0        0        0       82 2022-10-05 22:39:52.000000 telus_bulk-1.3.6/src/telus_bulk/helpers/mutiple_spaces.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:41:17.812106 telus_bulk-1.3.6/src/telus_bulk/helpers/web_methods/
+-rw-rw-rw-   0        0        0      200 2022-12-20 23:56:52.000000 telus_bulk-1.3.6/src/telus_bulk/helpers/web_methods/__init__.py
+-rw-rw-rw-   0        0        0     2627 2023-04-18 16:38:10.000000 telus_bulk-1.3.6/src/telus_bulk/helpers/web_methods/async_web_methods_helper.py
+-rw-rw-rw-   0        0        0     2560 2023-04-18 16:36:32.000000 telus_bulk-1.3.6/src/telus_bulk/helpers/web_methods/web_methods_helper.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:41:17.823106 telus_bulk-1.3.6/src/telus_bulk/models/
+-rw-rw-rw-   0        0        0       65 2022-09-14 17:56:07.000000 telus_bulk-1.3.6/src/telus_bulk/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:41:17.898729 telus_bulk-1.3.6/src/telus_bulk/models/ams/
+-rw-rw-rw-   0        0        0       75 2022-09-14 17:37:58.000000 telus_bulk-1.3.6/src/telus_bulk/models/ams/__init__.py
+-rw-rw-rw-   0        0        0     2788 2022-10-05 23:54:12.000000 telus_bulk-1.3.6/src/telus_bulk/models/ams/address_detail_model.py
+-rw-rw-rw-   0        0        0      470 2022-11-29 22:57:32.000000 telus_bulk-1.3.6/src/telus_bulk/models/ams/city_alias.py
+-rw-rw-rw-   0        0        0      519 2022-09-26 23:03:35.000000 telus_bulk-1.3.6/src/telus_bulk/models/ams/coordinate.py
+-rw-rw-rw-   0        0        0      230 2022-08-09 18:59:43.000000 telus_bulk-1.3.6/src/telus_bulk/models/ams/credentials_response.py
+-rw-rw-rw-   0        0        0      506 2022-09-12 17:32:45.000000 telus_bulk-1.3.6/src/telus_bulk/models/ams/e911_address.py
+-rw-rw-rw-   0        0        0      856 2022-10-05 23:50:04.000000 telus_bulk-1.3.6/src/telus_bulk/models/ams/fms_address.py
+-rw-rw-rw-   0        0        0      392 2022-10-05 23:46:20.000000 telus_bulk-1.3.6/src/telus_bulk/models/ams/reference_id.py
+-rw-rw-rw-   0        0        0      302 2022-10-05 23:52:28.000000 telus_bulk-1.3.6/src/telus_bulk/models/ams/reference_ids.py
+-rw-rw-rw-   0        0        0      657 2022-08-15 17:21:00.000000 telus_bulk-1.3.6/src/telus_bulk/models/ams/zone_attribute.py
+-rw-rw-rw-   0        0        0      464 2022-10-05 23:47:15.000000 telus_bulk-1.3.6/src/telus_bulk/models/ams/zone_info_item.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:41:17.912243 telus_bulk-1.3.6/src/telus_bulk/models/available_partners/
+-rw-rw-rw-   0        0        0      118 2022-09-29 17:42:55.000000 telus_bulk-1.3.6/src/telus_bulk/models/available_partners/__init__.py
+-rw-rw-rw-   0        0        0      352 2022-09-29 17:42:42.000000 telus_bulk-1.3.6/src/telus_bulk/models/available_partners/partners_enum.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:41:17.924243 telus_bulk-1.3.6/src/telus_bulk/models/clli/
+-rw-rw-rw-   0        0        0       50 2022-11-08 00:11:09.000000 telus_bulk-1.3.6/src/telus_bulk/models/clli/__init__.py
+-rw-rw-rw-   0        0        0      448 2022-11-18 22:55:35.000000 telus_bulk-1.3.6/src/telus_bulk/models/clli/clli_dto.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:41:17.931243 telus_bulk-1.3.6/src/telus_bulk/models/firestore/
+-rw-rw-rw-   0        0        0      821 2022-10-21 18:53:27.000000 telus_bulk-1.3.6/src/telus_bulk/models/firestore/firestore_reference.py
+-rw-rw-rw-   0        0        0       92 2022-10-18 17:59:41.000000 telus_bulk-1.3.6/src/telus_bulk/models/product_type.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:41:17.957242 telus_bulk-1.3.6/src/telus_bulk/models/reports/
+-rw-rw-rw-   0        0        0      155 2022-11-11 21:28:00.000000 telus_bulk-1.3.6/src/telus_bulk/models/reports/__init__.py
+-rw-rw-rw-   0        0        0     1208 2023-04-13 21:10:46.000000 telus_bulk-1.3.6/src/telus_bulk/models/reports/report_address.py
+-rw-rw-rw-   0        0        0      395 2022-11-17 17:58:06.000000 telus_bulk-1.3.6/src/telus_bulk/models/reports/report_qualification_detail.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:41:17.970245 telus_bulk-1.3.6/src/telus_bulk/models/tmf_620/
+-rw-rw-rw-   0        0        0       58 2022-12-30 21:59:38.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_620/__init__.py
+-rw-rw-rw-   0        0        0      109 2022-12-30 21:58:25.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_620/status_enum.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:41:18.308674 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/
+-rw-rw-rw-   0        0        0        0 2022-07-20 23:06:53.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/__init__.py
+-rw-rw-rw-   0        0        0     1078 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/addressable.py
+-rw-rw-rw-   0        0        0     1511 2022-09-14 17:54:30.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/alternate_service_proposal.py
+-rw-rw-rw-   0        0        0     1539 2022-09-14 17:54:33.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/characteristic.py
+-rw-rw-rw-   0        0        0     1220 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/characteristic_relationship.py
+-rw-rw-rw-   0        0        0     3724 2022-10-25 17:09:23.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification.py
+-rw-rw-rw-   0        0        0     2442 2022-09-14 17:54:33.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_attribute_value_change_event.py
+-rw-rw-rw-   0        0        0      993 2022-09-14 17:54:33.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_attribute_value_change_event_payload.py
+-rw-rw-rw-   0        0        0     2666 2022-11-09 14:29:21.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_create.py
+-rw-rw-rw-   0        0        0     2071 2022-09-14 17:54:33.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_create_event.py
+-rw-rw-rw-   0        0        0      937 2022-09-14 17:54:33.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_create_event_payload.py
+-rw-rw-rw-   0        0        0     2071 2022-09-14 17:54:33.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_delete_event.py
+-rw-rw-rw-   0        0        0      937 2022-09-14 17:54:33.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_delete_event_payload.py
+-rw-rw-rw-   0        0        0     2424 2022-09-14 17:54:33.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_information_required_event.py
+-rw-rw-rw-   0        0        0      989 2022-09-14 17:54:33.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_information_required_event_payload.py
+-rw-rw-rw-   0        0        0     4516 2022-10-31 17:35:23.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_item.py
+-rw-rw-rw-   0        0        0     2905 2022-09-14 17:54:33.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_queue_item.py
+-rw-rw-rw-   0        0        0     2152 2022-09-14 17:54:32.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_state_change_event.py
+-rw-rw-rw-   0        0        0      957 2022-09-14 17:54:32.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_state_change_event_payload.py
+-rw-rw-rw-   0        0        0     3362 2022-09-14 17:54:32.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_update.py
+-rw-rw-rw-   0        0        0     1407 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/constraint_ref.py
+-rw-rw-rw-   0        0        0     1271 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/entity_ref.py
+-rw-rw-rw-   0        0        0     1075 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/entity_value.py
+-rw-rw-rw-   0        0        0     1280 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/error.py
+-rw-rw-rw-   0        0        0      777 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/event_subscription.py
+-rw-rw-rw-   0        0        0      742 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/event_subscription_input.py
+-rw-rw-rw-   0        0        0      214 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/example.py
+-rw-rw-rw-   0        0        0      899 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/extensible.py
+-rw-rw-rw-   0        0        0      146 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/extra_models.py
+-rw-rw-rw-   0        0        0     1836 2022-09-14 17:54:32.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/feature.py
+-rw-rw-rw-   0        0        0     1400 2022-09-14 17:54:31.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/feature_relationship.py
+-rw-rw-rw-   0        0        0     1192 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/note.py
+-rw-rw-rw-   0        0        0      546 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/order_item_action_type.py
+-rw-rw-rw-   0        0        0     1659 2022-10-25 17:10:03.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/overall_process.py
+-rw-rw-rw-   0        0        0     1109 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/place.py
+-rw-rw-rw-   0        0        0     1261 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/place_ref.py
+-rw-rw-rw-   0        0        0     3301 2022-09-14 17:54:31.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/query_service_qualification.py
+-rw-rw-rw-   0        0        0     2094 2022-09-14 17:54:31.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/query_service_qualification_create.py
+-rw-rw-rw-   0        0        0     2071 2022-09-14 17:54:31.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/query_service_qualification_create_event.py
+-rw-rw-rw-   0        0        0      937 2022-09-14 17:54:31.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/query_service_qualification_create_event_payload.py
+-rw-rw-rw-   0        0        0     2071 2022-09-14 17:54:31.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/query_service_qualification_delete_event.py
+-rw-rw-rw-   0        0        0      937 2022-09-14 17:54:31.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/query_service_qualification_delete_event_payload.py
+-rw-rw-rw-   0        0        0     2152 2022-09-14 17:54:30.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/query_service_qualification_state_change_event.py
+-rw-rw-rw-   0        0        0      957 2022-09-14 17:54:30.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/query_service_qualification_state_change_event_payload.py
+-rw-rw-rw-   0        0        0     3014 2022-09-14 17:54:30.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/query_service_qualification_update.py
+-rw-rw-rw-   0        0        0     1494 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/related_entity_ref_or_value.py
+-rw-rw-rw-   0        0        0     1526 2022-12-12 21:11:57.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/related_party.py
+-rw-rw-rw-   0        0        0     1645 2023-01-26 22:32:07.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/related_place_ref_or_value.py
+-rw-rw-rw-   0        0        0     1780 2022-09-14 17:54:30.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/related_service_order_item.py
+-rw-rw-rw-   0        0        0     1277 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/resource_ref.py
+-rw-rw-rw-   0        0        0     4778 2022-09-14 17:54:30.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/service.py
+-rw-rw-rw-   0        0        0     1451 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/service_category_ref.py
+-rw-rw-rw-   0        0        0     1371 2022-10-24 21:26:56.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/service_eligibility_unavailability_reason.py
+-rw-rw-rw-   0        0        0     2572 2022-09-14 17:54:32.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/service_qualification.py
+-rw-rw-rw-   0        0        0     1990 2022-09-14 17:54:32.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/service_qualification_item.py
+-rw-rw-rw-   0        0        0     1314 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/service_qualification_item_relationship.py
+-rw-rw-rw-   0        0        0     1282 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/service_qualification_relationship.py
+-rw-rw-rw-   0        0        0     1281 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/service_ref.py
+-rw-rw-rw-   0        0        0     6545 2022-10-21 21:16:52.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/service_ref_or_value.py
+-rw-rw-rw-   0        0        0     1520 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/service_specification_ref.py
+-rw-rw-rw-   0        0        0      537 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/service_state_type.py
+-rw-rw-rw-   0        0        0      528 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/task_state_type.py
+-rw-rw-rw-   0        0        0     1118 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/termination_error.py
+-rw-rw-rw-   0        0        0     1143 2022-08-02 18:19:44.000000 telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/time_period.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:41:18.334269 telus_bulk-1.3.6/src/telus_bulk/models/worker_job/
+-rw-rw-rw-   0        0        0      173 2022-09-26 22:38:16.000000 telus_bulk-1.3.6/src/telus_bulk/models/worker_job/__init__.py
+-rw-rw-rw-   0        0        0     1169 2022-09-14 20:38:25.000000 telus_bulk-1.3.6/src/telus_bulk/models/worker_job/address_processing_job.py
+-rw-rw-rw-   0        0        0      426 2023-03-27 23:18:27.000000 telus_bulk-1.3.6/src/telus_bulk/models/worker_job/city_coverage_processed_job.py
+-rw-rw-rw-   0        0        0     1306 2023-01-26 22:56:40.000000 telus_bulk-1.3.6/src/telus_bulk/models/worker_job/place.py
+-rw-rw-rw-   0        0        0      418 2022-09-12 18:55:49.000000 telus_bulk-1.3.6/src/telus_bulk/models/worker_job/service_specification.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:41:18.354269 telus_bulk-1.3.6/src/telus_bulk/pagination/
+-rw-rw-rw-   0        0        0      113 2022-10-13 18:10:36.000000 telus_bulk-1.3.6/src/telus_bulk/pagination/__init__.py
+-rw-rw-rw-   0        0        0      349 2022-10-13 21:12:04.000000 telus_bulk-1.3.6/src/telus_bulk/pagination/page_dto.py
+-rw-rw-rw-   0        0        0      641 2022-10-13 21:39:09.000000 telus_bulk-1.3.6/src/telus_bulk/pagination/page_meta_dto.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:41:17.776108 telus_bulk-1.3.6/src/telus_bulk.egg-info/
+-rw-rw-rw-   0        0        0     5417 2023-04-18 16:41:17.000000 telus_bulk-1.3.6/src/telus_bulk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5932 2023-04-18 16:41:17.000000 telus_bulk-1.3.6/src/telus_bulk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 16:41:17.000000 telus_bulk-1.3.6/src/telus_bulk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-18 16:41:17.000000 telus_bulk-1.3.6/src/telus_bulk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 16:41:18.370931 telus_bulk-1.3.6/tests/
+-rw-rw-rw-   0        0        0      358 2022-09-29 18:01:51.000000 telus_bulk-1.3.6/tests/test_available_partner.py
+-rw-rw-rw-   0        0        0      325 2022-10-05 22:35:35.000000 telus_bulk-1.3.6/tests/test_helpers.py
+-rw-rw-rw-   0        0        0     1141 2022-11-09 14:32:32.000000 telus_bulk-1.3.6/tests/test_svc_create.py
```

### Comparing `telus_bulk-1.3.5/LICENSE` & `telus_bulk-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/PKG-INFO` & `telus_bulk-1.3.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telus_bulk
-Version: 1.3.5
+Version: 1.3.6
 Summary: A package to be used to store classes used among Telus Bulk repositories of TMF-645, TMF-620 and AMS models
 Author-email: Jose Olmedo <jose.olmedo@telusinternational.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -44,14 +44,17 @@
 ## PYTEST
 The .env file must have the PYTHONPATH variable  
 
     PYTHONPATH=src
 
 # Changelog
 
+1.3.6
+- Optional "timeout" parameter to http_get, http_post, async_http_get, async_http_post methods
+
 1.3.5
 - Added has_incomplete_items field to ReportAddress and ReportAddressUpdateDto
 
 1.3.4
 - Removed province_full_coverage and city_coverage flags from RelatedParty object, deprecated
 
 1.3.2
```

### Comparing `telus_bulk-1.3.5/README.md` & `telus_bulk-1.3.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 ## PYTEST
 The .env file must have the PYTHONPATH variable  
 
     PYTHONPATH=src
 
 # Changelog
 
+1.3.6
+- Optional "timeout" parameter to http_get, http_post, async_http_get, async_http_post methods
+
 1.3.5
 - Added has_incomplete_items field to ReportAddress and ReportAddressUpdateDto
 
 1.3.4
 - Removed province_full_coverage and city_coverage flags from RelatedParty object, deprecated
 
 1.3.2
```

### Comparing `telus_bulk-1.3.5/pyproject.toml` & `telus_bulk-1.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "google-cloud-core==2.3.2",
     "google-cloud-firestore==2.6.0",
     "googleapis-common-protos==1.56.4",
 ]
 build-backend = "setuptools.build_meta"
 [project]
 name = "telus_bulk"
-version = "1.3.5"
+version = "1.3.6"
 authors = [
   { name="Jose Olmedo", email="jose.olmedo@telusinternational.com" },
 ]
 description = "A package to be used to store classes used among Telus Bulk repositories of TMF-645, TMF-620 and AMS models"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10.7"
```

### Comparing `telus_bulk-1.3.5/src/telus_bulk/helpers/cron_job/thread_job.py` & `telus_bulk-1.3.6/src/telus_bulk/helpers/cron_job/thread_job.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/helpers/web_methods/async_web_methods_helper.py` & `telus_bulk-1.3.6/src/telus_bulk/helpers/web_methods/web_methods_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,76 +1,77 @@
 import httpx
 from typing import Literal, Optional
 from loguru import logger
 from httpx._types import QueryParamTypes
 
 
-async def async_http_get(
+def http_get(
     base_url: str,
     segment: str = "",
     params: QueryParamTypes = None,
     access_token: str = None,
+    timeout: int = 30,
 ):
     """
-    Async fetch get request
+    Fetch get request
     :param base_url: principal domain
     :param segment: request segment
     :param access_token: JWT access token
+    :param timeout: Timeout of the request in seconds
     :return: JSON response
     """
     headers = {
         "authorization": f"Bearer {access_token}",
     }
-    # USING ASYNC CLIENT
-    async with httpx.AsyncClient(
-        base_url=base_url, headers=headers, verify=False, timeout=30
+    with httpx.Client(
+        base_url=base_url, headers=headers, verify=False, timeout=timeout
     ) as client:
         try:
-            r = await client.get(url=segment, params=params)
+            r = client.get(url=segment, params=params)
             r.raise_for_status()
         except httpx.HTTPStatusError as exc:
             logger.error(
                 f"Error response {exc.response.status_code} while requesting {exc.request.url!r}"
             )
             return None
         except httpx.HTTPError as exc:
             logger.error(f"Error while requesting {exc.request.url!r}")
             return None
     return r.json()
 
 
-async def async_http_post(
+def http_post(
     base_url: str,
     segment: str = "",
     data: Optional[dict[str, str]] = None,
     content_type: Literal["JSON", "FORM-ENCODED"] = "FORM-ENCODED",
+    timeout: int = 30,
 ):
     """
-    Async post request
+    Fetch post request
     :param base_url: principal domain
     :param segment: request segment
     :param data: request payload
     :return: JSON response
     """
     if content_type == "JSON":
         headers = [
             (b"content-type", b"application/json"),
             (b"accept", b"application/json"),
         ]
     elif content_type == "FORM-ENCODED":
         headers = {"content-type": "application/x-www-form-urlencoded"}
-    # USING ASYNC CLIENT
-    async with httpx.AsyncClient(
-        base_url=base_url, headers=headers, verify=False, timeout=30
+    with httpx.Client(
+        base_url=base_url, headers=headers, verify=False, timeout=timeout
     ) as client:
         try:
             if content_type == "JSON":
-                r = await client.post(url=segment, json=data)
+                r = client.post(url=segment, json=data)
             else:
-                r = await client.post(url=segment, data=data)
+                r = client.post(url=segment, data=data)
             r.raise_for_status()
         except httpx.HTTPStatusError as exc:
             logger.error(
                 f"Error response {exc.response.status_code} while requesting {exc.request.url}"
             )
             return None
         except httpx.HTTPError as exc:
```

### Comparing `telus_bulk-1.3.5/src/telus_bulk/helpers/web_methods/web_methods_helper.py` & `telus_bulk-1.3.6/src/telus_bulk/helpers/web_methods/async_web_methods_helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,78 @@
 import httpx
 from typing import Literal, Optional
 from loguru import logger
 from httpx._types import QueryParamTypes
 
 
-def http_get(
+async def async_http_get(
     base_url: str,
     segment: str = "",
     params: QueryParamTypes = None,
     access_token: str = None,
+    timeout: int = 30,
 ):
     """
-    Fetch get request
+    Async fetch get request
     :param base_url: principal domain
     :param segment: request segment
     :param access_token: JWT access token
     :return: JSON response
     """
     headers = {
         "authorization": f"Bearer {access_token}",
     }
-    with httpx.Client(
-        base_url=base_url, headers=headers, verify=False, timeout=30
+    # USING ASYNC CLIENT
+    async with httpx.AsyncClient(
+        base_url=base_url, headers=headers, verify=False, timeout=timeout
     ) as client:
         try:
-            r = client.get(url=segment, params=params)
+            r = await client.get(url=segment, params=params)
             r.raise_for_status()
         except httpx.HTTPStatusError as exc:
             logger.error(
                 f"Error response {exc.response.status_code} while requesting {exc.request.url!r}"
             )
             return None
         except httpx.HTTPError as exc:
             logger.error(f"Error while requesting {exc.request.url!r}")
             return None
     return r.json()
 
 
-def http_post(
+async def async_http_post(
     base_url: str,
     segment: str = "",
     data: Optional[dict[str, str]] = None,
     content_type: Literal["JSON", "FORM-ENCODED"] = "FORM-ENCODED",
+    timeout: int = 30,
 ):
     """
-    Fetch post request
+    Async post request
     :param base_url: principal domain
     :param segment: request segment
     :param data: request payload
     :return: JSON response
     """
     if content_type == "JSON":
         headers = [
             (b"content-type", b"application/json"),
             (b"accept", b"application/json"),
         ]
     elif content_type == "FORM-ENCODED":
         headers = {"content-type": "application/x-www-form-urlencoded"}
-    with httpx.Client(
-        base_url=base_url, headers=headers, verify=False, timeout=30
+    # USING ASYNC CLIENT
+    async with httpx.AsyncClient(
+        base_url=base_url, headers=headers, verify=False, timeout=timeout
     ) as client:
         try:
             if content_type == "JSON":
-                r = client.post(url=segment, json=data)
+                r = await client.post(url=segment, json=data)
             else:
-                r = client.post(url=segment, data=data)
+                r = await client.post(url=segment, data=data)
             r.raise_for_status()
         except httpx.HTTPStatusError as exc:
             logger.error(
                 f"Error response {exc.response.status_code} while requesting {exc.request.url}"
             )
             return None
         except httpx.HTTPError as exc:
```

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/ams/address_detail_model.py` & `telus_bulk-1.3.6/src/telus_bulk/models/ams/address_detail_model.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/ams/coordinate.py` & `telus_bulk-1.3.6/src/telus_bulk/models/ams/coordinate.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/ams/fms_address.py` & `telus_bulk-1.3.6/src/telus_bulk/models/ams/fms_address.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/ams/zone_attribute.py` & `telus_bulk-1.3.6/src/telus_bulk/models/ams/zone_attribute.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/firestore/firestore_reference.py` & `telus_bulk-1.3.6/src/telus_bulk/models/firestore/firestore_reference.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/reports/report_address.py` & `telus_bulk-1.3.6/src/telus_bulk/models/reports/report_address.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/addressable.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/addressable.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/alternate_service_proposal.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/alternate_service_proposal.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/characteristic.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/characteristic.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/characteristic_relationship.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/characteristic_relationship.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_attribute_value_change_event.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_attribute_value_change_event.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_attribute_value_change_event_payload.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_attribute_value_change_event_payload.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_create.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_create.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_create_event.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_create_event.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_create_event_payload.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_create_event_payload.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_delete_event.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_delete_event.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_delete_event_payload.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_delete_event_payload.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_information_required_event.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_information_required_event.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_information_required_event_payload.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_information_required_event_payload.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_item.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_item.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_queue_item.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_queue_item.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_state_change_event.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_state_change_event.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_state_change_event_payload.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_state_change_event_payload.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/check_service_qualification_update.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/check_service_qualification_update.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/constraint_ref.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/constraint_ref.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/entity_ref.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/entity_ref.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/entity_value.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/entity_value.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/error.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/error.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/event_subscription.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/event_subscription.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/event_subscription_input.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/event_subscription_input.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/extensible.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/extensible.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/feature.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/feature.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/feature_relationship.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/feature_relationship.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/note.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/note.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/order_item_action_type.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/order_item_action_type.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/overall_process.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/overall_process.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/place.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/place.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/place_ref.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/place_ref.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/query_service_qualification.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/query_service_qualification.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/query_service_qualification_create.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/query_service_qualification_create.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/query_service_qualification_create_event.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/query_service_qualification_create_event.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/query_service_qualification_create_event_payload.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/query_service_qualification_create_event_payload.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/query_service_qualification_delete_event.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/query_service_qualification_delete_event.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/query_service_qualification_delete_event_payload.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/query_service_qualification_delete_event_payload.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/query_service_qualification_state_change_event.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/query_service_qualification_state_change_event.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/query_service_qualification_state_change_event_payload.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/query_service_qualification_state_change_event_payload.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/query_service_qualification_update.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/query_service_qualification_update.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/related_entity_ref_or_value.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/related_entity_ref_or_value.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/related_party.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/related_party.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/related_place_ref_or_value.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/related_place_ref_or_value.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/related_service_order_item.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/related_service_order_item.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/resource_ref.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/resource_ref.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/service.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/service.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/service_category_ref.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/service_category_ref.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/service_eligibility_unavailability_reason.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/service_eligibility_unavailability_reason.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/service_qualification.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/service_qualification.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/service_qualification_item.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/service_qualification_item.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/service_qualification_item_relationship.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/service_qualification_item_relationship.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/service_qualification_relationship.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/service_qualification_relationship.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/service_ref.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/service_ref.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/service_ref_or_value.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/service_ref_or_value.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/service_specification_ref.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/service_specification_ref.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/service_state_type.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/service_state_type.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/task_state_type.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/task_state_type.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/termination_error.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/termination_error.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/tmf_645/time_period.py` & `telus_bulk-1.3.6/src/telus_bulk/models/tmf_645/time_period.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/worker_job/address_processing_job.py` & `telus_bulk-1.3.6/src/telus_bulk/models/worker_job/address_processing_job.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/models/worker_job/place.py` & `telus_bulk-1.3.6/src/telus_bulk/models/worker_job/place.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk/pagination/page_meta_dto.py` & `telus_bulk-1.3.6/src/telus_bulk/pagination/page_meta_dto.py`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/src/telus_bulk.egg-info/PKG-INFO` & `telus_bulk-1.3.6/src/telus_bulk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telus-bulk
-Version: 1.3.5
+Version: 1.3.6
 Summary: A package to be used to store classes used among Telus Bulk repositories of TMF-645, TMF-620 and AMS models
 Author-email: Jose Olmedo <jose.olmedo@telusinternational.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -44,14 +44,17 @@
 ## PYTEST
 The .env file must have the PYTHONPATH variable  
 
     PYTHONPATH=src
 
 # Changelog
 
+1.3.6
+- Optional "timeout" parameter to http_get, http_post, async_http_get, async_http_post methods
+
 1.3.5
 - Added has_incomplete_items field to ReportAddress and ReportAddressUpdateDto
 
 1.3.4
 - Removed province_full_coverage and city_coverage flags from RelatedParty object, deprecated
 
 1.3.2
```

### Comparing `telus_bulk-1.3.5/src/telus_bulk.egg-info/SOURCES.txt` & `telus_bulk-1.3.6/src/telus_bulk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `telus_bulk-1.3.5/tests/test_svc_create.py` & `telus_bulk-1.3.6/tests/test_svc_create.py`

 * *Files identical despite different names*

